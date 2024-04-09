# Comparing `tmp/perceval-0.9.9.tar.gz` & `tmp/perceval-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/dist/perceval-0.9.9.tar", last modified: Fri Dec 29 08:20:30 2017, max compression
+gzip compressed data, was "perceval-1.0.0rc1.tar", max compression
```

## Comparing `perceval-0.9.9.tar` & `perceval-1.0.0rc1.tar`

### file list

```diff
@@ -1,53 +1,421 @@
-drwxr-xr-x   0 grimoirelab  (1000) grimoirelab  (1000)        0 2017-12-29 08:20:30.000000 perceval-0.9.9/
-drwxr-xr-x   0 grimoirelab  (1000) grimoirelab  (1000)        0 2017-12-29 08:20:30.000000 perceval-0.9.9/perceval.egg-info/
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     1336 2017-12-29 08:20:30.000000 perceval-0.9.9/perceval.egg-info/SOURCES.txt
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)      136 2017-12-29 08:20:30.000000 perceval-0.9.9/perceval.egg-info/requires.txt
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)        1 2017-12-29 08:20:30.000000 perceval-0.9.9/perceval.egg-info/not-zip-safe
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    12553 2017-12-29 08:20:30.000000 perceval-0.9.9/perceval.egg-info/PKG-INFO
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)        1 2017-12-29 08:20:30.000000 perceval-0.9.9/perceval.egg-info/dependency_links.txt
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)        9 2017-12-29 08:20:30.000000 perceval-0.9.9/perceval.egg-info/top_level.txt
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)      198 2017-12-29 08:20:30.000000 perceval-0.9.9/setup.cfg
-drwxr-xr-x   0 grimoirelab  (1000) grimoirelab  (1000)        0 2017-12-29 08:20:30.000000 perceval-0.9.9/bin/
--rwxr-xr-x   0 grimoirelab  (1000) grimoirelab  (1000)     6760 2017-12-29 08:20:29.000000 perceval-0.9.9/bin/perceval
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     8368 2017-12-29 08:20:29.000000 perceval-0.9.9/README.md
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)       18 2017-12-29 08:20:29.000000 perceval-0.9.9/MANIFEST.in
-drwxr-xr-x   0 grimoirelab  (1000) grimoirelab  (1000)        0 2017-12-29 08:20:30.000000 perceval-0.9.9/perceval/
-drwxr-xr-x   0 grimoirelab  (1000) grimoirelab  (1000)        0 2017-12-29 08:20:30.000000 perceval-0.9.9/perceval/backends/
-drwxr-xr-x   0 grimoirelab  (1000) grimoirelab  (1000)        0 2017-12-29 08:20:30.000000 perceval-0.9.9/perceval/backends/core/
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    11900 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/jira.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    11404 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/telegram.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     7596 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/jenkins.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    10128 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/stackexchange.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    23452 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/github.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    18036 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/askbot.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     8934 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/nntp.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    15295 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/meetup.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    15954 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/bugzillarest.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    14437 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/slack.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    12230 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/mbox.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     9512 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/pipermail.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     5138 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/rss.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    12329 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/discourse.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    20426 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/launchpad.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     6530 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/dockerhub.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    19036 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/bugzilla.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    19391 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/phabricator.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    42297 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/git.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    12352 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/gmane.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    12906 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/supybot.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)        0 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/__init__.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     8851 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/hyperkitty.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    16418 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/gerrit.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    13081 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/confluence.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    15361 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/redmine.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    19277 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/mediawiki.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)      879 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/__init__.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     9373 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/client.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     4900 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/cache.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     2071 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/errors.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    15249 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backend.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     1011 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/__init__.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)       97 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/_version.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     8300 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/utils.py
--rwxr-xr-x   0 grimoirelab  (1000) grimoirelab  (1000)     3008 2017-12-29 08:20:29.000000 perceval-0.9.9/setup.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    12553 2017-12-29 08:20:30.000000 perceval-0.9.9/PKG-INFO
+-rw-r--r--   0        0        0      372 2024-04-09 16:09:58.160790 perceval-1.0.0rc1/AUTHORS
+-rw-r--r--   0        0        0    35147 2024-04-09 16:09:58.160790 perceval-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0    27830 2024-04-09 16:09:58.160790 perceval-1.0.0rc1/NEWS
+-rw-r--r--   0        0        0    14910 2024-04-09 16:09:58.160790 perceval-1.0.0rc1/README.md
+-rw-r--r--   0        0        0       91 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/_version.py
+-rw-r--r--   0        0        0    16644 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/archive.py
+-rw-r--r--   0        0        0    48005 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backend.py
+-rw-r--r--   0        0        0      913 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/__init__.py
+-rw-r--r--   0        0        0    20584 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/askbot.py
+-rw-r--r--   0        0        0    19635 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/bugzilla.py
+-rw-r--r--   0        0        0    17429 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/bugzillarest.py
+-rw-r--r--   0        0        0    18002 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/confluence.py
+-rw-r--r--   0        0        0    14960 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/discourse.py
+-rw-r--r--   0        0        0     7067 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/dockerhub.py
+-rw-r--r--   0        0        0    18878 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/gerrit.py
+-rw-r--r--   0        0        0    52424 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/git.py
+-rw-r--r--   0        0        0    43434 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/github.py
+-rw-r--r--   0        0        0    17649 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/githubql.py
+-rw-r--r--   0        0        0    27653 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/gitlab.py
+-rw-r--r--   0        0        0    12438 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/gitter.py
+-rw-r--r--   0        0        0     8489 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/googlehits.py
+-rw-r--r--   0        0        0    12010 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/groupsio.py
+-rw-r--r--   0        0        0    10438 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/hyperkitty.py
+-rw-r--r--   0        0        0    11676 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/jenkins.py
+-rw-r--r--   0        0        0    15703 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/jira.py
+-rw-r--r--   0        0        0    17102 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/launchpad.py
+-rw-r--r--   0        0        0    17731 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/mattermost.py
+-rw-r--r--   0        0        0    14322 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/mbox.py
+-rw-r--r--   0        0        0    21374 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/mediawiki.py
+-rw-r--r--   0        0        0    16238 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/meetup.py
+-rw-r--r--   0        0        0    11554 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/nntp.py
+-rw-r--r--   0        0        0    14905 2024-04-09 16:09:58.164790 perceval-1.0.0rc1/perceval/backends/core/pagure.py
+-rw-r--r--   0        0        0    20949 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/backends/core/phabricator.py
+-rw-r--r--   0        0        0    10892 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/backends/core/pipermail.py
+-rw-r--r--   0        0        0    14273 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/backends/core/redmine.py
+-rw-r--r--   0        0        0    13851 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/backends/core/rocketchat.py
+-rw-r--r--   0        0        0     5761 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/backends/core/rss.py
+-rw-r--r--   0        0        0    15998 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/backends/core/slack.py
+-rw-r--r--   0        0        0    12685 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/backends/core/stackexchange.py
+-rw-r--r--   0        0        0    13727 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/backends/core/supybot.py
+-rw-r--r--   0        0        0    12519 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/backends/core/telegram.py
+-rw-r--r--   0        0        0    15640 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/backends/core/twitter.py
+-rw-r--r--   0        0        0    11883 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/client.py
+-rw-r--r--   0        0        0     2350 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/errors.py
+-rwxr-xr-x   0        0        0     7223 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/perceval.py
+-rw-r--r--   0        0        0     8559 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/perceval/utils.py
+-rw-r--r--   0        0        0     1762 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 16:09:58.168789 perceval-1.0.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0     1880 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/base.py
+-rw-r--r--   0        0        0     5757 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/api_24396_openstack.json
+-rw-r--r--   0        0        0     6055 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/askbot_2481_multicomments.json
+-rw-r--r--   0        0        0     1007 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/askbot_api_questions.json
+-rw-r--r--   0        0        0     2758 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/askbot_api_questions_2.json
+-rw-r--r--   0        0        0    82758 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/askbot_question.html
+-rw-r--r--   0        0        0    15771 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/askbot_question_empty.html
+-rw-r--r--   0        0        0   150456 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/askbot_question_multipage_1.html
+-rw-r--r--   0        0        0    81766 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/askbot_question_multipage_2.html
+-rw-r--r--   0        0        0   133477 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/html_148_comments_answer_2_openstack.html
+-rw-r--r--   0        0        0    94749 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/html_16_multicomment_answer_1_openstack.html
+-rw-r--r--   0        0        0   153064 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/html_24396_multipage_2_openstack.html
+-rw-r--r--   0        0        0   157831 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/html_24396_multipage_3_openstack.html
+-rw-r--r--   0        0        0    81807 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/html_24396_multipage_4_openstack.html
+-rw-r--r--   0        0        0   146501 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/html_24396_multipage_openstack.html
+-rw-r--r--   0        0        0   107008 2024-04-09 16:09:58.172789 perceval-1.0.0rc1/tests/data/askbot/html_26830_comments_question_openstack.html
+-rw-r--r--   0        0        0   155552 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/askbot/html_7893_answer_3_updated.html
+-rw-r--r--   0        0        0    71587 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/askbot/html_country_and_website.html
+-rw-r--r--   0        0        0     4140 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bug.xml
+-rw-r--r--   0        0        0    10630 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bug_activity.html
+-rw-r--r--   0        0        0    11983 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bug_activity_empty.html
+-rw-r--r--   0        0        0    11985 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bug_activity_empty_alt.html
+-rw-r--r--   0        0        0    11924 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bug_activity_not_valid.html
+-rw-r--r--   0        0        0      753 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_buglist.csv
+-rw-r--r--   0        0        0      304 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_buglist_next.csv
+-rw-r--r--   0        0        0    11373 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bugs_details.xml
+-rw-r--r--   0        0        0     4475 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bugs_details_next.xml
+-rw-r--r--   0        0        0     4850 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bugs_details_not_valid.xml
+-rw-r--r--   0        0        0    14409 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_bugs_invalid_chars.xml
+-rw-r--r--   0        0        0      246 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_no_version.xml
+-rw-r--r--   0        0        0     5666 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_rest_bugs.json
+-rw-r--r--   0        0        0      769 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_rest_bugs_attachments.json
+-rw-r--r--   0        0        0       68 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_rest_bugs_attachments_empty.json
+-rw-r--r--   0        0        0     5818 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_rest_bugs_comments.json
+-rw-r--r--   0        0        0       83 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_rest_bugs_comments_empty.json
+-rw-r--r--   0        0        0       19 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_rest_bugs_empty.json
+-rw-r--r--   0        0        0     3530 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_rest_bugs_history.json
+-rw-r--r--   0        0        0      123 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_rest_bugs_history_empty.json
+-rw-r--r--   0        0        0     6003 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_rest_bugs_next.json
+-rw-r--r--   0        0        0      165 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_rest_error.json
+-rw-r--r--   0        0        0      273 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/bugzilla/bugzilla_version.xml
+-rw-r--r--   0        0        0     3785 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/confluence/confluence_content_1_v1.json
+-rw-r--r--   0        0        0     6573 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/confluence/confluence_content_1_v2.json
+-rw-r--r--   0        0        0     2287 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/confluence/confluence_content_1_v3.json
+-rw-r--r--   0        0        0    11007 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/confluence/confluence_content_2_v1.json
+-rw-r--r--   0        0        0     2658 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/confluence/confluence_content_3.json
+-rw-r--r--   0        0        0     2196 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/confluence/confluence_content_att_v1.json
+-rw-r--r--   0        0        0     2698 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/confluence/confluence_content_space.json
+-rw-r--r--   0        0        0     3548 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/confluence/confluence_contents.json
+-rw-r--r--   0        0        0      275 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/confluence/confluence_contents_empty.json
+-rw-r--r--   0        0        0     1175 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/confluence/confluence_contents_next.json
+-rw-r--r--   0        0        0     2265 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/discourse/discourse_post.json
+-rw-r--r--   0        0        0    10341 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/discourse/discourse_posts.json
+-rw-r--r--   0        0        0    91062 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/discourse/discourse_topic_1148.json
+-rw-r--r--   0        0        0    42932 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/discourse/discourse_topic_1149.json
+-rw-r--r--   0        0        0    42931 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/discourse/discourse_topic_1150.json
+-rw-r--r--   0        0        0     4029 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/discourse/discourse_topics.json
+-rw-r--r--   0        0        0      199 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/discourse/discourse_topics_empty.json
+-rw-r--r--   0        0        0     3528 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/discourse/discourse_topics_last_posted_at_null.json
+-rw-r--r--   0        0        0     5902 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/discourse/discourse_topics_pinned.json
+-rw-r--r--   0        0        0     8371 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/dockerhub/dockerhub_repository_1.json
+-rw-r--r--   0        0        0    19166 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/gerrit/gerrit_reviews_page_1
+-rw-r--r--   0        0        0    11082 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/gerrit/gerrit_reviews_page_2
+-rw-r--r--   0        0        0    11073 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/gerrit/gerrit_reviews_page_3
+-rw-r--r--   0        0        0       36 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/gerrit/gerrit_version_214
+-rw-r--r--   0        0        0       20 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/gerrit/gerrit_version_313
+-rw-r--r--   0        0        0       33 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/gerrit/gerrit_version_unknown
+-rw-r--r--   0        0        0      412 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/git/git_bad_cr.txt
+-rw-r--r--   0        0        0      828 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/git/git_bad_encoding.txt
+-rw-r--r--   0        0        0     4635 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/git/git_log.txt
+-rw-r--r--   0        0        0        1 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/git/git_log_empty.txt
+-rw-r--r--   0        0        0      874 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/git/git_log_incompleted.txt
+-rw-r--r--   0        0        0     1098 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/git/git_log_merge.txt
+-rw-r--r--   0        0        0     1616 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/git/git_log_trailers.txt
+-rw-r--r--   0        0        0     9235 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/git/gitalternates.tar.gz
+-rw-r--r--   0        0        0    14520 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/git/gitdetached.tar.gz
+-rw-r--r--   0        0        0    16064 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/git/gittest-sub.tar.gz
+-rw-r--r--   0        0        0    30758 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/git/gittest-top-sub.tar.gz
+-rw-r--r--   0        0        0    14464 2024-04-09 16:09:58.176789 perceval-1.0.0rc1/tests/data/git/gittest.tar.gz
+-rw-r--r--   0        0        0     7232 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/git/gittest_no_refs.tar.gz
+-rw-r--r--   0        0        0     6108 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/git/gittestempty.tar.gz
+-rw-r--r--   0        0        0      192 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/abuse_rate_limit
+-rw-r--r--   0        0        0        3 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_empty_request
+-rw-r--r--   0        0        0      998 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_enterprise_request_requested_reviewers
+-rw-r--r--   0        0        0      253 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_events_error
+-rw-r--r--   0        0        0     1911 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_events_page_1
+-rw-r--r--   0        0        0     2419 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_events_page_2
+-rw-r--r--   0        0        0     1408 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_events_page_3
+-rw-r--r--   0        0        0     3609 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_events_pull_request_review
+-rw-r--r--   0        0        0     4727 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_issue_1
+-rw-r--r--   0        0        0     2678 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_issue_2
+-rw-r--r--   0        0        0     2574 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_issue_2_reactions
+-rw-r--r--   0        0        0     2992 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_issue_2_with_pr
+-rw-r--r--   0        0        0     2389 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_issue_comment_1_reactions
+-rw-r--r--   0        0        0        3 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_issue_comment_2_reactions
+-rw-r--r--   0        0        0     1761 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_issue_comments_1
+-rw-r--r--   0        0        0     1762 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_issue_comments_2
+-rw-r--r--   0        0        0     1310 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_login
+-rw-r--r--   0        0        0     1103 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_orgs
+-rw-r--r--   0        0        0     7135 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_repo
+-rw-r--r--   0        0        0     4819 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_request
+-rw-r--r--   0        0        0     2172 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_request_from_2016_03_01
+-rw-r--r--   0        0        0    25995 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_request_pull_request_1
+-rw-r--r--   0        0        0     5751 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_request_pull_request_1_comment_2_reactions
+-rw-r--r--   0        0        0     7951 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_request_pull_request_1_comments
+-rw-r--r--   0        0        0     4408 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_request_pull_request_1_commits
+-rw-r--r--   0        0        0     2499 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_request_pull_request_1_reviews
+-rw-r--r--   0        0        0    23553 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_request_pull_request_2
+-rw-r--r--   0        0        0    11230 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_request_pull_request_2_comments
+-rw-r--r--   0        0        0     4408 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_request_pull_request_2_commits
+-rw-r--r--   0        0        0     1773 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_request_pull_request_2_reviews
+-rw-r--r--   0        0        0     1150 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_request_requested_reviewers
+-rw-r--r--   0        0        0     1163 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/github_request_requested_reviewers_ghost
+-rw-r--r--   0        0        0      883 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/private.pem
+-rw-r--r--   0        0        0      484 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/rate_limit
+-rw-r--r--   0        0        0      480 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/rate_limit_aaa
+-rw-r--r--   0        0        0      484 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/github/rate_limit_bbb
+-rw-r--r--   0        0        0     1534 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/commits_1
+-rw-r--r--   0        0        0      581 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/commits_2
+-rw-r--r--   0        0        0      617 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/commits_3
+-rw-r--r--   0        0        0     1233 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/emoji
+-rw-r--r--   0        0        0        2 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/empty_emoji
+-rw-r--r--   0        0        0        2 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/empty_response
+-rw-r--r--   0        0        0     2379 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/issue_1
+-rw-r--r--   0        0        0     1311 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/issue_2
+-rw-r--r--   0        0        0     1164 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/issue_3
+-rw-r--r--   0        0        0     1411 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/issue_4
+-rw-r--r--   0        0        0     3708 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/issue_page_1
+-rw-r--r--   0        0        0     3378 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/issue_page_2
+-rw-r--r--   0        0        0     1735 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_1
+-rw-r--r--   0        0        0     3454 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_1_version_1
+-rw-r--r--   0        0        0     1001 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_1_version_2
+-rw-r--r--   0        0        0      778 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_1_versions
+-rw-r--r--   0        0        0     1872 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_2
+-rw-r--r--   0        0        0     2786 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_2_version_1
+-rw-r--r--   0        0        0      388 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_2_versions
+-rw-r--r--   0        0        0     2493 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_3
+-rw-r--r--   0        0        0     4320 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_3_version_1
+-rw-r--r--   0        0        0      388 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_3_versions
+-rw-r--r--   0        0        0      868 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_page_1
+-rw-r--r--   0        0        0      683 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_page_2
+-rw-r--r--   0        0        0      868 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_page_outdated
+-rw-r--r--   0        0        0      868 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/merge_page_updated
+-rw-r--r--   0        0        0     1316 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/notes_1
+-rw-r--r--   0        0        0      672 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/notes_2
+-rw-r--r--   0        0        0      626 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/notes_3
+-rw-r--r--   0        0        0      626 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/notes_4
+-rw-r--r--   0        0        0     2283 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitlab/project
+-rw-r--r--   0        0        0        2 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitter/message_empty
+-rw-r--r--   0        0        0      721 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitter/message_page_1
+-rw-r--r--   0        0        0      721 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitter/message_page_2
+-rw-r--r--   0        0        0     1316 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/gitter/rooms
+-rw-r--r--   0        0        0    78598 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/googlehits/hits_bitergia
+-rw-r--r--   0        0        0    69900 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/googlehits/hits_bitergia_grimoirelab
+-rw-r--r--   0        0        0    38721 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/googlehits/hits_zero
+-rw-r--r--   0        0        0      145 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/groupsio/empty.zip
+-rw-r--r--   0        0        0     1518 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/groupsio/login
+-rw-r--r--   0        0        0    33111 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/groupsio/messages.zip
+-rw-r--r--   0        0        0     3757 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/groupsio/subscriptions_page_1
+-rw-r--r--   0        0        0     3751 2024-04-09 16:09:58.180789 perceval-1.0.0rc1/tests/data/groupsio/subscriptions_page_2
+-rw-r--r--   0        0        0     6511 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/hyperkitty/hyperkitty_2016_april.mbox
+-rw-r--r--   0        0        0      875 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/hyperkitty/hyperkitty_2016_march.mbox
+-rw-r--r--   0        0        0     6547 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jenkins/jenkins_build.json
+-rw-r--r--   0        0        0   190490 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jenkins/jenkins_job_builds.json
+-rw-r--r--   0        0        0        3 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jenkins/jenkins_job_builds_empty.json
+-rw-r--r--   0        0        0    42326 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jenkins/jenkins_job_no_builds.json
+-rw-r--r--   0        0        0      890 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jenkins/jenkins_jobs.json
+-rw-r--r--   0        0        0        3 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jenkins/jenkins_jobs_empty.json
+-rw-r--r--   0        0        0    97205 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jenkins/jenkins_workflow_job_builds.json
+-rw-r--r--   0        0        0     1941 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jenkins/jenkins_workflow_jobs.json
+-rw-r--r--   0        0        0       77 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jira/jira_comments_issue_empty.json
+-rw-r--r--   0        0        0     7209 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jira/jira_comments_issue_page_1.json
+-rw-r--r--   0        0        0     7207 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jira/jira_comments_issue_page_2.json
+-rw-r--r--   0        0        0    14567 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jira/jira_fields.json
+-rw-r--r--   0        0        0    13217 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jira/jira_issues_page_1.json
+-rw-r--r--   0        0        0     6584 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jira/jira_issues_page_2.json
+-rw-r--r--   0        0        0       76 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jira/jira_issues_page_empty.json
+-rw-r--r--   0        0        0    12054 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/jira/jira_issues_parse_expected.json
+-rw-r--r--   0        0        0      159 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_empty_issue_activities
+-rw-r--r--   0        0        0      162 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_empty_issue_attachments
+-rw-r--r--   0        0        0      154 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_empty_issue_comments
+-rw-r--r--   0        0        0       46 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_empty_issues
+-rw-r--r--   0        0        0     2139 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1
+-rw-r--r--   0        0        0      827 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_activities
+-rw-r--r--   0        0        0     1610 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_activities_next_1
+-rw-r--r--   0        0        0     1509 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_activities_next_2
+-rw-r--r--   0        0        0      117 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_activities_no_entries
+-rw-r--r--   0        0        0     2571 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_attachments
+-rw-r--r--   0        0        0     1865 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_attachments_next_1
+-rw-r--r--   0        0        0     1769 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_attachments_next_2
+-rw-r--r--   0        0        0      117 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_attachments_no_entries
+-rw-r--r--   0        0        0     1925 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_comments
+-rw-r--r--   0        0        0     2039 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_comments_next_1
+-rw-r--r--   0        0        0     1916 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_comments_next_2
+-rw-r--r--   0        0        0      117 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_comments_no_entries
+-rw-r--r--   0        0        0    28963 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_expected
+-rw-r--r--   0        0        0     3981 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_expected_no_entries
+-rw-r--r--   0        0        0     2139 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_1_no_entries
+-rw-r--r--   0        0        0     2297 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_2
+-rw-r--r--   0        0        0      831 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_2_activities
+-rw-r--r--   0        0        0     1041 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_2_comments
+-rw-r--r--   0        0        0    17790 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_2_expected
+-rw-r--r--   0        0        0     2139 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_3
+-rw-r--r--   0        0        0     7538 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issue_3_expected
+-rw-r--r--   0        0        0     2208 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issues_page_1
+-rw-r--r--   0        0        0     1639 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issues_page_1_no_entries
+-rw-r--r--   0        0        0     1707 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issues_page_1_no_next
+-rw-r--r--   0        0        0     2309 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issues_page_2
+-rw-r--r--   0        0        0     1791 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_issues_page_3
+-rw-r--r--   0        0        0     3379 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/launchpad/launchpad_user_1
+-rw-r--r--   0        0        0      485 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mattermost/mattermost_channel.json
+-rw-r--r--   0        0        0      205 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mattermost/mattermost_erros.json
+-rw-r--r--   0        0        0     4014 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mattermost/mattermost_posts.json
+-rw-r--r--   0        0        0       37 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mattermost/mattermost_posts_empty.json
+-rw-r--r--   0        0        0     2812 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mattermost/mattermost_posts_next.json
+-rw-r--r--   0        0        0      507 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mattermost/mattermost_user_sduenas.json
+-rw-r--r--   0        0        0      892 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mattermost/mattermost_user_valcos.json
+-rw-r--r--   0        0        0     8584 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mbox/mbox_complex.mbox
+-rw-r--r--   0        0        0      953 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mbox/mbox_iso8859_encoding.mbox
+-rw-r--r--   0        0        0     9610 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mbox/mbox_multipart.mbox
+-rw-r--r--   0        0        0     1788 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mbox/mbox_no_fields.mbox
+-rw-r--r--   0        0        0      330 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mbox/mbox_single.mbox
+-rw-r--r--   0        0        0     2412 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mbox/mbox_unixfrom_encoding.mbox
+-rw-r--r--   0        0        0     1688 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mbox/mbox_unknown_encoding.mbox
+-rw-r--r--   0        0        0     9282 2024-04-09 16:09:58.184789 perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_namespaces.json
+-rw-r--r--   0        0        0   166125 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_page_476583_revisions.json
+-rw-r--r--   0        0        0      339 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_page_476589_revisions.json
+-rw-r--r--   0        0        0      339 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_page_476590_revisions.json
+-rw-r--r--   0        0        0      921 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_page_592384_revisions.json
+-rw-r--r--   0        0        0      555 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_pages_all.json
+-rw-r--r--   0        0        0      104 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_pages_all_empty.json
+-rw-r--r--   0        0        0     1823 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_pages_allrevisions.json
+-rw-r--r--   0        0        0      217 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_pages_allrevisions_empty.json
+-rw-r--r--   0        0        0     1831 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_pages_recent_changes.json
+-rw-r--r--   0        0        0     2139 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_siteinfo_1.23.json
+-rw-r--r--   0        0        0     3108 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/mediawiki/mediawiki_siteinfo_1.28.json
+-rw-r--r--   0        0        0     1670 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/meetup/meetup_comments.json
+-rw-r--r--   0        0        0    16033 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/meetup/meetup_events.json
+-rw-r--r--   0        0        0        3 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/meetup/meetup_events_empty.json
+-rw-r--r--   0        0        0    12659 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/meetup/meetup_events_next.json
+-rw-r--r--   0        0        0    11156 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/meetup/meetup_events_range.json
+-rw-r--r--   0        0        0     5071 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/meetup/meetup_rsvps.json
+-rw-r--r--   0        0        0     5405 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/nntp/nntp_1.txt
+-rw-r--r--   0        0        0     9233 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/nntp/nntp_2.txt
+-rw-r--r--   0        0        0     4113 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/nntp/nntp_parsing_error.txt
+-rw-r--r--   0        0        0        3 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/pagure/pagure_empty_request
+-rw-r--r--   0        0        0     3348 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/pagure/pagure_namespace_issue_2
+-rw-r--r--   0        0        0     1647 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/pagure/pagure_repo_issue_1
+-rw-r--r--   0        0        0     3216 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/pagure/pagure_repo_issue_2
+-rw-r--r--   0        0        0     2126 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/pagure/pagure_repo_issue_from_2020_03_07
+-rw-r--r--   0        0        0     2173 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/pagure/pagure_repo_only_issue_2
+-rw-r--r--   0        0        0      300 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_error.json
+-rw-r--r--   0        0        0      420 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_phid_herald.json
+-rw-r--r--   0        0        0      759 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_phids.json
+-rw-r--r--   0        0        0      417 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_project_bugreport.json
+-rw-r--r--   0        0        0      419 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_project_devel.json
+-rw-r--r--   0        0        0     4029 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_tasks.json
+-rw-r--r--   0        0        0      320 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_tasks_empty.json
+-rw-r--r--   0        0        0     1730 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_tasks_next.json
+-rw-r--r--   0        0        0    25354 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_transactions.json
+-rw-r--r--   0        0        0     9874 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_transactions_next.json
+-rw-r--r--   0        0        0      466 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_user_jane.json
+-rw-r--r--   0        0        0      453 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_user_janesmith.json
+-rw-r--r--   0        0        0      466 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_user_jdoe.json
+-rw-r--r--   0        0        0      441 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_user_jrae.json
+-rw-r--r--   0        0        0       69 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_user_jsmith.json
+-rw-r--r--   0        0        0     1601 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/phabricator/phabricator_users.json
+-rw-r--r--   0        0        0     6495 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/pipermail/pipermail_2015_november.mbox
+-rw-r--r--   0        0        0     6511 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/pipermail/pipermail_2016_april.mbox
+-rw-r--r--   0        0        0      875 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/pipermail/pipermail_2016_march.mbox
+-rw-r--r--   0        0        0     2170 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/pipermail/pipermail_apache_index.html
+-rw-r--r--   0        0        0     1867 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/pipermail/pipermail_index.html
+-rw-r--r--   0        0        0      593 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/pipermail/pipermail_index_empty.html
+-rw-r--r--   0        0        0     1414 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/redmine/redmine_issue_2.json
+-rw-r--r--   0        0        0     1426 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/redmine/redmine_issue_5.json
+-rw-r--r--   0        0        0    13221 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/redmine/redmine_issue_7311.json
+-rw-r--r--   0        0        0     1425 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/redmine/redmine_issue_9.json
+-rw-r--r--   0        0        0     2830 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/redmine/redmine_issues.json
+-rw-r--r--   0        0        0       76 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/redmine/redmine_issues_empty.json
+-rw-r--r--   0        0        0     1061 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/redmine/redmine_issues_next.json
+-rw-r--r--   0        0        0      292 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/redmine/redmine_user_24.json
+-rw-r--r--   0        0        0      292 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/redmine/redmine_user_25.json
+-rw-r--r--   0        0        0      291 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/redmine/redmine_user_3.json
+-rw-r--r--   0        0        0      291 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/redmine/redmine_user_4.json
+-rw-r--r--   0        0        0      896 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/rocketchat/channel_info.json
+-rw-r--r--   0        0        0       82 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/rocketchat/message_empty_2020_05_10.json
+-rw-r--r--   0        0        0     1408 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/rocketchat/message_page_1.json
+-rw-r--r--   0        0        0     1017 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/rocketchat/message_page_2.json
+-rw-r--r--   0        0        0      448 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/rocketchat/message_page_2020_05_03.json
+-rw-r--r--   0        0        0    18134 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/rss/rss_entries.xml
+-rw-r--r--   0        0        0       54 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/slack/slack_error.json
+-rw-r--r--   0        0        0     1752 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/slack/slack_history.json
+-rw-r--r--   0        0        0     1013 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/slack/slack_history_20150323.json
+-rw-r--r--   0        0        0       97 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/slack/slack_history_empty.json
+-rw-r--r--   0        0        0      393 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/slack/slack_history_next.json
+-rw-r--r--   0        0        0     1064 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/slack/slack_info.json
+-rw-r--r--   0        0        0     1063 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/slack/slack_info_archived.json
+-rw-r--r--   0        0        0     2225 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/slack/slack_members1.json
+-rw-r--r--   0        0        0     1445 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/slack/slack_members2.json
+-rw-r--r--   0        0        0     1252 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/slack/slack_user_U0001.json
+-rw-r--r--   0        0        0     1170 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/slack/slack_user_U0002.json
+-rw-r--r--   0        0        0     1060 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/slack/slack_user_U0003.json
+-rw-r--r--   0        0        0       51 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/slack/slack_user_U0004_private.json
+-rw-r--r--   0        0        0     2676 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/stackexchange/stackexchange_question
+-rw-r--r--   0        0        0     5189 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/stackexchange/stackexchange_question_backoff_page
+-rw-r--r--   0        0        0     5171 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/stackexchange/stackexchange_question_page
+-rw-r--r--   0        0        0     5172 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/stackexchange/stackexchange_question_page_2
+-rw-r--r--   0        0        0     4638 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/stackexchange/stackexchange_question_parse
+-rw-r--r--   0        0        0      883 2024-04-09 16:09:58.188789 perceval-1.0.0rc1/tests/data/supybot/supybot_2012_10_17.log
+-rw-r--r--   0        0        0      660 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/supybot/supybot_2012_10_18.log
+-rw-r--r--   0        0        0      181 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/supybot/supybot_date_without_tz.log
+-rw-r--r--   0        0        0      820 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/supybot/supybot_invalid_date.log
+-rw-r--r--   0        0        0      818 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/supybot/supybot_invalid_msg.log
+-rw-r--r--   0        0        0     7571 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/supybot/supybot_valid.log
+-rw-r--r--   0        0        0     1612 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/telegram/telegram_messages.json
+-rw-r--r--   0        0        0       27 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/telegram/telegram_messages_empty.json
+-rw-r--r--   0        0        0     1587 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/telegram/telegram_messages_next.json
+-rw-r--r--   0        0        0   731129 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/twitter/tweets.json
+-rw-r--r--   0        0        0    21985 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/twitter/tweets_page_1.json
+-rw-r--r--   0        0        0    24147 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/twitter/tweets_page_2.json
+-rw-r--r--   0        0        0      381 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/twitter/tweets_page_3.json
+-rw-r--r--   0        0        0     4140 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/utils/bugzilla_bug.xml
+-rw-r--r--   0        0        0    14409 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/utils/bugzilla_bugs_invalid_chars.xml
+-rw-r--r--   0        0        0     5429 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/utils/email_multipart_encoding.txt
+-rw-r--r--   0        0        0     4180 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/utils/email_multipart_no_encoding.txt
+-rw-r--r--   0        0        0      329 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/utils/email_single.txt
+-rw-r--r--   0        0        0      330 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/utils/mbox_single.mbox
+-rw-r--r--   0        0        0      420 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/data/utils/xml_invalid.xml
+-rw-r--r--   0        0        0        0 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/mocked_package/__init__.py
+-rw-r--r--   0        0        0     1270 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/mocked_package/backend.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/mocked_package/nested_package/__init__.py
+-rw-r--r--   0        0        0     1241 2024-04-09 16:09:58.192789 perceval-1.0.0rc1/tests/mocked_package/nested_package/nested_backend_b.py
+-rw-r--r--   0        0        0     1241 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/mocked_package/nested_package/nested_backend_c.py
+-rwxr-xr-x   0        0        0     1180 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/run_tests.py
+-rw-r--r--   0        0        0    18694 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_archive.py
+-rw-r--r--   0        0        0    29194 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_askbot.py
+-rw-r--r--   0        0        0    89739 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_backend.py
+-rw-r--r--   0        0        0    45401 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_bugzilla.py
+-rw-r--r--   0        0        0    34723 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_bugzillarest.py
+-rw-r--r--   0        0        0    19093 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_client.py
+-rw-r--r--   0        0        0    28276 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_confluence.py
+-rw-r--r--   0        0        0    46790 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_discourse.py
+-rw-r--r--   0        0        0     9175 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_dockerhub.py
+-rw-r--r--   0        0        0     4320 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_errors.py
+-rw-r--r--   0        0        0    21716 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_gerrit.py
+-rw-r--r--   0        0        0    82928 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_git.py
+-rw-r--r--   0        0        0   216577 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_github.py
+-rw-r--r--   0        0        0    38701 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_githubql.py
+-rw-r--r--   0        0        0    83197 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_gitlab.py
+-rw-r--r--   0        0        0    19906 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_gitter.py
+-rw-r--r--   0        0        0    13003 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_googlehits.py
+-rw-r--r--   0        0        0    21109 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_groupsio.py
+-rw-r--r--   0        0        0    18362 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_hyperkitty.py
+-rw-r--r--   0        0        0    38356 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_jenkins.py
+-rw-r--r--   0        0        0    40029 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_jira.py
+-rw-r--r--   0        0        0    54602 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_launchpad.py
+-rw-r--r--   0        0        0    31185 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_mattermost.py
+-rw-r--r--   0        0        0    27864 2024-04-09 16:09:58.196789 perceval-1.0.0rc1/tests/test_mbox.py
+-rw-r--r--   0        0        0    28609 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_mediawiki.py
+-rw-r--r--   0        0        0    37724 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_meetup.py
+-rw-r--r--   0        0        0    30330 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_pagure.py
+-rw-r--r--   0        0        0    45588 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_phabricator.py
+-rw-r--r--   0        0        0    27472 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_pipermail.py
+-rw-r--r--   0        0        0    23487 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_redmine.py
+-rw-r--r--   0        0        0    25298 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_rocketchat.py
+-rw-r--r--   0        0        0    10139 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_rss.py
+-rw-r--r--   0        0        0    35971 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_slack.py
+-rw-r--r--   0        0        0    22342 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_stackexchange.py
+-rw-r--r--   0        0        0    22836 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_supybot.py
+-rw-r--r--   0        0        0    18086 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_telegram.py
+-rw-r--r--   0        0        0    17146 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_twitter.py
+-rw-r--r--   0        0        0    11254 2024-04-09 16:09:58.200789 perceval-1.0.0rc1/tests/test_utils.py
+-rw-r--r--   0        0        0    16471 1970-01-01 00:00:00.000000 perceval-1.0.0rc1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `perceval-0.9.9/bin/perceval` & `perceval-1.0.0rc1/perceval/perceval.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,178 +1,172 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2017 Bitergia
+# Copyright (C) 2015-2020 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1335, USA.
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
+#     Alvaro del Castillo <acs@bitergia.com>
 #     Santiago Dueñas <sduenas@bitergia.com>
+#     Luis Cañas Díaz <lcanas@bitergia.com>
+#     Alberto Martín <alberto.martin@bitergia.com>
+#     Stephan Barth <stephan.barth@gmail.com>
+#     Valerio Cosentino <valcos@bitergia.com>
+#     Jesus M. Gonzalez-Barahona <jgb@gsyc.es>
+#     MalloZup <dmaiocchi@suse.com>
+#     Venu Vardhan Reddy Tekula <venuvardhanreddytekula8@gmail.com>
+#     animesh <animuz111@gmail.com>
+#     Nitish Gupta <imnitish.ng@gmail.com>
 #
 
 import argparse
-import configparser
 import logging
-import os.path
 import sys
 
 import perceval
-import perceval.backends
-
+import perceval.backend
+import perceval.backends.core
 
 PERCEVAL_USAGE_MSG = \
-"""%(prog)s [-c <file>] [-g] <backend> [<args>] | --help | --version"""
+    """%(prog)s [-g] <backend> [<args>] | --help | --version | --list"""
 
 PERCEVAL_DESC_MSG = \
-"""Send Sir Perceval on a quest to retrieve and gather data from software
+    """Send Sir Perceval on a quest to retrieve and gather data from software
 repositories.
 
 Repositories are reached using specific backends. The most common backends
 are:
 
     askbot           Fetch questions and answers from Askbot site
     bugzilla         Fetch bugs from a Bugzilla server
     bugzillarest     Fetch bugs from a Bugzilla server (>=5.0) using its REST API
     confluence       Fetch contents from a Confluence server
     discourse        Fetch posts from Discourse site
     dockerhub        Fetch repository data from Docker Hub site
     gerrit           Fetch reviews from a Gerrit server
     git              Fetch commits from Git
-    github           Fetch issues from GitHub
-    gmane            Fetch messages from Gmane
+    github           Fetch issues, pull requests and repository information from GitHub
+    gitlab           Fetch issues, merge requests from GitLab
+    gitter           Fetch messages from a Gitter room
+    googlehits       Fetch hits from Google API
+    groupsio         Fetch messages from Groups.io
     hyperkitty       Fetch messages from a HyperKitty archiver
     jenkins          Fetch builds from a Jenkins server
     jira             Fetch issues from JIRA issue tracker
     launchpad        Fetch issues from Launchpad issue tracker
+    mattermost       Fetch posts from a Mattermost server
     mbox             Fetch messages from MBox files
     mediawiki        Fetch pages and revisions from a MediaWiki site
     meetup           Fetch events from a Meetup group
     nntp             Fetch articles from a NNTP news group
+    pagure           Fetch issues from Pagure
     phabricator      Fetch tasks from a Phabricator site
     pipermail        Fetch messages from a Pipermail archiver
     redmine          Fetch issues from a Redmine server
+    rocketchat       Fetch messages from a Rocket.Chat channel
     rss              Fetch entries from a RSS feed server
     slack            Fetch messages from a Slack channel
     stackexchange    Fetch questions from StackExchange sites
     supybot          Fetch messages from Supybot log files
     telegram         Fetch messages from the Telegram server
+    twitter          Fetch tweets from the Twitter Search API
 
 optional arguments:
   -h, --help            show this help message and exit
   -v, --version         show version
-  -c FILE, --config FILE
-                        set configuration file
   -g, --debug           set debug mode on
+  -l, --list            show available backends
 """
 
 PERCEVAL_EPILOG_MSG = \
-"""Run '%(prog)s <backend> --help' to get information about a specific backend."""
+    """Run '%(prog)s <backend> --help' to get information about a specific backend."""
 
 PERCEVAL_VERSION_MSG = \
-"""%(prog)s """  + perceval.__version__
+    """%(prog)s """ + perceval.backends.core.__version__
 
 
 # Logging formats
 PERCEVAL_LOG_FORMAT = "[%(asctime)s] - %(message)s"
 PERCEVAL_DEBUG_LOG_FORMAT = "[%(asctime)s - %(name)s - %(levelname)s] - %(message)s"
 
 
-def main():
-    args = parse_args()
+class ListBackends(argparse.Action):
+
+    def __init__(self, option_strings, dest, **kwargs):
+        self.backends = kwargs.get('backends', None)
+        del kwargs['backends']
+        super().__init__(option_strings, dest, nargs=0, **kwargs)
+
+    def __call__(self, parser, namespace, values, option_string=None):
+        backends = sorted(self.backends.keys())
+        for backend in backends:
+            sys.stdout.write(backend + '\n')
+        parser.exit()
+
 
-    # Read default parameters from a configuration file
-    if args.config_file:
-        defaults = read_config_file(args.config_file, args.backend)
-    else:
-        defaults = {}
+def main():
+    _, PERCEVAL_CMDS = perceval.backend.find_backends(perceval.backends)
 
-    _, PERCEVAL_CMDS = perceval.find_backends(perceval.backends)
+    args = parse_args(PERCEVAL_CMDS)
 
     if args.backend not in PERCEVAL_CMDS:
         raise RuntimeError("Unknown backend %s" % args.backend)
-
     configure_logging(args.debug)
 
     logging.info("Sir Perceval is on his quest.")
-
     klass = PERCEVAL_CMDS[args.backend]
-    cmd = klass(*args.backend_args)
+    cmd = klass(*args.backend_args, debug=args.debug)
     cmd.run()
 
     logging.info("Sir Perceval completed his quest.")
 
 
-def parse_args():
+def parse_args(perceval_cmds):
     """Parse command line arguments"""
 
     parser = argparse.ArgumentParser(usage=PERCEVAL_USAGE_MSG,
                                      description=PERCEVAL_DESC_MSG,
                                      epilog=PERCEVAL_EPILOG_MSG,
                                      formatter_class=argparse.RawDescriptionHelpFormatter,
                                      add_help=False)
 
     parser.add_argument('-h', '--help', action='help',
                         help=argparse.SUPPRESS)
     parser.add_argument('-v', '--version', action='version',
                         version=PERCEVAL_VERSION_MSG,
                         help=argparse.SUPPRESS)
-    parser.add_argument('-c', '--config', dest='config_file',
-                        default=os.path.expanduser('~/.perceval/perceval.cfg'),
-                        help=argparse.SUPPRESS)
     parser.add_argument('-g', '--debug', dest='debug',
                         action='store_true',
                         help=argparse.SUPPRESS)
+    parser.add_argument('-l', '--list', backends=perceval_cmds, action=ListBackends,
+                        help=argparse.SUPPRESS)
 
     parser.add_argument('backend', help=argparse.SUPPRESS)
     parser.add_argument('backend_args', nargs=argparse.REMAINDER,
                         help=argparse.SUPPRESS)
 
     if len(sys.argv) == 1:
         parser.print_help()
         sys.exit(1)
 
     return parser.parse_args()
 
 
-def read_config_file(filepath, backend):
-    """Read a Perceval configuration file.
-
-    This function reads common and `backend` configuration parameters
-    from the given file.
-
-    :param filepath: path to the configuration file
-    :param backend: name of the backend which its parameters will be read
-
-    :returns: a configuration parameters dictionary
-    """
-    config = configparser.SafeConfigParser()
-    config.read(filepath)
-
-    args = {}
-    sections = ['cache', backend]
-
-    for section in sections:
-        if section in config.sections():
-            d = dict(config.items(section))
-            args.update(d)
-
-    return args
-
 def configure_logging(debug=False):
     """Configure Perceval logging
 
     The function configures the log messages produced by Perceval.
     By default, log messages are sent to stderr. Set the parameter
     `debug` to activate the debug mode.
```

### Comparing `perceval-0.9.9/README.md` & `perceval-1.0.0rc1/tests/data/dockerhub/dockerhub_repository_1.json`

 * *Files 25% similar despite different names*

```diff
@@ -1,523 +1,524 @@
-00000000: 2320 5065 7263 6576 616c 205b 215b 4275  # Perceval [![Bu
-00000010: 696c 6420 5374 6174 7573 5d28 6874 7470  ild Status](http
-00000020: 733a 2f2f 7472 6176 6973 2d63 692e 6f72  s://travis-ci.or
-00000030: 672f 6772 696d 6f69 7265 6c61 622f 7065  g/grimoirelab/pe
-00000040: 7263 6576 616c 2e73 7667 3f62 7261 6e63  rceval.svg?branc
-00000050: 683d 6d61 7374 6572 295d 2868 7474 7073  h=master)](https
-00000060: 3a2f 2f74 7261 7669 732d 6369 2e6f 7267  ://travis-ci.org
-00000070: 2f67 7269 6d6f 6972 656c 6162 2f70 6572  /grimoirelab/per
-00000080: 6365 7661 6c29 205b 215b 436f 7665 7261  ceval) [![Covera
-00000090: 6765 2053 7461 7475 735d 2868 7474 7073  ge Status](https
-000000a0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-000000b0: 6f2f 636f 7665 7261 6c6c 732f 6772 696d  o/coveralls/grim
-000000c0: 6f69 7265 6c61 622f 7065 7263 6576 616c  oirelab/perceval
-000000d0: 2e73 7667 295d 2868 7474 7073 3a2f 2f63  .svg)](https://c
-000000e0: 6f76 6572 616c 6c73 2e69 6f2f 722f 6772  overalls.io/r/gr
-000000f0: 696d 6f69 7265 6c61 622f 7065 7263 6576  imoirelab/percev
-00000100: 616c 3f62 7261 6e63 683d 6d61 7374 6572  al?branch=master
-00000110: 2920 5b21 5b50 7950 4920 7665 7273 696f  ) [![PyPI versio
-00000120: 6e5d 2868 7474 7073 3a2f 2f62 6164 6765  n](https://badge
-00000130: 2e66 7572 792e 696f 2f70 792f 7065 7263  .fury.io/py/perc
-00000140: 6576 616c 2e73 7667 295d 2868 7474 7073  eval.svg)](https
-00000150: 3a2f 2f62 6164 6765 2e66 7572 792e 696f  ://badge.fury.io
-00000160: 2f70 792f 7065 7263 6576 616c 290a 0a53  /py/perceval)..S
-00000170: 656e 6420 5369 7220 5065 7263 6576 616c  end Sir Perceval
-00000180: 206f 6e20 6120 7175 6573 7420 746f 2072   on a quest to r
-00000190: 6574 7269 6576 6520 616e 6420 6761 7468  etrieve and gath
-000001a0: 6572 2064 6174 6120 6672 6f6d 2073 6f66  er data from sof
-000001b0: 7477 6172 650a 7265 706f 7369 746f 7269  tware.repositori
-000001c0: 6573 2e0a 0a23 2320 5573 6167 650a 0a60  es...## Usage..`
-000001d0: 6060 0a75 7361 6765 3a20 7065 7263 6576  ``.usage: percev
-000001e0: 616c 205b 2d63 203c 6669 6c65 3e5d 205b  al [-c <file>] [
-000001f0: 2d67 5d20 3c62 6163 6b65 6e64 3e20 5b3c  -g] <backend> [<
-00000200: 6172 6773 3e5d 207c 202d 2d68 656c 7020  args>] | --help 
-00000210: 7c20 2d2d 7665 7273 696f 6e0a 0a52 6570  | --version..Rep
-00000220: 6f73 6974 6f72 6965 7320 6172 6520 7265  ositories are re
-00000230: 6163 6865 6420 7573 696e 6720 7370 6563  ached using spec
-00000240: 6966 6963 2062 6163 6b65 6e64 732e 2054  ific backends. T
-00000250: 6865 206d 6f73 7420 636f 6d6d 6f6e 2062  he most common b
-00000260: 6163 6b65 6e64 730a 6172 653a 0a20 2020  ackends.are:.   
-00000270: 2061 736b 626f 7420 2020 2020 2020 2020   askbot         
-00000280: 2020 4665 7463 6820 7175 6573 7469 6f6e    Fetch question
-00000290: 7320 616e 6420 616e 7377 6572 7320 6672  s and answers fr
-000002a0: 6f6d 2041 736b 626f 7420 7369 7465 0a20  om Askbot site. 
-000002b0: 2020 2062 7567 7a69 6c6c 6120 2020 2020     bugzilla     
-000002c0: 2020 2020 4665 7463 6820 6275 6773 2066      Fetch bugs f
-000002d0: 726f 6d20 6120 4275 677a 696c 6c61 2073  rom a Bugzilla s
-000002e0: 6572 7665 720a 2020 2020 6275 677a 696c  erver.    bugzil
-000002f0: 6c61 7265 7374 2020 2020 2046 6574 6368  larest     Fetch
-00000300: 2062 7567 7320 6672 6f6d 2061 2042 7567   bugs from a Bug
-00000310: 7a69 6c6c 6120 7365 7276 6572 2028 3e3d  zilla server (>=
-00000320: 352e 3029 2075 7369 6e67 2069 7473 2052  5.0) using its R
-00000330: 4553 5420 4150 490a 2020 2020 636f 6e66  EST API.    conf
-00000340: 6c75 656e 6365 2020 2020 2020 2046 6574  luence       Fet
-00000350: 6368 2063 6f6e 7465 6e74 7320 6672 6f6d  ch contents from
-00000360: 2061 2043 6f6e 666c 7565 6e63 6520 7365   a Confluence se
-00000370: 7276 6572 0a20 2020 2064 6973 636f 7572  rver.    discour
-00000380: 7365 2020 2020 2020 2020 4665 7463 6820  se        Fetch 
-00000390: 706f 7374 7320 6672 6f6d 2044 6973 636f  posts from Disco
-000003a0: 7572 7365 2073 6974 650a 2020 2020 646f  urse site.    do
-000003b0: 636b 6572 6875 6220 2020 2020 2020 2046  ckerhub        F
-000003c0: 6574 6368 2072 6570 6f73 6974 6f72 7920  etch repository 
-000003d0: 6461 7461 2066 726f 6d20 446f 636b 6572  data from Docker
-000003e0: 2048 7562 2073 6974 650a 2020 2020 6765   Hub site.    ge
-000003f0: 7272 6974 2020 2020 2020 2020 2020 2046  rrit           F
-00000400: 6574 6368 2072 6576 6965 7773 2066 726f  etch reviews fro
-00000410: 6d20 6120 4765 7272 6974 2073 6572 7665  m a Gerrit serve
-00000420: 720a 2020 2020 6769 7420 2020 2020 2020  r.    git       
-00000430: 2020 2020 2020 2046 6574 6368 2063 6f6d         Fetch com
-00000440: 6d69 7473 2066 726f 6d20 4769 740a 2020  mits from Git.  
-00000450: 2020 6769 7468 7562 2020 2020 2020 2020    github        
-00000460: 2020 2046 6574 6368 2069 7373 7565 7320     Fetch issues 
-00000470: 6672 6f6d 2047 6974 4875 620a 2020 2020  from GitHub.    
-00000480: 676d 616e 6520 2020 2020 2020 2020 2020  gmane           
-00000490: 2046 6574 6368 206d 6573 7361 6765 7320   Fetch messages 
-000004a0: 6672 6f6d 2047 6d61 6e65 0a20 2020 2068  from Gmane.    h
-000004b0: 7970 6572 6b69 7474 7920 2020 2020 2020  yperkitty       
-000004c0: 4665 7463 6820 6d65 7373 6167 6573 2066  Fetch messages f
-000004d0: 726f 6d20 6120 4879 7065 724b 6974 7479  rom a HyperKitty
-000004e0: 2061 7263 6869 7665 720a 2020 2020 6a65   archiver.    je
-000004f0: 6e6b 696e 7320 2020 2020 2020 2020 2046  nkins          F
-00000500: 6574 6368 2062 7569 6c64 7320 6672 6f6d  etch builds from
-00000510: 2061 204a 656e 6b69 6e73 2073 6572 7665   a Jenkins serve
-00000520: 720a 2020 2020 6a69 7261 2020 2020 2020  r.    jira      
-00000530: 2020 2020 2020 2046 6574 6368 2069 7373         Fetch iss
-00000540: 7565 7320 6672 6f6d 204a 4952 4120 6973  ues from JIRA is
-00000550: 7375 6520 7472 6163 6b65 720a 2020 2020  sue tracker.    
-00000560: 6c61 756e 6368 7061 6420 2020 2020 2020  launchpad       
-00000570: 2046 6574 6368 2069 7373 7565 7320 6672   Fetch issues fr
-00000580: 6f6d 204c 6175 6e63 6870 6164 2069 7373  om Launchpad iss
-00000590: 7565 2074 7261 636b 6572 0a20 2020 206d  ue tracker.    m
-000005a0: 626f 7820 2020 2020 2020 2020 2020 2020  box             
-000005b0: 4665 7463 6820 6d65 7373 6167 6573 2066  Fetch messages f
-000005c0: 726f 6d20 4d42 6f78 2066 696c 6573 0a20  rom MBox files. 
-000005d0: 2020 206d 6564 6961 7769 6b69 2020 2020     mediawiki    
-000005e0: 2020 2020 4665 7463 6820 7061 6765 7320      Fetch pages 
-000005f0: 616e 6420 7265 7669 7369 6f6e 7320 6672  and revisions fr
-00000600: 6f6d 2061 204d 6564 6961 5769 6b69 2073  om a MediaWiki s
-00000610: 6974 650a 2020 2020 6d65 6574 7570 2020  ite.    meetup  
-00000620: 2020 2020 2020 2020 2046 6574 6368 2065           Fetch e
-00000630: 7665 6e74 7320 6672 6f6d 2061 204d 6565  vents from a Mee
-00000640: 7475 7020 6772 6f75 700a 2020 2020 6e6e  tup group.    nn
-00000650: 7470 2020 2020 2020 2020 2020 2020 2046  tp             F
-00000660: 6574 6368 2061 7274 6963 6c65 7320 6672  etch articles fr
-00000670: 6f6d 2061 204e 4e54 5020 6e65 7773 2067  om a NNTP news g
-00000680: 726f 7570 0a20 2020 2070 6861 6272 6963  roup.    phabric
-00000690: 6174 6f72 2020 2020 2020 4665 7463 6820  ator      Fetch 
-000006a0: 7461 736b 7320 6672 6f6d 2061 2050 6861  tasks from a Pha
-000006b0: 6272 6963 6174 6f72 2073 6974 650a 2020  bricator site.  
-000006c0: 2020 7069 7065 726d 6169 6c20 2020 2020    pipermail     
-000006d0: 2020 2046 6574 6368 206d 6573 7361 6765     Fetch message
-000006e0: 7320 6672 6f6d 2061 2050 6970 6572 6d61  s from a Piperma
-000006f0: 696c 2061 7263 6869 7665 720a 2020 2020  il archiver.    
-00000700: 7265 646d 696e 6520 2020 2020 2020 2020  redmine         
-00000710: 2046 6574 6368 2069 7373 7565 7320 6672   Fetch issues fr
-00000720: 6f6d 2061 2052 6564 6d69 6e65 2073 6572  om a Redmine ser
-00000730: 7665 720a 2020 2020 7273 7320 2020 2020  ver.    rss     
-00000740: 2020 2020 2020 2020 2046 6574 6368 2065           Fetch e
-00000750: 6e74 7269 6573 2066 726f 6d20 6120 5253  ntries from a RS
-00000760: 5320 6665 6564 2073 6572 7665 720a 2020  S feed server.  
-00000770: 2020 736c 6163 6b20 2020 2020 2020 2020    slack         
-00000780: 2020 2046 6574 6368 206d 6573 7361 6765     Fetch message
-00000790: 7320 6672 6f6d 2061 2053 6c61 636b 2063  s from a Slack c
-000007a0: 6861 6e6e 656c 0a20 2020 2073 7461 636b  hannel.    stack
-000007b0: 6578 6368 616e 6765 2020 2020 4665 7463  exchange    Fetc
-000007c0: 6820 7175 6573 7469 6f6e 7320 6672 6f6d  h questions from
-000007d0: 2053 7461 636b 4578 6368 616e 6765 2073   StackExchange s
-000007e0: 6974 6573 0a20 2020 2073 7570 7962 6f74  ites.    supybot
-000007f0: 2020 2020 2020 2020 2020 4665 7463 6820            Fetch 
-00000800: 6d65 7373 6167 6573 2066 726f 6d20 5375  messages from Su
-00000810: 7079 626f 7420 6c6f 6720 6669 6c65 730a  pybot log files.
-00000820: 2020 2020 7465 6c65 6772 616d 2020 2020      telegram    
-00000830: 2020 2020 2046 6574 6368 206d 6573 7361       Fetch messa
-00000840: 6765 7320 6672 6f6d 2074 6865 2054 656c  ges from the Tel
-00000850: 6567 7261 6d20 7365 7276 6572 0a0a 6f70  egram server..op
-00000860: 7469 6f6e 616c 2061 7267 756d 656e 7473  tional arguments
-00000870: 3a0a 2020 2d68 2c20 2d2d 6865 6c70 2020  :.  -h, --help  
-00000880: 2020 2020 2020 2020 2020 7368 6f77 2074            show t
-00000890: 6869 7320 6865 6c70 206d 6573 7361 6765  his help message
-000008a0: 2061 6e64 2065 7869 740a 2020 2d76 2c20   and exit.  -v, 
-000008b0: 2d2d 7665 7273 696f 6e20 2020 2020 2020  --version       
-000008c0: 2020 7368 6f77 2076 6572 7369 6f6e 0a20    show version. 
-000008d0: 202d 6320 4649 4c45 2c20 2d2d 636f 6e66   -c FILE, --conf
-000008e0: 6967 2046 494c 450a 2020 2020 2020 2020  ig FILE.        
-000008f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000900: 7365 7420 636f 6e66 6967 7572 6174 696f  set configuratio
-00000910: 6e20 6669 6c65 0a20 202d 672c 202d 2d64  n file.  -g, --d
-00000920: 6562 7567 2020 2020 2020 2020 2020 2073  ebug           s
-00000930: 6574 2064 6562 7567 206d 6f64 6520 6f6e  et debug mode on
-00000940: 0a0a 5275 6e20 2770 6572 6365 7661 6c20  ..Run 'perceval 
-00000950: 3c62 6163 6b65 6e64 3e20 2d2d 6865 6c70  <backend> --help
-00000960: 2720 746f 2067 6574 2069 6e66 6f72 6d61  ' to get informa
-00000970: 7469 6f6e 2061 626f 7574 2061 2073 7065  tion about a spe
-00000980: 6369 6669 6320 6261 636b 656e 642e 0a60  cific backend..`
-00000990: 6060 0a0a 2323 2052 6571 7569 7265 6d65  ``..## Requireme
-000009a0: 6e74 730a 0a2a 2050 7974 686f 6e20 3e3d  nts..* Python >=
-000009b0: 2033 2e34 0a2a 2070 7974 686f 6e33 2d64   3.4.* python3-d
-000009c0: 6174 6575 7469 6c20 3e3d 2032 2e36 0a2a  ateutil >= 2.6.*
-000009d0: 2070 7974 686f 6e33 2d72 6571 7565 7374   python3-request
-000009e0: 7320 3e3d 2032 2e37 0a2a 2070 7974 686f  s >= 2.7.* pytho
-000009f0: 6e33 2d62 7334 2028 6265 6175 7469 6675  n3-bs4 (beautifu
-00000a00: 6c73 6f75 7034 2920 3e3d 2034 2e33 0a2a  lsoup4) >= 4.3.*
-00000a10: 2070 7974 686f 6e33 2d66 6565 6470 6172   python3-feedpar
-00000a20: 7365 7220 3e3d 2035 2e31 2e33 0a2a 2070  ser >= 5.1.3.* p
-00000a30: 7974 686f 6e33 2d64 756c 7769 6368 203e  ython3-dulwich >
-00000a40: 3d20 302e 3138 2e35 0a2a 2067 7269 6d6f  = 0.18.5.* grimo
-00000a50: 6972 656c 6162 2d74 6f6f 6c6b 6974 203e  irelab-toolkit >
-00000a60: 3d20 302e 312e 300a 0a23 2320 496e 7374  = 0.1.0..## Inst
-00000a70: 616c 6c61 7469 6f6e 0a0a 5468 6572 6520  allation..There 
-00000a80: 6172 6520 7365 7665 7261 6c20 7761 7973  are several ways
-00000a90: 2066 6f72 2069 6e73 7461 6c6c 696e 6720   for installing 
-00000aa0: 5065 7263 6576 616c 206f 6e20 796f 7572  Perceval on your
-00000ab0: 2073 7973 7465 6d3a 2066 726f 6d20 7061   system: from pa
-00000ac0: 636b 6167 6573 2c0a 6672 6f6d 2061 2064  ckages,.from a d
-00000ad0: 6f63 6b65 7220 696d 6167 6520 6f72 2066  ocker image or f
-00000ae0: 726f 6d20 7468 6520 736f 7572 6365 2063  rom the source c
-00000af0: 6f64 652e 0a0a 2323 2320 5069 700a 0a50  ode...### Pip..P
-00000b00: 6572 6365 7661 6c20 6361 6e20 6265 2069  erceval can be i
-00000b10: 6e73 7461 6c6c 6564 2075 7369 6e67 205b  nstalled using [
-00000b20: 7069 705d 2868 7474 7073 3a2f 2f70 6970  pip](https://pip
-00000b30: 2e70 7970 612e 696f 2f65 6e2f 7374 6162  .pypa.io/en/stab
-00000b40: 6c65 2f29 2c20 6120 746f 6f6c 0a66 6f72  le/), a tool.for
-00000b50: 2069 6e73 7461 6c6c 696e 6720 5079 7468   installing Pyth
-00000b60: 6f6e 2070 6163 6b61 6765 732e 2054 6f20  on packages. To 
-00000b70: 646f 2069 742c 2072 756e 2074 6865 206e  do it, run the n
-00000b80: 6578 7420 636f 6d6d 616e 643a 0a0a 6060  ext command:..``
-00000b90: 600a 2420 7069 7033 2069 6e73 7461 6c6c  `.$ pip3 install
-00000ba0: 2070 6572 6365 7661 6c0a 6060 600a 0a23   perceval.```..#
-00000bb0: 2323 2044 6f63 6b65 720a 0a41 2050 6572  ## Docker..A Per
-00000bc0: 6365 7661 6c20 446f 636b 6572 2069 6d61  ceval Docker ima
-00000bd0: 6765 2069 7320 6176 6169 6c61 626c 6520  ge is available 
-00000be0: 6174 205b 446f 636b 6572 4875 625d 2868  at [DockerHub](h
-00000bf0: 7474 7073 3a2f 2f68 7562 2e64 6f63 6b65  ttps://hub.docke
-00000c00: 722e 636f 6d2f 722f 6772 696d 6f69 7265  r.com/r/grimoire
-00000c10: 6c61 622f 7065 7263 6576 616c 2f29 2e0a  lab/perceval/)..
-00000c20: 0a44 6574 6169 6c65 6420 696e 666f 726d  .Detailed inform
-00000c30: 6174 696f 6e20 6f6e 2068 6f77 2074 6f20  ation on how to 
-00000c40: 7275 6e20 616e 642f 6f72 2062 7569 6c64  run and/or build
-00000c50: 2074 6869 7320 696d 6167 6520 6361 6e20   this image can 
-00000c60: 6265 2066 6f75 6e64 205b 6865 7265 5d28  be found [here](
-00000c70: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000c80: 6f6d 2f67 7269 6d6f 6972 656c 6162 2f70  om/grimoirelab/p
-00000c90: 6572 6365 7661 6c2f 7472 6565 2f6d 6173  erceval/tree/mas
-00000ca0: 7465 722f 646f 636b 6572 2f69 6d61 6765  ter/docker/image
-00000cb0: 732f 292e 0a0a 2323 2320 536f 7572 6365  s/)...### Source
-00000cc0: 2063 6f64 650a 0a54 6f20 696e 7374 616c   code..To instal
-00000cd0: 6c20 6672 6f6d 2074 6865 2073 6f75 7263  l from the sourc
-00000ce0: 6520 636f 6465 2079 6f75 2077 696c 6c20  e code you will 
-00000cf0: 6e65 6564 2074 6f20 636c 6f6e 6520 7468  need to clone th
-00000d00: 6520 7265 706f 7369 746f 7279 2066 6972  e repository fir
-00000d10: 7374 3a0a 0a60 6060 0a24 2067 6974 2063  st:..```.$ git c
-00000d20: 6c6f 6e65 2068 7474 7073 3a2f 2f67 6974  lone https://git
-00000d30: 6875 622e 636f 6d2f 6772 696d 6f69 7265  hub.com/grimoire
-00000d40: 6c61 622f 7065 7263 6576 616c 2e67 6974  lab/perceval.git
-00000d50: 0a60 6060 0a0a 496e 2074 6869 7320 6361  .```..In this ca
-00000d60: 7365 2c20 5b73 6574 7570 746f 6f6c 735d  se, [setuptools]
-00000d70: 2868 7474 703a 2f2f 7365 7475 7074 6f6f  (http://setuptoo
-00000d80: 6c73 2e72 6561 6474 6865 646f 6373 2e69  ls.readthedocs.i
-00000d90: 6f2f 656e 2f6c 6174 6573 742f 2920 7061  o/en/latest/) pa
-00000da0: 636b 6167 6520 7769 6c6c 2062 6520 7265  ckage will be re
-00000db0: 7175 6972 6564 2e0a 4d61 6b65 2073 7572  quired..Make sur
-00000dc0: 6520 6974 2069 7320 696e 7374 616c 6c65  e it is installe
-00000dd0: 6420 6265 666f 7265 2072 756e 6e69 6e67  d before running
-00000de0: 2074 6865 206e 6578 7420 636f 6d6d 616e   the next comman
-00000df0: 6473 3a0a 0a60 6060 0a24 2070 6970 3320  ds:..```.$ pip3 
-00000e00: 696e 7374 616c 6c20 2d72 2072 6571 7569  install -r requi
-00000e10: 7265 6d65 6e74 732e 7478 740a 2420 7079  rements.txt.$ py
-00000e20: 7468 6f6e 3320 7365 7475 702e 7079 2069  thon3 setup.py i
-00000e30: 6e73 7461 6c6c 0a60 6060 0a0a 2323 2044  nstall.```..## D
-00000e40: 6f63 756d 656e 7461 7469 6f6e 0a0a 446f  ocumentation..Do
-00000e50: 6375 6d65 6e74 6174 696f 6e20 6973 2067  cumentation is g
-00000e60: 656e 6572 6174 6564 2061 7574 6f6d 6167  enerated automag
-00000e70: 6963 616c 6c79 2069 6e20 7468 6520 5b52  ically in the [R
-00000e80: 6561 6454 6865 446f 6373 2050 6572 6365  eadTheDocs Perce
-00000e90: 7661 6c20 7369 7465 5d28 6874 7470 3a2f  val site](http:/
-00000ea0: 2f70 6572 6365 7661 6c2e 7265 6164 7468  /perceval.readth
-00000eb0: 6564 6f63 732e 6f72 672f 292e 0a0a 2323  edocs.org/)...##
-00000ec0: 2045 7861 6d70 6c65 730a 0a23 2323 2041   Examples..### A
-00000ed0: 736b 626f 740a 6060 600a 2420 7065 7263  skbot.```.$ perc
-00000ee0: 6576 616c 2061 736b 626f 7420 2768 7474  eval askbot 'htt
-00000ef0: 703a 2f2f 6173 6b62 6f74 2e6f 7267 2f27  p://askbot.org/'
-00000f00: 202d 2d66 726f 6d2d 6461 7465 2027 3230   --from-date '20
-00000f10: 3136 2d30 312d 3031 270a 6060 600a 0a23  16-01-01'.```..#
-00000f20: 2323 2042 7567 7a69 6c6c 610a 546f 2066  ## Bugzilla.To f
-00000f30: 6574 6368 2062 7567 7320 6672 6f6d 2042  etch bugs from B
-00000f40: 7567 7a69 6c6c 612c 2079 6f75 2068 6176  ugzilla, you hav
-00000f50: 6520 7477 6f20 6f70 7469 6f6e 733a 0a0a  e two options:..
-00000f60: 6129 2055 7365 2074 6865 2074 7261 6469  a) Use the tradi
-00000f70: 7469 6f6e 616c 2062 6163 6b65 6e64 0a0a  tional backend..
-00000f80: 6060 600a 2420 7065 7263 6576 616c 2062  ```.$ perceval b
-00000f90: 7567 7a69 6c6c 6120 2768 7474 7073 3a2f  ugzilla 'https:/
-00000fa0: 2f62 7567 7a69 6c6c 612e 7265 6468 6174  /bugzilla.redhat
-00000fb0: 2e63 6f6d 2f27 202d 2d62 6163 6b65 6e64  .com/' --backend
-00000fc0: 2d75 7365 7220 7573 6572 202d 2d62 6163  -user user --bac
-00000fd0: 6b65 6e64 2d70 6173 7377 6f72 6420 7061  kend-password pa
-00000fe0: 7373 202d 2d66 726f 6d2d 6461 7465 2027  ss --from-date '
-00000ff0: 3230 3136 2d30 312d 3031 270a 6060 600a  2016-01-01'.```.
-00001000: 0a62 2920 5573 6520 7468 6520 5245 5354  .b) Use the REST
-00001010: 2041 5049 2062 6163 6b65 6e64 2066 6f72   API backend for
-00001020: 2042 757a 696c 6c61 2035 2e30 2028 6f72   Buzilla 5.0 (or
-00001030: 2068 6967 6865 7229 2073 6572 7665 7273   higher) servers
-00001040: 2e20 5765 2073 7472 6f6e 676c 7920 7265  . We strongly re
-00001050: 636f 6d6d 656e 640a 7468 6973 2062 6163  commend.this bac
-00001060: 6b65 6e64 2077 6865 6e20 6461 7461 2069  kend when data i
-00001070: 7320 6665 7463 6865 6420 6672 6f6d 2076  s fetched from v
-00001080: 6572 7369 6f6e 2073 6572 7665 7273 203e  ersion servers >
-00001090: 3d35 2e30 2062 6563 6175 7365 2074 6865  =5.0 because the
-000010a0: 2072 6574 7269 6576 616c 0a70 726f 6365   retrieval.proce
-000010b0: 7373 2069 7320 6d75 6368 2066 6173 7465  ss is much faste
-000010c0: 722e 0a0a 6060 600a 2420 7065 7263 6576  r...```.$ percev
-000010d0: 616c 2062 7567 7a69 6c6c 6172 6573 7420  al bugzillarest 
-000010e0: 2768 7474 7073 3a2f 2f62 7567 7a69 6c6c  'https://bugzill
-000010f0: 612e 6d6f 7a69 6c6c 612e 6f72 672f 2720  a.mozilla.org/' 
-00001100: 2d2d 6261 636b 656e 642d 7573 6572 2075  --backend-user u
-00001110: 7365 7220 2d2d 6261 636b 656e 642d 7061  ser --backend-pa
-00001120: 7373 776f 7264 2070 6173 7320 2d2d 6672  ssword pass --fr
-00001130: 6f6d 2d64 6174 6520 2732 3031 362d 3031  om-date '2016-01
-00001140: 2d30 3127 0a60 6060 0a0a 2323 2320 436f  -01'.```..### Co
-00001150: 6e66 6c75 656e 6365 0a60 6060 0a24 2070  nfluence.```.$ p
-00001160: 6572 6365 7661 6c20 636f 6e66 6c75 656e  erceval confluen
-00001170: 6365 2027 6874 7470 733a 2f2f 7769 6b69  ce 'https://wiki
-00001180: 2e6f 706e 6676 2e6f 7267 2f27 202d 2d66  .opnfv.org/' --f
-00001190: 726f 6d2d 6461 7465 2027 3230 3136 2d30  rom-date '2016-0
-000011a0: 312d 3031 270a 6060 600a 0a23 2323 2044  1-01'.```..### D
-000011b0: 6973 636f 7572 7365 0a60 6060 0a24 2070  iscourse.```.$ p
-000011c0: 6572 6365 7661 6c20 6469 7363 6f75 7273  erceval discours
-000011d0: 6520 2768 7474 7073 3a2f 2f66 6f72 6f2e  e 'https://foro.
-000011e0: 6d6f 7a69 6c6c 612d 6869 7370 616e 6f2e  mozilla-hispano.
-000011f0: 6f72 672f 2720 2d2d 6672 6f6d 2d64 6174  org/' --from-dat
-00001200: 6520 2732 3031 362d 3031 2d30 3127 0a60  e '2016-01-01'.`
-00001210: 6060 0a0a 2323 2320 446f 636b 6572 2048  ``..### Docker H
-00001220: 7562 0a60 6060 0a24 2070 6572 6365 7661  ub.```.$ perceva
-00001230: 6c20 646f 636b 6572 6875 6220 6772 696d  l dockerhub grim
-00001240: 6f69 7265 6c61 6220 7065 7263 6576 616c  oirelab perceval
-00001250: 0a60 6060 0a0a 2323 2320 4765 7272 6974  .```..### Gerrit
-00001260: 0a54 6f20 7275 6e20 6765 7272 6974 2c20  .To run gerrit, 
-00001270: 796f 7520 7769 6c6c 206e 6565 6420 616e  you will need an
-00001280: 2061 7574 686f 7269 7a65 6420 5353 4820   authorized SSH 
-00001290: 7072 6976 6174 6520 6b65 793a 0a0a 6060  private key:..``
-000012a0: 600a 2420 6576 616c 2060 7373 682d 6167  `.$ eval `ssh-ag
-000012b0: 656e 7420 2d73 600a 2420 7373 682d 6164  ent -s`.$ ssh-ad
-000012c0: 6420 7e2f 2e73 7368 2f69 645f 7273 610a  d ~/.ssh/id_rsa.
-000012d0: 4964 656e 7469 7479 2061 6464 6564 3a20  Identity added: 
-000012e0: 2f68 6f6d 652f 7573 6572 2f2e 7373 682f  /home/user/.ssh/
-000012f0: 6964 5f72 7361 2028 2f68 6f6d 652f 7573  id_rsa (/home/us
-00001300: 6572 2f2e 7373 682f 6964 5f72 7361 290a  er/.ssh/id_rsa).
-00001310: 6060 600a 0a54 6f20 7275 6e20 7468 6520  ```..To run the 
-00001320: 6261 636b 656e 642c 2065 7865 6375 7465  backend, execute
-00001330: 2074 6865 206e 6578 7420 636f 6d6d 616e   the next comman
-00001340: 643a 0a0a 6060 600a 2420 7065 7263 6576  d:..```.$ percev
-00001350: 616c 2067 6572 7269 7420 2d2d 7573 6572  al gerrit --user
-00001360: 2075 7365 7220 2772 6576 6965 772e 6f70   user 'review.op
-00001370: 656e 7374 6163 6b2e 6f72 6727 202d 2d66  enstack.org' --f
-00001380: 726f 6d2d 6461 7465 2027 3230 3136 2d30  rom-date '2016-0
-00001390: 312d 3031 270a 6060 600a 0a23 2323 2047  1-01'.```..### G
-000013a0: 6974 0a0a 546f 2072 756e 2074 6869 7320  it..To run this 
-000013b0: 6261 636b 656e 6420 6578 6563 7574 6520  backend execute 
-000013c0: 7468 6520 6e65 7874 2063 6f6d 6d61 6e64  the next command
-000013d0: 2e20 5461 6b65 2069 6e74 6f20 6163 636f  . Take into acco
-000013e0: 756e 7420 7468 6174 2074 6f20 7275 6e0a  unt that to run.
-000013f0: 7468 6973 2062 6163 6b65 6e64 2047 6974  this backend Git
-00001400: 2070 726f 6772 616d 2068 6173 2074 6f20   program has to 
-00001410: 6265 2069 6e73 7461 6c6c 6564 206f 6e20  be installed on 
-00001420: 796f 7572 2073 7973 7465 6d2e 0a0a 6060  your system...``
-00001430: 600a 2420 7065 7263 6576 616c 2067 6974  `.$ perceval git
-00001440: 2027 6874 7470 733a 2f2f 6769 7468 7562   'https://github
-00001450: 2e63 6f6d 2f67 7269 6d6f 6972 656c 6162  .com/grimoirelab
-00001460: 2f70 6572 6365 7661 6c2e 6769 7427 202d  /perceval.git' -
-00001470: 2d66 726f 6d2d 6461 7465 2027 3230 3136  -from-date '2016
-00001480: 2d30 312d 3031 270a 6060 600a 0a47 6974  -01-01'.```..Git
-00001490: 2062 6163 6b65 6e64 2063 616e 2061 6c73   backend can als
-000014a0: 6f20 776f 726b 2077 6974 6820 6120 4769  o work with a Gi
-000014b0: 7420 6c6f 6720 6669 6c65 2061 7320 696e  t log file as in
-000014c0: 7075 742e 2057 6520 7265 636f 6d6d 656e  put. We recommen
-000014d0: 6420 746f 2075 7365 2074 6865 206e 6578  d to use the nex
-000014e0: 7420 636f 6d6d 616e 6420 746f 2067 6574  t command to get
-000014f0: 2074 6865 206d 6f73 7420 636f 6d70 6c65   the most comple
-00001500: 7465 206c 6f67 2066 696c 652e 0a0a 6060  te log file...``
-00001510: 600a 6769 7420 6c6f 6720 2d2d 7261 7720  `.git log --raw 
-00001520: 2d2d 6e75 6d73 7461 7420 2d2d 7072 6574  --numstat --pret
-00001530: 7479 3d66 756c 6c65 7220 2d2d 6465 636f  ty=fuller --deco
-00001540: 7261 7465 3d66 756c 6c20 2d2d 7061 7265  rate=full --pare
-00001550: 6e74 7320 2d2d 7265 7665 7273 6520 2d2d  nts --reverse --
-00001560: 746f 706f 2d6f 7264 6572 202d 4d20 2d43  topo-order -M -C
-00001570: 202d 6320 2d2d 7265 6d6f 7465 733d 6f72   -c --remotes=or
-00001580: 6967 696e 202d 2d61 6c6c 203e 202f 746d  igin --all > /tm
-00001590: 702f 6769 746c 6f67 2e6c 6f67 0a60 6060  p/gitlog.log.```
-000015a0: 0a0a 5468 656e 2c20 746f 2072 756e 2074  ..Then, to run t
-000015b0: 6865 2062 6163 6b65 6e64 2c20 6a75 7374  he backend, just
-000015c0: 2065 7865 6375 7465 2061 6e79 206f 6620   execute any of 
-000015d0: 7468 6520 6e65 7874 2063 6f6d 6d61 6e64  the next command
-000015e0: 733a 0a0a 6060 600a 2420 7065 7263 6576  s:..```.$ percev
-000015f0: 616c 2067 6974 202d 2d67 6974 2d6c 6f67  al git --git-log
-00001600: 2027 2f74 6d70 2f67 6974 6c6f 672e 6c6f   '/tmp/gitlog.lo
-00001610: 6727 2027 6669 6c65 3a2f 2f2f 6d79 7265  g' 'file:///myre
-00001620: 706f 2e67 6974 270a 6060 600a 0a6f 720a  po.git'.```..or.
-00001630: 0a60 6060 0a24 2070 6572 6365 7661 6c20  .```.$ perceval 
-00001640: 6769 7420 272f 746d 702f 6769 746c 6f67  git '/tmp/gitlog
-00001650: 2e6c 6f67 270a 6060 600a 0a23 2323 2047  .log'.```..### G
-00001660: 6974 4875 620a 6060 600a 2420 7065 7263  itHub.```.$ perc
-00001670: 6576 616c 2067 6974 6875 6220 656c 6173  eval github elas
-00001680: 7469 6320 6c6f 6773 7461 7368 202d 2d66  tic logstash --f
-00001690: 726f 6d2d 6461 7465 2027 3230 3136 2d30  rom-date '2016-0
-000016a0: 312d 3031 270a 6060 600a 0a23 2323 2047  1-01'.```..### G
-000016b0: 6d61 6e65 0a60 6060 0a24 2070 6572 6365  mane.```.$ perce
-000016c0: 7661 6c20 676d 616e 6520 2d2d 6f66 6673  val gmane --offs
-000016d0: 6574 2032 3030 3020 2765 7669 6e63 652d  et 2000 'evince-
-000016e0: 6c69 7374 4067 6e6f 6d65 2e6f 7267 270a  list@gnome.org'.
-000016f0: 6060 600a 0a23 2323 2048 7970 6572 4b69  ```..### HyperKi
-00001700: 7474 790a 6060 600a 2420 7065 7263 6576  tty.```.$ percev
-00001710: 616c 2068 7970 6572 6b69 7474 7920 2768  al hyperkitty 'h
-00001720: 7474 7073 3a2f 2f6c 6973 7473 2e6d 6169  ttps://lists.mai
-00001730: 6c6d 616e 332e 6f72 672f 6172 6368 6976  lman3.org/archiv
-00001740: 6573 2f6c 6973 742f 6d61 696c 6d61 6e2d  es/list/mailman-
-00001750: 7573 6572 7340 6d61 696c 6d61 6e33 2e6f  users@mailman3.o
-00001760: 7267 2720 2d2d 6672 6f6d 2d64 6174 6520  rg' --from-date 
-00001770: 3230 3137 2d30 312d 3031 0a60 6060 0a0a  2017-01-01.```..
-00001780: 2323 2320 4a65 6e6b 696e 730a 6060 600a  ### Jenkins.```.
-00001790: 2420 7065 7263 6576 616c 206a 656e 6b69  $ perceval jenki
-000017a0: 6e73 2027 6874 7470 3a2f 2f6a 656e 6b69  ns 'http://jenki
-000017b0: 6e73 2e63 7961 6e6f 6765 6e6d 6f64 2e6f  ns.cyanogenmod.o
-000017c0: 7267 2f27 0a60 6060 0a0a 2323 2320 4a49  rg/'.```..### JI
-000017d0: 5241 0a60 6060 0a24 2070 6572 6365 7661  RA.```.$ perceva
-000017e0: 6c20 6a69 7261 2027 6874 7470 733a 2f2f  l jira 'https://
-000017f0: 7469 636b 6574 732e 7075 7070 6574 6c61  tickets.puppetla
-00001800: 6273 2e63 6f6d 2720 2d2d 7072 6f6a 6563  bs.com' --projec
-00001810: 7420 5055 5020 2d2d 6672 6f6d 2d64 6174  t PUP --from-dat
-00001820: 6520 2732 3031 362d 3031 2d30 3127 0a60  e '2016-01-01'.`
-00001830: 6060 0a0a 2323 2320 4c61 756e 6368 7061  ``..### Launchpa
-00001840: 640a 6060 600a 2420 7065 7263 6576 616c  d.```.$ perceval
-00001850: 206c 6175 6e63 6870 6164 2075 6275 6e74   launchpad ubunt
-00001860: 7520 2d2d 6672 6f6d 2d64 6174 6520 2732  u --from-date '2
-00001870: 3031 362d 3031 2d30 3127 0a60 6060 0a0a  016-01-01'.```..
-00001880: 2323 2320 4d42 6f78 0a60 6060 0a24 2070  ### MBox.```.$ p
-00001890: 6572 6365 7661 6c20 6d62 6f78 2027 6874  erceval mbox 'ht
-000018a0: 7470 3a2f 2f65 7861 6d70 6c65 2e63 6f6d  tp://example.com
-000018b0: 2720 2f74 6d70 2f6d 626f 7865 732f 0a60  ' /tmp/mboxes/.`
-000018c0: 6060 0a0a 2323 2320 4d65 6469 6157 696b  ``..### MediaWik
-000018d0: 690a 6060 600a 2420 7065 7263 6576 616c  i.```.$ perceval
-000018e0: 206d 6564 6961 7769 6b69 2027 6874 7470   mediawiki 'http
-000018f0: 733a 2f2f 7769 6b69 2e6d 6f7a 696c 6c61  s://wiki.mozilla
-00001900: 2e6f 7267 2720 2d2d 6672 6f6d 2d64 6174  .org' --from-dat
-00001910: 6520 2732 3031 362d 3036 2d33 3027 0a60  e '2016-06-30'.`
-00001920: 6060 0a0a 2323 2320 4d65 6574 7570 0a60  ``..### Meetup.`
-00001930: 6060 0a24 2070 6572 6365 7661 6c20 6d65  ``.$ perceval me
-00001940: 6574 7570 2027 536f 6674 7761 7265 2d44  etup 'Software-D
-00001950: 6576 656c 6f70 6d65 6e74 2d41 6e61 6c79  evelopment-Analy
-00001960: 7469 6373 2720 2d2d 6672 6f6d 2d64 6174  tics' --from-dat
-00001970: 6520 2732 3031 362d 3036 2d30 3127 202d  e '2016-06-01' -
-00001980: 7420 6162 6364 6566 6768 696a 6b0a 6060  t abcdefghijk.``
-00001990: 600a 0a23 2323 204e 4e54 500a 6060 600a  `..### NNTP.```.
-000019a0: 2420 7065 7263 6576 616c 206e 6e74 7020  $ perceval nntp 
-000019b0: 276e 6577 732e 6d6f 7a69 6c6c 612e 6f72  'news.mozilla.or
-000019c0: 6727 2027 6d6f 7a69 6c6c 612e 6465 762e  g' 'mozilla.dev.
-000019d0: 7072 6f6a 6563 742d 6c69 6e6b 2720 2d2d  project-link' --
-000019e0: 6f66 6673 6574 2031 300a 6060 600a 0a23  offset 10.```..#
-000019f0: 2323 2050 6861 6272 6963 6174 6f72 0a60  ## Phabricator.`
-00001a00: 6060 0a24 2070 6572 6365 7661 6c20 7068  ``.$ perceval ph
-00001a10: 6162 7269 6361 746f 7220 2768 7474 7073  abricator 'https
-00001a20: 3a2f 2f73 6563 7572 652e 7068 6162 7269  ://secure.phabri
-00001a30: 6361 746f 722e 636f 6d2f 2720 2d74 2031  cator.com/' -t 1
-00001a40: 3233 3435 3637 3839 6162 6365 6665 0a60  23456789abcefe.`
-00001a50: 6060 0a0a 2323 2320 5069 7065 726d 6169  ``..### Pipermai
-00001a60: 6c0a 6060 600a 2420 7065 7263 6576 616c  l.```.$ perceval
-00001a70: 2070 6970 6572 6d61 696c 2027 6874 7470   pipermail 'http
-00001a80: 733a 2f2f 6d61 696c 2e67 6e6f 6d65 2e6f  s://mail.gnome.o
-00001a90: 7267 2f61 7263 6869 7665 732f 6c69 6261  rg/archives/liba
-00001aa0: 7274 2d68 6163 6b65 7273 2f27 0a60 6060  rt-hackers/'.```
-00001ab0: 0a0a 5069 7065 726d 6169 6c20 616c 736f  ..Pipermail also
-00001ac0: 2069 7320 6162 6c65 2074 6f20 6665 7463   is able to fetc
-00001ad0: 6820 6461 7461 2066 726f 6d20 4170 6163  h data from Apac
-00001ae0: 6865 2773 2060 6d6f 645f 626f 7860 2069  he's `mod_box` i
-00001af0: 6e74 6572 6661 6365 3a0a 6060 600a 2420  nterface:.```.$ 
-00001b00: 7065 7263 6576 616c 2070 6970 6572 6d61  perceval piperma
-00001b10: 696c 2027 6874 7470 3a2f 2f6d 6169 6c2d  il 'http://mail-
-00001b20: 6172 6368 6976 6573 2e61 7061 6368 652e  archives.apache.
-00001b30: 6f72 672f 6d6f 645f 6d62 6f78 2f68 7474  org/mod_mbox/htt
-00001b40: 7064 2d64 6576 2f27 0a60 6060 0a0a 2323  pd-dev/'.```..##
-00001b50: 2320 5265 646d 696e 650a 6060 600a 2420  # Redmine.```.$ 
-00001b60: 7065 7263 6576 616c 2072 6564 6d69 6e65  perceval redmine
-00001b70: 2027 6874 7470 733a 2f2f 7777 772e 7265   'https://www.re
-00001b80: 646d 696e 652e 6f72 672f 2720 2d2d 6672  dmine.org/' --fr
-00001b90: 6f6d 2d64 6174 6520 2732 3031 362d 3031  om-date '2016-01
-00001ba0: 2d30 3127 202d 7420 6162 6364 6566 6768  -01' -t abcdefgh
-00001bb0: 696a 6b0a 6060 600a 0a23 2323 2052 5353  ijk.```..### RSS
-00001bc0: 0a60 6060 0a24 2070 6572 6365 7661 6c20  .```.$ perceval 
-00001bd0: 7273 7320 2768 7474 7073 3a2f 2f62 6c6f  rss 'https://blo
-00001be0: 672e 6269 7465 7267 6961 2e63 6f6d 2f66  g.bitergia.com/f
-00001bf0: 6565 642f 270a 6060 600a 0a23 2323 2053  eed/'.```..### S
-00001c00: 6c61 636b 0a60 6060 0a24 2070 6572 6365  lack.```.$ perce
-00001c10: 7661 6c20 736c 6163 6b20 4330 3030 3120  val slack C0001 
-00001c20: 2d2d 6672 6f6d 2d64 6174 6520 3230 3136  --from-date 2016
-00001c30: 2d30 312d 3132 202d 7420 6162 6365 6465  -01-12 -t abcede
-00001c40: 6667 6869 6a6b 0a60 6060 0a0a 2323 2320  fghijk.```..### 
-00001c50: 5374 6163 6b45 7863 6861 6e67 650a 6060  StackExchange.``
-00001c60: 600a 2420 7065 7263 6576 616c 2073 7461  `.$ perceval sta
-00001c70: 636b 6578 6368 616e 6765 202d 2d73 6974  ckexchange --sit
-00001c80: 6520 7374 6163 6b6f 7665 7266 6c6f 7720  e stackoverflow 
-00001c90: 2d2d 7461 6767 6564 2070 7974 686f 6e20  --tagged python 
-00001ca0: 2d2d 6672 6f6d 2d64 6174 6520 2732 3031  --from-date '201
-00001cb0: 362d 3031 2d30 3127 202d 2d74 6f6b 656e  6-01-01' --token
-00001cc0: 2061 6263 6461 6263 6461 6263 6461 6263   abcdabcdabcdabc
-00001cd0: 640a 6060 600a 0a23 2323 2053 7570 7962  d.```..### Supyb
-00001ce0: 6f74 0a60 6060 0a24 2070 6572 6365 7661  ot.```.$ perceva
-00001cf0: 6c20 7375 7079 626f 7420 2768 7474 703a  l supybot 'http:
-00001d00: 2f2f 6368 616e 6e65 6c2e 6578 616d 706c  //channel.exampl
-00001d10: 652e 636f 6d27 202f 746d 702f 7375 7079  e.com' /tmp/supy
-00001d20: 626f 742f 0a60 6060 0a0a 2323 2320 5465  bot/.```..### Te
-00001d30: 6c65 6772 616d 0a0a 5465 6c65 6772 616d  legram..Telegram
-00001d40: 2062 6163 6b65 6e64 206e 6565 6473 2061   backend needs a
-00001d50: 6e20 4150 4920 746f 6b65 6e20 746f 2061  n API token to a
-00001d60: 7574 6865 6e74 6963 6174 6520 7468 6520  uthenticate the 
-00001d70: 626f 742e 2049 6e20 6164 6469 7469 6f6e  bot. In addition
-00001d80: 2061 6e64 0a69 6e20 6f72 6465 7220 746f   and.in order to
-00001d90: 2066 6574 6368 206d 6573 7361 6765 7320   fetch messages 
-00001da0: 6672 6f6d 2061 2067 726f 7570 206f 7220  from a group or 
-00001db0: 6368 616e 6e65 6c2c 2070 7269 7661 6379  channel, privacy
-00001dc0: 2073 6574 7469 6e67 7320 6d75 7374 2062   settings must b
-00001dd0: 650a 6469 7361 626c 6564 2e20 546f 206b  e.disabled. To k
-00001de0: 6e6f 7720 686f 7720 746f 2063 7265 6174  now how to creat
-00001df0: 6520 6120 626f 742c 2074 6f20 6f62 7461  e a bot, to obta
-00001e00: 696e 2069 7473 2074 6f6b 656e 2061 6e64  in its token and
-00001e10: 2074 6f20 636f 6e66 6967 7572 6520 6974   to configure it
-00001e20: 0a70 6c65 6173 6520 7265 6164 2074 6865  .please read the
-00001e30: 205b 5465 6c65 6772 616d 2042 6f74 7320   [Telegram Bots 
-00001e40: 646f 6373 2070 6167 6573 5d28 6874 7470  docs pages](http
-00001e50: 733a 2f2f 636f 7265 2e74 656c 6567 7261  s://core.telegra
-00001e60: 6d2e 6f72 672f 626f 7473 292e 0a0a 6060  m.org/bots)...``
-00001e70: 600a 2420 7065 7263 6576 616c 2074 656c  `.$ perceval tel
-00001e80: 6567 7261 6d20 6d79 626f 7420 2d74 2031  egram mybot -t 1
-00001e90: 3233 3435 3637 3861 6263 6465 6667 6820  2345678abcdefgh 
-00001ea0: 2d2d 6368 6174 7320 3120 3220 2d31 300a  --chats 1 2 -10.
-00001eb0: 6060 600a 0a23 2320 5275 6e6e 696e 6720  ```..## Running 
-00001ec0: 7465 7374 730a 0a50 6572 6365 7661 6c20  tests..Perceval 
-00001ed0: 636f 6d65 7320 7769 7468 2061 2063 6f6d  comes with a com
-00001ee0: 7072 6568 656e 7369 7665 206c 6973 7420  prehensive list 
-00001ef0: 6f66 2075 6e69 7420 7465 7374 732e 0a54  of unit tests..T
-00001f00: 6f20 7275 6e20 7468 656d 2c20 696e 2061  o run them, in a
-00001f10: 6464 6974 696f 6e20 746f 2074 6865 2064  ddition to the d
-00001f20: 6570 656e 6465 6e63 6965 7320 696e 7374  ependencies inst
-00001f30: 616c 6c65 6420 7769 7468 2050 6572 6365  alled with Perce
-00001f40: 7661 6c2c 0a79 6f75 206e 6565 6420 7665  val,.you need ve
-00001f50: 7273 696f 6e20 302e 382e 3620 6f66 2020  rsion 0.8.6 of  
-00001f60: 6068 7474 7072 6574 7479 602e 0a43 7572  `httpretty`..Cur
-00001f70: 7265 6e74 6c79 2c20 6c61 7465 7374 2076  rently, latest v
-00001f80: 6572 7369 6f6e 2069 6e20 7079 7069 2069  ersion in pypi i
-00001f90: 7320 302e 382e 3134 2c0a 7768 6963 6820  s 0.8.14,.which 
-00001fa0: 7365 656d 7320 746f 2068 6176 6520 6120  seems to have a 
-00001fb0: 6275 6720 6578 706f 7365 6420 6279 2073  bug exposed by s
-00001fc0: 6f6d 6520 5065 7263 6576 616c 2074 6573  ome Perceval tes
-00001fd0: 7473 2e0a 536f 2c20 656e 7375 7265 2079  ts..So, ensure y
-00001fe0: 6f75 2069 6e73 7461 6c6c 2030 2e38 2e36  ou install 0.8.6
-00001ff0: 2c20 7768 6963 6820 6973 206b 6e6f 776e  , which is known
-00002000: 2074 6f20 776f 726b 2077 6974 6820 7468   to work with th
-00002010: 656d 3a0a 0a60 6060 0a24 2070 6970 2069  em:..```.$ pip i
-00002020: 6e73 7461 6c6c 2068 7474 7072 6574 7479  nstall httpretty
-00002030: 3d3d 302e 382e 360a 2420 6364 2074 6573  ==0.8.6.$ cd tes
-00002040: 7473 0a24 2070 7974 686f 6e33 2072 756e  ts.$ python3 run
-00002050: 5f74 6573 7473 2e70 790a 6060 600a 0a23  _tests.py.```..#
-00002060: 2320 4c69 6365 6e73 650a 0a4c 6963 656e  # License..Licen
-00002070: 7365 6420 756e 6465 7220 474e 5520 4765  sed under GNU Ge
-00002080: 6e65 7261 6c20 5075 626c 6963 204c 6963  neral Public Lic
-00002090: 656e 7365 2028 4750 4c29 2c20 7665 7273  ense (GPL), vers
-000020a0: 696f 6e20 3320 6f72 206c 6174 6572 2e0a  ion 3 or later..
+00000000: 7b0a 2020 2020 2275 7365 7222 3a20 2267  {.    "user": "g
+00000010: 7269 6d6f 6972 656c 6162 222c 0a20 2020  rimoirelab",.   
+00000020: 2022 6e61 6d65 223a 2022 7065 7263 6576   "name": "percev
+00000030: 616c 222c 0a20 2020 2022 6e61 6d65 7370  al",.    "namesp
+00000040: 6163 6522 3a20 2267 7269 6d6f 6972 656c  ace": "grimoirel
+00000050: 6162 222c 0a20 2020 2022 7265 706f 7369  ab",.    "reposi
+00000060: 746f 7279 5f74 7970 6522 3a20 2269 6d61  tory_type": "ima
+00000070: 6765 222c 0a20 2020 2022 7374 6174 7573  ge",.    "status
+00000080: 223a 2031 2c0a 2020 2020 2264 6573 6372  ": 1,.    "descr
+00000090: 6970 7469 6f6e 223a 2022 5065 7263 6576  iption": "Percev
+000000a0: 616c 2044 6f63 6b65 7220 696d 6167 6520  al Docker image 
+000000b0: 746f 2077 6f72 6b20 696e 2073 7461 6e64  to work in stand
+000000c0: 616c 6f6e 6520 6d6f 6465 222c 0a20 2020  alone mode",.   
+000000d0: 2022 6973 5f70 7269 7661 7465 223a 2066   "is_private": f
+000000e0: 616c 7365 2c0a 2020 2020 2269 735f 6175  alse,.    "is_au
+000000f0: 746f 6d61 7465 6422 3a20 7472 7565 2c0a  tomated": true,.
+00000100: 2020 2020 2263 616e 5f65 6469 7422 3a20      "can_edit": 
+00000110: 6661 6c73 652c 0a20 2020 2022 7374 6172  false,.    "star
+00000120: 5f63 6f75 6e74 223a 2031 2c0a 2020 2020  _count": 1,.    
+00000130: 2270 756c 6c5f 636f 756e 7422 3a20 3339  "pull_count": 39
+00000140: 382c 0a20 2020 2022 6c61 7374 5f75 7064  8,.    "last_upd
+00000150: 6174 6564 223a 2022 3230 3137 2d30 352d  ated": "2017-05-
+00000160: 3130 5430 383a 3132 3a35 322e 3231 3737  10T08:12:52.2177
+00000170: 3837 5a22 2c0a 2020 2020 2262 7569 6c64  87Z",.    "build
+00000180: 5f6f 6e5f 636c 6f75 6422 3a20 6e75 6c6c  _on_cloud": null
+00000190: 2c0a 2020 2020 2268 6173 5f73 7461 7272  ,.    "has_starr
+000001a0: 6564 223a 2066 616c 7365 2c0a 2020 2020  ed": false,.    
+000001b0: 2266 756c 6c5f 6465 7363 7269 7074 696f  "full_descriptio
+000001c0: 6e22 3a20 2223 2050 6572 6365 7661 6c20  n": "# Perceval 
+000001d0: 5b21 5b42 7569 6c64 2053 7461 7475 735d  [![Build Status]
+000001e0: 2868 7474 7073 3a2f 2f74 7261 7669 732d  (https://travis-
+000001f0: 6369 2e6f 7267 2f67 7269 6d6f 6972 656c  ci.org/grimoirel
+00000200: 6162 2f70 6572 6365 7661 6c2e 7376 673f  ab/perceval.svg?
+00000210: 6272 616e 6368 3d6d 6173 7465 7229 5d28  branch=master)](
+00000220: 6874 7470 733a 2f2f 7472 6176 6973 2d63  https://travis-c
+00000230: 692e 6f72 672f 6772 696d 6f69 7265 6c61  i.org/grimoirela
+00000240: 622f 7065 7263 6576 616c 2920 5b21 5b43  b/perceval) [![C
+00000250: 6f76 6572 6167 6520 5374 6174 7573 5d28  overage Status](
+00000260: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000270: 6c64 732e 696f 2f63 6f76 6572 616c 6c73  lds.io/coveralls
+00000280: 2f67 7269 6d6f 6972 656c 6162 2f70 6572  /grimoirelab/per
+00000290: 6365 7661 6c2e 7376 6729 5d28 6874 7470  ceval.svg)](http
+000002a0: 733a 2f2f 636f 7665 7261 6c6c 732e 696f  s://coveralls.io
+000002b0: 2f72 2f67 7269 6d6f 6972 656c 6162 2f70  /r/grimoirelab/p
+000002c0: 6572 6365 7661 6c3f 6272 616e 6368 3d6d  erceval?branch=m
+000002d0: 6173 7465 7229 5c6e 5c6e 5365 6e64 2053  aster)\n\nSend S
+000002e0: 6972 2050 6572 6365 7661 6c20 6f6e 2061  ir Perceval on a
+000002f0: 2071 7565 7374 2074 6f20 7265 7472 6965   quest to retrie
+00000300: 7665 2061 6e64 2067 6174 6865 7220 6461  ve and gather da
+00000310: 7461 2066 726f 6d20 736f 6674 7761 7265  ta from software
+00000320: 5c6e 7265 706f 7369 746f 7269 6573 2e5c  \nrepositories.\
+00000330: 6e5c 6e23 2320 5573 6167 655c 6e5c 6e60  n\n## Usage\n\n`
+00000340: 6060 5c6e 7573 6167 653a 2070 6572 6365  ``\nusage: perce
+00000350: 7661 6c20 5b2d 6320 3c66 696c 653e 5d20  val [-c <file>] 
+00000360: 5b2d 675d 203c 6261 636b 656e 643e 205b  [-g] <backend> [
+00000370: 3c61 7267 733e 5d20 7c20 2d2d 6865 6c70  <args>] | --help
+00000380: 207c 202d 2d76 6572 7369 6f6e 5c6e 5c6e   | --version\n\n
+00000390: 5265 706f 7369 746f 7269 6573 2061 7265  Repositories are
+000003a0: 2072 6561 6368 6564 2075 7369 6e67 2073   reached using s
+000003b0: 7065 6369 6669 6320 6261 636b 656e 6473  pecific backends
+000003c0: 2e20 5468 6520 6d6f 7374 2063 6f6d 6d6f  . The most commo
+000003d0: 6e20 6261 636b 656e 6473 5c6e 6172 653a  n backends\nare:
+000003e0: 5c6e 2020 2020 6173 6b62 6f74 2020 2020  \n    askbot    
+000003f0: 2020 2020 2020 2046 6574 6368 2071 7565         Fetch que
+00000400: 7374 696f 6e73 2061 6e64 2061 6e73 7765  stions and answe
+00000410: 7273 2066 726f 6d20 4173 6b62 6f74 2073  rs from Askbot s
+00000420: 6974 655c 6e20 2020 2062 7567 7a69 6c6c  ite\n    bugzill
+00000430: 6120 2020 2020 2020 2020 4665 7463 6820  a         Fetch 
+00000440: 6275 6773 2066 726f 6d20 6120 4275 677a  bugs from a Bugz
+00000450: 696c 6c61 2073 6572 7665 725c 6e20 2020  illa server\n   
+00000460: 2062 7567 7a69 6c6c 6172 6573 7420 2020   bugzillarest   
+00000470: 2020 4665 7463 6820 6275 6773 2066 726f    Fetch bugs fro
+00000480: 6d20 6120 4275 677a 696c 6c61 2073 6572  m a Bugzilla ser
+00000490: 7665 7220 283e 3d35 2e30 2920 7573 696e  ver (>=5.0) usin
+000004a0: 6720 6974 7320 5245 5354 2041 5049 5c6e  g its REST API\n
+000004b0: 2020 2020 636f 6e66 6c75 656e 6365 2020      confluence  
+000004c0: 2020 2020 2046 6574 6368 2063 6f6e 7465       Fetch conte
+000004d0: 6e74 7320 6672 6f6d 2061 2043 6f6e 666c  nts from a Confl
+000004e0: 7565 6e63 6520 7365 7276 6572 5c6e 2020  uence server\n  
+000004f0: 2020 6469 7363 6f75 7273 6520 2020 2020    discourse     
+00000500: 2020 2046 6574 6368 2070 6f73 7473 2066     Fetch posts f
+00000510: 726f 6d20 4469 7363 6f75 7273 6520 7369  rom Discourse si
+00000520: 7465 5c6e 2020 2020 6765 7272 6974 2020  te\n    gerrit  
+00000530: 2020 2020 2020 2020 2046 6574 6368 2072           Fetch r
+00000540: 6576 6965 7773 2066 726f 6d20 6120 4765  eviews from a Ge
+00000550: 7272 6974 2073 6572 7665 725c 6e20 2020  rrit server\n   
+00000560: 2067 6974 2020 2020 2020 2020 2020 2020   git            
+00000570: 2020 4665 7463 6820 636f 6d6d 6974 7320    Fetch commits 
+00000580: 6672 6f6d 2047 6974 5c6e 2020 2020 6769  from Git\n    gi
+00000590: 7468 7562 2020 2020 2020 2020 2020 2046  thub           F
+000005a0: 6574 6368 2069 7373 7565 7320 6672 6f6d  etch issues from
+000005b0: 2047 6974 4875 625c 6e20 2020 2067 6d61   GitHub\n    gma
+000005c0: 6e65 2020 2020 2020 2020 2020 2020 4665  ne            Fe
+000005d0: 7463 6820 6d65 7373 6167 6573 2066 726f  tch messages fro
+000005e0: 6d20 476d 616e 655c 6e20 2020 2068 7970  m Gmane\n    hyp
+000005f0: 6572 6b69 7474 7920 2020 2020 2020 4665  erkitty       Fe
+00000600: 7463 6820 6d65 7373 6167 6573 2066 726f  tch messages fro
+00000610: 6d20 6120 4879 7065 724b 6974 7479 2061  m a HyperKitty a
+00000620: 7263 6869 7665 725c 6e20 2020 206a 656e  rchiver\n    jen
+00000630: 6b69 6e73 2020 2020 2020 2020 2020 4665  kins          Fe
+00000640: 7463 6820 6275 696c 6473 2066 726f 6d20  tch builds from 
+00000650: 6120 4a65 6e6b 696e 7320 7365 7276 6572  a Jenkins server
+00000660: 5c6e 2020 2020 6a69 7261 2020 2020 2020  \n    jira      
+00000670: 2020 2020 2020 2046 6574 6368 2069 7373         Fetch iss
+00000680: 7565 7320 6672 6f6d 204a 4952 4120 6973  ues from JIRA is
+00000690: 7375 6520 7472 6163 6b65 725c 6e20 2020  sue tracker\n   
+000006a0: 206d 626f 7820 2020 2020 2020 2020 2020   mbox           
+000006b0: 2020 4665 7463 6820 6d65 7373 6167 6573    Fetch messages
+000006c0: 2066 726f 6d20 4d42 6f78 2066 696c 6573   from MBox files
+000006d0: 5c6e 2020 2020 6d65 6469 6177 696b 6920  \n    mediawiki 
+000006e0: 2020 2020 2020 2046 6574 6368 2070 6167         Fetch pag
+000006f0: 6573 2061 6e64 2072 6576 6973 696f 6e73  es and revisions
+00000700: 2066 726f 6d20 6120 4d65 6469 6157 696b   from a MediaWik
+00000710: 6920 7369 7465 5c6e 2020 2020 6d65 6574  i site\n    meet
+00000720: 7570 2020 2020 2020 2020 2020 2046 6574  up           Fet
+00000730: 6368 2065 7665 6e74 7320 6672 6f6d 2061  ch events from a
+00000740: 204d 6565 7475 7020 6772 6f75 705c 6e20   Meetup group\n 
+00000750: 2020 206e 6e74 7020 2020 2020 2020 2020     nntp         
+00000760: 2020 2020 4665 7463 6820 6172 7469 636c      Fetch articl
+00000770: 6573 2066 726f 6d20 6120 4e4e 5450 206e  es from a NNTP n
+00000780: 6577 7320 6772 6f75 705c 6e20 2020 2070  ews group\n    p
+00000790: 6861 6272 6963 6174 6f72 2020 2020 2020  habricator      
+000007a0: 4665 7463 6820 7461 736b 7320 6672 6f6d  Fetch tasks from
+000007b0: 2061 2050 6861 6272 6963 6174 6f72 2073   a Phabricator s
+000007c0: 6974 655c 6e20 2020 2070 6970 6572 6d61  ite\n    piperma
+000007d0: 696c 2020 2020 2020 2020 4665 7463 6820  il        Fetch 
+000007e0: 6d65 7373 6167 6573 2066 726f 6d20 6120  messages from a 
+000007f0: 5069 7065 726d 6169 6c20 6172 6368 6976  Pipermail archiv
+00000800: 6572 5c6e 2020 2020 7265 646d 696e 6520  er\n    redmine 
+00000810: 2020 2020 2020 2020 2046 6574 6368 2069           Fetch i
+00000820: 7373 7565 7320 6672 6f6d 2061 2052 6564  ssues from a Red
+00000830: 6d69 6e65 2073 6572 7665 725c 6e20 2020  mine server\n   
+00000840: 2072 7373 2020 2020 2020 2020 2020 2020   rss            
+00000850: 2020 4665 7463 6820 656e 7472 6965 7320    Fetch entries 
+00000860: 6672 6f6d 2061 2052 5353 2066 6565 6420  from a RSS feed 
+00000870: 7365 7276 6572 5c6e 2020 2020 736c 6163  server\n    slac
+00000880: 6b20 2020 2020 2020 2020 2020 2046 6574  k            Fet
+00000890: 6368 206d 6573 7361 6765 7320 6672 6f6d  ch messages from
+000008a0: 2061 2053 6c61 636b 2063 6861 6e6e 656c   a Slack channel
+000008b0: 5c6e 2020 2020 7374 6163 6b65 7863 6861  \n    stackexcha
+000008c0: 6e67 6520 2020 2046 6574 6368 2071 7565  nge    Fetch que
+000008d0: 7374 696f 6e73 2066 726f 6d20 5374 6163  stions from Stac
+000008e0: 6b45 7863 6861 6e67 6520 7369 7465 735c  kExchange sites\
+000008f0: 6e20 2020 2073 7570 7962 6f74 2020 2020  n    supybot    
+00000900: 2020 2020 2020 4665 7463 6820 6d65 7373        Fetch mess
+00000910: 6167 6573 2066 726f 6d20 5375 7079 626f  ages from Supybo
+00000920: 7420 6c6f 6720 6669 6c65 735c 6e20 2020  t log files\n   
+00000930: 2074 656c 6567 7261 6d20 2020 2020 2020   telegram       
+00000940: 2020 4665 7463 6820 6d65 7373 6167 6573    Fetch messages
+00000950: 2066 726f 6d20 7468 6520 5465 6c65 6772   from the Telegr
+00000960: 616d 2073 6572 7665 725c 6e5c 6e6f 7074  am server\n\nopt
+00000970: 696f 6e61 6c20 6172 6775 6d65 6e74 733a  ional arguments:
+00000980: 5c6e 2020 2d68 2c20 2d2d 6865 6c70 2020  \n  -h, --help  
+00000990: 2020 2020 2020 2020 2020 7368 6f77 2074            show t
+000009a0: 6869 7320 6865 6c70 206d 6573 7361 6765  his help message
+000009b0: 2061 6e64 2065 7869 745c 6e20 202d 762c   and exit\n  -v,
+000009c0: 202d 2d76 6572 7369 6f6e 2020 2020 2020   --version      
+000009d0: 2020 2073 686f 7720 7665 7273 696f 6e5c     show version\
+000009e0: 6e20 202d 6320 4649 4c45 2c20 2d2d 636f  n  -c FILE, --co
+000009f0: 6e66 6967 2046 494c 455c 6e20 2020 2020  nfig FILE\n     
+00000a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a10: 2020 2073 6574 2063 6f6e 6669 6775 7261     set configura
+00000a20: 7469 6f6e 2066 696c 655c 6e20 202d 672c  tion file\n  -g,
+00000a30: 202d 2d64 6562 7567 2020 2020 2020 2020   --debug        
+00000a40: 2020 2073 6574 2064 6562 7567 206d 6f64     set debug mod
+00000a50: 6520 6f6e 5c6e 5c6e 5275 6e20 2770 6572  e on\n\nRun 'per
+00000a60: 6365 7661 6c20 3c62 6163 6b65 6e64 3e20  ceval <backend> 
+00000a70: 2d2d 6865 6c70 2720 746f 2067 6574 2069  --help' to get i
+00000a80: 6e66 6f72 6d61 7469 6f6e 2061 626f 7574  nformation about
+00000a90: 2061 2073 7065 6369 6669 6320 6261 636b   a specific back
+00000aa0: 656e 642e 5c6e 6060 605c 6e5c 6e23 2320  end.\n```\n\n## 
+00000ab0: 5265 7175 6972 656d 656e 7473 5c6e 5c6e  Requirements\n\n
+00000ac0: 2a20 5079 7468 6f6e 203e 3d20 332e 345c  * Python >= 3.4\
+00000ad0: 6e2a 2070 7974 686f 6e33 2d64 6174 6575  n* python3-dateu
+00000ae0: 7469 6c20 3e3d 2032 2e36 5c6e 2a20 7079  til >= 2.6\n* py
+00000af0: 7468 6f6e 332d 7265 7175 6573 7473 203e  thon3-requests >
+00000b00: 3d20 322e 375c 6e2a 2070 7974 686f 6e33  = 2.7\n* python3
+00000b10: 2d62 7334 2028 6265 6175 7469 6675 6c73  -bs4 (beautifuls
+00000b20: 6f75 7034 2920 3e3d 2034 2e33 5c6e 2a20  oup4) >= 4.3\n* 
+00000b30: 7079 7468 6f6e 332d 6665 6564 7061 7273  python3-feedpars
+00000b40: 6572 203e 3d20 352e 312e 335c 6e5c 6e23  er >= 5.1.3\n\n#
+00000b50: 2320 496e 7374 616c 6c61 7469 6f6e 5c6e  # Installation\n
+00000b60: 5c6e 5468 6572 6520 6172 6520 7365 7665  \nThere are seve
+00000b70: 7261 6c20 7761 7973 2066 6f72 2069 6e73  ral ways for ins
+00000b80: 7461 6c6c 696e 6720 5065 7263 6576 616c  talling Perceval
+00000b90: 206f 6e20 796f 7572 2073 7973 7465 6d3a   on your system:
+00000ba0: 2066 726f 6d20 7061 636b 6167 6573 2c5c   from packages,\
+00000bb0: 6e66 726f 6d20 6120 646f 636b 6572 2069  nfrom a docker i
+00000bc0: 6d61 6765 206f 7220 6672 6f6d 2074 6865  mage or from the
+00000bd0: 2073 6f75 7263 6520 636f 6465 2e5c 6e5c   source code.\n\
+00000be0: 6e23 2323 2050 6970 5c6e 5c6e 5065 7263  n### Pip\n\nPerc
+00000bf0: 6576 616c 2063 616e 2062 6520 696e 7374  eval can be inst
+00000c00: 616c 6c65 6420 7573 696e 6720 5b70 6970  alled using [pip
+00000c10: 5d28 6874 7470 733a 2f2f 7069 702e 7079  ](https://pip.py
+00000c20: 7061 2e69 6f2f 656e 2f73 7461 626c 652f  pa.io/en/stable/
+00000c30: 292c 2061 2074 6f6f 6c5c 6e66 6f72 2069  ), a tool\nfor i
+00000c40: 6e73 7461 6c6c 696e 6720 5079 7468 6f6e  nstalling Python
+00000c50: 2070 6163 6b61 6765 732e 2054 6f20 646f   packages. To do
+00000c60: 2069 742c 2072 756e 2074 6865 206e 6578   it, run the nex
+00000c70: 7420 636f 6d6d 616e 643a 5c6e 5c6e 6060  t command:\n\n``
+00000c80: 605c 6e24 2070 6970 3320 696e 7374 616c  `\n$ pip3 instal
+00000c90: 6c20 7065 7263 6576 616c 5c6e 6060 605c  l perceval\n```\
+00000ca0: 6e5c 6e23 2323 2044 6f63 6b65 725c 6e5c  n\n### Docker\n\
+00000cb0: 6e41 2050 6572 6365 7661 6c20 446f 636b  nA Perceval Dock
+00000cc0: 6572 2069 6d61 6765 2069 7320 6176 6169  er image is avai
+00000cd0: 6c61 626c 6520 6174 205b 446f 636b 6572  lable at [Docker
+00000ce0: 4875 625d 2868 7474 7073 3a2f 2f68 7562  Hub](https://hub
+00000cf0: 2e64 6f63 6b65 722e 636f 6d2f 722f 6772  .docker.com/r/gr
+00000d00: 696d 6f69 7265 6c61 622f 7065 7263 6576  imoirelab/percev
+00000d10: 616c 2f29 2e5c 6e5c 6e44 6574 6169 6c65  al/).\n\nDetaile
+00000d20: 6420 696e 666f 726d 6174 696f 6e20 6f6e  d information on
+00000d30: 2068 6f77 2074 6f20 7275 6e20 616e 642f   how to run and/
+00000d40: 6f72 2062 7569 6c64 2074 6869 7320 696d  or build this im
+00000d50: 6167 6520 6361 6e20 6265 2066 6f75 6e64  age can be found
+00000d60: 205b 6865 7265 5d28 6874 7470 733a 2f2f   [here](https://
+00000d70: 6769 7468 7562 2e63 6f6d 2f67 7269 6d6f  github.com/grimo
+00000d80: 6972 656c 6162 2f70 6572 6365 7661 6c2f  irelab/perceval/
+00000d90: 7472 6565 2f6d 6173 7465 722f 646f 636b  tree/master/dock
+00000da0: 6572 2f69 6d61 6765 732f 292e 5c6e 5c6e  er/images/).\n\n
+00000db0: 2323 2320 536f 7572 6365 2063 6f64 655c  ### Source code\
+00000dc0: 6e5c 6e54 6f20 696e 7374 616c 6c20 6672  n\nTo install fr
+00000dd0: 6f6d 2074 6865 2073 6f75 7263 6520 636f  om the source co
+00000de0: 6465 2079 6f75 2077 696c 6c20 6e65 6564  de you will need
+00000df0: 2074 6f20 636c 6f6e 6520 7468 6520 7265   to clone the re
+00000e00: 706f 7369 746f 7279 2066 6972 7374 3a5c  pository first:\
+00000e10: 6e5c 6e60 6060 5c6e 2420 6769 7420 636c  n\n```\n$ git cl
+00000e20: 6f6e 6520 6874 7470 733a 2f2f 6769 7468  one https://gith
+00000e30: 7562 2e63 6f6d 2f67 7269 6d6f 6972 656c  ub.com/grimoirel
+00000e40: 6162 2f70 6572 6365 7661 6c2e 6769 745c  ab/perceval.git\
+00000e50: 6e60 6060 5c6e 5c6e 496e 2074 6869 7320  n```\n\nIn this 
+00000e60: 6361 7365 2c20 5b73 6574 7570 746f 6f6c  case, [setuptool
+00000e70: 735d 2868 7474 703a 2f2f 7365 7475 7074  s](http://setupt
+00000e80: 6f6f 6c73 2e72 6561 6474 6865 646f 6373  ools.readthedocs
+00000e90: 2e69 6f2f 656e 2f6c 6174 6573 742f 2920  .io/en/latest/) 
+00000ea0: 7061 636b 6167 6520 7769 6c6c 2062 6520  package will be 
+00000eb0: 7265 7175 6972 6564 2e5c 6e4d 616b 6520  required.\nMake 
+00000ec0: 7375 7265 2069 7420 6973 2069 6e73 7461  sure it is insta
+00000ed0: 6c6c 6564 2062 6566 6f72 6520 7275 6e6e  lled before runn
+00000ee0: 696e 6720 7468 6520 6e65 7874 2063 6f6d  ing the next com
+00000ef0: 6d61 6e64 733a 5c6e 5c6e 6060 605c 6e24  mands:\n\n```\n$
+00000f00: 2070 6970 3320 696e 7374 616c 6c20 2d72   pip3 install -r
+00000f10: 2072 6571 7569 7265 6d65 6e74 732e 7478   requirements.tx
+00000f20: 745c 6e24 2070 7974 686f 6e33 2073 6574  t\n$ python3 set
+00000f30: 7570 2e70 7920 696e 7374 616c 6c5c 6e60  up.py install\n`
+00000f40: 6060 5c6e 5c6e 2323 2044 6f63 756d 656e  ``\n\n## Documen
+00000f50: 7461 7469 6f6e 5c6e 5c6e 446f 6375 6d65  tation\n\nDocume
+00000f60: 6e74 6174 696f 6e20 6973 2067 656e 6572  ntation is gener
+00000f70: 6174 6564 2061 7574 6f6d 6167 6963 616c  ated automagical
+00000f80: 6c79 2069 6e20 7468 6520 5b52 6561 6454  ly in the [ReadT
+00000f90: 6865 446f 6373 2050 6572 6365 7661 6c20  heDocs Perceval 
+00000fa0: 7369 7465 5d28 6874 7470 3a2f 2f70 6572  site](http://per
+00000fb0: 6365 7661 6c2e 7265 6164 7468 6564 6f63  ceval.readthedoc
+00000fc0: 732e 6f72 672f 292e 5c6e 5c6e 2323 2045  s.org/).\n\n## E
+00000fd0: 7861 6d70 6c65 735c 6e5c 6e23 2323 2041  xamples\n\n### A
+00000fe0: 736b 626f 745c 6e60 6060 5c6e 2420 7065  skbot\n```\n$ pe
+00000ff0: 7263 6576 616c 2061 736b 626f 7420 2768  rceval askbot 'h
+00001000: 7474 703a 2f2f 6173 6b62 6f74 2e6f 7267  ttp://askbot.org
+00001010: 2f27 202d 2d66 726f 6d2d 6461 7465 2027  /' --from-date '
+00001020: 3230 3136 2d30 312d 3031 275c 6e60 6060  2016-01-01'\n```
+00001030: 5c6e 5c6e 2323 2320 4275 677a 696c 6c61  \n\n### Bugzilla
+00001040: 5c6e 546f 2066 6574 6368 2062 7567 7320  \nTo fetch bugs 
+00001050: 6672 6f6d 2042 7567 7a69 6c6c 612c 2079  from Bugzilla, y
+00001060: 6f75 2068 6176 6520 7477 6f20 6f70 7469  ou have two opti
+00001070: 6f6e 733a 5c6e 5c6e 6129 2055 7365 2074  ons:\n\na) Use t
+00001080: 6865 2074 7261 6469 7469 6f6e 616c 2062  he traditional b
+00001090: 6163 6b65 6e64 5c6e 5c6e 6060 605c 6e24  ackend\n\n```\n$
+000010a0: 2070 6572 6365 7661 6c20 6275 677a 696c   perceval bugzil
+000010b0: 6c61 2027 6874 7470 733a 2f2f 6275 677a  la 'https://bugz
+000010c0: 696c 6c61 2e72 6564 6861 742e 636f 6d2f  illa.redhat.com/
+000010d0: 2720 2d2d 6261 636b 656e 642d 7573 6572  ' --backend-user
+000010e0: 2075 7365 7220 2d2d 6261 636b 656e 642d   user --backend-
+000010f0: 7061 7373 776f 7264 2070 6173 7320 2d2d  password pass --
+00001100: 6672 6f6d 2d64 6174 6520 2732 3031 362d  from-date '2016-
+00001110: 3031 2d30 3127 5c6e 6060 605c 6e5c 6e62  01-01'\n```\n\nb
+00001120: 2920 5573 6520 7468 6520 5245 5354 2041  ) Use the REST A
+00001130: 5049 2062 6163 6b65 6e64 2066 6f72 2042  PI backend for B
+00001140: 757a 696c 6c61 2035 2e30 2028 6f72 2068  uzilla 5.0 (or h
+00001150: 6967 6865 7229 2073 6572 7665 7273 2e20  igher) servers. 
+00001160: 5765 2073 7472 6f6e 676c 7920 7265 636f  We strongly reco
+00001170: 6d6d 656e 645c 6e74 6869 7320 6261 636b  mmend\nthis back
+00001180: 656e 6420 7768 656e 2064 6174 6120 6973  end when data is
+00001190: 2066 6574 6368 6564 2066 726f 6d20 7665   fetched from ve
+000011a0: 7273 696f 6e20 7365 7276 6572 7320 3e3d  rsion servers >=
+000011b0: 352e 3020 6265 6361 7573 6520 7468 6520  5.0 because the 
+000011c0: 7265 7472 6965 7661 6c5c 6e70 726f 6365  retrieval\nproce
+000011d0: 7373 2069 7320 6d75 6368 2066 6173 7465  ss is much faste
+000011e0: 722e 5c6e 5c6e 6060 605c 6e24 2070 6572  r.\n\n```\n$ per
+000011f0: 6365 7661 6c20 6275 677a 696c 6c61 7265  ceval bugzillare
+00001200: 7374 2027 6874 7470 733a 2f2f 6275 677a  st 'https://bugz
+00001210: 696c 6c61 2e6d 6f7a 696c 6c61 2e6f 7267  illa.mozilla.org
+00001220: 2f27 202d 2d62 6163 6b65 6e64 2d75 7365  /' --backend-use
+00001230: 7220 7573 6572 202d 2d62 6163 6b65 6e64  r user --backend
+00001240: 2d70 6173 7377 6f72 6420 7061 7373 202d  -password pass -
+00001250: 2d66 726f 6d2d 6461 7465 2027 3230 3136  -from-date '2016
+00001260: 2d30 312d 3031 275c 6e60 6060 5c6e 5c6e  -01-01'\n```\n\n
+00001270: 2323 2320 436f 6e66 6c75 656e 6365 5c6e  ### Confluence\n
+00001280: 6060 605c 6e24 2070 6572 6365 7661 6c20  ```\n$ perceval 
+00001290: 636f 6e66 6c75 656e 6365 2027 6874 7470  confluence 'http
+000012a0: 733a 2f2f 7769 6b69 2e6f 706e 6676 2e6f  s://wiki.opnfv.o
+000012b0: 7267 2f27 202d 2d66 726f 6d2d 6461 7465  rg/' --from-date
+000012c0: 2027 3230 3136 2d30 312d 3031 275c 6e60   '2016-01-01'\n`
+000012d0: 6060 5c6e 5c6e 2323 2320 4469 7363 6f75  ``\n\n### Discou
+000012e0: 7273 655c 6e60 6060 5c6e 2420 7065 7263  rse\n```\n$ perc
+000012f0: 6576 616c 2064 6973 636f 7572 7365 2027  eval discourse '
+00001300: 6874 7470 733a 2f2f 666f 726f 2e6d 6f7a  https://foro.moz
+00001310: 696c 6c61 2d68 6973 7061 6e6f 2e6f 7267  illa-hispano.org
+00001320: 2f27 202d 2d66 726f 6d2d 6461 7465 2027  /' --from-date '
+00001330: 3230 3136 2d30 312d 3031 275c 6e60 6060  2016-01-01'\n```
+00001340: 5c6e 5c6e 2323 2320 4765 7272 6974 5c6e  \n\n### Gerrit\n
+00001350: 546f 2072 756e 2067 6572 7269 742c 2079  To run gerrit, y
+00001360: 6f75 2077 696c 6c20 6e65 6564 2061 6e20  ou will need an 
+00001370: 6175 7468 6f72 697a 6564 2053 5348 2070  authorized SSH p
+00001380: 7269 7661 7465 206b 6579 3a5c 6e5c 6e60  rivate key:\n\n`
+00001390: 6060 5c6e 2420 6576 616c 2060 7373 682d  ``\n$ eval `ssh-
+000013a0: 6167 656e 7420 2d73 605c 6e24 2073 7368  agent -s`\n$ ssh
+000013b0: 2d61 6464 207e 2f2e 7373 682f 6964 5f72  -add ~/.ssh/id_r
+000013c0: 7361 5c6e 4964 656e 7469 7479 2061 6464  sa\nIdentity add
+000013d0: 6564 3a20 2f68 6f6d 652f 7573 6572 2f2e  ed: /home/user/.
+000013e0: 7373 682f 6964 5f72 7361 2028 2f68 6f6d  ssh/id_rsa (/hom
+000013f0: 652f 7573 6572 2f2e 7373 682f 6964 5f72  e/user/.ssh/id_r
+00001400: 7361 295c 6e60 6060 5c6e 5c6e 546f 2072  sa)\n```\n\nTo r
+00001410: 756e 2074 6865 2062 6163 6b65 6e64 2c20  un the backend, 
+00001420: 6578 6563 7574 6520 7468 6520 6e65 7874  execute the next
+00001430: 2063 6f6d 6d61 6e64 3a5c 6e5c 6e60 6060   command:\n\n```
+00001440: 5c6e 2420 7065 7263 6576 616c 2067 6572  \n$ perceval ger
+00001450: 7269 7420 2d2d 7573 6572 2075 7365 7220  rit --user user 
+00001460: 2772 6576 6965 772e 6f70 656e 7374 6163  'review.openstac
+00001470: 6b2e 6f72 6727 202d 2d66 726f 6d2d 6461  k.org' --from-da
+00001480: 7465 2027 3230 3136 2d30 312d 3031 275c  te '2016-01-01'\
+00001490: 6e60 6060 5c6e 5c6e 2323 2320 4769 745c  n```\n\n### Git\
+000014a0: 6e5c 6e54 6f20 7275 6e20 7468 6973 2062  n\nTo run this b
+000014b0: 6163 6b65 6e64 2065 7865 6375 7465 2074  ackend execute t
+000014c0: 6865 206e 6578 7420 636f 6d6d 616e 642e  he next command.
+000014d0: 2054 616b 6520 696e 746f 2061 6363 6f75   Take into accou
+000014e0: 6e74 2074 6861 7420 746f 2072 756e 5c6e  nt that to run\n
+000014f0: 7468 6973 2062 6163 6b65 6e64 2047 6974  this backend Git
+00001500: 2070 726f 6772 616d 2068 6173 2074 6f20   program has to 
+00001510: 6265 2069 6e73 7461 6c6c 6564 206f 6e20  be installed on 
+00001520: 796f 7572 2073 7973 7465 6d2e 5c6e 5c6e  your system.\n\n
+00001530: 6060 605c 6e24 2070 6572 6365 7661 6c20  ```\n$ perceval 
+00001540: 6769 7420 2768 7474 7073 3a2f 2f67 6974  git 'https://git
+00001550: 6875 622e 636f 6d2f 6772 696d 6f69 7265  hub.com/grimoire
+00001560: 6c61 622f 7065 7263 6576 616c 2e67 6974  lab/perceval.git
+00001570: 2720 2d2d 6672 6f6d 2d64 6174 6520 2732  ' --from-date '2
+00001580: 3031 362d 3031 2d30 3127 5c6e 6060 605c  016-01-01'\n```\
+00001590: 6e5c 6e47 6974 2062 6163 6b65 6e64 2063  n\nGit backend c
+000015a0: 616e 2061 6c73 6f20 776f 726b 2077 6974  an also work wit
+000015b0: 6820 6120 4769 7420 6c6f 6720 6669 6c65  h a Git log file
+000015c0: 2061 7320 696e 7075 742e 2057 6520 7265   as input. We re
+000015d0: 636f 6d6d 656e 6420 746f 2075 7365 2074  commend to use t
+000015e0: 6865 206e 6578 7420 636f 6d6d 616e 6420  he next command 
+000015f0: 746f 2067 6574 2074 6865 206d 6f73 7420  to get the most 
+00001600: 636f 6d70 6c65 7465 206c 6f67 2066 696c  complete log fil
+00001610: 652e 5c6e 5c6e 6060 605c 6e67 6974 206c  e.\n\n```\ngit l
+00001620: 6f67 202d 2d72 6177 202d 2d6e 756d 7374  og --raw --numst
+00001630: 6174 202d 2d70 7265 7474 793d 6675 6c6c  at --pretty=full
+00001640: 6572 202d 2d64 6563 6f72 6174 653d 6675  er --decorate=fu
+00001650: 6c6c 202d 2d70 6172 656e 7473 202d 2d72  ll --parents --r
+00001660: 6576 6572 7365 202d 2d74 6f70 6f2d 6f72  everse --topo-or
+00001670: 6465 7220 2d4d 202d 4320 2d63 202d 2d72  der -M -C -c --r
+00001680: 656d 6f74 6573 3d6f 7269 6769 6e20 2d2d  emotes=origin --
+00001690: 616c 6c20 3e20 2f74 6d70 2f67 6974 6c6f  all > /tmp/gitlo
+000016a0: 672e 6c6f 675c 6e60 6060 5c6e 5c6e 5468  g.log\n```\n\nTh
+000016b0: 656e 2c20 746f 2072 756e 2074 6865 2062  en, to run the b
+000016c0: 6163 6b65 6e64 2c20 6a75 7374 2065 7865  ackend, just exe
+000016d0: 6375 7465 2061 6e79 206f 6620 7468 6520  cute any of the 
+000016e0: 6e65 7874 2063 6f6d 6d61 6e64 733a 5c6e  next commands:\n
+000016f0: 5c6e 6060 605c 6e24 2070 6572 6365 7661  \n```\n$ perceva
+00001700: 6c20 6769 7420 2d2d 6769 742d 6c6f 6720  l git --git-log 
+00001710: 272f 746d 702f 6769 746c 6f67 2e6c 6f67  '/tmp/gitlog.log
+00001720: 2720 2766 696c 653a 2f2f 2f6d 7972 6570  ' 'file:///myrep
+00001730: 6f2e 6769 7427 5c6e 6060 605c 6e5c 6e6f  o.git'\n```\n\no
+00001740: 725c 6e5c 6e60 6060 5c6e 2420 7065 7263  r\n\n```\n$ perc
+00001750: 6576 616c 2067 6974 2027 2f74 6d70 2f67  eval git '/tmp/g
+00001760: 6974 6c6f 672e 6c6f 6727 5c6e 6060 605c  itlog.log'\n```\
+00001770: 6e5c 6e23 2323 2047 6974 4875 625c 6e60  n\n### GitHub\n`
+00001780: 6060 5c6e 2420 7065 7263 6576 616c 2067  ``\n$ perceval g
+00001790: 6974 6875 6220 656c 6173 7469 6320 6c6f  ithub elastic lo
+000017a0: 6773 7461 7368 202d 2d66 726f 6d2d 6461  gstash --from-da
+000017b0: 7465 2027 3230 3136 2d30 312d 3031 275c  te '2016-01-01'\
+000017c0: 6e60 6060 5c6e 5c6e 2323 2320 476d 616e  n```\n\n### Gman
+000017d0: 655c 6e60 6060 5c6e 2420 7065 7263 6576  e\n```\n$ percev
+000017e0: 616c 2067 6d61 6e65 202d 2d6f 6666 7365  al gmane --offse
+000017f0: 7420 3230 3030 2027 6576 696e 6365 2d6c  t 2000 'evince-l
+00001800: 6973 7440 676e 6f6d 652e 6f72 6727 5c6e  ist@gnome.org'\n
+00001810: 6060 605c 6e5c 6e23 2323 2048 7970 6572  ```\n\n### Hyper
+00001820: 4b69 7474 795c 6e60 6060 5c6e 2420 7065  Kitty\n```\n$ pe
+00001830: 7263 6576 616c 2068 7970 6572 6b69 7474  rceval hyperkitt
+00001840: 7920 2768 7474 7073 3a2f 2f6c 6973 7473  y 'https://lists
+00001850: 2e6d 6169 6c6d 616e 332e 6f72 672f 6172  .mailman3.org/ar
+00001860: 6368 6976 6573 2f6c 6973 742f 6d61 696c  chives/list/mail
+00001870: 6d61 6e2d 7573 6572 7340 6d61 696c 6d61  man-users@mailma
+00001880: 6e33 2e6f 7267 2720 2d2d 6672 6f6d 2d64  n3.org' --from-d
+00001890: 6174 6520 3230 3137 2d30 312d 3031 5c6e  ate 2017-01-01\n
+000018a0: 6060 605c 6e5c 6e23 2323 204a 656e 6b69  ```\n\n### Jenki
+000018b0: 6e73 5c6e 6060 605c 6e24 2070 6572 6365  ns\n```\n$ perce
+000018c0: 7661 6c20 6a65 6e6b 696e 7320 2768 7474  val jenkins 'htt
+000018d0: 703a 2f2f 6a65 6e6b 696e 732e 6379 616e  p://jenkins.cyan
+000018e0: 6f67 656e 6d6f 642e 6f72 672f 275c 6e60  ogenmod.org/'\n`
+000018f0: 6060 5c6e 5c6e 2323 2320 4a49 5241 5c6e  ``\n\n### JIRA\n
+00001900: 6060 605c 6e24 2070 6572 6365 7661 6c20  ```\n$ perceval 
+00001910: 6a69 7261 2027 6874 7470 733a 2f2f 7469  jira 'https://ti
+00001920: 636b 6574 732e 7075 7070 6574 6c61 6273  ckets.puppetlabs
+00001930: 2e63 6f6d 2720 2d2d 7072 6f6a 6563 7420  .com' --project 
+00001940: 5055 5020 2d2d 6672 6f6d 2d64 6174 6520  PUP --from-date 
+00001950: 2732 3031 362d 3031 2d30 3127 5c6e 6060  '2016-01-01'\n``
+00001960: 605c 6e5c 6e23 2323 204d 426f 785c 6e60  `\n\n### MBox\n`
+00001970: 6060 5c6e 2420 7065 7263 6576 616c 206d  ``\n$ perceval m
+00001980: 626f 7820 2768 7474 703a 2f2f 6578 616d  box 'http://exam
+00001990: 706c 652e 636f 6d27 202f 746d 702f 6d62  ple.com' /tmp/mb
+000019a0: 6f78 6573 2f5c 6e60 6060 5c6e 5c6e 2323  oxes/\n```\n\n##
+000019b0: 2320 4d65 6469 6157 696b 695c 6e60 6060  # MediaWiki\n```
+000019c0: 5c6e 2420 7065 7263 6576 616c 206d 6564  \n$ perceval med
+000019d0: 6961 7769 6b69 2027 6874 7470 733a 2f2f  iawiki 'https://
+000019e0: 7769 6b69 2e6d 6f7a 696c 6c61 2e6f 7267  wiki.mozilla.org
+000019f0: 2720 2d2d 6672 6f6d 2d64 6174 6520 2732  ' --from-date '2
+00001a00: 3031 362d 3036 2d33 3027 5c6e 6060 605c  016-06-30'\n```\
+00001a10: 6e5c 6e23 2323 204d 6565 7475 705c 6e60  n\n### Meetup\n`
+00001a20: 6060 5c6e 2420 7065 7263 6576 616c 206d  ``\n$ perceval m
+00001a30: 6565 7475 7020 2753 6f66 7477 6172 652d  eetup 'Software-
+00001a40: 4465 7665 6c6f 706d 656e 742d 416e 616c  Development-Anal
+00001a50: 7974 6963 7327 202d 2d66 726f 6d2d 6461  ytics' --from-da
+00001a60: 7465 2027 3230 3136 2d30 362d 3031 2720  te '2016-06-01' 
+00001a70: 2d74 2061 6263 6465 6667 6869 6a6b 5c6e  -t abcdefghijk\n
+00001a80: 6060 605c 6e5c 6e23 2323 204e 4e54 505c  ```\n\n### NNTP\
+00001a90: 6e60 6060 5c6e 2420 7065 7263 6576 616c  n```\n$ perceval
+00001aa0: 206e 6e74 7020 276e 6577 732e 6d6f 7a69   nntp 'news.mozi
+00001ab0: 6c6c 612e 6f72 6727 2027 6d6f 7a69 6c6c  lla.org' 'mozill
+00001ac0: 612e 6465 762e 7072 6f6a 6563 742d 6c69  a.dev.project-li
+00001ad0: 6e6b 2720 2d2d 6f66 6673 6574 2031 305c  nk' --offset 10\
+00001ae0: 6e60 6060 5c6e 5c6e 2323 2320 5068 6162  n```\n\n### Phab
+00001af0: 7269 6361 746f 725c 6e60 6060 5c6e 2420  ricator\n```\n$ 
+00001b00: 7065 7263 6576 616c 2070 6861 6272 6963  perceval phabric
+00001b10: 6174 6f72 2027 6874 7470 733a 2f2f 7365  ator 'https://se
+00001b20: 6375 7265 2e70 6861 6272 6963 6174 6f72  cure.phabricator
+00001b30: 2e63 6f6d 2f27 202d 7420 3132 3334 3536  .com/' -t 123456
+00001b40: 3738 3961 6263 6566 655c 6e60 6060 5c6e  789abcefe\n```\n
+00001b50: 5c6e 2323 2320 5069 7065 726d 6169 6c5c  \n### Pipermail\
+00001b60: 6e60 6060 5c6e 2420 7065 7263 6576 616c  n```\n$ perceval
+00001b70: 2070 6970 6572 6d61 696c 2027 6874 7470   pipermail 'http
+00001b80: 733a 2f2f 6d61 696c 2e67 6e6f 6d65 2e6f  s://mail.gnome.o
+00001b90: 7267 2f61 7263 6869 7665 732f 6c69 6261  rg/archives/liba
+00001ba0: 7274 2d68 6163 6b65 7273 2f27 5c6e 6060  rt-hackers/'\n``
+00001bb0: 605c 6e5c 6e50 6970 6572 6d61 696c 2061  `\n\nPipermail a
+00001bc0: 6c73 6f20 6973 2061 626c 6520 746f 2066  lso is able to f
+00001bd0: 6574 6368 2064 6174 6120 6672 6f6d 2041  etch data from A
+00001be0: 7061 6368 6527 7320 606d 6f64 5f62 6f78  pache's `mod_box
+00001bf0: 6020 696e 7465 7266 6163 653a 5c6e 6060  ` interface:\n``
+00001c00: 605c 6e24 2070 6572 6365 7661 6c20 7069  `\n$ perceval pi
+00001c10: 7065 726d 6169 6c20 2768 7474 703a 2f2f  permail 'http://
+00001c20: 6d61 696c 2d61 7263 6869 7665 732e 6170  mail-archives.ap
+00001c30: 6163 6865 2e6f 7267 2f6d 6f64 5f6d 626f  ache.org/mod_mbo
+00001c40: 782f 6874 7470 642d 6465 762f 275c 6e60  x/httpd-dev/'\n`
+00001c50: 6060 5c6e 5c6e 2323 2320 5265 646d 696e  ``\n\n### Redmin
+00001c60: 655c 6e60 6060 5c6e 2420 7065 7263 6576  e\n```\n$ percev
+00001c70: 616c 2072 6564 6d69 6e65 2027 6874 7470  al redmine 'http
+00001c80: 733a 2f2f 7777 772e 7265 646d 696e 652e  s://www.redmine.
+00001c90: 6f72 672f 2720 2d2d 6672 6f6d 2d64 6174  org/' --from-dat
+00001ca0: 6520 2732 3031 362d 3031 2d30 3127 202d  e '2016-01-01' -
+00001cb0: 7420 6162 6364 6566 6768 696a 6b5c 6e60  t abcdefghijk\n`
+00001cc0: 6060 5c6e 5c6e 2323 2320 5253 535c 6e60  ``\n\n### RSS\n`
+00001cd0: 6060 5c6e 2420 7065 7263 6576 616c 2072  ``\n$ perceval r
+00001ce0: 7373 2027 6874 7470 733a 2f2f 626c 6f67  ss 'https://blog
+00001cf0: 2e62 6974 6572 6769 612e 636f 6d2f 6665  .bitergia.com/fe
+00001d00: 6564 2f27 5c6e 6060 605c 6e5c 6e23 2323  ed/'\n```\n\n###
+00001d10: 2053 6c61 636b 5c6e 6060 605c 6e24 2070   Slack\n```\n$ p
+00001d20: 6572 6365 7661 6c20 736c 6163 6b20 4330  erceval slack C0
+00001d30: 3030 3120 2d2d 6672 6f6d 2d64 6174 6520  001 --from-date 
+00001d40: 3230 3136 2d30 312d 3132 202d 7420 6162  2016-01-12 -t ab
+00001d50: 6365 6465 6667 6869 6a6b 5c6e 6060 605c  cedefghijk\n```\
+00001d60: 6e5c 6e23 2323 2053 7461 636b 4578 6368  n\n### StackExch
+00001d70: 616e 6765 5c6e 6060 605c 6e24 2070 6572  ange\n```\n$ per
+00001d80: 6365 7661 6c20 7374 6163 6b65 7863 6861  ceval stackexcha
+00001d90: 6e67 6520 2d2d 7369 7465 2073 7461 636b  nge --site stack
+00001da0: 6f76 6572 666c 6f77 202d 2d74 6167 6765  overflow --tagge
+00001db0: 6420 7079 7468 6f6e 202d 2d66 726f 6d2d  d python --from-
+00001dc0: 6461 7465 2027 3230 3136 2d30 312d 3031  date '2016-01-01
+00001dd0: 2720 2d2d 746f 6b65 6e20 6162 6364 6162  ' --token abcdab
+00001de0: 6364 6162 6364 6162 6364 5c6e 6060 605c  cdabcdabcd\n```\
+00001df0: 6e5c 6e23 2323 2053 7570 7962 6f74 5c6e  n\n### Supybot\n
+00001e00: 6060 605c 6e24 2070 6572 6365 7661 6c20  ```\n$ perceval 
+00001e10: 7375 7079 626f 7420 2768 7474 703a 2f2f  supybot 'http://
+00001e20: 6368 616e 6e65 6c2e 6578 616d 706c 652e  channel.example.
+00001e30: 636f 6d27 202f 746d 702f 7375 7079 626f  com' /tmp/supybo
+00001e40: 742f 5c6e 6060 605c 6e5c 6e23 2323 2054  t/\n```\n\n### T
+00001e50: 656c 6567 7261 6d5c 6e5c 6e54 656c 6567  elegram\n\nTeleg
+00001e60: 7261 6d20 6261 636b 656e 6420 6e65 6564  ram backend need
+00001e70: 7320 616e 2041 5049 2074 6f6b 656e 2074  s an API token t
+00001e80: 6f20 6175 7468 656e 7469 6361 7465 2074  o authenticate t
+00001e90: 6865 2062 6f74 2e20 496e 2061 6464 6974  he bot. In addit
+00001ea0: 696f 6e20 616e 645c 6e69 6e20 6f72 6465  ion and\nin orde
+00001eb0: 7220 746f 2066 6574 6368 206d 6573 7361  r to fetch messa
+00001ec0: 6765 7320 6672 6f6d 2061 2067 726f 7570  ges from a group
+00001ed0: 206f 7220 6368 616e 6e65 6c2c 2070 7269   or channel, pri
+00001ee0: 7661 6379 2073 6574 7469 6e67 7320 6d75  vacy settings mu
+00001ef0: 7374 2062 655c 6e64 6973 6162 6c65 642e  st be\ndisabled.
+00001f00: 2054 6f20 6b6e 6f77 2068 6f77 2074 6f20   To know how to 
+00001f10: 6372 6561 7465 2061 2062 6f74 2c20 746f  create a bot, to
+00001f20: 206f 6274 6169 6e20 6974 7320 746f 6b65   obtain its toke
+00001f30: 6e20 616e 6420 746f 2063 6f6e 6669 6775  n and to configu
+00001f40: 7265 2069 745c 6e70 6c65 6173 6520 7265  re it\nplease re
+00001f50: 6164 2074 6865 205b 5465 6c65 6772 616d  ad the [Telegram
+00001f60: 2042 6f74 7320 646f 6373 2070 6167 6573   Bots docs pages
+00001f70: 5d28 6874 7470 733a 2f2f 636f 7265 2e74  ](https://core.t
+00001f80: 656c 6567 7261 6d2e 6f72 672f 626f 7473  elegram.org/bots
+00001f90: 292e 5c6e 5c6e 6060 605c 6e24 2070 6572  ).\n\n```\n$ per
+00001fa0: 6365 7661 6c20 7465 6c65 6772 616d 206d  ceval telegram m
+00001fb0: 7962 6f74 202d 7420 3132 3334 3536 3738  ybot -t 12345678
+00001fc0: 6162 6364 6566 6768 202d 2d63 6861 7473  abcdefgh --chats
+00001fd0: 2031 2032 202d 3130 5c6e 6060 605c 6e5c   1 2 -10\n```\n\
+00001fe0: 6e23 2320 4c69 6365 6e73 655c 6e5c 6e4c  n## License\n\nL
+00001ff0: 6963 656e 7365 6420 756e 6465 7220 474e  icensed under GN
+00002000: 5520 4765 6e65 7261 6c20 5075 626c 6963  U General Public
+00002010: 204c 6963 656e 7365 2028 4750 4c29 2c20   License (GPL), 
+00002020: 7665 7273 696f 6e20 3320 6f72 206c 6174  version 3 or lat
+00002030: 6572 2e5c 6e22 2c0a 2020 2020 2261 6666  er.\n",.    "aff
+00002040: 696c 6961 7469 6f6e 223a 206e 756c 6c2c  iliation": null,
+00002050: 0a20 2020 2022 7065 726d 6973 7369 6f6e  .    "permission
+00002060: 7322 3a20 7b0a 2020 2020 2020 2020 2272  s": {.        "r
+00002070: 6561 6422 3a20 7472 7565 2c0a 2020 2020  ead": true,.    
+00002080: 2020 2020 2277 7269 7465 223a 2066 616c      "write": fal
+00002090: 7365 2c0a 2020 2020 2020 2020 2261 646d  se,.        "adm
+000020a0: 696e 223a 2066 616c 7365 0a20 2020 207d  in": false.    }
+000020b0: 0a7d 0a                                  .}.
```

### Comparing `perceval-0.9.9/perceval/backends/core/jira.py` & `perceval-1.0.0rc1/perceval/backends/core/groupsio.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,388 +1,358 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2016-2017 Bitergia
+# Copyright (C) 2015-2020 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1335, USA.
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
-#     Alberto Martín <alberto.martin@bitergia.com>
+#     Valerio Cosentino <valcos@bitergia.com>
+#     Harshal Mittal <harshalmittal4@gmail.com>
 #     Santiago Dueñas <sduenas@bitergia.com>
 #
 
-import json
 import logging
-
+import os
 import requests
 
-from requests.packages.urllib3.exceptions import InsecureRequestWarning
-
-from grimoirelab.toolkit.datetime import datetime_to_utc, str_to_datetime
-from grimoirelab.toolkit.uris import urijoin
+from grimoirelab_toolkit.datetime import datetime_to_utc
+from grimoirelab_toolkit.uris import urijoin
 
-from ...backend import (Backend,
-                        BackendCommand,
+from .mbox import MBox, MailingList, CATEGORY_MESSAGE
+from ...backend import (BackendCommand,
                         BackendCommandArgumentParser,
-                        metadata)
-from ...client import HttpClient
-from ...errors import CacheError
+                        DEFAULT_SEARCH_FIELD)
+from ...errors import BackendError
 from ...utils import DEFAULT_DATETIME
 
+MBOX_FILE = 'messages.zip'
 
-MAX_ISSUES = 100  # Maximum number of issues per query
-
-logger = logging.getLogger(__name__)
-
-
-def map_custom_field(custom_fields, fields):
-    """Add extra information for custom fields.
+GROUPSIO_URL = 'https://groups.io/'
+GROUPSIO_API_URL = 'https://groups.io/api/v1'
 
-    :param custom_fields: set of custom fields with the extra information
-    :param fields: fields of the issue where to add the extra information
+PER_PAGE = 100
 
-    :returns: an set of items with the extra information mapped
-    """
-    def build_cf(cf, v):
-        return {'id': cf['id'], 'name': cf['name'], 'value': v}
-
-    return {
-        k: build_cf(custom_fields[k], v)
-        for k, v in fields.items()
-        if k in custom_fields
-    }
 
+logger = logging.getLogger(__name__)
 
-def filter_custom_fields(fields):
-    """Filter custom fields from a given set of fields.
 
-    :param fields: set of fields
+class Groupsio(MBox):
+    """Groups.io backend.
 
-    :returns: an object with the filtered custom fields
+    This class allows the fetch the messages of a Groups.io group.
+    Initialize this class passing the name of the group, the
+    directory path where the mbox files will be fetched and
+    stored, and the email and password of the Groupsio user.
+    The origin of the data will be set to the url of the group
+    on Groups.io.
+
+    In order to know the group names where you are subscribed,
+    you can use the following script:
+    https://gist.github.com/valeriocos/2e2231e17fd3052800303bf99bd0c7c4
+
+    :param group_name: Name of the group
+    :param dirpath: directory path where the mboxes are stored
+    :param email: Groupsio user email
+    :param password: Groupsio user password
+    :param tag: label used to mark the data
+    :param archive: archive to store/retrieve items
+    :param ssl_verify: enable/disable SSL verification
     """
+    version = '1.0.0'
 
-    custom_fields = {}
+    CATEGORIES = [CATEGORY_MESSAGE]
 
-    sorted_fields = [field for field in fields if field['custom'] is True]
+    def __init__(self, group_name, dirpath, email, password, tag=None, archive=None, ssl_verify=True):
+        url = urijoin(GROUPSIO_URL, 'g', group_name)
+        super().__init__(url, dirpath, tag=tag, archive=archive, ssl_verify=ssl_verify)
+        self.email = email
+        self.password = password
+        self.group_name = group_name
 
-    for custom_field in sorted_fields:
-        custom_fields[custom_field['id']] = custom_field
+    def search_fields(self, item):
+        """Add search fields to an item.
 
-    return custom_fields
+        It adds the values of `metadata_id` plus the `group_name`
 
+        :param item: the item to extract the search fields values
 
-class Jira(Backend):
-    """JIRA backend for Perceval.
+        :returns: a dict of search fields
+        """
+        search_fields = {
+            DEFAULT_SEARCH_FIELD: self.metadata_id(item)
+        }
 
-    This class retrieves the issues stored in JIRA issue tracking
-    system. To initialize this class the URL must be provided.
-    The `url` will be set as the origin of the data.
+        origin_parts = self.origin.split('/')
+        search_fields['group_name'] = origin_parts[-1]
 
-    :param url: JIRA's endpoint
-    :param project: filter issues by project
-    :param user: Jira user
-    :param password: Jira user password
-    :param verify: allows to disable SSL verification
-    :param cert: SSL certificate path (PEM)
-    :param tag: label used to mark the data
-    :param cache: cache object to store raw data
-    """
-    version = '0.8.0'
+        return search_fields
 
-    def __init__(self, url, project=None,
-                 user=None, password=None,
-                 verify=None, cert=None,
-                 max_issues=None, tag=None, cache=None):
-        origin = url
-
-        super().__init__(origin, tag=tag, cache=cache)
-        self.url = url
-        self.project = project
-        self.user = user
-        self.password = password
-        self.verify = verify
-        self.cert = cert
-        self.max_issues = max_issues
-        self.client = JiraClient(url, project, user, password,
-                                 verify, cert, max_issues)
-
-    @metadata
-    def fetch(self, from_date=DEFAULT_DATETIME):
-        """Fetch the issues from the site.
+    def fetch(self, category=CATEGORY_MESSAGE, from_date=DEFAULT_DATETIME):
+        """Fetch the messages from a Groups.io group.
 
-        The method retrieves, from a JIRA site, the
-        issues updated since the given date.
+        The method fetches the mbox files from a remote Groups.io group
+        and retrieves the messages stored on them.
 
-        :param from_date: retrieve issues updated from this date
+        :param category: the category of items to fetch
+        :param from_date: obtain messages since this date
 
-        :returns: a generator of issues
+        :returns: a generator of messages
         """
-        if not from_date:
-            from_date = DEFAULT_DATETIME
-
-        logger.info("Looking for issues at site '%s', in project '%s' and updated from '%s'",
-                    self.url, self.project, str(from_date))
-
-        self._purge_cache_queue()
+        items = super().fetch(category, from_date)
 
-        from_date = datetime_to_utc(from_date)
+        return items
 
-        whole_pages = self.client.get_issues(from_date)
+    def fetch_items(self, category, **kwargs):
+        """Fetch the messages
 
-        fields = json.loads(self.client.get_fields())
-        custom_fields = filter_custom_fields(fields)
+        :param category: the category of items to fetch
+        :param kwargs: backend arguments
 
-        for whole_page in whole_pages:
-            self._push_cache_queue(whole_page)
-            self._flush_cache_queue()
-            issues = self.parse_issues(whole_page)
-            for issue in issues:
-                mapping = map_custom_field(custom_fields, issue['fields'])
-                for k, v in mapping.items():
-                    issue['fields'][k] = v
-                yield issue
+        :returns: a generator of items
+        """
+        from_date = kwargs['from_date']
 
-    @metadata
-    def fetch_from_cache(self):
-        """Fetch the issues from the cache.
+        logger.info("Looking for messages from '%s' since %s",
+                    self.uri, str(from_date))
 
-        :returns: a generator of issues
+        mailing_list = GroupsioClient(self.group_name, self.dirpath,
+                                      self.email, self.password, self.ssl_verify)
+        mailing_list.fetch(from_date)
 
-        :raises CacheError: raised when an error occurs accessing the
-            cache
-        """
-        if not self.cache:
-            raise CacheError(cause="cache instance was not provided")
+        messages = self._fetch_and_parse_messages(mailing_list, from_date)
 
-        cache_items = self.cache.retrieve()
+        for message in messages:
+            yield message
 
-        for items in cache_items:
-            issues = self.parse_issues(items)
-            for issue in issues:
-                yield issue
+        logger.info("Fetch process completed")
 
     @classmethod
-    def has_caching(cls):
-        """Returns whether it supports caching items on the fetch process.
+    def has_archiving(cls):
+        """Returns whether it supports archiving items on the fetch process.
 
-        :returns: this backend supports items cache
+        :returns: this backend does not support items archive
         """
-        return True
+        return False
 
     @classmethod
     def has_resuming(cls):
         """Returns whether it supports to resume the fetch process.
 
         :returns: this backend supports items resuming
         """
         return True
 
-    @staticmethod
-    def metadata_id(item):
-        """Extracts the identifier from a Jira item."""
 
-        return str(item['id'])
+class GroupsioClient(MailingList):
+    """Manage mailing list archives stored by Groups.io.
 
-    @staticmethod
-    def metadata_updated_on(item):
-        """Extracts the update time from a Jira item.
+    This class gives access to remote and local mboxes archives
+    from a mailing list stored by Groups.io. This class also allows
+    to keep them in sync.
+
+    :param group_name: Name of the group
+    :param dirpath: directory path where the mboxes are stored
+    :param email: Groupsio user email
+    :param password: Groupsio user password
+    :param ssl_verify: enable/disable SSL verification
+    """
+    # API resources
+    RDOWNLOAD_ARCHIVES = 'downloadarchives'
+    RGET_SUBSCRIPTIONS = 'getsubs'
+    RLOGIN = 'login'
+
+    # Resource parameters
+    PGROUP_ID = 'group_id'
+    PSTART_TIME = 'start_time'
+    PLIMIT = 'limit'
+    PPAGE_TOKEN = 'page_token'
+    PEMAIL = 'email'
+    PPASSWORD = 'password'
+
+    def __init__(self, group_name, dirpath, email, password, ssl_verify=True):
+        url = urijoin(GROUPSIO_URL, 'g', group_name)
+        super().__init__(url, dirpath)
+
+        self.session = requests.Session()
+        self.group_name = group_name
+        self.ssl_verify = ssl_verify
+        self.__login(email, password)
+
+    def fetch(self, from_date=None):
+        """Fetch the mbox files from the remote archiver.
+
+        Stores the archives in the path given during the initialization
+        of this object. Those archives which a not valid extension will
+        be ignored.
 
-        The timestamp used is extracted from 'updated' field.
-        This date is converted to UNIX timestamp format taking
-        into account the timezone of the date.
+        Groups.io archives are returned as a .zip file, which contains
+        one file in mbox format.
 
-        :param item: item generated by the backend
+        :param from_date: fetch messages after a given date (included) expressed in ISO format
 
-        :returns: a UNIX timestamp
+        :returns: a list of tuples, storing the links and paths of the
+            fetched archives
         """
-        ts = item['fields']['updated']
-        ts = str_to_datetime(ts)
+        logger.info("Downloading mboxes from '%s'", self.uri)
+        logger.debug("Storing mboxes in '%s'", self.dirpath)
 
-        return ts.timestamp()
+        if not os.path.exists(self.dirpath):
+            os.makedirs(self.dirpath)
 
-    @staticmethod
-    def metadata_category(item):
-        """Extracts the category from a Jira item.
-
-        This backend only generates one type of item which is
-        'issue'.
-        """
-        return 'issue'
+        group_id, group_download_archive = self.__find_group_info()
 
-    @staticmethod
-    def parse_issues(raw_page):
-        """Parse a JIRA API raw response.
+        if not group_download_archive:
+            msg = "Download archive permission disabled for the group %s" % self.group_name
+            logger.error(msg)
+            raise BackendError(cause=msg)
 
-        The method parses the API response retrieving the
-        issues from the received items
+        url = urijoin(GROUPSIO_API_URL, self.RDOWNLOAD_ARCHIVES)
+        payload = {
+            self.PGROUP_ID: group_id
+        }
 
-        :param items: items from where to parse the issues
+        if from_date:
+            payload[self.PSTART_TIME] = datetime_to_utc(from_date).isoformat()
 
-        :returns: a generator of issues
-        """
-        raw_issues = json.loads(raw_page)
-        issues = raw_issues['issues']
-        for issue in issues:
-            yield issue
-
-
-class JiraClient(HttpClient):
-    """JIRA API client.
-
-    This class implements a simple client to retrieve issues from
-    any JIRA issue tracking system.
-
-    :param URL: URL of the JIRA server
-    :param project: filter issues by project
-    :param user: JIRA's username
-    :param password: JIRA's password
-    :param verify: allows to disable SSL verification
-    :param cert: SSL certificate
-    :param max_issues: max number of issues per query
+        filepath = os.path.join(self.dirpath, MBOX_FILE)
+        success = self._download_archive(url, payload, filepath)
 
-    :raises HTTPError: when an error occurs doing the request
-    """
+        return success
 
-    EXPAND = 'renderedFields,transitions,operations,changelog'
-    VERSION_API = '2'
-    RESOURCE = 'rest/api'
-
-    def __init__(self, url, project, user, password, verify, cert, max_issues):
-        super().__init__(url)
-        self.project = project
-        self.user = user
-        self.password = password
-        self.verify = verify
-        self.cert = cert
-        self.max_issues = max_issues
-
-        self.__init_session()
-
-    def __build_jql_query(self, from_date):
-        AND_OP = 'AND'
-        UPDATED_OP = 'updated >'
-        PROJECT_OP = 'project ='
-        ORDER_BY_OP = 'order by'
-        ASC_OP = 'asc'
-
-        # Convert datetime to milliseconds since 1970-01-01.
-        # This allows us to use the timezone of the given date
-        strdate = str(int(from_date.timestamp() * 1000))
-
-        if self.project:
-            jql_query = ' '.join([PROJECT_OP, self.project, AND_OP,
-                                  UPDATED_OP, strdate])
-        else:
-            jql_query = ' '.join([UPDATED_OP, strdate])
+    def subscriptions(self, per_page=PER_PAGE):
+        """Fetch the groupsio paginated subscriptions for a given token
 
-        jql_query += ' '.join(['', ORDER_BY_OP, 'updated', ASC_OP])
+        :param per_page: number of subscriptions per page
 
-        return jql_query
+        :returns: an iterator of subscriptions
+        """
+        url = urijoin(GROUPSIO_API_URL, self.RGET_SUBSCRIPTIONS)
+        logger.debug("Get groupsio paginated subscriptions from " + url)
 
-    def __build_payload(self, start_at, from_date):
+        keep_fetching = True
         payload = {
-            'jql': self.__build_jql_query(from_date),
-            'startAt': start_at,
-            'expand': self.EXPAND,
-            'maxResults': self.max_issues
+            self.PLIMIT: per_page
         }
-        return payload
 
-    def __log_status(self, max_issues, total):
-        if (total != 0):
-            nissues = min(max_issues, total)
-            logger.info("Fetching issues: %s/%s" % (nissues,
-                                                    total))
-        else:
-            logger.info("No issues were found.")
+        while keep_fetching:
+            r = self.__fetch(url, payload)
+            response_raw = r.json()
+            subscriptions = response_raw['data']
+            yield subscriptions
+
+            total_subscriptions = response_raw['total_count']
+            logger.debug("Subscriptions: %i/%i" % (response_raw['end_item'], total_subscriptions))
+
+            payload[self.PPAGE_TOKEN] = response_raw['next_page_token']
+            keep_fetching = response_raw['has_more']
+
+    def _download_archive(self, url, payload, filepath):
+        r = self.session.get(url, params=payload, stream=True, verify=self.ssl_verify)
+        try:
+            r.raise_for_status()
+            self._write_archive(r, filepath)
+        except requests.exceptions.HTTPError as e:
+            logger.error("Impossible to download archives from %s. Error info: %s",
+                         self.uri, str(e.response.text))
+            raise e
+        except OSError as e:
+            logger.warning("Ignoring %s archive due to: %s", self.uri, str(e))
+            return False
 
-    def __init_session(self):
-        if (self.user and self.password) is not None:
-            self.session.auth = (self.user, self.password)
+        logger.debug("%s archive downloaded and stored in %s", self.uri, filepath)
 
-        if self.cert:
-            self.session.cert = self.cert
+        return True
 
-        if self.verify is not True:
-            requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
-            self.session.verify = False
+    @staticmethod
+    def _write_archive(r, filepath):
+        with open(filepath, 'wb') as fd:
+            fd.write(r.raw.read())
+
+    def __find_group_info(self):
+        """Find the id and download archive permission of a group given
+        its name by iterating on the list of subscriptions
+        """
+        group_subscriptions = self.subscriptions()
 
-    def get_issues(self, from_date):
-        """Retrieve all the issues from a given date.
+        for subscriptions in group_subscriptions:
+            for sub in subscriptions:
+                if sub['group_name'] == self.group_name:
+                    return sub['group_id'], sub['perms']['download_archives']
 
-        :param from_date: obtain issues updated since this date
-        """
-        start_at = 0
+        msg = "Group id not found for group name %s" % self.group_name
+        raise BackendError(cause=msg)
 
-        url = urijoin(self.base_url, self.RESOURCE, self.VERSION_API, 'search')
-        req = self.fetch(url, payload=self.__build_payload(start_at, from_date))
-        issues = req.text
+    def __fetch(self, url, payload):
+        """Fetch requests from groupsio API"""
 
-        data = req.json()
-        tissues = data['total']
-        nissues = data['maxResults']
+        r = self.session.get(url, params=payload, verify=self.ssl_verify)
+        try:
+            r.raise_for_status()
+        except requests.exceptions.HTTPError as e:
+            raise e
 
-        start_at += min(nissues, tissues)
-        self.__log_status(start_at, tissues)
+        return r
 
-        while issues:
-            yield issues
-            issues = None
+    def __login(self, email, password):
+        """Login a user to the server based on email and password.
 
-            if data['startAt'] + nissues < tissues:
-                req = self.fetch(url, payload=self.__build_payload(start_at, from_date))
+        :param email: Groupsio user email
+        :param password: Groupsio user password
+        """
+        url = urijoin(GROUPSIO_API_URL, self.RLOGIN)
 
-                data = req.json()
-                start_at += nissues
-                issues = req.text
-                self.__log_status(start_at, tissues)
+        payload = {
+            self.PEMAIL: email,
+            self.PPASSWORD: password
+        }
 
-    def get_fields(self):
-        """Retrieve all the fields available."""
+        self.session.post(url, params=payload)
+        logger.debug("Groupsio email %s authenticated in %s",
+                     email, GROUPSIO_API_URL)
 
-        url = urijoin(self.base_url, self.RESOURCE, self.VERSION_API, 'field')
-        req = self.fetch(url)
 
-        return req.text
+class GroupsioCommand(BackendCommand):
+    """Class to run Groupsio backend from the command line."""
 
+    BACKEND = Groupsio
 
-class JiraCommand(BackendCommand):
-    """Class to run Jira backend from the command line."""
+    def _pre_init(self):
+        """Initialize mailing lists directory path"""
 
-    BACKEND = Jira
+        if not self.parsed_args.mboxes_path:
+            base_path = os.path.expanduser('~/.perceval/mailinglists/')
+            dirpath = os.path.join(base_path, GROUPSIO_URL, 'g', self.parsed_args.group_name)
+        else:
+            dirpath = self.parsed_args.mboxes_path
 
-    @staticmethod
-    def setup_cmd_parser():
-        """Returns the Jira argument parser."""
+        setattr(self.parsed_args, 'dirpath', dirpath)
+
+    @classmethod
+    def setup_cmd_parser(cls):
+        """Returns the Groupsio argument parser."""
 
-        parser = BackendCommandArgumentParser(from_date=True,
-                                              basic_auth=True,
-                                              cache=True)
-
-        # JIRA options
-        group = parser.parser.add_argument_group('JIRA arguments')
-        group.add_argument('--project',
-                           help="filter issues by Project")
-        group.add_argument('--verify', default=True,
-                           help="Value 'False' disables SSL verification")
-        group.add_argument('--cert',
-                           help="SSL certificate path (PEM)")
-        group.add_argument('--max-issues', dest='max_issues',
-                           type=int, default=MAX_ISSUES,
-                           help="Maximum number of issues requested in the same query")
+        parser = BackendCommandArgumentParser(cls.BACKEND,
+                                              from_date=True,
+                                              ssl_verify=True)
+
+        # Optional arguments
+        group = parser.parser.add_argument_group('Groupsio arguments')
+        group.add_argument('--mboxes-path', dest='mboxes_path',
+                           help="Path where mbox files will be stored")
 
         # Required arguments
-        parser.parser.add_argument('url',
-                                   help="JIRA's url")
+        parser.parser.add_argument('group_name', help="Name of the group on Groups.io")
+        parser.parser.add_argument('-e', '--email', dest='email', help="Groupsio user email")
+        parser.parser.add_argument('-p', '--password', dest='password', help="Groupsio user password")
 
         return parser
```

### Comparing `perceval-0.9.9/perceval/backends/core/telegram.py` & `perceval-1.0.0rc1/perceval/backends/core/telegram.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,64 +1,49 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2017 Bitergia
+# Copyright (C) 2015-2020 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1335, USA.
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #     Santiago Dueñas <sduenas@bitergia.com>
+#     Stephan Barth <stephan.barth@gmail.com>
+#     Valerio Cosentino <valcos@bitergia.com>
+#     Jesus M. Gonzalez-Barahona <jgb@gsyc.es>
+#     Harshal Mittal <harshalmittal4@gmail.com>
 #
 
-import functools
 import json
 import logging
+import re
 
-from grimoirelab.toolkit.uris import urijoin
+from grimoirelab_toolkit.uris import urijoin
 
 from ...backend import (Backend,
                         BackendCommand,
-                        BackendCommandArgumentParser,
-                        metadata)
+                        BackendCommandArgumentParser)
 from ...client import HttpClient
-from ...errors import CacheError
-
-
-logger = logging.getLogger(__name__)
 
+CATEGORY_MESSAGE = "message"
 
 TELEGRAM_URL = 'https://telegram.org'
 DEFAULT_OFFSET = 1
 
-
-def telegram_metadata(func):
-    """Telegram metadata decorator.
-
-    This decorator takes an item and overrides `metadata` decorator
-    to add extra information related to Telegram.
-
-    Currently, it adds the 'offset' keyword.
-    """
-    @functools.wraps(func)
-    def decorator(self, *args, **kwargs):
-        for item in func(self, *args, **kwargs):
-            item['offset'] = item['data']['update_id']
-            yield item
-    return decorator
+logger = logging.getLogger(__name__)
 
 
 class Telegram(Backend):
     """Telegram backend.
 
     The Telegram backend fetches the messages that a Telegram bot can
     receive. Usually, these messages are direct or private messages but
@@ -74,68 +59,86 @@
 
     The origin of the data will be set to the `TELEGRAM_URL` plus the name
     of the bot; i.e 'http://telegram.org/mybot'.
 
     :param bot: name of the bot
     :param bot_token: authentication token used by the bot
     :param tag: label used to mark the data
-    :param cache: cache object to store raw data
+    :param archive: archive to store/retrieve items
+    :param ssl_verify: enable/disable SSL verification
     """
-    version = '0.6.0'
+    version = '1.0.0'
+
+    CATEGORIES = [CATEGORY_MESSAGE]
+    EXTRA_SEARCH_FIELDS = {
+        'chat_name': ['message', 'chat', 'title'],
+        'chat_id': ['message', 'chat', 'id']
+    }
 
-    def __init__(self, bot, bot_token, tag=None, cache=None):
+    def __init__(self, bot, bot_token, tag=None, archive=None, ssl_verify=True):
         origin = urijoin(TELEGRAM_URL, bot)
 
-        super().__init__(origin, tag=tag, cache=cache)
+        super().__init__(origin, tag=tag, archive=archive, ssl_verify=ssl_verify)
         self.bot = bot
-        self.client = TelegramBotClient(bot_token)
+        self.bot_token = bot_token
+
+        self.client = None
 
-    @telegram_metadata
-    @metadata
-    def fetch(self, offset=DEFAULT_OFFSET, chats=None):
+    def fetch(self, category=CATEGORY_MESSAGE, offset=DEFAULT_OFFSET, chats=None):
         """Fetch the messages the bot can read from the server.
 
         The method retrieves, from the Telegram server, the messages
         sent with an offset equal or greater than the given.
 
         A list of chats, groups and channels identifiers can be set
         using the parameter `chats`. When it is set, only those
         messages sent to any of these will be returned. An empty list
         will return no messages.
 
+        :param category: the category of items to fetch
         :param offset: obtain messages from this offset
         :param chats: list of chat names used to filter messages
 
         :returns: a generator of messages
 
         :raises ValueError: when `chats` is an empty list
         """
+        if not offset:
+            offset = DEFAULT_OFFSET
+
+        kwargs = {"offset": offset, "chats": chats}
+        items = super().fetch(category, **kwargs)
+
+        return items
+
+    def fetch_items(self, category, **kwargs):
+        """Fetch the messages
+
+        :param category: the category of items to fetch
+        :param kwargs: backend arguments
+
+        :returns: a generator of items
+        """
+        offset = kwargs['offset']
+        chats = kwargs['chats']
+
         logger.info("Looking for messages of '%s' bot from offset '%s'",
                     self.bot, offset)
 
         if chats is not None:
             if len(chats) == 0:
                 logger.warning("Chat list filter is empty. No messages will be returned")
             else:
                 logger.info("Messages which belong to chats %s will be fetched",
                             '[' + ','.join(str(ch_id) for ch_id in chats) + ']')
 
-        self._purge_cache_queue()
-
         nmsgs = 0
 
         while True:
             raw_json = self.client.updates(offset=offset)
-
-            # Due to Telegram deletes the messages from the server
-            # when they are fetched, the backend stores these messages
-            # in the cache before doing anything.
-            self._push_cache_queue(raw_json)
-            self._flush_cache_queue()
-
             messages = [msg for msg in self.parse_messages(raw_json)]
 
             if len(messages) == 0:
                 break
 
             for msg in messages:
                 offset = max(msg['update_id'], offset)
@@ -149,72 +152,35 @@
                 nmsgs += 1
 
             offset += 1
 
         logger.info("Fetch process completed: %s messages fetched",
                     nmsgs)
 
-    @telegram_metadata
-    @metadata
-    def fetch_from_cache(self):
-        """Fetch the messages from the cache.
-
-        It returns the messages stored in the cache object provided during
-        the initialization of the object. If this method is called but
-        no cache object was provided, the method will raise a `CacheError`
-        exception.
+    def metadata(self, item, filter_classified=False):
+        """Telegram metadata.
 
-        :returns: a generator of messages
-
-        :raises CacheError: raised when an error occurs accesing the
-            cache
-        """
-        if not self.cache:
-            raise CacheError(cause="cache instance was not provided")
-
-        logger.info("Retrieving cached messages: '%s'", self.bot)
-
-        cache_items = self.cache.retrieve()
-
-        nmsgs = 0
-
-        for raw_json in cache_items:
-            messages = [msg for msg in self.parse_messages(raw_json)]
-
-            for msg in messages:
-                yield msg
-                nmsgs += 1
-
-        logger.info("Retrieval process completed: %s messages retrieved from cache",
-                    nmsgs)
+        The method takes an item and overrides the `metadata` information
+        to add extra information related to Telegram.
 
-    def _filter_message_by_chats(self, message, chats):
-        """Check if a message can be filtered based in a list of chats.
-
-        This method returns `True` when the message was sent to a chat
-        of the given list. It also returns `True` when chats is `None`.
+        Currently, it adds the 'offset' keyword.
 
-        :param message: Telegram message
-        :param chats: list of chat, groups and channels identifiers
-
-        :returns: `True` when the message can be filtered; otherwise,
-            it returns `False`
+        :param item: an item fetched by a backend
+        :param filter_classified: sets if classified fields were filtered
         """
-        if chats is None:
-            return True
+        item = super().metadata(item, filter_classified=filter_classified)
+        item['offset'] = item['data']['update_id']
 
-        chat_id = message['message']['chat']['id']
-
-        return chat_id in chats
+        return item
 
     @classmethod
-    def has_caching(cls):
-        """Returns whether it supports caching items on the fetch process.
+    def has_archiving(cls):
+        """Returns whether it supports archiving items on the fetch process.
 
-        :returns: this backend supports items cache
+        :returns: this backend supports items archive
         """
         return True
 
     @classmethod
     def has_resuming(cls):
         """Returns whether it supports to resume the fetch process.
 
@@ -248,15 +214,15 @@
     @staticmethod
     def metadata_category(item):
         """Extracts the category from a Telegram item.
 
         This backend only generates one type of item which is
         'message'.
         """
-        return 'message'
+        return CATEGORY_MESSAGE
 
     @staticmethod
     def parse_messages(raw_json):
         """Parse a Telegram JSON messages list.
 
         The method parses the JSON stream and returns an iterator of
         dictionaries. Each one of this, contains a Telegram message.
@@ -265,33 +231,68 @@
 
         :returns: a generator of parsed messages
         """
         result = json.loads(raw_json)
 
         messages = result['result']
         for msg in messages:
+
+            if 'edited_message' in msg:
+                edit_message = msg.pop('edited_message')
+                edit_date = edit_message.pop('edit_date')
+                msg['message'] = edit_message
+                msg['message']['date'] = edit_date
+                msg['message']['edited'] = True
+                logger.debug("Message %s is edited", msg['message']['message_id'])
+
             yield msg
 
+    def _init_client(self, from_archive=False):
+        """Init client"""
+
+        return TelegramBotClient(self.bot_token, self.archive, from_archive, self.ssl_verify)
+
+    def _filter_message_by_chats(self, message, chats):
+        """Check if a message can be filtered based in a list of chats.
+
+        This method returns `True` when the message was sent to a chat
+        of the given list. It also returns `True` when chats is `None`.
+
+        :param message: Telegram message
+        :param chats: list of chat, groups and channels identifiers
+
+        :returns: `True` when the message can be filtered; otherwise,
+            it returns `False`
+        """
+        if chats is None:
+            return True
+
+        chat_id = message['message']['chat']['id']
+
+        return chat_id in chats
+
 
 class TelegramCommand(BackendCommand):
     """Class to run Telegram backend from the command line."""
 
     BACKEND = Telegram
 
-    @staticmethod
-    def setup_cmd_parser():
+    @classmethod
+    def setup_cmd_parser(cls):
         """Returns the Telegram argument parser."""
 
         aliases = {
             'bot_token': 'api_token'
         }
-        parser = BackendCommandArgumentParser(offset=True,
+        parser = BackendCommandArgumentParser(cls.BACKEND,
+                                              offset=True,
                                               token_auth=True,
-                                              cache=True,
-                                              aliases=aliases)
+                                              archive=True,
+                                              aliases=aliases,
+                                              ssl_verify=True)
 
         # Backend token is required
         action = parser.parser._option_string_actions['--api-token']
         action.required = True
 
         # Telegram options
         group = parser.parser.add_argument_group('Telegram arguments')
@@ -310,22 +311,25 @@
     """Telegram Bot API 2.0 client.
 
     This class implements a simple client to retrieve those messages
     sent to a Telegram bot. This includes personal messages or
     messages sent to a channel (when privacy settings are disabled).
 
     :param bot_token: token for the bot
+    :param archive: an archive to store/read fetched data
+    :param from_archive: it tells whether to write/read the archive
+    :param ssl_verify: enable/disable SSL verification
     """
     API_URL = "https://api.telegram.org/bot%(token)s/%(method)s"
 
     UPDATES_METHOD = 'getUpdates'
     OFFSET = 'offset'
 
-    def __init__(self, bot_token):
-        super().__init__(self.API_URL)
+    def __init__(self, bot_token, archive=None, from_archive=False, ssl_verify=True):
+        super().__init__(self.API_URL, archive=archive, from_archive=from_archive, ssl_verify=ssl_verify)
         self.bot_token = bot_token
 
     def updates(self, offset=None):
         """Fetch the messages that a bot can read.
 
         When the `offset` is given it will retrieve all the messages
         that are greater or equal to that offset. Take into account
@@ -339,18 +343,33 @@
         if offset:
             params[self.OFFSET] = offset
 
         response = self._call(self.UPDATES_METHOD, params)
 
         return response
 
+    @staticmethod
+    def sanitize_for_archive(url, headers, payload):
+        """Sanitize URL of a HTTP request by removing the token information
+        before storing/retrieving archived items
+
+        :param: url: HTTP url request
+        :param: headers: HTTP headers request
+        :param: payload: HTTP payload request
+
+        :returns the sanitized url, plus the headers and payload
+        """
+        url = re.sub('bot.*/', 'botXXXXX/', url)
+
+        return url, headers, payload
+
     def _call(self, method, params):
         """Retrive the given resource.
 
-        :param resource: resource to retrieve
+        :param method: resource to retrieve
         :param params: dict with the HTTP parameters needed to retrieve
             the given resource
         """
         url = self.base_url % {'token': self.bot_token, 'method': method}
 
         logger.debug("Telegram bot calls method: %s params: %s",
                      method, str(params))
```

### Comparing `perceval-0.9.9/perceval/backends/core/askbot.py` & `perceval-1.0.0rc1/perceval/backends/core/askbot.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,87 +1,111 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2016-2017 Bitergia
+# Copyright (C) 2015-2020 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1335, USA.
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #     Alberto Martín <alberto.martin@bitergia.com>
 #     Santiago Dueñas <sduenas@bitergia.com>
+#     Stephan Barth <stephan.barth@gmail.com>
+#     Valerio Cosentino <valcos@bitergia.com>
+#     Jesus M. Gonzalez-Barahona <jgb@gsyc.es>
+#     Harshal Mittal <harshalmittal4@gmail.com>
+#     animesh <animuz111@gmail.com>
 #
 
 import json
 import logging
 import re
 
 import bs4
 import requests
 
-from grimoirelab.toolkit.datetime import datetime_to_utc, str_to_datetime
-from grimoirelab.toolkit.uris import urijoin
+from grimoirelab_toolkit.datetime import datetime_to_utc, str_to_datetime
+from grimoirelab_toolkit.uris import urijoin
 
 from ...backend import (Backend,
                         BackendCommand,
-                        BackendCommandArgumentParser,
-                        metadata)
+                        BackendCommandArgumentParser)
 from ...client import HttpClient
 from ...utils import DEFAULT_DATETIME
 
+CATEGORY_QUESTION = 'question'
 
 logger = logging.getLogger(__name__)
 
 
 class Askbot(Backend):
     """Askbot backend.
 
-    This class retrieves the questions posted in an Askbot site.
+    This class retrieves the questions posted on an Askbot site.
     To initialize this class the URL must be provided. The `url`
     will be set as the origin of the data.
 
     :param url: Askbot site URL
     :param tag: label used to mark the data
+    :param archive: archive to store/retrieve items
+    :param ssl_verify: enable/disable SSL verification
     """
-    version = '0.3.0'
+    version = '1.0.0'
 
-    def __init__(self, url, tag=None):
+    CATEGORIES = [CATEGORY_QUESTION]
+    EXTRA_SEARCH_FIELDS = {
+        'tags': ['tags']
+    }
+
+    def __init__(self, url, tag=None, archive=None, ssl_verify=True):
         origin = url
 
-        super().__init__(origin, tag=tag)
+        super().__init__(origin, tag=tag, archive=archive, ssl_verify=ssl_verify)
         self.url = url
-        self.client = AskbotClient(url)
+        self.client = None
         self.ab_parser = AskbotParser()
 
-    @metadata
-    def fetch(self, from_date=DEFAULT_DATETIME):
+    def fetch(self, category=CATEGORY_QUESTION, from_date=DEFAULT_DATETIME):
         """Fetch the questions/answers from the repository.
 
         The method retrieves, from an Askbot site, the questions and answers
         updated since the given date.
 
+        :param category: the category of items to fetch
         :param from_date: obtain questions/answers updated since this date
 
         :returns: a generator of items
         """
-
         if not from_date:
             from_date = DEFAULT_DATETIME
+        logger.info(f"Pulling Askbot data from {from_date}")
+        kwargs = {'from_date': from_date}
+        items = super().fetch(category, **kwargs)
+
+        return items
+
+    def fetch_items(self, category, **kwargs):
+        """Fetch the questions
 
-        from_date = datetime_to_utc(from_date).timestamp()
+        :param category: the category of items to fetch
+        :param kwargs: backend arguments
+
+        :returns: a generator of items
+        """
+
+        from_date = datetime_to_utc(kwargs['from_date']).timestamp()
 
         questions_groups = self.client.get_api_questions(AskbotClient.API_QUESTIONS)
         for questions in questions_groups:
 
             for question in questions['questions']:
                 updated_at = int(question['last_activity_at'])
                 if updated_at > from_date:
@@ -91,107 +115,112 @@
 
                     logger.debug("Fetching HTML question %s", question['id'])
                     comments = self.__fetch_comments(question)
                     question_obj = self.__build_question(html_question, question, comments)
                     question.update(question_obj)
                     yield question
 
+    @classmethod
+    def has_resuming(cls):
+        """Returns whether it supports to resume the fetch process.
+
+        :returns: this backend supports items resuming
+        """
+        return True
+
+    @classmethod
+    def has_archiving(cls):
+        """Returns whether it supports archiving items on the fetch process.
+
+        :returns: this backend supports items archive
+        """
+        return True
+
+    @staticmethod
+    def metadata_category(item):
+        """Extracts the category from an Askbot item.
+
+        This backend only generates one type of item which is
+        'question'.
+        """
+        return CATEGORY_QUESTION
+
+    @staticmethod
+    def metadata_id(item):
+        """Extracts the identifier from an Askbot question item."""
+
+        return str(item['id'])
+
+    @staticmethod
+    def metadata_updated_on(item):
+        """Extracts the update time from an Askbot item.
+
+        The timestamp is extracted from 'last_activity_at' field.
+        This date is a UNIX timestamp but needs to be converted to
+        a float value.
+
+        :param item: item generated by the backend
+
+        :returns: a UNIX timestamp
+        """
+        return float(item['last_activity_at'])
+
+    def _init_client(self, from_archive=False):
+        """Init client"""
+
+        return AskbotClient(self.url, self.archive, from_archive, self.ssl_verify)
+
     def __fetch_question(self, question):
         """Fetch an Askbot HTML question body.
 
-        The method fetchs the HTML question retrieving the
+        The method fetches the HTML question retrieving the
         question body of the item question received
 
         :param question: item with the question itself
 
         :returns: a list of HTML page/s for the question
         """
-
         html_question_items = []
 
         npages = 1
         next_request = True
 
         while next_request:
             try:
                 html_question = self.client.get_html_question(question['id'], npages)
                 html_question_items.append(html_question)
                 tpages = self.ab_parser.parse_number_of_html_pages(html_question)
-
+                logger.info(f"{tpages} of questions found")
                 if npages == tpages:
                     next_request = False
 
                 npages = npages + 1
             except requests.exceptions.TooManyRedirects as e:
                 logger.warning("%s, data not retrieved for question %s", e, question['id'])
                 next_request = False
 
         return html_question_items
 
     def __fetch_comments(self, question):
         """Fetch all the comments of an Askbot question and answers.
 
-        The method fetchs the list of every comment existing in a question and
+        The method fetches the list of every comment existing in a question and
         its answers.
 
         :param question: item with the question itself
 
         :returns: a list of comments with the ids as hashes
         """
         comments = {}
         comments[question['id']] = json.loads(self.client.get_comments(question['id']))
         for object_id in question['answer_ids']:
             comments[object_id] = json.loads(self.client.get_comments(object_id))
+        logger.debug(f"{len(comments)} comments found")
         return comments
 
-    @classmethod
-    def has_resuming(cls):
-        """Returns whether it supports to resume the fetch process.
-
-        :returns: this backend supports items resuming
-        """
-        return True
-
-    @classmethod
-    def has_caching(cls):
-        """Returns whether it supports caching items on the fetch process.
-
-        :returns: this backend does not support items cache
-        """
-        return False
-
-    @staticmethod
-    def metadata_category(item):
-        """Extracts the category from an Askbot item.
-
-        This backend only generates one type of item which is
-        'question'.
-        """
-        return 'question'
-
-    @staticmethod
-    def metadata_id(item):
-        """Extracts the identifier from an Askbot question item."""
-
-        return str(item['id'])
-
-    @staticmethod
-    def metadata_updated_on(item):
-        """Extracts the update time from an Askbot item.
-
-        The timestamp is extracted from 'last_activity_at' field.
-        This date is a UNIX timestamp but needs to be converted to
-        a float value.
-
-        :param item: item generated by the backend
-
-        :returns: a UNIX timestamp
-        """
-        return float(item['last_activity_at'])
-
     @staticmethod
     def __build_question(html_question, question, comments):
         """Build an Askbot HTML response.
 
         The method puts together all the information regarding a question
 
         :param html_question: array of HTML raw pages
@@ -226,45 +255,64 @@
 class AskbotClient(HttpClient):
     """Askbot client.
 
     This class implements a simple client to retrieve distinct
     kind of data from an Askbot site.
 
     :param base_url: URL of the Askbot site
+    :param archive: an archive to store/read fetched data
+    :param from_archive: it tells whether to write/read the archive
+    :param ssl_verify: enable/disable SSL verification
 
     :raises HTTPError: when an error occurs doing the request
     """
 
     API_QUESTIONS = 'api/v1/questions/'
-    HTML_QUESTION = 'question/'
-    ORDER_API = 'activity-asc'
-    ORDER_HTML = 'votes'
-    COMMENTS = 's/post_comments'
-    COMMENTS_OLD = 'post_comments'
 
-    def __init__(self, base_url):
-        super().__init__(base_url)
+    # API resources
+    RHTML_QUESTION = 'question/'
+    RCOMMENTS = 's/post_comments'
+    RCOMMENTS_OLD = 'post_comments'
+
+    # API header
+    HREQUEST_WITH = 'X-Requested-With'
+
+    # Resource parameters
+    PPAGE = 'page'
+    PSORT = 'sort'
+    PPOST_ID = 'post_id'
+    PPOST_TYPE = 'post_type'
+    PAVATAR_SIZE = 'avatar_size'
+
+    # Predefined values
+    VORDER_API = 'activity-asc'
+    VORDER_HTML = 'votes'
+    VANSWER = 'answer'
+    VAVATAR_SIZE = 0
+    VHTTP_REQUEST = 'XMLHttpRequest'
+
+    def __init__(self, base_url, archive=None, from_archive=False, ssl_verify=True):
+        super().__init__(base_url, archive=archive, from_archive=from_archive, ssl_verify=ssl_verify)
         self._use_new_urls = True
 
     def get_api_questions(self, path):
         """Retrieve a question page using the API.
 
         :param page: page to retrieve
         """
-
         npages = 1
         next_request = True
-
+        logger.debug("Retrieving question pages")
         path = urijoin(self.base_url, path)
         while next_request:
 
             try:
                 params = {
-                    'page': npages,
-                    'sort': self.ORDER_API
+                    self.PPAGE: npages,
+                    self.PSORT: self.VORDER_API
                 }
 
                 response = self.fetch(path, payload=params)
 
                 whole_page = response.text
 
                 raw_questions = json.loads(whole_page)
@@ -285,48 +333,54 @@
 
     def get_html_question(self, question_id, page=1):
         """Retrieve a raw HTML question and all it's information.
 
         :param question_id: question identifier
         :param page: page to retrieve
         """
-        path = urijoin(self.base_url, self.HTML_QUESTION, question_id)
+        path = urijoin(self.base_url, self.RHTML_QUESTION, question_id)
+        logger.debug(f"Raw html retrieved: {path}")
         params = {
-            'page': page,
-            'sort': self.ORDER_HTML
+            self.PPAGE: page,
+            self.PSORT: self.VORDER_HTML
         }
 
         response = self.fetch(path, payload=params)
         return response.text
 
     def get_comments(self, post_id):
         """Retrieve a list of comments by a given id.
 
         :param object_id: object identifiere
         """
-        path = urijoin(self.base_url, self.COMMENTS if self._use_new_urls else self.COMMENTS_OLD)
+        path = urijoin(self.base_url, self.RCOMMENTS if self._use_new_urls else self.RCOMMENTS_OLD)
         params = {
-            'post_id': post_id,
-            'post_type': 'answer',
-            'avatar_size': 0
+            self.PPOST_ID: post_id,
+            self.PPOST_TYPE: self.VANSWER,
+            self.PAVATAR_SIZE: self.VAVATAR_SIZE
         }
-        headers = {'X-Requested-With': 'XMLHttpRequest'}
+        headers = {self.HREQUEST_WITH: self.VHTTP_REQUEST}
 
         try:
             response = self.fetch(path, payload=params, headers=headers)
+            raw = response.text
         except requests.exceptions.HTTPError as ex:
             if ex.response.status_code == 404:
                 logger.debug("Comments URL did not work. Using old URL schema.")
                 self._use_new_urls = False
-                path = urijoin(self.base_url, self.COMMENTS_OLD)
+                path = urijoin(self.base_url, self.RCOMMENTS_OLD)
                 response = self.fetch(path, payload=params, headers=headers)
+                raw = response.text
+            elif ex.response.status_code == 500:
+                logger.warning("Comments not retrieved due to %s", ex)
+                raw = '[]'
             else:
                 raise ex
 
-        return response.text
+        return raw
 
 
 class AskbotParser:
     """Askbot HTML parser.
 
     This class parses a plain HTML document, converting questions, answers,
     comments and user information into dict items.
@@ -334,16 +388,16 @@
 
     @staticmethod
     def parse_question_container(html_question):
         """Parse the question info container of a given HTML question.
 
         The method parses the information available in the question information
         container. The container can have up to 2 elements: the first one
-        contains the information related with the user who generated the question
-        and the date (if any). The second one contains the date of the updated,
+        contains the information related to the user who generated the question
+        and the date (if any). The second one contains the date of the update
         and the user who updated it (if not the same who generated the question).
 
         :param html_question: raw HTML question element
 
         :returns: an object with the parsed information
         """
         container_info = {}
@@ -356,15 +410,15 @@
             container[1]
         except IndexError:
             pass
         else:
             updated = container[1]
             if AskbotParser.parse_user_info(updated):
                 container_info['updated_by'] = AskbotParser.parse_user_info(updated)
-
+        logger.debug("Container info parsed")
         return container_info
 
     @staticmethod
     def parse_answers(html_question):
         """Parse the answers of a given HTML question.
 
         The method parses the answers related with a given HTML question,
@@ -376,16 +430,16 @@
         """
 
         def parse_answer_container(update_info):
             """Parse the answer info container of a given HTML question.
 
             The method parses the information available in the answer information
             container. The container can have up to 2 elements: the first one
-            contains the information related with the user who generated the question
-            and the date (if any). The second one contains the date of the updated,
+            contains the information related to the user who generated the question
+            and the date (if any). The second one contains the date of the update
             and the user who updated it (if not the same who generated the question).
 
             :param update_info: beautiful soup update_info container element
 
             :returns: an object with the parsed information
             """
             container_info = {}
@@ -407,34 +461,38 @@
                     container_info['updated_by'] = AskbotParser.parse_user_info(updated)
             return container_info
 
         answer_list = []
         # Select all the answers
         bs_question = bs4.BeautifulSoup(html_question, "html.parser")
         bs_answers = bs_question.select("div.answer")
+        logger.debug(f"{str(len(bs_answers))} answers found")
         for bs_answer in bs_answers:
             answer_id = bs_answer.attrs["data-post-id"]
             votes_element = bs_answer.select("div.vote-number")[0].text
+            accepted_answer = bs_answer.select("div.answer-img-accept")[0].get('title').endswith("correct")
             # Select the body of the answer
             body = bs_answer.select("div.post-body")
             # Get the user information container and parse it
             update_info = body[0].select("div.post-update-info")
             answer_container = parse_answer_container(update_info)
             # Remove the update-info-container div to be able to get the body
             body[0].div.extract().select("div.post-update-info-container")
             # Override the body with a clean one
             body = body[0].get_text(strip=True)
             # Generate the answer object
             answer = {'id': answer_id,
                       'score': votes_element,
-                      'summary': body
+                      'summary': body,
+                      'accepted': accepted_answer
                       }
             # Update the object with the information in the answer container
             answer.update(answer_container)
             answer_list.append(answer)
+        logger.debug("Answers parsed")
         return answer_list
 
     @staticmethod
     def parse_number_of_html_pages(html_question):
         """Parse number of answer pages to paginate over them.
 
         :param html_question: raw HTML question element
@@ -464,33 +522,29 @@
         """
         user_info = {}
         if update_info.select("div.user-info"):
             # Get all the <a> elements in the container. First <a> contains the user
             # information, second one (if exists), the website of the user.
             elements = update_info.select("div.user-info")[0].find_all("a")
             href = elements[0].attrs["href"]
-            user_info['id'] = re.search('\d+', href).group(0)
+            user_info['id'] = re.search(r'\d+', href).group(0)
             user_info['username'] = elements[0].text
             user_info['reputation'] = update_info.select('span.reputation-score')[0].text
             user_info['badges'] = update_info.select("span.badges")[0].attrs["title"]
             try:
                 elements[1]
             except IndexError:
                 pass
             else:
                 user_info['website'] = elements[1].attrs["href"]
             if update_info.select("img.flag"):
                 flag = update_info.select("img.flag")[0].attrs["alt"]
                 user_info['country'] = re.sub("flag of ", "", flag)
-            return user_info
-        elif update_info.select("p.tip"):
-            user_info = "This post is a wiki"
-            return user_info
-        else:
-            return
+        logger.debug("User info parsed")
+        return user_info
 
     @staticmethod
     def _find_question_container(bs_question):
         questions = bs_question.find_all("div",
                                          attrs={'class': re.compile(".*question")})
         for question in questions:
             if 'post' in question.attrs['class']:
@@ -498,18 +552,21 @@
 
 
 class AskbotCommand(BackendCommand):
     """Class to run Askbot backend from the command line."""
 
     BACKEND = Askbot
 
-    @staticmethod
-    def setup_cmd_parser():
+    @classmethod
+    def setup_cmd_parser(cls):
         """Returns the Askbot argument parser."""
 
-        parser = BackendCommandArgumentParser(from_date=True)
+        parser = BackendCommandArgumentParser(cls.BACKEND,
+                                              from_date=True,
+                                              archive=True,
+                                              ssl_verify=True)
 
         # Required arguments
         parser.parser.add_argument('url',
                                    help="URL of the Askbot server")
 
         return parser
```

### Comparing `perceval-0.9.9/perceval/backends/core/nntp.py` & `perceval-1.0.0rc1/perceval/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,295 +1,273 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2017 Bitergia
+# Copyright (C) 2015-2020 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1335, USA.
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #     Santiago Dueñas <sduenas@bitergia.com>
+#     Germán Poo-Caamaño <gpoo@gnome.org>
+#     Stephan Barth <stephan.barth@gmail.com>
+#     anveshc05 <anveshc10047@gmail.com>
+#     Valerio Cosentino <valcos@bitergia.com>
+#     Harshal Mittal <harshalmittal4@gmail.com>
 #
 
-import functools
-import io
+import datetime
+import email
 import logging
-import nntplib
+import mailbox
+import re
+import sys
 
-import email.parser
+import xml.etree.ElementTree
 
-from grimoirelab.toolkit.datetime import str_to_datetime
+import dateutil.rrule
+import dateutil.tz
 
-from ...backend import (Backend,
-                        BackendCommand,
-                        BackendCommandArgumentParser,
-                        metadata)
-from ...errors import CacheError, ParseError
-from ...utils import message_to_dict
+import requests
 
+from .errors import ParseError
 
-# Hack to avoid "line too long" errors
-nntplib._MAXLINE = 4096
 
 logger = logging.getLogger(__name__)
 
-DEFAULT_OFFSET = 1
 
+DEFAULT_DATETIME = datetime.datetime(1970, 1, 1, 0, 0, 0,
+                                     tzinfo=dateutil.tz.tzutc())
+DEFAULT_LAST_DATETIME = datetime.datetime(2100, 1, 1, 0, 0, 0,
+                                          tzinfo=dateutil.tz.tzutc())
 
-def nntp_metadata(func):
-    """NNTP metadata decorator.
 
-    This decorator takes items, overriding `metadata` decorator,
-    to add extra information related to NNTP.
-    """
-    @functools.wraps(func)
-    def decorator(self, *args, **kwargs):
-        for item in func(self, *args, **kwargs):
-            item['offset'] = item['data']['offset']
-            yield item
-    return decorator
-
-
-class NNTP(Backend):
-    """NNTP backend.
-
-    This class allows to fetch the articles published on a news group
-    using NNTP. It is initialized giving the host and the name of the
-    news group.
-
-    :param host: host
-    :param group: name of the group
-    :param tag: label used to mark the data
-    :param cache: cache object to store raw data
-    """
-    version = '0.2.5'
-
-    def __init__(self, host, group, tag=None, cache=None):
-        origin = host + '-' + group
-
-        super().__init__(origin, tag=tag, cache=cache)
-        self.host = host
-        self.group = group
-
-    @nntp_metadata
-    @metadata
-    def fetch(self, offset=DEFAULT_OFFSET):
-        """Fetch articles posted on a news group.
-
-        This method fetches those messages or articles published
-        on a news group starting on the given offset.
-
-        :param offset: obtain messages from this offset
-
-        :returns: a generator of articles
-        """
-        logger.info("Fetching articles of '%s' group on '%s' offset %s",
-                    self.group, self.host, str(offset))
-
-        self._purge_cache_queue()
-
-        narts, iarts, tarts = (0, 0, 0)
-
-        # Connect with the server and select the given group
-        with nntplib.NNTP(self.host) as client:
-            _, _, first, last, _ = client.group(self.group)
-
-            if offset <= last:
-                first = max(first, offset)
-                _, overview = client.over((first, last))
-            else:
-                overview = []
+def check_compressed_file_type(filepath):
+    """Check if filename is a compressed file supported by the tool.
 
-            tarts = len(overview)
+    This function uses magic numbers (first four bytes) to determine
+    the type of the file. Supported types are 'gz' and 'bz2'. When
+    the filetype is not supported, the function returns `None`.
 
-            logger.debug("Total number of articles to fetch: %s", tarts)
+    :param filepath: path to the file
 
-            for article_id, _ in overview:
-                try:
-                    article = self.__fetch_and_parse_article(client, article_id)
-                except ParseError:
-                    logger.warning("Error parsing %s article; skipping",
-                                   article_id)
-                    iarts += 1
-                    continue
-                except nntplib.NNTPTemporaryError as e:
-                    logger.warning("Error '%s' fetching article %s; skipping",
-                                   e.response, article_id)
-                    iarts += 1
-                    continue
-
-                yield article
-                narts += 1
-
-                self._flush_cache_queue()
-
-        logger.info("Fetch process completed: %s/%s articles fetched; %s ignored",
-                    narts, tarts, iarts)
+    :returns: 'gz' or 'bz2'; `None` if the type is not supported
+    """
+    def compressed_file_type(content):
+        magic_dict = {
+            b'\x1f\x8b\x08': 'gz',
+            b'\x42\x5a\x68': 'bz2',
+            b'PK\x03\x04': 'zip'
+        }
 
-    @nntp_metadata
-    @metadata
-    def fetch_from_cache(self):
-        """Fetch the articles from the cache.
+        for magic, filetype in magic_dict.items():
+            if content.startswith(magic):
+                return filetype
 
-        It returns the articles stored in the cache object, provided during
-        the initialization of the object. If this method is called but
-        no cache object was provided, the method will raise a `CacheError`
-        exception.
+        return None
 
-        :returns: a generator of articles
+    with open(filepath, mode='rb') as f:
+        magic_number = f.read(4)
+    return compressed_file_type(magic_number)
 
-        :raises CacheError: raised when an error occurs accessing the
-            cache
-        """
-        if not self.cache:
-            raise CacheError(cause="cache instance was not provided")
 
-        logger.info("Retrieving cached articles of '%s' group on '%s'",
-                    self.group, self.host)
+def months_range(from_date, to_date):
+    """Generate a months range.
 
-        cache_items = self.cache.retrieve()
+    Generator of months starting on `from_date` util `to_date`. Each
+    returned item is a tuple of two datatime objects like in (month, month+1).
+    Thus, the result will follow the sequence:
+        ((fd, fd+1), (fd+1, fd+2), ..., (td-2, td-1), (td-1, td))
 
-        narts = 0
+    :param from_date: generate dates starting on this month
+    :param to_date: generate dates until this month
 
-        for raw_item in cache_items:
-            reader = io.BytesIO(b'\n'.join(raw_item['lines']))
-            raw_article = reader.read().decode('utf-8', errors='surrogateescape')
-            data = self.parse_article(raw_article)
+    :result: a generator of months range
+    """
+    start = datetime.datetime(from_date.year, from_date.month, 1)
+    end = datetime.datetime(to_date.year, to_date.month, 1)
 
-            article = self.__build_article(data,
-                                           raw_item['message_id'],
-                                           raw_item['number'])
+    month_gen = dateutil.rrule.rrule(freq=dateutil.rrule.MONTHLY,
+                                     dtstart=start, until=end)
+    months = [d for d in month_gen]
 
-            yield article
-            narts += 1
+    pos = 0
+    for x in range(1, len(months)):
+        yield months[pos], months[x]
+        pos = x
 
-        logger.info("Retrieval process completed: %s articles retrieved from cache",
-                    narts)
 
-    def __fetch_and_parse_article(self, client, article_id):
-        _, info = client.article(article_id)
+def message_to_dict(msg):
+    """Convert an email message into a dictionary.
 
-        # Store data on the cache
-        cache_data = {
-            'number': info.number,
-            'message_id': info.message_id,
-            'lines': info.lines
-        }
-        self._push_cache_queue(cache_data)
+    This function transforms an `email.message.Message` object
+    into a dictionary. Headers are stored as key:value pairs
+    while the body of the message is stored inside `body` key.
+    Body may have two other keys inside, 'plain', for plain body
+    messages and 'html', for HTML encoded messages.
 
-        # Parse article data
-        reader = io.BytesIO(b'\n'.join(info.lines))
-        raw_article = reader.read().decode('utf-8', errors='surrogateescape')
-        data = self.parse_article(raw_article)
+    The returned dictionary has the type `requests.structures.CaseInsensitiveDict`
+    due to same headers with different case formats can appear in
+    the same message.
 
-        article = self.__build_article(data,
-                                       info.message_id,
-                                       info.number)
+    :param msg: email message of type `email.message.Message`
 
-        logger.debug("Article %s (offset: %s) parsed",
-                     article['message_id'], article['offset'])
+    :returns : dictionary of type `requests.structures.CaseInsensitiveDict`
 
-        return article
+    :raises ParseError: when an error occurs transforming the message
+        to a dictionary
+    """
+    def parse_headers(msg):
+        headers = {}
 
-    def __build_article(self, article, message_id, offset):
-        a = {k: v for k, v in article.items()}
-        a['message_id'] = message_id
-        a['offset'] = offset
-        return a
+        for header, value in msg.items():
+            hv = []
 
-    @classmethod
-    def has_caching(cls):
-        """Returns whether it supports caching items on the fetch process.
+            for text, charset in email.header.decode_header(value):
+                if type(text) == bytes:
+                    charset = charset if charset else 'utf-8'
+                    try:
+                        text = text.decode(charset, errors='surrogateescape')
+                    except (UnicodeError, LookupError):
+                        # Try again with a 7bit encoding
+                        text = text.decode('ascii', errors='surrogateescape')
+                hv.append(text)
+
+            v = ' '.join(hv)
+            headers[header] = v if v else None
+
+        return headers
+
+    def parse_payload(msg):
+        body = {}
+
+        if not msg.is_multipart():
+            payload = decode_payload(msg)
+            subtype = msg.get_content_subtype()
+            body[subtype] = [payload]
+        else:
+            # Include all the attached texts if it is multipart
+            # Ignores binary parts by default
+            for part in email.iterators.typed_subpart_iterator(msg):
+                payload = decode_payload(part)
+                subtype = part.get_content_subtype()
+                body.setdefault(subtype, []).append(payload)
+
+        return {k: '\n'.join(v) for k, v in body.items()}
+
+    def decode_payload(msg_or_part):
+        charset = msg_or_part.get_content_charset('utf-8')
+        payload = msg_or_part.get_payload(decode=True)
 
-        :returns: this backend supports items cache
-        """
-        return True
+        try:
+            payload = payload.decode(charset, errors='surrogateescape')
+        except (UnicodeError, LookupError):
+            # Try again with a 7bit encoding
+            payload = payload.decode('ascii', errors='surrogateescape')
+        return payload
+
+    # The function starts here
+    message = requests.structures.CaseInsensitiveDict()
+
+    if isinstance(msg, mailbox.mboxMessage):
+        message['unixfrom'] = msg.get_from()
+    else:
+        message['unixfrom'] = None
+
+    try:
+        for k, v in parse_headers(msg).items():
+            message[k] = v
+        message['body'] = parse_payload(msg)
+    except UnicodeError as e:
+        raise ParseError(cause=str(e))
+
+    return message
+
+
+def remove_invalid_xml_chars(raw_xml):
+    """Remove control and invalid characters from an xml stream.
+
+    Looks for invalid characters and subtitutes them with whitespaces.
+    This solution is based on these two posts: Olemis Lang's reponse
+    on StackOverflow (http://stackoverflow.com/questions/1707890) and
+    lawlesst's on GitHub Gist (https://gist.github.com/lawlesst/4110923),
+    that is based on the previous answer.
 
-    @classmethod
-    def has_resuming(cls):
-        """Returns whether it supports to resume the fetch process.
+    :param xml: XML stream
 
-        :returns: this backend supports items resuming
-        """
-        return True
+    :returns: a purged XML stream
+    """
+    illegal_unichrs = [(0x00, 0x08), (0x0B, 0x1F),
+                       (0x7F, 0x84), (0x86, 0x9F)]
 
-    @staticmethod
-    def metadata_id(item):
-        """Extracts the identifier from a NNTP item."""
+    illegal_ranges = ['%s-%s' % (chr(low), chr(high))
+                      for (low, high) in illegal_unichrs
+                      if low < sys.maxunicode]
 
-        return item['message_id']
+    illegal_xml_re = re.compile('[%s]' % ''.join(illegal_ranges))
 
-    @staticmethod
-    def metadata_updated_on(item):
-        """Extracts the update time from a NNTP item.
+    purged_xml = ''
 
-        The timestamp is extracted from 'Date' field and
-        converted to a UNIX timestamp.
+    for c in raw_xml:
+        if illegal_xml_re.search(c) is not None:
+            c = ' '
+        purged_xml += c
 
-        :param item: item generated by the backend
+    return purged_xml
 
-        :returns: a UNIX timestamp
-        """
-        ts = item['Date']
-        ts = str_to_datetime(ts)
 
-        return ts.timestamp()
+def xml_to_dict(raw_xml):
+    """Convert a XML stream into a dictionary.
 
-    @staticmethod
-    def metadata_category(item):
-        """Extracts the category from a NNTP item.
+    This function transforms a xml stream into a dictionary. The
+    attributes are stored as single elements while child nodes are
+    stored into lists. The text node is stored using the special
+    key '__text__'.
 
-        This backend only generates one type of item which is
-        'article'.
-        """
-        return 'article'
+    This code is based on Winston Ewert's solution to this problem.
+    See http://codereview.stackexchange.com/questions/10400/convert-elementtree-to-dict
+    for more info. The code was licensed as cc by-sa 3.0.
 
-    @staticmethod
-    def parse_article(raw_article):
-        """Parse a NNTP article.
+    :param raw_xml: XML stream
 
-        This method parses a NNTP article stored in a string object
-        and returns an dictionary.
+    :returns: a dict with the XML data
 
-        :param raw_article: NNTP article string
+    :raises ParseError: raised when an error occurs parsing the given
+        XML stream
+    """
+    def node_to_dict(node):
+        d = {}
+        d.update(node.items())
 
-        :returns: a dictionary of type `requests.structures.CaseInsensitiveDict`
+        text = getattr(node, 'text', None)
 
-        :raises ParseError: when an error is found parsing the article
-        """
-        try:
-            message = email.message_from_string(raw_article)
-            article = message_to_dict(message)
-        except UnicodeEncodeError as e:
-            raise ParseError(cause=str(e))
-        return article
+        if text is not None:
+            d['__text__'] = text
 
+        childs = {}
+        for child in node:
+            childs.setdefault(child.tag, []).append(node_to_dict(child))
 
-class NNTPCommand(BackendCommand):
-    """Class to run NNTP backend from the command line."""
+        d.update(childs.items())
 
-    BACKEND = NNTP
+        return d
 
-    @staticmethod
-    def setup_cmd_parser():
-        """Returns the NNTP argument parser."""
+    purged_xml = remove_invalid_xml_chars(raw_xml)
 
-        parser = BackendCommandArgumentParser(offset=True,
-                                              cache=True)
+    try:
+        tree = xml.etree.ElementTree.fromstring(purged_xml)
+    except xml.etree.ElementTree.ParseError as e:
+        cause = "XML stream %s" % (str(e))
+        raise ParseError(cause=cause)
 
-        # Required arguments
-        parser.parser.add_argument('host',
-                                   help="NNTP server host")
-        parser.parser.add_argument('group',
-                                   help="Name of the NNTP group")
+    d = node_to_dict(tree)
 
-        return parser
+    return d
```

### Comparing `perceval-0.9.9/perceval/backends/core/meetup.py` & `perceval-1.0.0rc1/perceval/backends/core/meetup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,248 +1,189 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2017 Bitergia
+# Copyright (C) 2015-2020 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1335, USA.
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
+#     Valerio Cosentino <valcos@bitergia.com>
 #     Santiago Dueñas <sduenas@bitergia.com>
+#     Jesus M. Gonzalez-Barahona <jgb@gsyc.es>
+#     Harshal Mittal <harshalmittal4@gmail.com>
 #
 
 import json
 import logging
+import requests
 
-from grimoirelab.toolkit.datetime import datetime_to_utc
-from grimoirelab.toolkit.uris import urijoin
+from grimoirelab_toolkit.datetime import datetime_to_utc
+from grimoirelab_toolkit.uris import urijoin
 
 from ...backend import (Backend,
                         BackendCommand,
-                        BackendCommandArgumentParser,
-                        metadata)
+                        BackendCommandArgumentParser)
 from ...client import HttpClient, RateLimitHandler
-from ...errors import CacheError
+from ...errors import RepositoryError
 from ...utils import DEFAULT_DATETIME
 
 
-logger = logging.getLogger(__name__)
-
+CATEGORY_EVENT = "event"
 
 MEETUP_URL = 'https://meetup.com/'
 MEETUP_API_URL = 'https://api.meetup.com/'
 MAX_ITEMS = 200
 
 
 # Range before sleeping until rate limit reset
 MIN_RATE_LIMIT = 1
 
 # Time to avoid too many request exception
 SLEEP_TIME = 30
 
+logger = logging.getLogger(__name__)
+
 
 class Meetup(Backend):
     """Meetup backend.
 
     This class allows to fetch the events of a group from the
-    Meetup server. Initialize this class passing API key needed
-    for authentication with the parameter `api_key`.
+    Meetup server. Initialize this class passing the OAuth2 token needed
+    for authentication with the parameter `api_token`.
 
     :param group: name of the group where data will be fetched
-    :param api_token: token or key needed to use the API
+    :param api_token: OAuth2 token to access the API
     :param max_items:  maximum number of issues requested on the same query
     :param tag: label used to mark the data
-    :param cache: cache object to store raw data
+    :param archive: archive to store/retrieve items
     :param sleep_for_rate: sleep until rate limit is reset
     :param min_rate_to_sleep: minimun rate needed to sleep until
          it will be reset
-    :param sleep_time: minimun waiting time to avoid too many request
-         exception
+    :param sleep_time: time (in seconds) to sleep in case
+        of connection problems
+    :param ssl_verify: enable/disable SSL verification
     """
-    version = '0.7.0'
+    version = '1.0.0'
 
-    def __init__(self, group, api_token, max_items=MAX_ITEMS,
-                 tag=None, cache=None,
+    CATEGORIES = [CATEGORY_EVENT]
+    CLASSIFIED_FIELDS = [
+        ['group', 'topics'],
+        ['event_hosts'],
+        ['rsvps'],
+        ['venue']
+    ]
+    EXTRA_SEARCH_FIELDS = {
+        'group_name': ['group', 'name'],
+        'group_id': ['group', 'id']
+    }
+
+    def __init__(self, group, api_token,
+                 max_items=MAX_ITEMS, tag=None, archive=None,
                  sleep_for_rate=False, min_rate_to_sleep=MIN_RATE_LIMIT,
-                 sleep_time=SLEEP_TIME):
+                 sleep_time=SLEEP_TIME, ssl_verify=True):
         origin = MEETUP_URL
 
-        super().__init__(origin, tag=tag, cache=cache)
+        super().__init__(origin, tag=tag, archive=archive, ssl_verify=ssl_verify)
         self.group = group
         self.max_items = max_items
-        self.client = MeetupClient(api_token, max_items=max_items,
-                                   sleep_for_rate=sleep_for_rate,
-                                   min_rate_to_sleep=min_rate_to_sleep,
-                                   sleep_time=sleep_time)
+        self.api_token = api_token
+        self.sleep_for_rate = sleep_for_rate
+        self.min_rate_to_sleep = min_rate_to_sleep
+        self.sleep_time = sleep_time
+
+        self.client = None
 
-    @metadata
-    def fetch(self, from_date=DEFAULT_DATETIME, to_date=None):
+    def fetch(self, category=CATEGORY_EVENT, from_date=DEFAULT_DATETIME, to_date=None,
+              filter_classified=False):
         """Fetch the events from the server.
 
         This method fetches those events of a group stored on the server
         that were updated since the given date. Data comments and rsvps
         are included within each event.
 
+        :param category: the category of items to fetch
         :param from_date: obtain events updated since this date
         :param to_date: obtain events updated before this date
+        :param filter_classified: remove classified fields from the resulting items
 
         :returns: a generator of events
         """
+        if not from_date:
+            from_date = DEFAULT_DATETIME
+
+        from_date = datetime_to_utc(from_date)
+
+        kwargs = {"from_date": from_date, "to_date": to_date}
+        items = super().fetch(category,
+                              filter_classified=filter_classified,
+                              **kwargs)
+
+        return items
+
+    def fetch_items(self, category, **kwargs):
+        """Fetch the events
+
+        :param category: the category of items to fetch
+        :param kwargs: backend arguments
+
+        :returns: a generator of items
+        """
+        from_date = kwargs['from_date']
+        to_date = kwargs['to_date']
+
         logger.info("Fetching events of '%s' group from %s to %s",
                     self.group, str(from_date),
                     str(to_date) if to_date else '--')
 
-        self._purge_cache_queue()
-
-        from_date = datetime_to_utc(from_date)
         to_date_ts = datetime_to_utc(to_date).timestamp() if to_date else None
 
         nevents = 0
         stop_fetching = False
 
         ev_pages = self.client.events(self.group, from_date=from_date)
 
         for evp in ev_pages:
-            self._push_cache_queue(evp)
-
             events = [event for event in self.parse_json(evp)]
 
             for event in events:
                 event_id = event['id']
 
                 event['comments'] = self.__fetch_and_parse_comments(event_id)
                 event['rsvps'] = self.__fetch_and_parse_rsvps(event_id)
 
                 # Check events updated before 'to_date'
                 event_ts = self.metadata_updated_on(event)
 
                 if to_date_ts and event_ts >= to_date_ts:
-                    # Comments and RSVPS of items from the current
-                    # page be fetched to avoid problems with the cache
                     stop_fetching = True
                     continue
 
                 yield event
                 nevents += 1
 
-            self._flush_cache_queue()
-
             if stop_fetching:
                 break
 
         logger.info("Fetch process completed: %s events fetched", nevents)
 
-    @metadata
-    def fetch_from_cache(self):
-        """Fetch the events from the cache.
-
-        It returns the events stored in the cache object, provided during
-        the initialization of the object. If this method is called but
-        no cache object was provided, the method will raise a `CacheError`
-        exception.
-
-        :returns: a generator of events
-
-        :raises CacheError: raised when an error occurs accesing the
-            cache
-        """
-        if not self.cache:
-            raise CacheError(cause="cache instance was not provided")
-
-        logger.info("Retrieving cached events: %s", self.origin)
-
-        nevents = 0
-
-        for event in self.__fetch_from_cache():
-            yield event
-            nevents += 1
-
-        logger.info("Retrieval process completed: %s events retrieved from cache",
-                    nevents)
-
-    def __fetch_from_cache(self):
-        def fetch_items_from_cache(cache_items, checkpoint):
-            items = []
-
-            while True:
-                raw_page = next(cache_items)
-                if raw_page == checkpoint:
-                    break
-                items += [item for item in self.parse_json(raw_page)]
-            return items
-
-        # Fetch from cache starts here
-        cache_items = self.cache.retrieve()
-
-        while True:
-            try:
-                raw_events = next(cache_items)
-            except StopIteration:
-                break
-
-            events = [event for event in self.parse_json(raw_events)]
-
-            for event in events:
-                comments = fetch_items_from_cache(cache_items, '{ENDCOMMENTS}')
-                rsvps = fetch_items_from_cache(cache_items, '{ENDRSVPS}')
-
-                event['comments'] = comments
-                event['rsvps'] = rsvps
-
-                yield event
-
-    def __fetch_and_parse_comments(self, event_id):
-        logger.debug("Fetching and parsing comments from group '%s' event '%s'",
-                     self.group, str(event_id))
-
-        comments = []
-        raw_pages = self.client.comments(self.group, event_id)
-
-        for raw_page in raw_pages:
-            self._push_cache_queue(raw_page)
-
-            for comment in self.parse_json(raw_page):
-                comments.append(comment)
-
-        self._push_cache_queue('{ENDCOMMENTS}')
-
-        return comments
-
-    def __fetch_and_parse_rsvps(self, event_id):
-        logger.debug("Fetching and parsing rsvps from group '%s' event '%s'",
-                     self.group, str(event_id))
-
-        rsvps = []
-        raw_pages = self.client.rsvps(self.group, event_id)
-
-        for raw_page in raw_pages:
-            self._push_cache_queue(raw_page)
-
-            for rsvp in self.parse_json(raw_page):
-                rsvps.append(rsvp)
-
-        self._push_cache_queue('{ENDRSVPS}')
-
-        return rsvps
-
     @classmethod
-    def has_caching(cls):
-        """Returns whether it supports caching items on the fetch process.
+    def has_archiving(cls):
+        """Returns whether it supports archiving items on the fetch process.
 
-        :returns: this backend supports items cache
+        :returns: this backend supports items archive
         """
         return True
 
     @classmethod
     def has_resuming(cls):
         """Returns whether it supports to resume the fetch process.
 
@@ -276,15 +217,15 @@
     @staticmethod
     def metadata_category(item):
         """Extracts the category from a Meetup item.
 
         This backend only generates one type of item which is
         'event'.
         """
-        return 'event'
+        return CATEGORY_EVENT
 
     @staticmethod
     def parse_json(raw_json):
         """Parse a Meetup JSON stream.
 
         The method parses a JSON stream and returns a list
         with the parsed data.
@@ -292,28 +233,65 @@
         :param raw_json: JSON string to parse
 
         :returns: a list with the parsed data
         """
         result = json.loads(raw_json)
         return result
 
+    def _init_client(self, from_archive=False):
+        """Init client"""
+
+        return MeetupClient(self.api_token, self.max_items,
+                            self.sleep_for_rate, self.min_rate_to_sleep, self.sleep_time,
+                            self.archive, from_archive, self.ssl_verify)
+
+    def __fetch_and_parse_comments(self, event_id):
+        logger.debug("Fetching and parsing comments from group '%s' event '%s'",
+                     self.group, str(event_id))
+
+        comments = []
+        raw_pages = self.client.comments(self.group, event_id)
+
+        for raw_page in raw_pages:
+
+            for comment in self.parse_json(raw_page):
+                comments.append(comment)
+
+        return comments
+
+    def __fetch_and_parse_rsvps(self, event_id):
+        logger.debug("Fetching and parsing rsvps from group '%s' event '%s'",
+                     self.group, str(event_id))
+
+        rsvps = []
+        raw_pages = self.client.rsvps(self.group, event_id)
+
+        for raw_page in raw_pages:
+
+            for rsvp in self.parse_json(raw_page):
+                rsvps.append(rsvp)
+
+        return rsvps
+
 
 class MeetupCommand(BackendCommand):
     """Class to run Meetup backend from the command line."""
 
     BACKEND = Meetup
 
-    @staticmethod
-    def setup_cmd_parser():
+    @classmethod
+    def setup_cmd_parser(cls):
         """Returns the Meetup argument parser."""
 
-        parser = BackendCommandArgumentParser(from_date=True,
+        parser = BackendCommandArgumentParser(cls.BACKEND,
+                                              from_date=True,
                                               to_date=True,
                                               token_auth=True,
-                                              cache=True)
+                                              archive=True,
+                                              ssl_verify=True)
 
         # Meetup options
         group = parser.parser.add_argument_group('Meetup arguments')
         group.add_argument('--max-items', dest='max_items',
                            type=int, default=MAX_ITEMS,
                            help="Maximum number of items requested on the same query")
         group.add_argument('--sleep-for-rate', dest='sleep_for_rate',
@@ -335,50 +313,63 @@
 
 class MeetupClient(HttpClient, RateLimitHandler):
     """Meetup API client.
 
     Client for fetching information from the Meetup server
     using its REST API v3.
 
-    :param api_key: key needed to use the API
+    :param api_token: OAuth2 token needed to access the API
     :param max_items: maximum number of items per request
+    :param sleep_for_rate: sleep until rate limit is reset
+    :param min_rate_to_sleep: minimun rate needed to sleep until
+         it will be reset
+    :param sleep_time: time (in seconds) to sleep in case
+        of connection problems
+    :param archive: an archive to store/read fetched data
+    :param from_archive: it tells whether to write/read the archive
+    :param ssl_verify: enable/disable SSL verification
     """
+    EXTRA_STATUS_FORCELIST = [429]
     RCOMMENTS = 'comments'
     REVENTS = 'events'
     RRSVPS = 'rsvps'
 
     PFIELDS = 'fields'
-    PKEY = 'key'
+    PKEY_OAUTH2 = 'Authorization'
     PORDER = 'order'
     PPAGE = 'page'
     PRESPONSE = 'response'
     PSCROLL = 'scroll'
-    PSIGN = 'sign'
     PSTATUS = 'status'
 
     VEVENT_FIELDS = ['event_hosts', 'featured', 'group_topics',
                      'plain_text_description', 'rsvpable', 'series']
     VRSVP_FIELDS = ['attendance_status']
     VRESPONSE = ['yes', 'no']
     # FIXME: Add 'draft' status when the bug in the Meetup API gets fixed.
     # More info in https://github.com/meetup/api/issues/260
     VSTATUS = ['cancelled', 'upcoming', 'past', 'proposed', 'suggested']
     VUPDATED = 'updated'
 
-    def __init__(self, api_key, max_items=MAX_ITEMS,
-                 sleep_for_rate=False, min_rate_to_sleep=MIN_RATE_LIMIT, sleep_time=SLEEP_TIME):
-        self.api_key = api_key
+    def __init__(self, api_token, max_items=MAX_ITEMS,
+                 sleep_for_rate=False, min_rate_to_sleep=MIN_RATE_LIMIT, sleep_time=SLEEP_TIME,
+                 archive=None, from_archive=False, ssl_verify=True):
+        self.api_token = api_token
         self.max_items = max_items
 
-        super().__init__(MEETUP_API_URL, default_sleep_time=sleep_time, extra_status_forcelist=[429])
+        super().__init__(MEETUP_API_URL, sleep_time=sleep_time,
+                         extra_status_forcelist=self.EXTRA_STATUS_FORCELIST,
+                         archive=archive, from_archive=from_archive, ssl_verify=ssl_verify)
         super().setup_rate_limit_handler(sleep_for_rate=sleep_for_rate, min_rate_to_sleep=min_rate_to_sleep)
 
     def calculate_time_to_reset(self):
         """Number of seconds to wait. They are contained in the rate limit reset header"""
-        return self.rate_limit_reset_ts
+
+        time_to_reset = 0 if self.rate_limit_reset_ts < 0 else self.rate_limit_reset_ts
+        return time_to_reset
 
     def events(self, group, from_date=DEFAULT_DATETIME):
         """Fetch the events pages of a given group."""
 
         date = datetime_to_utc(from_date)
         date = date.strftime("since:%Y-%m-%dT%H:%M:%S.000Z")
 
@@ -396,16 +387,23 @@
 
         params = {
             self.PORDER: self.VUPDATED,
             self.PSCROLL: date,
             self.PPAGE: self.max_items
         }
 
-        for page in self._fetch(resource, params):
-            yield page
+        try:
+            for page in self._fetch(resource, params):
+                yield page
+        except requests.exceptions.HTTPError as error:
+            if error.response.status_code == 410:
+                msg = "Group is no longer accessible: {}".format(error)
+                raise RepositoryError(cause=msg)
+            else:
+                raise error
 
     def comments(self, group, event_id):
         """Fetch the comments of a given event."""
 
         resource = urijoin(group, self.REVENTS, event_id, self.RCOMMENTS)
 
         params = {
@@ -428,44 +426,58 @@
         params = {
             self.PPAGE: self.max_items
         }
 
         for page in self._fetch(resource, params):
             yield page
 
+    @staticmethod
+    def sanitize_for_archive(url, headers, payload):
+        """Sanitize payload of a HTTP request by removing the token information
+        before storing/retrieving archived items
+        :param: url: HTTP url request
+        :param: headers: HTTP headers request
+        :param: payload: HTTP payload request
+        :returns url, headers and the sanitized payload
+        """
+        if MeetupClient.PKEY_OAUTH2 in headers:
+            headers.pop(MeetupClient.PKEY_OAUTH2)
+
+        return url, headers, payload
+
     def _fetch(self, resource, params):
         """Fetch a resource.
 
         Method to fetch and to iterate over the contents of a
         type of resource. The method returns a generator of
         pages for that resource and parameters.
 
         :param resource: type of the resource
         :param params: parameters to filter
 
         :returns: a generator of pages for the requeste resource
         """
         url = urijoin(self.base_url, resource)
-
-        params[self.PKEY] = self.api_key
-        params[self.PSIGN] = 'true',
+        headers = {
+            self.PKEY_OAUTH2: 'Bearer {}'.format(self.api_token)
+        }
 
         do_fetch = True
 
         while do_fetch:
             logger.debug("Meetup client calls resource: %s params: %s",
                          resource, str(params))
 
-            self.sleep_for_rate_limit()
-            r = self.fetch(url, payload=params)
-            self.update_rate_limit(r)
+            if not self.from_archive:
+                self.sleep_for_rate_limit()
+
+            r = self.fetch(url, payload=params, headers=headers)
+
+            if not self.from_archive:
+                self.update_rate_limit(r)
 
             yield r.text
 
             if r.links and 'next' in r.links:
                 url = r.links['next']['url']
-                params = {
-                    self.PKEY: self.api_key,
-                    self.PSIGN: 'true'
-                }
             else:
                 do_fetch = False
```

### Comparing `perceval-0.9.9/perceval/backends/core/bugzillarest.py` & `perceval-1.0.0rc1/perceval/backends/core/slack.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,499 +1,500 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2017 Bitergia
+# Copyright (C) 2015-2020 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1335, USA.
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #     Santiago Dueñas <sduenas@bitergia.com>
-#     Alvaro del Castillo San Felix <acs@bitergia.com>
+#     Valerio Cosentino <valcos@bitergia.com>
+#     Jesus M. Gonzalez-Barahona <jgb@gsyc.es>
+#     Harshal Mittal <harshalmittal4@gmail.com>
 #
 
 import json
 import logging
 
-import requests
-
-from grimoirelab.toolkit.datetime import datetime_to_utc, str_to_datetime
-from grimoirelab.toolkit.uris import urijoin
+from grimoirelab_toolkit.datetime import datetime_to_utc, datetime_utcnow
+from grimoirelab_toolkit.uris import urijoin
 
 from ...backend import (Backend,
                         BackendCommand,
-                        BackendCommandArgumentParser,
-                        metadata)
+                        BackendCommandArgumentParser)
 from ...client import HttpClient
-from ...errors import BaseError, BackendError, CacheError
+from ...errors import BaseError
 from ...utils import DEFAULT_DATETIME
 
+CATEGORY_MESSAGE = "message"
 
-logger = logging.getLogger(__name__)
-
+SLACK_URL = 'https://slack.com/'
+MAX_ITEMS = 1000
+FLOAT_FORMAT = '{:.6f}'
 
-MAX_BUGS = 500  # Maximum number of bugs per query
-MAX_CONTENTS = 25  # Maximum number of bug contents (history, comments) per query
+logger = logging.getLogger(__name__)
 
 
-class BugzillaREST(Backend):
-    """Bugzilla backend that uses its API REST.
+class Slack(Backend):
+    """Slack backend.
 
-    This class allows the fetch the bugs stored in Bugzilla
-    server (version 5.0 or later). To initialize this class
-    the URL of the server must be provided. The `url` will be
-    set as the origin of the data.
-
-    :param url: Bugzilla server URL
-    :param user: Bugzilla user
-    :param password: Bugzilla user password
-    :param api_token: Bugzilla token
-    :param max_bugs: maximum number of bugs requested on the same query
+    This class retrieves the messages sent to a Slack channel.
+    To access the server an API token is required, which must
+    have enough permissions to read from the given channel.
+
+    The origin of the data will be set to the `SLACK_URL` plus the
+    identifier of the channel; i.e 'https://slack.com/C01234ABC'.
+
+    :param channel: identifier of the channel where data will be fetched
+    :param api_token: token or key needed to use the API
+    :param max_items: maximum number of message requested on the same query
     :param tag: label used to mark the data
-    :param cache: cache object to store raw data
+    :param archive: archive to store/retrieve items
+    :param ssl_verify: enable/disable SSL verification
     """
-    version = '0.6.0'
+    version = '1.0.0'
+
+    CATEGORIES = [CATEGORY_MESSAGE]
+    EXTRA_SEARCH_FIELDS = {
+        'channel_name': ['channel_info', 'name'],
+        'channel_id': ['channel_info', 'id']
+    }
 
-    def __init__(self, url, user=None, password=None, api_token=None,
-                 max_bugs=MAX_BUGS, tag=None, cache=None):
-        origin = url
+    def __init__(self, channel, api_token, max_items=MAX_ITEMS,
+                 tag=None, archive=None, ssl_verify=True):
+        origin = urijoin(SLACK_URL, channel)
 
-        super().__init__(origin, tag=tag, cache=cache)
-        self.url = url
-        self.max_bugs = max(1, max_bugs)
-        self.client = BugzillaRESTClient(url, user=user, password=password,
-                                         api_token=api_token)
+        super().__init__(origin, tag=tag, archive=archive, ssl_verify=ssl_verify)
+        self.channel = channel
+        self.api_token = api_token
+        self.max_items = max_items
+        self.client = None
 
-    @metadata
-    def fetch(self, from_date=DEFAULT_DATETIME):
-        """Fetch the bugs from the repository.
+        self._users = {}
 
-        The method retrieves, from a Bugzilla repository, the bugs
-        updated since the given date.
+    def fetch(self, category=CATEGORY_MESSAGE, from_date=DEFAULT_DATETIME):
+        """Fetch the messages from the channel.
 
-        :param from_date: obtain bugs updated since this date
+        This method fetches the messages stored on the channel that were
+        sent since the given date.
 
-        :returns: a generator of bugs
+        :param category: the category of items to fetch
+        :param from_date: obtain messages sent since this date
+
+        :returns: a generator of messages
         """
         if not from_date:
             from_date = DEFAULT_DATETIME
 
-        logger.info("Looking for bugs: '%s' updated from '%s'",
-                    self.url, str(from_date))
+        from_date = datetime_to_utc(from_date)
+        latest = datetime_utcnow().timestamp()
 
-        self._purge_cache_queue()
+        kwargs = {'from_date': from_date, 'latest': latest}
+        items = super().fetch(category, **kwargs)
 
-        nbugs = 0
-        for bug in self.__fetch_and_parse_bugs(from_date):
-            nbugs += 1
-            yield bug
-
-        logger.info("Fetch process completed: %s bugs fetched", nbugs)
-
-    @metadata
-    def fetch_from_cache(self):
-        """Fetch bugs from the cache.
-
-        :returns: a generator of bugs
-
-        :raises CacheError: raised when an error occurs accessing the
-            cache
-        """
-        if not self.cache:
-            raise CacheError(cause="cache instance was not provided")
-
-        logger.info("Retrieving cached bugs: '%s'", self.url)
-        nbugs = 0
-
-        for bug in self.__retrieve_bugs_from_cache():
-            nbugs += 1
-            yield bug
-
-        logger.info("Retrieval process completed: %s bugs retrieved from cache",
-                    nbugs)
-
-    def __fetch_and_parse_bugs(self, from_date):
-        max_contents = min(MAX_CONTENTS, self.max_bugs)
-        offset = 0
-
-        while True:
-            logger.debug("Fetching and parsing bugs from: %s, offset: %s, limit: %s ",
-                         str(from_date), offset, self.max_bugs)
-            raw_bugs = self.client.bugs(from_date=from_date, offset=offset,
-                                        max_bugs=self.max_bugs)
-            self._push_cache_queue(raw_bugs)
-
-            data = json.loads(raw_bugs)
-            buglist = data['bugs']
-
-            tbugs = len(buglist)
-
-            if tbugs == 0:
-                break
-
-            for i in range(0, tbugs, max_contents):
-                chunk = buglist[i:i + max_contents]
-                bug_ids = [b['id'] for b in chunk]
-
-                comments = self.__fetch_and_parse_comments(*bug_ids)
-                histories = self.__fetch_and_parse_histories(*bug_ids)
-                attachments = self.__fetch_and_parse_attachments(*bug_ids)
-
-                for bug in chunk:
-                    bug_id = str(bug['id'])
-                    bug['comments'] = comments[bug_id]
-                    bug['history'] = histories[bug_id]
-                    bug['attachments'] = attachments[bug_id]
-                    yield bug
-
-            self._flush_cache_queue()
-            offset += self.max_bugs
-
-    def __fetch_and_parse_comments(self, *bug_ids):
-        logger.debug("Fetching and parsing comments")
-        raw_comments = self.client.comments(*bug_ids)
-        self._push_cache_queue(raw_comments)
-        return self.__parse_comments(raw_comments)
-
-    def __fetch_and_parse_histories(self, *bug_ids):
-        logger.debug("Fetching and parsing histories")
-        raw_histories = self.client.history(*bug_ids)
-        self._push_cache_queue(raw_histories)
-        return self.__parse_histories(raw_histories)
-
-    def __fetch_and_parse_attachments(self, *bug_ids):
-        logger.debug("Fetching and parsing attachments")
-        raw_attachments = self.client.attachments(*bug_ids)
-        self._push_cache_queue(raw_attachments)
-        return self.__parse_attachments(raw_attachments)
-
-    def __retrieve_bugs_from_cache(self):
-        def recover_extra_data(cache_items):
-            try:
-                comments = self.__parse_comments(next(cache_items))
-                histories = self.__parse_histories(next(cache_items))
-                attachments = self.__parse_attachments(next(cache_items))
-            except StopIteration:
-                # Fatal error. The code should not reach here.
-                # Cache should had stored an activity item per parsed bug.
-                cause = "cache is exhausted but more items were expected"
-                raise CacheError(cause=cause)
-            return comments, histories, attachments
-
-        cache_items = self.cache.retrieve()
-
-        while True:
-            try:
-                raw_bugs = next(cache_items)
-            except StopIteration:
-                break
-
-            bugs = json.loads(raw_bugs)['bugs']
-
-            if len(bugs) == 0:
-                continue
-
-            comments, histories, attachments = recover_extra_data(cache_items)
-
-            while bugs:
-                bug = bugs.pop(0)
-                bug_id = str(bug['id'])
-
-                try:
-                    bug['comments'] = comments.pop(bug_id)
-                    bug['history'] = histories.pop(bug_id)
-                    bug['attachments'] = attachments.pop(bug_id)
-                except KeyError:
-                    # Fatal error. Keys must exist.
-                    cause = "invalid cached data, bug id %s not found" % bug_id
-                    raise CacheError(cause=cause)
+        return items
 
-                yield bug
+    def fetch_items(self, category, **kwargs):
+        """Fetch the messages
 
-                if bugs and (len(comments) + len(histories) + len(attachments) == 0):
-                    comments, histories, attachments = recover_extra_data(cache_items)
+        :param category: the category of items to fetch
+        :param kwargs: backend arguments
 
-    @staticmethod
-    def __parse_comments(raw_comments):
-        contents = json.loads(raw_comments)['bugs']
-        comments = {k: v['comments'] for k, v in contents.items()}
-        return comments
+        :returns: a generator of items
+        """
+        from_date = kwargs['from_date']
+        latest = kwargs['latest']
 
-    @staticmethod
-    def __parse_histories(raw_histories):
-        contents = json.loads(raw_histories)['bugs']
-        history = {str(c['id']): c['history'] for c in contents}
-        return history
+        logger.info("Fetching messages of '%s' channel from %s",
+                    self.channel, str(from_date))
 
-    @staticmethod
-    def __parse_attachments(raw_attachments):
-        contents = json.loads(raw_attachments)['bugs']
-        attachments = {k: v for k, v in contents.items()}
-        return attachments
+        raw_info = self.client.channel_info(self.channel)
+
+        channel_info = self.parse_channel_info(raw_info)
+
+        if channel_info['is_archived']:
+            channel_info['num_members'] = None
+            logger.warning("channel_info.num_members is None for archived channels %s", self.channel)
+        else:
+            channel_info['num_members'] = self.client.conversation_members(self.channel)
+
+        oldest = datetime_to_utc(from_date).timestamp()
+
+        fetching = True
+        nmsgs = 0
+
+        while fetching:
+            raw_history = self.client.history(self.channel,
+                                              oldest=oldest, latest=latest)
+            messages, fetching = self.parse_history(raw_history)
+
+            for message in messages:
+                # Fetch user data
+                user_id = None
+                if 'user' in message:
+                    user_id = message['user']
+                elif 'comment' in message:
+                    user_id = message['comment']['user']
+
+                if user_id:
+                    message['user_data'] = self.__get_or_fetch_user(user_id)
+
+                message['channel_info'] = channel_info
+                yield message
+
+                nmsgs += 1
+
+                if fetching:
+                    latest = float(message['ts'])
+
+        logger.info("Fetch process completed: %s message fetched", nmsgs)
 
     @classmethod
-    def has_caching(cls):
-        """Returns whether it supports caching items on the fetch process.
+    def has_archiving(cls):
+        """Returns whether it supports archiving items on the fetch process.
 
-        :returns: this backend supports items cache
+        :returns: this backend supports items archive
         """
         return True
 
     @classmethod
     def has_resuming(cls):
         """Returns whether it supports to resume the fetch process.
 
-        :returns: this backend supports items resuming
+        :returns: this backend does not support items resuming
         """
-        return True
+        return False
 
     @staticmethod
     def metadata_id(item):
-        """Extracts the identifier from a Bugzilla item."""
+        """Extracts the identifier from a Slack item.
+
+        This identifier will be the mix of two fields because Slack
+        messages does not have any unique identifier. In this case,
+        'ts' and 'user' values (or 'bot_id' when the message is sent by a bot)
+        are combined because there have been cases where two messages were sent
+        by different users at the same time.
+
+        In the case where neither the 'user', 'bot_id', or 'username' attributes
+        are present (e.g, bot deleted), the fallback option is to generate the
+        identifier using the 'ts' value.
+        """
+        if 'user' in item:
+            nick = item['user']
+        elif 'comment' in item:
+            nick = item['comment']['user']
+        elif 'bot_id' in item:
+            nick = item['bot_id']
+        elif 'username' in item:
+            nick = item['username']
+        else:
+            nick = ""
 
-        return str(item['id'])
+        return item['ts'] + nick
 
     @staticmethod
     def metadata_updated_on(item):
-        """Extracts the update time from a Bugzilla item.
+        """Extracts and coverts the update time from a Slack item.
 
-        The timestamp used is extracted from 'last_change_time' field.
-        This date is converted to UNIX timestamp format taking into
-        account the timezone of the date.
+        The timestamp is extracted from 'ts' field and converted
+        to a UNIX timestamp.
 
         :param item: item generated by the backend
 
         :returns: a UNIX timestamp
         """
-        ts = item['last_change_time']
-        ts = str_to_datetime(ts)
+        ts = float(item['ts'])
 
-        return ts.timestamp()
+        return ts
 
     @staticmethod
     def metadata_category(item):
-        """Extracts the category from a Bugzilla item.
+        """Extracts the category from a Slack item.
 
         This backend only generates one type of item which is
-        'bug'.
+        'message'.
         """
-        return 'bug'
+        return CATEGORY_MESSAGE
 
+    @staticmethod
+    def parse_channel_info(raw_channel_info):
+        """Parse a channel info JSON stream.
 
-class BugzillaRESTError(BaseError):
-    """Raised when an error occurs using the API"""
-
-    message = "%(error)s (code: %(code)s)"
+        This method parses a JSON stream, containing the information
+        from a channel, and returns a dict with the parsed data.
 
+        :param raw_channel_info
 
-class BugzillaRESTClient(HttpClient):
-    """Bugzilla REST API client.
+        :returns: a dict with the parsed information about a channel
+        """
+        result = json.loads(raw_channel_info)
+        return result['channel']
 
-    This class implements a simple client to retrieve distinct
-    kind of data from a Bugzilla > 5.0 repository using its
-    REST API.
+    @staticmethod
+    def parse_history(raw_history):
+        """Parse a channel history JSON stream.
 
-    When `user` and `password` parameters are given it logs in
-    the server. Further requests will use the token obtained
-    during the sign in phase.
+        This method parses a JSON stream, containing the history of
+        a channel, and returns a list with the parsed data. It also
+        returns if there are more messages that are not included on
+        this stream.
 
-    :param base_url: URL of the Bugzilla server
-    :param user: Bugzilla user
-    :param password: user password
-    :param api_token: api token for user; when this is provided
-        `user` and `password` parameters will be ignored
+        :param raw_history: JSON string to parse
 
-    :raises BackendError: when an error occurs initilizing the
-        client
-    """
-    URL = "%(base)s/rest/%(resource)s"
+        :returns: a tuple with a list of dicts with the parsed messages
+            and 'has_more' value
+        """
+        result = json.loads(raw_history)
+        return result['messages'], result['has_more']
 
-    # API resources
-    RBUG = 'bug'
-    RATTACHMENT = 'attachment'
-    RCOMMENT = 'comment'
-    RHISTORY = 'history'
-    RLOGIN = 'login'
-
-    # Resource parameters
-    PBUGZILLA_LOGIN = 'login'
-    PBUGZILLA_PASSWORD = 'password'
-    PBUGZILLA_TOKEN = 'token'
-    PIDS = 'ids'
-    PLAST_CHANGE_TIME = 'last_change_time'
-    PLIMIT = 'limit'
-    POFFSET = 'offset'
-    PORDER = 'order'
-    PINCLUDE_FIELDS = 'include_fields'
-    PEXCLUDE_FIELDS = 'exclude_fields'
-
-    # Predefined values
-    VCHANGE_DATE_ORDER = 'changeddate'
-    VINCLUDE_ALL = '_all'
-    VEXCLUDE_ATTCH_DATA = 'data'
-
-    def __init__(self, base_url, user=None, password=None, api_token=None):
-        super().__init__(base_url)
-        self.api_token = api_token if api_token else None
+    @staticmethod
+    def parse_user(raw_user):
+        """Parse a user's info JSON stream.
 
-        if user is not None and password is not None:
-            self.login(user, password)
+        This method parses a JSON stream, containing the information
+        from a user, and returns a dict with the parsed data.
 
-    def login(self, user, password):
-        """Authenticate a user in the server.
+        :param raw_user: JSON string to parse
 
-        :param user: Bugzilla user
-        :param password: user password
+        :returns: a dict with the parsed user's information
         """
-        params = {
-            self.PBUGZILLA_LOGIN: user,
-            self.PBUGZILLA_PASSWORD: password
-        }
+        result = json.loads(raw_user)
+        return result['user']
+
+    def _init_client(self, from_archive=False):
+        """Init client"""
+
+        return SlackClient(self.api_token, self.max_items, self.archive,
+                           from_archive, self.ssl_verify)
+
+    def __get_or_fetch_user(self, user_id):
+        if user_id in self._users:
+            return self._users[user_id]
 
-        try:
-            r = self.call(self.RLOGIN, params)
-        except requests.exceptions.HTTPError as e:
-            cause = ("Bugzilla REST client could not authenticate user %s. "
-                     "See exception: %s") % (user, str(e))
-            raise BackendError(cause=cause)
-
-        data = json.loads(r)
-        self.api_token = data['token']
-
-    def bugs(self, from_date=DEFAULT_DATETIME, offset=None, max_bugs=MAX_BUGS):
-        """Get the information of a list of bugs.
-
-        :param from_date: retrieve bugs that where updated from that date;
-            dates are converted to UTC
-        :param offset: starting position for the search; i.e to return 11th
-            element, set this value to 10.
-        :param max_bugs: maximum number of bugs to reteurn per query
+        logger.debug("User %s not found on client cache; fetching it", user_id)
+
+        raw_user = self.client.user(user_id)
+        user = self.parse_user(raw_user)
+
+        self._users[user_id] = user
+        return user
+
+
+class SlackClientError(BaseError):
+    """Raised when an error occurs using the Slack client"""
+
+    message = "%(error)s"
+
+
+class SlackClient(HttpClient):
+    """Slack API client.
+
+    Client for fetching information from the Slack server
+    using its REST API.
+
+    :param api_token: key needed to use the API
+    :param max_items: maximum number of items per request
+    :param archive: an archive to store/read fetched data
+    :param from_archive: it tells whether to write/read the archive
+    :param ssl_verify: enable/disable SSL verification
+    """
+    URL = urijoin(SLACK_URL, 'api', '%(resource)s')
+
+    AUTHORIZATION_HEADER = 'Authorization'
+    RCONVERSATION_MEMBERS = 'conversations.members'
+    RCONVERSATION_INFO = 'conversations.info'
+    RCONVERSATION_HISTORY = 'conversations.history'
+    RUSER_INFO = 'users.info'
+
+    PCHANNEL = 'channel'
+    PCOUNT = 'count'
+    POLDEST = 'oldest'
+    PLATEST = 'latest'
+    PTOKEN = 'token'
+    PUSER = 'user'
+
+    def __init__(self, api_token, max_items=MAX_ITEMS, archive=None, from_archive=False, ssl_verify=True):
+        super().__init__(SLACK_URL, archive=archive, from_archive=from_archive, ssl_verify=ssl_verify)
+        self.api_token = api_token
+        self.max_items = max_items
+
+    def conversation_members(self, conversation):
+        """Fetch the number of members in a conversation, which is a supertype for public and
+        private ones, DM and group DM.
+
+        :param conversation: the ID of the conversation
         """
-        date = datetime_to_utc(from_date)
-        date = date.strftime("%Y-%m-%dT%H:%M:%SZ")
+        members = 0
+
+        resource = self.RCONVERSATION_MEMBERS
 
         params = {
-            self.PLAST_CHANGE_TIME: date,
-            self.PLIMIT: max_bugs,
-            self.PORDER: self.VCHANGE_DATE_ORDER,
-            self.PINCLUDE_FIELDS: self.VINCLUDE_ALL
+            self.PCHANNEL: conversation,
         }
 
-        if offset:
-            params[self.POFFSET] = offset
+        raw_response = self._fetch(resource, params)
+        response = json.loads(raw_response)
 
-        response = self.call(self.RBUG, params)
+        members += len(response["members"])
+        while 'next_cursor' in response['response_metadata'] and response['response_metadata']['next_cursor']:
+            params['cursor'] = response['response_metadata']['next_cursor']
+            raw_response = self._fetch(resource, params)
+            response = json.loads(raw_response)
+            members += len(response["members"])
 
-        return response
+        return members
 
-    def comments(self, *bug_ids):
-        """Get the comments of the given bugs.
+    def channel_info(self, channel):
+        """Fetch information about a channel."""
 
-        :param bug_ids: list of bug identifiers
-        """
-        # Hack. The first value must be a valid bug id
-        resource = urijoin(self.RBUG, bug_ids[0], self.RCOMMENT)
+        resource = self.RCONVERSATION_INFO
 
         params = {
-            self.PIDS: bug_ids
+            self.PCHANNEL: channel,
         }
 
-        response = self.call(resource, params)
+        response = self._fetch(resource, params)
 
         return response
 
-    def history(self, *bug_ids):
-        """Get the history of the given bugs.
+    def history(self, channel, oldest=None, latest=None):
+        """Fetch the history of a channel."""
 
-        :param bug_ids: list of bug identifiers
-        """
-        resource = urijoin(self.RBUG, bug_ids[0], self.RHISTORY)
+        resource = self.RCONVERSATION_HISTORY
 
         params = {
-            self.PIDS: bug_ids
+            self.PCHANNEL: channel,
+            self.PCOUNT: self.max_items
         }
 
-        response = self.call(resource, params)
+        if oldest is not None:
+            formatted_oldest = self.__format_timestamp(oldest, subtract=True)
+            params[self.POLDEST] = formatted_oldest
+        if latest is not None:
+            formatted_latest = self.__format_timestamp(latest)
+            params[self.PLATEST] = formatted_latest
+
+        response = self._fetch(resource, params)
 
         return response
 
-    def attachments(self, *bug_ids):
-        """Get the attachments of the given bugs.
+    def user(self, user_id):
+        """Fetch user info."""
 
-        :param bug_id: list of bug identifiers
-        """
-        resource = urijoin(self.RBUG, bug_ids[0], self.RATTACHMENT)
+        resource = self.RUSER_INFO
 
         params = {
-            self.PIDS: bug_ids,
-            self.PEXCLUDE_FIELDS: self.VEXCLUDE_ATTCH_DATA
+            self.PUSER: user_id
         }
 
-        response = self.call(resource, params)
+        response = self._fetch(resource, params)
 
         return response
 
-    def call(self, resource, params):
-        """Retrive the given resource.
+    @staticmethod
+    def sanitize_for_archive(url, headers, payload):
+        """Sanitize payload of a HTTP request by removing the token information
+        before storing/retrieving archived items
 
-        :param resource: resource to retrieve
-        :param params: dict with the HTTP parameters needed to retrieve
-            the given resource
+        :param: url: HTTP url request
+        :param: headers: HTTP headers request
+        :param: payload: HTTP payload request
 
-        :raises BugzillaRESTError: raised when an error is returned by
-            the server
+        :returns url, headers and the sanitized payload
         """
-        url = self.URL % {'base': self.base_url, 'resource': resource}
+        if SlackClient.AUTHORIZATION_HEADER in headers:
+            headers.pop(SlackClient.AUTHORIZATION_HEADER)
 
-        if self.api_token:
-            params[self.PBUGZILLA_TOKEN] = self.api_token
+        return url, headers, payload
 
-        logger.debug("Bugzilla REST client requests: %s params: %s",
+    def _fetch(self, resource, params):
+        """Fetch a resource.
+
+        :param resource: resource to get
+        :param params: dict with the HTTP parameters needed to get
+            the given resource
+        """
+        url = self.URL % {'resource': resource}
+        headers = {
+            self.AUTHORIZATION_HEADER: 'Bearer {}'.format(self.api_token)
+        }
+
+        logger.debug("Slack client requests: %s params: %s",
                      resource, str(params))
 
-        r = self.fetch(url, payload=params)
+        r = self.fetch(url, payload=params, headers=headers)
 
-        # Check for possible Bugzilla API errors
+        # Check for possible API errors
         result = r.json()
 
-        if result.get('error', False):
-            raise BugzillaRESTError(error=result['message'],
-                                    code=result['code'])
+        if not result['ok']:
+            if result['error'] == 'user_not_found':
+                return '{"ok":false,"user":null}'
+            raise SlackClientError(error=result['error'])
 
         return r.text
 
+    def __format_timestamp(self, ts, subtract=False):
+        """Handle the timestamp value to be passed to the channels.history API endpoint. In
+        particular, two cases are covered:
 
-class BugzillaRESTCommand(BackendCommand):
-    """Class to run BugzillaREST backend from the command line."""
+        - Since the minimum value supported by Slack is 0, the value 0.0 must be converted.
+        - Slack does not include in its result the lower limit of the search if it has
+          the same date of 'oldest'. To get this messages too, we subtract a low value to
+          be sure the dates are not the same. To avoid precision problems it is subtracted
+          by five decimals and not by six.
 
-    BACKEND = BugzillaREST
+        :param ts: timestamp float value
+        :param subtract: if True, `ts` is decreased by 0.00001
+        """
+        if ts == 0.0:
+            return "0"
 
-    @staticmethod
-    def setup_cmd_parser():
-        """Returns the BugzillaREST argument parser."""
+        processed = ts
+        if processed > 0.0 and subtract:
+            processed -= .00001
+
+        processed = FLOAT_FORMAT.format(processed)
+
+        return processed
+
+
+class SlackCommand(BackendCommand):
+    """Class to run Slack backend from the command line."""
+
+    BACKEND = Slack
+
+    @classmethod
+    def setup_cmd_parser(cls):
+        """Returns the Slack argument parser."""
 
-        parser = BackendCommandArgumentParser(from_date=True,
-                                              basic_auth=True,
+        parser = BackendCommandArgumentParser(cls.BACKEND,
+                                              from_date=True,
                                               token_auth=True,
-                                              cache=True)
+                                              archive=True,
+                                              ssl_verify=True)
 
-        # BugzillaREST options
-        group = parser.parser.add_argument_group('Bugzilla REST arguments')
-        group.add_argument('--max-bugs', dest='max_bugs',
-                           type=int, default=MAX_BUGS,
-                           help="Maximum number of bugs requested on the same query")
+        # Backend token is required
+        action = parser.parser._option_string_actions['--api-token']
+        action.required = True
+
+        # Slack options
+        group = parser.parser.add_argument_group('Slack arguments')
+        group.add_argument('--max-items', dest='max_items',
+                           type=int, default=MAX_ITEMS,
+                           help="Maximum number of items requested on the same query")
 
         # Required arguments
-        parser.parser.add_argument('url',
-                                   help="URL of the Bugzilla server")
+        parser.parser.add_argument('channel',
+                                   help="Slack channel identifier")
 
         return parser
```

### Comparing `perceval-0.9.9/perceval/backends/core/slack.py` & `perceval-1.0.0rc1/perceval/backends/core/rocketchat.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,471 +1,404 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2017 Bitergia
+# Copyright (C) 2015-2020 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1335, USA.
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
-#     Santiago Dueñas <sduenas@bitergia.com>
+#     Aditya Prajapati <aditya10699@gmail.com>
+#     Animesh Kumar <animuz111@gmail.com>
 #
 
-import json
 import logging
+import json
 
-from grimoirelab.toolkit.datetime import datetime_to_utc, datetime_utcnow
-from grimoirelab.toolkit.uris import urijoin
+from grimoirelab_toolkit.uris import urijoin
+from grimoirelab_toolkit.datetime import (datetime_utcnow,
+                                          datetime_to_utc,
+                                          str_to_datetime)
 
 from ...backend import (Backend,
                         BackendCommand,
-                        BackendCommandArgumentParser,
-                        metadata)
-from ...client import HttpClient
-from ...errors import BaseError, CacheError
+                        BackendCommandArgumentParser)
+from ...client import HttpClient, RateLimitHandler
 from ...utils import DEFAULT_DATETIME
 
+CATEGORY_MESSAGE = "message"
 
-logger = logging.getLogger(__name__)
+API_EXTENSION = "/api/v1/"
 
-SLACK_URL = 'https://slack.com/'
-MAX_ITEMS = 1000
+MIN_RATE_LIMIT = 10
+MAX_ITEMS = 100
 
+logger = logging.getLogger(__name__)
 
-class Slack(Backend):
-    """Slack backend.
 
-    This class retrieves the messages sent to a Slack channel.
-    To access the server an API token is required, which must
-    have enough permissions to read from the given channel.
+class RocketChat(Backend):
+    """Rocket.Chat backend.
 
-    The origin of the data will be set to the `SLACK_URL` plus the
-    identifier of the channel; i.e 'https://slack.com/C01234ABC'.
+    This class allows to fetch messages from a channel(room) on a Rocket.Chat server.
+    An API token and a User Id is required to access the server.
 
-    :param channel: identifier of the channel where data will be fetched
-    :param api_token: token or key needed to use the API
+    :param url: server url from where messages are to be fetched
+    :param channel: name of the channel from where data will be fetched
+    :param user_id: generated User Id using your Rocket.Chat account
+    :param api_token: token needed to use the API
     :param max_items: maximum number of message requested on the same query
+    :param sleep_for_rate: sleep until rate limit is reset
+    :param min_rate_to_sleep: minimum rate needed to sleep until
+         it will be reset
     :param tag: label used to mark the data
-    :param cache: cache object to store raw data
+    :param archive: archive to store/retrieve items
+    :param ssl_verify: enable/disable SSL verification
     """
-    version = '0.3.0'
+    version = '1.0.0'
+
+    CATEGORIES = [CATEGORY_MESSAGE]
+    EXTRA_SEARCH_FIELDS = {
+        'channel_name': ['channel_info', 'name'],
+        'channel_id': ['channel_info', '_id']
+    }
+
+    def __init__(self, url, channel, user_id, api_token, max_items=MAX_ITEMS,
+                 sleep_for_rate=False, min_rate_to_sleep=MIN_RATE_LIMIT,
+                 tag=None, archive=None, ssl_verify=True):
+        origin = urijoin(url, channel)
 
-    def __init__(self, channel, api_token, max_items=MAX_ITEMS,
-                 tag=None, cache=None):
-        origin = urijoin(SLACK_URL, channel)
+        super().__init__(origin, tag=tag, archive=archive, ssl_verify=ssl_verify)
 
-        super().__init__(origin, tag=tag, cache=cache)
+        self.url = url
         self.channel = channel
+        self.user_id = user_id
+        self.api_token = api_token
         self.max_items = max_items
-        self.client = SlackClient(api_token, max_items=max_items)
-        self._users = {}
+        self.sleep_for_rate = sleep_for_rate
+        self.min_rate_to_sleep = min_rate_to_sleep
+        self.client = None
 
-    @metadata
-    def fetch(self, from_date=DEFAULT_DATETIME):
+    def fetch(self, category=CATEGORY_MESSAGE, from_date=DEFAULT_DATETIME, filter_classified=False):
         """Fetch the messages from the channel.
 
         This method fetches the messages stored on the channel that were
         sent since the given date.
 
+        :param category: the category of items to fetch
         :param from_date: obtain messages sent since this date
+        :param filter_classified: remove classified fields from the resulting items
 
         :returns: a generator of messages
         """
-        logger.info("Fetching messages of '%s' channel from %s",
-                    self.channel, str(from_date))
+        if not from_date:
+            from_date = DEFAULT_DATETIME
+        from_date = datetime_to_utc(from_date)
 
-        self._purge_cache_queue()
+        kwargs = {'from_date': from_date}
 
-        raw_info = self.client.channel_info(self.channel)
-        self._push_cache_queue(raw_info)
-        channel_info = self.parse_channel_info(raw_info)
-
-        oldest = datetime_to_utc(from_date).timestamp()
-        latest = datetime_utcnow().timestamp()
-
-        # Minimum value supported by Slack is 0 not 0.0
-        if oldest == 0.0:
-            oldest = 0
-
-        # Slack does not include on its result the lower limit
-        # of the search if it has the same date of 'oldest'. To get
-        # this messages too, we substract a low value to be sure
-        # the dates are not the same. To avoid precision problems
-        # it is substracted by five decimals and not by six.
-        if oldest > 0.0:
-            oldest -= .00001
+        items = super().fetch(category, **kwargs)
 
-        fetching = True
-        nmsgs = 0
+        return items
 
-        while fetching:
-            raw_history = self.client.history(self.channel,
-                                              oldest=oldest, latest=latest)
-            messages, fetching = self.parse_history(raw_history)
+    def fetch_items(self, category, **kwargs):
+        """Fetch the messages.
 
-            self._push_cache_queue(raw_history)
+        :param category: the category of items to fetch
+        :param kwargs: backend arguments
 
-            for message in messages:
-                # Fetch user data
-                user_id = None
-                if 'user' in message:
-                    user_id = message['user']
-                elif 'comment' in message:
-                    user_id = message['comment']['user']
+        :returns: a generator of items
+        """
+        from_date = kwargs['from_date']
+        logger.info("Fetching messages of channel: %s from date: %s",
+                    self.channel, from_date)
 
-                if user_id:
-                    message['user_data'] = self.__get_or_fetch_user(user_id)
+        raw_channel_info = self.client.channel_info(self.channel)
+        channel_info = self.parse_channel_info(raw_channel_info)
 
-                message['channel_info'] = channel_info
-                yield message
+        fetching = True
+        nmsgs = 0
+        offset = 0
+
+        while fetching:
+            raw_messages = self.client.messages(self.channel, from_date, offset)
+            messages, total = self.parse_messages(raw_messages)
 
+            for message in messages:
+                message["channel_info"] = channel_info
                 nmsgs += 1
+                yield message
 
-                if fetching:
-                    latest = float(message['ts'])
+            offset += len(messages)
 
-            # Checkpoint. A set of messages ends here.
-            self._push_cache_queue('{}')
-            self._flush_cache_queue()
-
-        # Checkpoint for batch. A batch ends here.
-        self._push_cache_queue('{END}')
-        self._flush_cache_queue()
+            if offset == total:
+                fetching = False
 
         logger.info("Fetch process completed: %s message fetched", nmsgs)
 
-    @metadata
-    def fetch_from_cache(self):
-        """Fetch the messages from the cache.
-
-        It returns the messages stored in the cache object, provided during
-        the initialization of the object. If this method is called but
-        no cache object was provided, the method will raise a `CacheError`
-        exception.
+    @staticmethod
+    def parse_messages(raw_messages):
+        """Parse a channel messages JSON stream.
 
-        :returns: a generator of messages
+        This method parses a JSON stream, containing the
+        history of a channel. It returns a list of messages
+        and the total messages count in that channel.
 
-        :raises CacheError: raised when an error occurs accesing the
-            cache
-        """
-        if not self.cache:
-            raise CacheError(cause="cache instance was not provided")
+        :param raw_messages: JSON string to parse
 
-        logger.info("Retrieving cached messages: '%s'", self.channel)
+        :returns: a tuple with a list of dicts with the parsed messages
+            and a total messages count in the channel.
+        """
+        result = json.loads(raw_messages)
+        return result['messages'], result['total']
 
-        cache_items = self.cache.retrieve()
-        cached_users = {}
-        channel_info = None
+    @staticmethod
+    def parse_channel_info(raw_channel_info):
+        """Parse a channel's information JSON stream.
 
-        nmsgs = 0
-        start_batch = True
+        This method parses a JSON stream, containing the information
+        of the channel, and returns a dict with the parsed data.
 
-        try:
-            while True:
-                try:
-                    raw_json = next(cache_items)
-                except StopIteration:
-                    break
-
-                if start_batch:
-                    channel_info = self.parse_channel_info(raw_json)
-                    start_batch = False
-                    continue
-                elif raw_json == '{END}':
-                    start_batch = True
-                    continue
-                else:
-                    raw_history = raw_json
-
-                checkpoint = False
-
-                while not checkpoint:
-                    raw_item = next(cache_items)
-
-                    if raw_item != '{}':
-                        user = self.parse_user(raw_item)
-                        cached_users[user['id']] = user
-                    else:
-                        checkpoint = True
-
-                messages, _ = self.parse_history(raw_history)
-
-                for message in messages:
-                    user_id = None
-                    if 'user' in message:
-                        user_id = message['user']
-                    elif 'comment' in message:
-                        user_id = message['comment']['user']
-
-                    if user_id:
-                        message['user_data'] = cached_users[user_id]
-
-                    message['channel_info'] = channel_info
-                    yield message
-                    nmsgs += 1
-        except StopIteration:
-            # Fatal error. The code should not reach here.
-            # Cache should had stored an activity item per parsed bug.
-            cause = "cache is exhausted but more items were expected"
-            raise CacheError(cause=cause)
-
-        logger.info("Retrieval process completed: %s messages retrieved from cache",
-                    nmsgs)
-
-    def __get_or_fetch_user(self, user_id):
-        if user_id in self._users:
-            return self._users[user_id]
-
-        logger.debug("User %s not found on client cache; fetching it", user_id)
-
-        raw_user = self.client.user(user_id)
-        user = self.parse_user(raw_user)
-        self._push_cache_queue(raw_user)
+        :param raw_channel_info: JSON string to parse
 
-        self._users[user_id] = user
-        return user
+        :returns: a dict with the parsed channel's information
+        """
+        result = json.loads(raw_channel_info)
+        return result['channel']
 
     @classmethod
-    def has_caching(cls):
-        """Returns whether it supports caching items on the fetch process.
+    def has_archiving(cls):
+        """Returns whether it supports archiving items on the fetch process.
 
-        :returns: this backend supports items cache
+        :returns: this backend supports items archive
         """
         return True
 
     @classmethod
     def has_resuming(cls):
         """Returns whether it supports to resume the fetch process.
 
-        :returns: this backend does not support items resuming
+        :returns: this backend supports items resuming
         """
-        return False
+        return True
 
     @staticmethod
     def metadata_id(item):
-        """Extracts the identifier from a Slack item.
+        """Extracts the identifier from a Rocket.Chat item."""
 
-        This identifier will be the mix of two fields because Slack
-        messages does not have any unique identifier. In this case,
-        'ts' and 'user' values (or 'bot_id' when the message is sent by a bot)
-        are combined because there have been cases where two messages were sent
-        by different users at the same time.
-        """
-        if 'user' in item:
-            nick = item['user']
-        elif 'comment' in item:
-            nick = item['comment']['user']
-        else:
-            nick = item['bot_id']
-
-        return item['ts'] + nick
+        return item["_id"]
 
     @staticmethod
     def metadata_updated_on(item):
-        """Extracts and coverts the update time from a Slack item.
+        """Extracts the update time from a Rocket.Chat item.
 
-        The timestamp is extracted from 'ts' field and converted
-        to a UNIX timestamp.
+        The timestamp is extracted from 'ts' field,
+        and then converted into a UNIX timestamp.
 
         :param item: item generated by the backend
 
-        :returns: a UNIX timestamp
+        :returns: extracted timestamp
         """
-        ts = float(item['ts'])
-
+        ts = str_to_datetime(item['_updatedAt']).timestamp()
         return ts
 
     @staticmethod
     def metadata_category(item):
-        """Extracts the category from a Slack item.
+        """Extracts the category from a Rocket.Chat item.
 
         This backend only generates one type of item which is
         'message'.
         """
-        return 'message'
-
-    @staticmethod
-    def parse_channel_info(raw_channel_info):
-        """Parse a channel info JSON stream.
+        return CATEGORY_MESSAGE
 
-        This method parses a JSON stream, containing the information
-        from a channel, and returns a dict with the parsed data.
+    def _init_client(self, from_archive=False):
+        """Init client"""
 
-        :param raw_channel_info
+        return RocketChatClient(self.url, self.user_id, self.api_token,
+                                self.max_items, self.sleep_for_rate,
+                                self.min_rate_to_sleep, from_archive, self.archive, self.ssl_verify)
 
-        :returns: a dict with the parsed information about a channel
-        """
-        result = json.loads(raw_channel_info)
-        return result['channel']
 
-    @staticmethod
-    def parse_history(raw_history):
-        """Parse a channel history JSON stream.
-
-        This method parses a JSON stream, containing the history of
-        a channel, and returns a list with the parsed data. It also
-        returns if there are more messages that are not included on
-        this stream.
-
-        :param raw_history: JSON string to parse
-
-        :returns: a tuple with a list of dicts with the parsed messages
-            and 'has_more' value
-        """
-        result = json.loads(raw_history)
-        return result['messages'], result['has_more']
-
-    @staticmethod
-    def parse_user(raw_user):
-        """Parse a user's info JSON stream.
-
-        This method parses a JSON stream, containing the information
-        from a user, and returns a dict with the parsed data.
-
-        :param raw_user: JSON string to parse
-
-        :returns: a dict with the parsed user's information
-        """
-        result = json.loads(raw_user)
-        return result['user']
+class RocketChatClient(HttpClient, RateLimitHandler):
+    """Rocket.Chat API client.
 
+    Client for fetching information from the Rocket.Chat server
+    using its REST API.
 
-class SlackClientError(BaseError):
-    """Raised when an error occurs using the Slack client"""
+    :param url: server url from where messages are to be fetched
+    :param user_id: generated User Id using your Rocket.Chat account
+    :param api_token: token needed to use the API
+    :param max_items: maximum number of message requested on the same query
+    :param sleep_for_rate: sleep until rate limit is reset
+    :param min_rate_to_sleep: minimum rate needed to sleep until
+         it will be reset
+    :param from_archive: it tells whether to write/read the archive
+    :param archive: archive to store/retrieve items
+    :param ssl_verify: enable/disable SSL verification
+    """
+    RCHANNEL_MESSAGES = 'channels.messages'
+    RCHANNEL_INFO = 'channels.info'
 
-    message = "%(error)s"
+    HAUTH_TOKEN = 'X-Auth-Token'
+    HUSER_ID = 'X-User-Id'
 
+    PCHANNEL_NAME = 'roomName'
+    PCOUNT = "count"
+    POLDEST = "oldest"
+
+    def __init__(self, url, user_id, api_token, max_items=MAX_ITEMS,
+                 sleep_for_rate=False, min_rate_to_sleep=MIN_RATE_LIMIT,
+                 from_archive=False, archive=None, ssl_verify=True):
 
-class SlackClient(HttpClient):
-    """Slack API client.
+        base_url = urijoin(url, API_EXTENSION)
+        self.user_id = user_id
+        self.api_token = api_token
+        self.max_items = max_items
 
-    Client for fetching information from the Slack server
-    using its REST API.
+        super().__init__(base_url, archive=archive, from_archive=from_archive,
+                         ssl_verify=ssl_verify)
+        super().setup_rate_limit_handler(sleep_for_rate=sleep_for_rate, min_rate_to_sleep=min_rate_to_sleep)
 
-    :param api_key: key needed to use the API
-    :param max_items: maximum number of items per request
-    """
-    URL = urijoin(SLACK_URL, 'api', '%(resource)s')
+    def calculate_time_to_reset(self):
+        """Number of seconds to wait. They are contained in the rate limit reset header."""
 
-    RCHANNEL_INFO = 'channels.info'
-    RCHANNEL_HISTORY = 'channels.history'
-    RUSER_INFO = 'users.info'
+        time_to_reset = self.rate_limit_reset_ts - (datetime_utcnow().replace(microsecond=0).timestamp() + 1) * 1000
+        time_to_reset /= 1000
 
-    PCHANNEL = 'channel'
-    PCOUNT = 'count'
-    POLDEST = 'oldest'
-    PLATEST = 'latest'
-    PTOKEN = 'token'
-    PUSER = 'user'
+        if time_to_reset < 0:
+            time_to_reset = 0
 
-    def __init__(self, api_token, max_items=MAX_ITEMS):
-        super().__init__(SLACK_URL)
-        self.api_token = api_token
-        self.max_items = max_items
+        return time_to_reset
 
     def channel_info(self, channel):
         """Fetch information about a channel."""
 
-        resource = self.RCHANNEL_INFO
-
         params = {
-            self.PCHANNEL: channel,
+            self.PCHANNEL_NAME: channel,
         }
 
-        response = self._fetch(resource, params)
+        path = urijoin(self.base_url, self.RCHANNEL_INFO)
+        response = self.fetch(path, params)
 
         return response
 
-    def history(self, channel, oldest=None, latest=None):
-        """Fetch the history of a channel."""
+    def messages(self, channel, from_date, offset):
+        """Fetch messages from a channel.
 
-        resource = self.RCHANNEL_HISTORY
+        The messages are fetch in ascending order i.e. from the oldest
+        to the latest based on the time they were last updated. A query is
+        also passed as a param to fetch the messages from a given date.
+        """
+        query = '{"_updatedAt": {"$gte": {"$date": "%s"}}}' % from_date.isoformat()
 
+        # The 'sort' param accepts a field based on which the messages are sorted.
+        # The value of the field can be 1 for ascending order or -1 for descending order.
         params = {
-            self.PCHANNEL: channel,
-            self.PCOUNT: self.max_items
+            "roomName": channel,
+            "sort": '{"_updatedAt": 1}',
+            "count": self.max_items,
+            "offset": offset,
+            "query": query
         }
 
-        if oldest is not None:
-            params[self.POLDEST] = oldest
-        if latest is not None:
-            params[self.PLATEST] = latest
-
-        response = self._fetch(resource, params)
+        path = urijoin(self.base_url, self.RCHANNEL_MESSAGES)
+        response = self.fetch(path, params)
 
         return response
 
-    def user(self, user_id):
-        """Fetch user info."""
-
-        resource = self.RUSER_INFO
+    def fetch(self, url, payload=None, headers=None):
+        """Fetch the data from a given URL.
 
-        params = {
-            self.PUSER: user_id
+        :param url: link to the resource
+        :param payload: payload of the request
+        :param headers: headers of the request
+
+        :returns a response object
+        """
+        headers = {
+            self.HAUTH_TOKEN: self.api_token,
+            self.HUSER_ID: self.user_id
         }
 
-        response = self._fetch(resource, params)
+        logger.debug("Rocket.Chat client message request with params: %s", str(payload))
 
-        return response
+        if not self.from_archive:
+            self.sleep_for_rate_limit()
 
-    def _fetch(self, resource, params):
-        """Fetch a resource.
+        response = super().fetch(url, payload, headers=headers)
 
-        :param resource: resource to get
-        :param params: dict with the HTTP parameters needed to get
-            the given resource
-        """
-        url = self.URL % {'resource': resource}
-        params[self.PTOKEN] = self.api_token
+        if not self.from_archive:
+            self.update_rate_limit(response)
 
-        logger.debug("Slack client requests: %s params: %s",
-                     resource, str(params))
+        return response.text
 
-        r = self.fetch(url, payload=params)
+    @staticmethod
+    def sanitize_for_archive(url, headers, payload):
+        """Sanitize payload of a HTTP request by removing the token and
+         user id information before storing/retrieving archived items.
 
-        # Check for possible API errors
-        result = r.json()
+        :param: url: HTTP url request
+        :param: headers: HTTP headers request
+        :param: payload: HTTP payload request
 
-        if not result['ok']:
-            raise SlackClientError(error=result['error'])
+        :returns: url, headers and the sanitized payload
+        """
+        if RocketChatClient.HAUTH_TOKEN in headers:
+            headers.pop(RocketChatClient.HAUTH_TOKEN)
 
-        return r.text
+        if RocketChatClient.HUSER_ID in headers:
+            headers.pop(RocketChatClient.HUSER_ID)
 
+        return url, headers, payload
 
-class SlackCommand(BackendCommand):
-    """Class to run Slack backend from the command line."""
 
-    BACKEND = Slack
+class RocketChatCommand(BackendCommand):
+    """Class to run Rocket.Chat backend from the command line."""
 
-    @staticmethod
-    def setup_cmd_parser():
-        """Returns the Slack argument parser."""
+    BACKEND = RocketChat
+
+    @classmethod
+    def setup_cmd_parser(cls):
+        """Returns the Rocket.Chat argument parser."""
 
-        parser = BackendCommandArgumentParser(from_date=True,
+        parser = BackendCommandArgumentParser(cls.BACKEND,
+                                              from_date=True,
                                               token_auth=True,
-                                              cache=True)
+                                              archive=True,
+                                              ssl_verify=True)
 
         # Backend token is required
         action = parser.parser._option_string_actions['--api-token']
         action.required = True
 
-        # Slack options
-        group = parser.parser.add_argument_group('Slack arguments')
+        parser.parser.add_argument('-u', '--user-id', dest='user_id',
+                                   required=True,
+                                   help="User Id to fetch messages")
+
+        # Required positional arguments
+        parser.parser.add_argument('url',
+                                   help="URL of the Rocket.Chat server")
+
+        parser.parser.add_argument('channel',
+                                   help="Rocket.Chat channel(room) name")
+
+        # Rocket.Chat options
+        group = parser.parser.add_argument_group('Rocket.Chat arguments')
         group.add_argument('--max-items', dest='max_items',
                            type=int, default=MAX_ITEMS,
                            help="Maximum number of items requested on the same query")
-
-        # Required arguments
-        parser.parser.add_argument('channel',
-                                   help="Slack channel identifier")
+        group.add_argument('--sleep-for-rate', dest='sleep_for_rate',
+                           action='store_true',
+                           help="sleep for getting more rate")
+        group.add_argument('--min-rate-to-sleep', dest='min_rate_to_sleep',
+                           default=MIN_RATE_LIMIT, type=int,
+                           help="sleep until reset when the rate limit reaches this value")
 
         return parser
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `perceval-0.9.9/perceval/backends/core/mbox.py` & `perceval-1.0.0rc1/perceval/backends/core/mbox.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,52 +1,57 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2017 Bitergia
+# Copyright (C) 2015-2020 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1335, USA.
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #     Santiago Dueñas <sduenas@bitergia.com>
 #     Germán Poo-Caamaño <gpoo@gnome.org>
+#     Stephan Barth <stephan.barth@gmail.com>
+#     Valerio Cosentino <valcos@bitergia.com>
+#     Jesus M. Gonzalez-Barahona <jgb@gsyc.es>
+#     Harshal Mittal <harshalmittal4@gmail.com>
 #
-# Note: some ot this code was taken from the MailingListStats project
-#
+
+# Note: some of this code was taken from the MailingListStats project
 
 import logging
 import mailbox
 import os
 import tempfile
 
 import gzip
 import bz2
+import zipfile
 
-from grimoirelab.toolkit.datetime import (InvalidDateError,
+from grimoirelab_toolkit.datetime import (InvalidDateError,
                                           datetime_to_utc,
                                           str_to_datetime)
 
 from ...backend import (Backend,
                         BackendCommand,
-                        BackendCommandArgumentParser,
-                        metadata)
+                        BackendCommandArgumentParser)
 from ...utils import (DEFAULT_DATETIME,
+                      DEFAULT_LAST_DATETIME,
                       check_compressed_file_type,
                       message_to_dict)
 
+CATEGORY_MESSAGE = "message"
 
 logger = logging.getLogger(__name__)
 
 
 class MBox(Backend):
     """MBox backend.
 
@@ -55,107 +60,213 @@
     the mbox files are stored. The origin of the data will be set to to
     the value of `uri`.
 
     :param uri: URI of the mboxes; typically, the URL of their
         mailing list
     :param dirpath: directory path where the mboxes are stored
     :param tag: label used to mark the data
-    :param cache: cache object to store raw data
+    :param archive: archive to store/retrieve items
+    :param ssl_verify: enable/disable SSL verification
     """
-    version = '0.7.4'
+    version = '1.0.0'
+
+    CATEGORIES = [CATEGORY_MESSAGE]
 
     DATE_FIELD = 'Date'
     MESSAGE_ID_FIELD = 'Message-ID'
 
-    def __init__(self, uri, dirpath, tag=None, cache=None):
+    def __init__(self, uri, dirpath, tag=None, archive=None, ssl_verify=True):
         origin = uri
 
-        super().__init__(origin, tag=tag, cache=cache)
+        super().__init__(origin, tag=tag, archive=archive, ssl_verify=ssl_verify)
         self.uri = uri
         self.dirpath = dirpath
 
-    @metadata
-    def fetch(self, from_date=DEFAULT_DATETIME):
+    def fetch(self, category=CATEGORY_MESSAGE, from_date=DEFAULT_DATETIME, to_date=DEFAULT_LAST_DATETIME):
         """Fetch the messages from a set of mbox files.
 
         The method retrieves, from mbox files, the messages stored in
         these containers.
 
+        :param category: the category of items to fetch
         :param from_date: obtain messages since this date
+        :param to_date: obtain messages until this date
 
         :returns: a generator of messages
         """
-        logger.info("Looking for messages from '%s' on '%s' since %s",
-                    self.uri, self.dirpath, str(from_date))
+        if not from_date:
+            from_date = DEFAULT_DATETIME
+        if not to_date:
+            to_date = DEFAULT_LAST_DATETIME
+
+        kwargs = {
+            'from_date': from_date,
+            'to_date': to_date
+        }
+        items = super().fetch(category, **kwargs)
+
+        return items
+
+    def fetch_items(self, category, **kwargs):
+        """Fetch the messages
+
+        :param category: the category of items to fetch
+        :param kwargs: backend arguments
+
+        :returns: a generator of items
+        """
+        from_date = kwargs['from_date']
+        to_date = kwargs['to_date']
+
+        logger.info("Looking for messages from '%s' on '%s' since %s until %s",
+                    self.uri, self.dirpath, str(from_date), str(to_date))
 
         mailing_list = MailingList(self.uri, self.dirpath)
 
-        messages = self._fetch_and_parse_messages(mailing_list, from_date)
+        messages = self._fetch_and_parse_messages(mailing_list, from_date, to_date)
 
         for message in messages:
             yield message
 
         logger.info("Fetch process completed")
 
-    def _fetch_and_parse_messages(self, mailing_list, from_date):
+    @classmethod
+    def has_archiving(cls):
+        """Returns whether it supports archiving items on the fetch process.
+
+        :returns: this backend does not support items archive
+        """
+        return False
+
+    @classmethod
+    def has_resuming(cls):
+        """Returns whether it supports to resume the fetch process.
+
+        :returns: this backend supports items resuming
+        """
+        return True
+
+    @staticmethod
+    def metadata_id(item):
+        """Extracts the identifier from a MBox item."""
+
+        return item[MBox.MESSAGE_ID_FIELD]
+
+    @staticmethod
+    def metadata_updated_on(item):
+        """Extracts the update time from a MBox item.
+
+        The timestamp used is extracted from 'Date' field in its
+        several forms. This date is converted to UNIX timestamp
+        format.
+
+        :param item: item generated by the backend
+
+        :returns: a UNIX timestamp
+        """
+        ts = item[MBox.DATE_FIELD]
+        ts = str_to_datetime(ts)
+
+        return ts.timestamp()
+
+    @staticmethod
+    def metadata_category(item):
+        """Extracts the category from a MBox item.
+
+        This backend only generates one type of item which is
+        'message'.
+        """
+        return CATEGORY_MESSAGE
+
+    @staticmethod
+    def parse_mbox(filepath):
+        """Parse a mbox file.
+
+        This method parses a mbox file and returns an iterator of dictionaries.
+        Each one of this contains an email message.
+
+        :param filepath: path of the mbox to parse
+
+        :returns : generator of messages; each message is stored in a
+            dictionary of type `requests.structures.CaseInsensitiveDict`
+        """
+        mbox = _MBox(filepath, create=False)
+
+        for msg in mbox:
+            message = message_to_dict(msg)
+            yield message
+
+    def _init_client(self, from_archive=False):
+        pass
+
+    def _fetch_and_parse_messages(self, mailing_list, from_date, to_date=DEFAULT_LAST_DATETIME):
         """Fetch and parse the messages from a mailing list"""
 
         from_date = datetime_to_utc(from_date)
+        to_date = datetime_to_utc(to_date)
 
         nmsgs, imsgs, tmsgs = (0, 0, 0)
 
         for mbox in mailing_list.mboxes:
+            tmp_path = None
+
             try:
                 tmp_path = self._copy_mbox(mbox)
 
                 for message in self.parse_mbox(tmp_path):
                     tmsgs += 1
 
                     if not self._validate_message(message):
                         imsgs += 1
                         continue
 
-                    # Ignore those messages sent before the given date
+                    # Ignore those messages sent before from date and after to date
                     dt = str_to_datetime(message[MBox.DATE_FIELD])
 
                     if dt < from_date:
                         logger.debug("Message %s sent before %s; skipped",
                                      message['unixfrom'], str(from_date))
                         tmsgs -= 1
                         continue
 
+                    if dt > to_date:
+                        logger.debug("Message %s sent after %s; skipped",
+                                     message['unixfrom'], str(to_date))
+                        tmsgs -= 1
+                        continue
+
                     # Convert 'CaseInsensitiveDict' to dict
                     message = self._casedict_to_dict(message)
 
                     nmsgs += 1
                     logger.debug("Message %s parsed", message['unixfrom'])
 
                     yield message
-            except OSError as e:
+            except (OSError, EOFError) as e:
                 logger.warning("Ignoring %s mbox due to: %s", mbox.filepath, str(e))
             except Exception as e:
-                if os.path.exists(tmp_path):
+                if tmp_path and os.path.exists(tmp_path):
                     os.remove(tmp_path)
                 raise e
             finally:
-                if os.path.exists(tmp_path):
+                if tmp_path and os.path.exists(tmp_path):
                     os.remove(tmp_path)
 
         logger.info("Done. %s/%s messages fetched; %s ignored",
                     nmsgs, tmsgs, imsgs)
 
     def _copy_mbox(self, mbox):
         """Copy the contents of a mbox to a temporary file"""
 
         tmp_path = tempfile.mktemp(prefix='perceval_')
 
         with mbox.container as f_in:
             with open(tmp_path, mode='wb') as f_out:
-                for l in f_in:
-                    f_out.write(l)
+                for line in f_in:
+                    f_out.write(line)
         return tmp_path
 
     def _validate_message(self, message):
         """Check if the given message has the mandatory fields"""
 
         # This check is "case insensitive" because we're
         # using 'CaseInsensitiveDict' from requests.structures
@@ -200,80 +311,14 @@
 
         msg = {k: v for k, v in message.items()}
         msg[self.MESSAGE_ID_FIELD] = message_id
         msg[self.DATE_FIELD] = date
 
         return msg
 
-    @classmethod
-    def has_caching(cls):
-        """Returns whether it supports caching items on the fetch process.
-
-        :returns: this backend does not support items cache
-        """
-        return False
-
-    @classmethod
-    def has_resuming(cls):
-        """Returns whether it supports to resume the fetch process.
-
-        :returns: this backend supports items resuming
-        """
-        return True
-
-    @staticmethod
-    def metadata_id(item):
-        """Extracts the identifier from a MBox item."""
-
-        return item[MBox.MESSAGE_ID_FIELD]
-
-    @staticmethod
-    def metadata_updated_on(item):
-        """Extracts the update time from a MBox item.
-
-        The timestamp used is extracted from 'Date' field in its
-        several forms. This date is converted to UNIX timestamp
-        format.
-
-        :param item: item generated by the backend
-
-        :returns: a UNIX timestamp
-        """
-        ts = item[MBox.DATE_FIELD]
-        ts = str_to_datetime(ts)
-
-        return ts.timestamp()
-
-    @staticmethod
-    def metadata_category(item):
-        """Extracts the category from a MBox item.
-
-        This backend only generates one type of item which is
-        'message'.
-        """
-        return 'message'
-
-    @staticmethod
-    def parse_mbox(filepath):
-        """Parse a mbox file.
-
-        This method parses a mbox file and returns an iterator of dictionaries.
-        Each one of this contains an email message.
-
-        :param filepath: path of the mbox to parse
-
-        :returns : generator of messages; each message is stored in a
-            dictionary of type `requests.structures.CaseInsensitiveDict`
-        """
-        mbox = _MBox(filepath, create=False)
-
-        for msg in mbox:
-            message = message_to_dict(msg)
-            yield message
-
 
 class _MBox(mailbox.mbox):
     """Wrapper of `mailbox.mbox` to catch unhandled errors"""
 
     def get_message(self, key):
         """Return a Message representation or raise a KeyError."""
 
@@ -298,34 +343,37 @@
 
 
 class MBoxCommand(BackendCommand):
     """Class to run MBox backend from the command line."""
 
     BACKEND = MBox
 
-    @staticmethod
-    def setup_cmd_parser():
+    @classmethod
+    def setup_cmd_parser(cls):
         """Returns the MBox argument parser."""
 
-        parser = BackendCommandArgumentParser(from_date=True)
+        parser = BackendCommandArgumentParser(cls.BACKEND,
+                                              from_date=True,
+                                              to_date=True,
+                                              ssl_verify=True)
 
         # Required arguments
         parser.parser.add_argument('uri',
                                    help="URI of the mboxes, usually the URL to their mailing list")
         parser.parser.add_argument('dirpath',
                                    help="Path to the mbox directory")
 
         return parser
 
 
 class MBoxArchive(object):
     """Class to access a mbox archive.
 
     MBOX archives can be stored into plain or compressed files
-    (gzip and bz2).
+    (gzip, bz2 or zip).
 
     :param filepath: path to the mbox file
     """
     def __init__(self, filepath):
         self._filepath = filepath
         self._compressed = check_compressed_file_type(filepath)
 
@@ -338,14 +386,19 @@
         if not self.is_compressed():
             return open(self.filepath, mode='rb')
 
         if self.compressed_type == 'bz2':
             return bz2.open(self.filepath, mode='rb')
         elif self.compressed_type == 'gz':
             return gzip.open(self.filepath, mode='rb')
+        elif self.compressed_type == "zip":
+            _zip = zipfile.ZipFile(self.filepath)
+            if len(_zip.infolist()) > 1:
+                logger.error("Zip %s contains more than one file, only the first uncompressed", self.filepath)
+            return _zip.open(_zip.infolist()[0].filename)
 
     @property
     def compressed_type(self):
         return self._compressed
 
     def is_compressed(self):
         return self._compressed is not None
```

### Comparing `perceval-0.9.9/perceval/backends/core/pipermail.py` & `perceval-1.0.0rc1/perceval/backends/core/pipermail.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,108 +1,127 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2017 Bitergia
+# Copyright (C) 2015-2020 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1335, USA.
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #     Santiago Dueñas <sduenas@bitergia.com>
 #     Germán Poo-Caamaño <gpoo@gnome.org>
+#     Stephan Barth <stephan.barth@gmail.com>
+#     Valerio Cosentino <valcos@bitergia.com>
+#     Jesus M. Gonzalez-Barahona <jgb@gsyc.es>
+#     Harshal Mittal <harshalmittal4@gmail.com>
 #
-# Note: some ot this code was based on parts of the MailingListStats project
-#
+
+# Note: some of this code was based on parts of the MailingListStats project
 
 import datetime
 import logging
 import os
 
 import bs4
 import dateutil
 import requests
 
-from grimoirelab.toolkit.datetime import datetime_to_utc
-from grimoirelab.toolkit.uris import urijoin
+from grimoirelab_toolkit.datetime import datetime_to_utc
+from grimoirelab_toolkit.uris import urijoin
 
-from .mbox import MBox, MailingList
-from ...backend import BackendCommand, BackendCommandArgumentParser, metadata
+from .mbox import MBox, MailingList, CATEGORY_MESSAGE
+from ...backend import (BackendCommand,
+                        BackendCommandArgumentParser)
 from ...utils import DEFAULT_DATETIME
 
-
-logger = logging.getLogger(__name__)
-
-
 PIPERMAIL_COMPRESSED_TYPES = ['.gz', '.bz2', '.zip',
                               '.tar', '.tar.gz', '.tar.bz2',
                               '.tgz', '.tbz']
 PIPERMAIL_ACCEPTED_TYPES = ['.mbox', '.txt']
 PIPERMAIL_TYPES = PIPERMAIL_COMPRESSED_TYPES + PIPERMAIL_ACCEPTED_TYPES
 
 MOD_MBOX_THREAD_STR = "/thread"
 
+logger = logging.getLogger(__name__)
+
 
 class Pipermail(MBox):
     """Pipermail backend.
 
     This class allows the fetch the email messages stored on a Pipermail
     archiver. Initialize this class passing the URL where the archiver is
     and the directory path where the mbox files will be fetched and
     stored. The origin of the data will be set to the value of `url`.
 
     :param url: URL to the Pipermail archiver
     :param dirpath: directory path where the mboxes are stored
     :param tag: label used to mark the data
-    :param cache: cache object to store raw data
+    :param archive: archive to store/retrieve items
+    :param ssl_verify: enable/disable SSL verification
     """
-    version = '0.4.3'
+    version = '1.0.0'
+
+    CATEGORIES = [CATEGORY_MESSAGE]
 
-    def __init__(self, url, dirpath, tag=None, cache=None):
-        super().__init__(url, dirpath, tag=tag, cache=cache)
+    def __init__(self, url, dirpath, tag=None, archive=None, ssl_verify=True):
+        super().__init__(url, dirpath, tag=tag, archive=archive, ssl_verify=ssl_verify)
         self.url = url
 
-    @metadata
-    def fetch(self, from_date=DEFAULT_DATETIME):
+    def fetch(self, category=CATEGORY_MESSAGE, from_date=DEFAULT_DATETIME):
         """Fetch the messages from the Pipermail archiver.
 
         The method fetches the mbox files from a remote Pipermail
         archiver and retrieves the messages stored on them.
 
+        :param category: the category of items to fetch
         :param from_date: obtain messages since this date
 
         :returns: a generator of messages
         """
+        items = super().fetch(category, from_date)
+
+        return items
+
+    def fetch_items(self, category, **kwargs):
+        """Fetch the messages
+
+        :param category: the category of items to fetch
+        :param kwargs: backend arguments
+
+        :returns: a generator of items
+        """
+        from_date = kwargs['from_date']
+
         logger.info("Looking for messages from '%s' since %s",
                     self.url, str(from_date))
 
-        mailing_list = PipermailList(self.url, self.dirpath)
+        mailing_list = PipermailList(self.url, self.dirpath, self.ssl_verify)
         mailing_list.fetch(from_date=from_date)
 
         messages = self._fetch_and_parse_messages(mailing_list, from_date)
 
         for message in messages:
             yield message
 
         logger.info("Fetch process completed")
 
     @classmethod
-    def has_caching(cls):
-        """Returns whether it supports caching items on the fetch process.
+    def has_archiving(cls):
+        """Returns whether it supports archiving items on the fetch process.
 
-        :returns: this backend dooes not support items cache
+        :returns: this backend does not support items archive
         """
         return False
 
     @classmethod
     def has_resuming(cls):
         """Returns whether it supports to resume the fetch process.
 
@@ -123,19 +142,21 @@
             base_path = os.path.expanduser('~/.perceval/mailinglists/')
             dirpath = os.path.join(base_path, self.parsed_args.url)
         else:
             dirpath = self.parsed_args.mboxes_path
 
         setattr(self.parsed_args, 'dirpath', dirpath)
 
-    @staticmethod
-    def setup_cmd_parser():
+    @classmethod
+    def setup_cmd_parser(cls):
         """Returns the Pipermail argument parser."""
 
-        parser = BackendCommandArgumentParser(from_date=True)
+        parser = BackendCommandArgumentParser(cls.BACKEND,
+                                              from_date=True,
+                                              ssl_verify=True)
 
         # Optional arguments
         group = parser.parser.add_argument_group('Pipermail arguments')
         group.add_argument('--mboxes-path', dest='mboxes_path',
                            help="Path where mbox files will be stored")
 
         # Required arguments
@@ -150,18 +171,20 @@
 
     This class gives access to remote and local mboxes archives
     from a mailing list stored by Pipermail. This class also allows
     to keep them in sync.
 
     :param url: URL to the Pipermail archiver for this list
     :param dirpath: path to the local mboxes archives
+    :param ssl_verify: enable/disable SSL verification
     """
-    def __init__(self, url, dirpath):
+    def __init__(self, url, dirpath, ssl_verify=True):
         super().__init__(url, dirpath)
         self.url = url
+        self.ssl_verify = ssl_verify
 
     def fetch(self, from_date=DEFAULT_DATETIME):
         """Fetch the mbox files from the remote archiver.
 
         Stores the archives in the path given during the initialization
         of this object. Those archives which a not valid extension will
         be ignored.
@@ -180,38 +203,38 @@
         """
         logger.info("Downloading mboxes from '%s' to since %s",
                     self.url, str(from_date))
         logger.debug("Storing mboxes in '%s'", self.dirpath)
 
         from_date = datetime_to_utc(from_date)
 
-        r = requests.get(self.url)
+        r = requests.get(self.url, verify=self.ssl_verify)
         r.raise_for_status()
 
         links = self._parse_archive_links(r.text)
 
         fetched = []
 
         if not os.path.exists(self.dirpath):
             os.makedirs(self.dirpath)
 
-        for l in links:
-            filename = os.path.basename(l)
+        for link in links:
+            filename = os.path.basename(link)
 
             mbox_dt = self._parse_date_from_filepath(filename)
 
             if ((from_date.year == mbox_dt.year and
                 from_date.month == mbox_dt.month) or
                 from_date < mbox_dt):
 
                 filepath = os.path.join(self.dirpath, filename)
-                success = self._download_archive(l, filepath)
+                success = self._download_archive(link, filepath)
 
                 if success:
-                    fetched.append((l, filepath))
+                    fetched.append((link, filepath))
 
         logger.info("%s/%s MBoxes downloaded", len(fetched), len(links))
 
         return fetched
 
     @property
     def mboxes(self):
@@ -228,15 +251,15 @@
             archives.append((dt, mbox))
 
         archives.sort(key=lambda x: x[0])
 
         return [a[1] for a in archives]
 
     def _parse_archive_links(self, raw_html):
-        bs = bs4.BeautifulSoup(raw_html)
+        bs = bs4.BeautifulSoup(raw_html, 'html.parser')
 
         candidates = [a['href'] for a in bs.find_all('a', href=True)]
         links = []
 
         for candidate in candidates:
             # Links from Apache's 'mod_mbox' plugin contain
             # trailing "/thread" substrings. Remove them to get
@@ -271,20 +294,29 @@
             logger.debug("Date of file %s not detected due to %s",
                          filepath, str(e))
             logger.debug("Date set to default: %s", str(dt))
 
         return dt
 
     def _download_archive(self, url, filepath):
-        r = requests.get(url, stream=True)
-        r.raise_for_status()
-
         try:
-            with open(filepath, 'wb') as fd:
-                fd.write(r.raw.read())
+            r = requests.get(url, stream=True, verify=self.ssl_verify)
+            r.raise_for_status()
+            self._write_archive(r, filepath)
+        except requests.exceptions.HTTPError as e:
+            if e.response.status_code == 403:
+                logger.warning("Ignoring %s archive due to: %s", url, str(e))
+                return False
+            else:
+                raise e
         except OSError as e:
             logger.warning("Ignoring %s archive due to: %s", url, str(e))
             return False
 
         logger.debug("%s archive downloaded and stored in %s", url, filepath)
 
         return True
+
+    @staticmethod
+    def _write_archive(r, filepath):
+        with open(filepath, 'wb') as fd:
+            fd.write(r.raw.read())
```

### Comparing `perceval-0.9.9/perceval/backends/core/rss.py` & `perceval-1.0.0rc1/perceval/backends/core/rss.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,117 +1,115 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2016-2017 Bitergia
+# Copyright (C) 2015-2020 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1335, USA.
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #     Alvaro del Castillo <acs@bitergia.com>
+#     Santiago Dueñas <sduenas@bitergia.com>
+#     Stephan Barth <stephan.barth@gmail.com>
+#     Valerio Cosentino <valcos@bitergia.com>
+#     Jesus M. Gonzalez-Barahona <jgb@gsyc.es>
+#     Harshal Mittal <harshalmittal4@gmail.com>
 #
 
 import logging
 
 import feedparser
 
-from grimoirelab.toolkit.datetime import str_to_datetime
+from grimoirelab_toolkit.datetime import str_to_datetime
 
 from ...backend import (Backend,
                         BackendCommand,
-                        BackendCommandArgumentParser,
-                        metadata)
+                        BackendCommandArgumentParser)
 from ...client import HttpClient
-from ...errors import CacheError
 
+CATEGORY_ENTRY = "entry"
 
 logger = logging.getLogger(__name__)
 
 
 class RSS(Backend):
     """RSS backend for Perceval.
 
     This class retrieves the entries from a RSS feed.
     To initialize this class the URL must be provided.
     The `url` will be set as the origin of the data.
 
     :param url: RSS url
     :param tag: label used to mark the data
-    :param cache: cache object to store raw data
+    :param archive: archive to store/retrieve items
+    :param ssl_verify: enable/disable SSL verification
     """
-    version = '0.2.0'
+    version = '1.0.0'
 
-    def __init__(self, url, tag=None, cache=None):
+    CATEGORIES = [CATEGORY_ENTRY]
+
+    def __init__(self, url, tag=None, archive=None, ssl_verify=True):
         origin = url
 
-        super().__init__(origin, tag=tag, cache=cache)
+        super().__init__(origin, tag=tag, archive=archive, ssl_verify=ssl_verify)
         self.url = url
-        self.client = RSSClient(url)
+        self.client = None
 
-    @metadata
-    def fetch(self):
+    def fetch(self, category=CATEGORY_ENTRY):
         """Fetch the entries from the url.
 
         The method retrieves all entries from a RSS url
 
+        :param category: the category of items to fetch
+
         :returns: a generator of entries
         """
+        kwargs = {}
+        items = super().fetch(category, **kwargs)
+
+        return items
+
+    def fetch_items(self, category, **kwargs):
+        """Fetch the entries
+
+        :param category: the category of items to fetch
+        :param kwargs: backend arguments
 
+        :returns: a generator of items
+        """
         logger.info("Looking for rss entries at feed '%s'", self.url)
 
-        self._purge_cache_queue()
         nentries = 0  # number of entries
 
         raw_entries = self.client.get_entries()
-        self._push_cache_queue(raw_entries)
         entries = self.parse_feed(raw_entries)['entries']
-        self._flush_cache_queue()
         for item in entries:
             yield item
             nentries += 1
 
         logger.info("Total number of entries: %i", nentries)
 
     @classmethod
     def parse_feed(self, raw_entries):
         return feedparser.parse(raw_entries)
 
-    @metadata
-    def fetch_from_cache(self):
-        """Fetch the entries from the cache.
-
-        :returns: a generator of entries
-
-        :raises CacheError: raised when an error occurs accessing the
-            cache
-        """
-        if not self.cache:
-            raise CacheError(cause="cache instance was not provided")
-
-        cache_entries = next(self.cache.retrieve())
-        entries = feedparser.parse(cache_entries)['entries']
-
-        for item in entries:
-            yield item
-
     @classmethod
-    def has_caching(cls):
-        """Returns whether it supports caching entries on the fetch process.
+    def has_archiving(cls):
+        """Returns whether it supports archiving entries on the fetch process.
 
-        :returns: this backend supports entries cache
+        :returns: this backend supports entries archive
         """
         return True
 
     @classmethod
     def has_resuming(cls):
         """Returns whether it supports to resume the fetch process.
 
@@ -143,47 +141,57 @@
     @staticmethod
     def metadata_category(item):
         """Extracts the category from a RSS item.
 
         This backend only generates one type of item which is
         'entry'.
         """
-        return 'entry'
+        return CATEGORY_ENTRY
+
+    def _init_client(self, from_archive=False):
+        """Init client"""
+
+        return RSSClient(self.url, self.archive, from_archive, self.ssl_verify)
 
 
 class RSSClient(HttpClient):
     """RSS API client.
 
     This class implements a simple client to retrieve entries from
     projects in a RSS node.
 
     :param url: URL of rss node: https://item.opnfv.org/ci
+    :param archive: an archive to store/read fetched data
+    :param from_archive: it tells whether to write/read the archive
+    :param ssl_verify: enable/disable SSL verification
 
     :raises HTTPError: when an error occurs doing the request
     """
 
-    def __init__(self, url):
-        super().__init__(url)
+    def __init__(self, url, archive=None, from_archive=False, ssl_verify=True):
+        super().__init__(url, archive=archive, from_archive=from_archive, ssl_verify=ssl_verify)
 
     def get_entries(self):
         """ Retrieve all entries from a RSS feed"""
 
         req = self.fetch(self.base_url)
         return req.text
 
 
 class RSSCommand(BackendCommand):
     """Class to run RSS backend from the command line."""
 
     BACKEND = RSS
 
-    @staticmethod
-    def setup_cmd_parser():
+    @classmethod
+    def setup_cmd_parser(cls):
         """Returns the RSS argument parser."""
 
-        parser = BackendCommandArgumentParser(cache=True)
+        parser = BackendCommandArgumentParser(cls.BACKEND,
+                                              archive=True,
+                                              ssl_verify=True)
 
         # Required arguments
         parser.parser.add_argument('url',
                                    help="URL of the RSS feed")
 
         return parser
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `perceval-0.9.9/perceval/backends/core/discourse.py` & `perceval-1.0.0rc1/perceval/backends/core/nntp.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,407 +1,390 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2016-2017 Bitergia
+# Copyright (C) 2015-2020 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1335, USA.
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
-#    Santiago Dueñas <sduenas@bitergia.com>
-#    J. Manrique López de la Fuente <jsmanrique@bitergia.com>
-#    Alvaro del Castillo San Felix <acs@bitergia.com>
+#     Santiago Dueñas <sduenas@bitergia.com>
+#     Valerio Cosentino <valcos@bitergia.com>
+#     Jesus M. Gonzalez-Barahona <jgb@gsyc.es>
+#     Harshal Mittal <harshalmittal4@gmail.com>
 #
 
-import json
+import io
 import logging
+import nntplib
+import email
 
-from grimoirelab.toolkit.datetime import datetime_to_utc, str_to_datetime
-from grimoirelab.toolkit.uris import urijoin
+from grimoirelab_toolkit.datetime import str_to_datetime, InvalidDateError
 
 from ...backend import (Backend,
                         BackendCommand,
-                        BackendCommandArgumentParser,
-                        metadata)
-from ...client import HttpClient
-from ...errors import CacheError
-from ...utils import DEFAULT_DATETIME
+                        BackendCommandArgumentParser)
+from ...errors import ArchiveError, ParseError
+from ...utils import message_to_dict
+
+CATEGORY_ARTICLE = "article"
+DEFAULT_OFFSET = 1
+FALLBACK_DATE = '1970-01-01'
 
+# Hack to avoid "line too long" errors
+nntplib._MAXLINE = 65536
 
 logger = logging.getLogger(__name__)
 
 
-class Discourse(Backend):
-    """Discourse backend for Perceval.
+class NNTP(Backend):
+    """NNTP backend.
 
-    This class retrieves the topics posted in a Discourse board.
-    To initialize this class the URL must be provided. The `url`
-    will be set as the origin of the data.
+    This class allows to fetch the articles published on a news group
+    using NNTP. It is initialized giving the host and the name of the
+    news group.
 
-    :param url: Discourse URL
-    :param api_token: Discourse API access token
+    :param host: host
+    :param group: name of the group
     :param tag: label used to mark the data
-    :param cache: cache object to store raw data
+    :param archive: archive to store/retrieve items
     """
-    version = '0.6.0'
+    version = '1.0.0'
 
-    def __init__(self, url, api_token=None,
-                 tag=None, cache=None):
-        origin = url
+    CATEGORIES = [CATEGORY_ARTICLE]
+    EXTRA_SEARCH_FIELDS = {
+        'newsgroups': ['Newsgroups']
+    }
 
-        super().__init__(origin, tag=tag, cache=cache)
-        self.url = url
-        self.client = DiscourseClient(url, api_key=api_token)
+    def __init__(self, host, group, tag=None, archive=None):
+        origin = host + '-' + group
 
-    @metadata
-    def fetch(self, from_date=DEFAULT_DATETIME):
-        """Fetch the topics from the Discurse board.
+        super().__init__(origin, tag=tag, archive=archive)
+        self.host = host
+        self.group = group
+        self.client = None
 
-        The method retrieves, from a Discourse board the topics
-        updated since the given date.
+    def fetch(self, category=CATEGORY_ARTICLE, offset=DEFAULT_OFFSET):
+        """Fetch articles posted on a news group.
 
-        :param from_date: obtain topics updated since this date
+        This method fetches those messages or articles published
+        on a news group starting on the given offset.
 
-        :returns: a generator of topics
-        """
-        if not from_date:
-            from_date = DEFAULT_DATETIME
-        else:
-            from_date = datetime_to_utc(from_date)
+        :param category: the category of items to fetch
+        :param offset: obtain messages from this offset
 
-        logger.info("Looking for topics at '%s', updated from '%s'",
-                    self.url, str(from_date))
+        :returns: a generator of articles
+        """
+        if not offset:
+            offset = DEFAULT_OFFSET
 
-        self._purge_cache_queue()
+        kwargs = {'offset': offset}
+        items = super().fetch(category, **kwargs)
 
-        ntopics = 0
+        return items
 
-        topics_ids = self.__fetch_and_parse_topics_ids(from_date)
+    def fetch_items(self, category, **kwargs):
+        """Fetch the articles
 
-        for topic_id in topics_ids:
-            topic = self.__fetch_and_parse_topic(topic_id)
-            ntopics += 1
-            yield topic
-            self._flush_cache_queue()
+        :param category: the category of items to fetch
+        :param kwargs: backend arguments
 
-        logger.info("Fetch process completed: %s topics fetched",
-                    ntopics)
+        :returns: a generator of items
+        """
+        offset = kwargs['offset']
 
-    @metadata
-    def fetch_from_cache(self):
-        """Fetch topics from the cache.
+        logger.info("Fetching articles of '%s' group on '%s' offset %s",
+                    self.group, self.host, str(offset))
 
-        :returns: a generator of topics
+        narts, iarts, tarts = (0, 0, 0)
 
-        :raises CacheError: raised when an error occurs accessing the
-            cache
-        """
-        if not self.cache:
-            raise CacheError(cause="cache instance was not provided")
+        _, _, first, last, _ = self.client.group(self.group)
 
-        logger.info("Retrieving cached topics: '%s'", self.url)
+        if offset <= last:
+            first = max(first, offset)
+            _, overview = self.client.over((first, last))
+        else:
+            overview = []
 
-        cache_items = self.cache.retrieve()
+        tarts = len(overview)
 
-        ntopics = 0
+        logger.debug("Total number of articles to fetch: %s", tarts)
 
-        while True:
+        for article_id, _ in overview:
             try:
-                raw_topic = next(cache_items)
-            except StopIteration:
-                break
-
-            topic = json.loads(raw_topic)
-
-            # Retrieve remaining posts for this topic
-            posts_sz = topic['posts_count']
-            chunk_sz = topic['chunk_size']
-
-            if posts_sz > chunk_sz:
-                for _ in range(posts_sz - chunk_sz):
-                    try:
-                        raw_post = next(cache_items)
-                    except StopIteration:
-                        # Fatal error. The code should not reach here.
-                        # Cache should had stored posts_sz - chunk_sz posts
-                        # if the code is running this loop
-                        cause = "cache is exhausted but more items were expected"
-                        raise CacheError(cause=cause)
-
-                    post = json.loads(raw_post)
-                    topic['post_stream']['posts'].append(post)
-
-            ntopics += 1
-            yield topic
-
-        logger.info("Retrieval process completed: %s topics retrieved from cache",
-                    ntopics)
-
-    def __fetch_and_parse_topics_ids(self, from_date):
-        logger.debug("Fetching and parsing topics ids from %s",
-                     str(from_date))
-
-        candidates = []
-        page = 0
-        fetching = True
-
-        while fetching:
-            response = self.client.topics_page(page)
-            topics = self.__parse_topics_page(response)
-
-            if not topics:
-                fetching = False
-
-            # Topics are sorted by updated date from the newest
-            # to the oldest. When a date is older than 'from_date'
-            # we have reached to the end. Pinned topics are
-            # ignored but added to the list if the date is in range.
-            for topic in topics:
-                # Pinned
-                if topic[2] and topic[1] < from_date:
-                    continue
-                elif topic[1] < from_date:
-                    fetching = False
-                    break
-                else:
-                    candidates.append(topic)
-
-            page += 1
-
-        # Sort topics by date and in reverse order to fetch them from
-        # the oldest to the newest
-        candidates = sorted(candidates, key=lambda x: x[1])
-        topics_ids = [topic[0] for topic in candidates]
-
-        return topics_ids
-
-    def __fetch_and_parse_topic(self, topic_id):
-        logger.debug("Fetching and parsing topic %s", topic_id)
-
-        raw_topic = self.client.topic(topic_id)
-        self._push_cache_queue(raw_topic)
-
-        topic = json.loads(raw_topic)
-
-        # There are posts that could not included in the topic.
-        # When post_count is greater than chunk_size, we have
-        # to fetch the remaining posts
-        posts_sz = topic['posts_count']
-        chunk_sz = topic['chunk_size']
-
-        if posts_sz > chunk_sz:
-            posts_ids = topic['post_stream']['stream']
-            posts_ids = posts_ids[chunk_sz:]
-
-            for post_id in posts_ids:
-                logger.debug("Fetching and parsing post %s", post_id)
-                post = self.__fetch_and_parse_post(post_id)
-                topic['post_stream']['posts'].append(post)
-
-        return topic
-
-    def __fetch_and_parse_post(self, post_id):
-        logger.debug("Fetching and parsing post %s", post_id)
-        raw_post = self.client.post(post_id)
-        self._push_cache_queue(raw_post)
-        post = json.loads(raw_post)
-        return post
-
-    def __parse_topics_page(self, raw_json):
-        """Parse a topics page stream.
-
-        The result of parsing process is a generator of tuples. Each
-        tuple contains de identifier of the topic, the last date
-        when it was updated and whether is pinned or not.
-
-        :param raw_json: JSON stream to parse
-
-        :returns: a generator of parsed bugs
-        """
-        topics_page = json.loads(raw_json)
-
-        topics_ids = []
-
-        for topic in topics_page['topic_list']['topics']:
-            topic_id = topic['id']
-            if topic['last_posted_at'] is None:
-                logger.warning("Topic %s with last_posted_at null. Ignoring it.", topic['title'])
+                article_raw = self.client.article(article_id)
+                article = self.__parse_article(article_raw)
+            except ParseError:
+                logger.warning("Error parsing %s article; skipping",
+                               article_id)
+                iarts += 1
                 continue
-            updated_at = str_to_datetime(topic['last_posted_at'])
-            pinned = topic['pinned']
-            topics_ids.append((topic_id, updated_at, pinned))
+            except nntplib.NNTPTemporaryError as e:
+                logger.warning("Error '%s' fetching article %s; skipping",
+                               e.response, article_id)
+                iarts += 1
+                continue
+
+            yield article
+            narts += 1
+
+    def metadata(self, item, filter_classified=False):
+        """NNTP metadata.
+
+        This method takes items, overriding `metadata` decorator,
+        to add extra information related to NNTP.
+
+        :param item: an item fetched by a backend
+        :param filter_classified: sets if classified fields were filtered
+        """
+        item = super().metadata(item, filter_classified=filter_classified)
+        item['offset'] = item['data']['offset']
 
-        return topics_ids
+        return item
 
     @classmethod
-    def has_caching(cls):
-        """Returns whether it supports caching items on the fetch process.
+    def has_archiving(cls):
+        """Returns whether it supports archiving items on the fetch process.
 
-        :returns: this backend supports items cache
+        :returns: this backend supports items archive
         """
         return True
 
     @classmethod
     def has_resuming(cls):
         """Returns whether it supports to resume the fetch process.
 
         :returns: this backend supports items resuming
         """
         return True
 
     @staticmethod
     def metadata_id(item):
-        """Extracts the identifier from a Discourse item."""
+        """Extracts the identifier from a NNTP item."""
 
-        return str(item['id'])
+        return item['message_id']
 
     @staticmethod
     def metadata_updated_on(item):
-        """Extracts the update time from a Discourse item.
+        """Extracts the update time from a NNTP item.
 
-        The timestamp used is extracted from 'last_posted_at' field.
-        This date is converted to UNIX timestamp format taking into
-        account the timezone of the date.
+        The timestamp is extracted from 'Date' field and
+        converted to a UNIX timestamp.
 
         :param item: item generated by the backend
 
         :returns: a UNIX timestamp
         """
-        ts = item['last_posted_at']
-        ts = str_to_datetime(ts)
+        if 'Date' in item:
+            ts = item['Date']
+        elif 'DATE' in item:
+            ts = item['DATE']
+
+        try:
+            ts = str_to_datetime(ts)
+        except InvalidDateError as e:
+            # Set to the FALLBACK_DATE when it is not a valid date
+            logger.warning("%s from Message-ID: %s. Set the fallback date: %s" %
+                           (e, item['Message-ID'], FALLBACK_DATE))
+            ts = str_to_datetime(FALLBACK_DATE)
 
         return ts.timestamp()
 
     @staticmethod
     def metadata_category(item):
-        """Extracts the category from a Discourse item.
+        """Extracts the category from a NNTP item.
 
         This backend only generates one type of item which is
-        'topic'.
+        'article'.
         """
-        return 'topic'
+        return CATEGORY_ARTICLE
+
+    @staticmethod
+    def parse_article(raw_article):
+        """Parse a NNTP article.
+
+        This method parses a NNTP article stored in a string object
+        and returns an dictionary.
+
+        :param raw_article: NNTP article string
+
+        :returns: a dictionary of type `requests.structures.CaseInsensitiveDict`
+
+        :raises ParseError: when an error is found parsing the article
+        """
+        try:
+            message = email.message_from_string(raw_article)
+            article = message_to_dict(message)
+        except UnicodeEncodeError as e:
+            raise ParseError(cause=str(e))
+        return article
+
+    def _init_client(self, from_archive=False):
+        """Init client"""
+
+        return NNTTPClient(self.host, self.archive, from_archive)
+
+    def __parse_article(self, info):
+        reader = io.BytesIO(b'\n'.join(info['lines']))
+        raw_article = reader.read().decode('utf-8', errors='surrogateescape')
+        data = self.parse_article(raw_article)
+
+        article = self.__build_article(data,
+                                       info['message_id'],
+                                       info['number'])
+
+        logger.debug("Article %s (offset: %s) parsed",
+                     article['message_id'], article['offset'])
 
+        return article
 
-class DiscourseClient(HttpClient):
-    """Discourse API client.
+    def __build_article(self, article, message_id, offset):
+        a = {k: v for k, v in article.items()}
+        a['message_id'] = message_id
+        a['offset'] = offset
+        return a
 
-    This class implements a simple client to retrieve topics from
-    any Discourse board.
 
-    :param url: URL of the Discourse site
-    :param api_key: Discourse API access token
+class NNTTPClient():
+    """NNTP client
 
-    :raises HTTPError: when an error occurs doing the request
+    :param host: host
+    :param group: name of the group
+    :param archive: an archive to store/read fetched data
+    :param from_archive: it tells whether to write/read the archive
     """
-    # Static resources
-    ALL_TOPICS = None  # Topics do not need a resource
-    TOPICS_SUMMARY = 'latest'
-    TOPIC = 't'
-    POSTS = 'posts'
-
-    # Params
-    PKEY = 'api_key'
-    PPAGE = 'page'
-
-    # Data type
-    TJSON = '.json'
-
-    def __init__(self, base_url, api_key=None):
-        super().__init__(base_url)
-        self.api_key = api_key
-
-    def topics_page(self, page=None):
-        """Retrieve the #page summaries of the latest topics.
-
-        :param page: number of page to retrieve
-        """
-        params = {
-            self.PKEY: self.api_key,
-            self.PPAGE: page
-        }
 
-        # http://example.com/latest.json
-        response = self._call(self.ALL_TOPICS, self.TOPICS_SUMMARY,
-                              params=params)
+    GROUP = "group"
+    ARTICLE = "article"
+    OVER = "over"
+
+    def __init__(self, host, archive=None, from_archive=False):
+        self.host = host
+        self.archive = archive
+        self.from_archive = from_archive
+
+        if not self.from_archive:
+            self.handler = nntplib.NNTP(self.host)
 
-        return response
+    def __del__(self):
+        if not self.from_archive:
+            self.quit()
 
-    def topic(self, topic_id):
-        """Retrive the topic with `topic_id` identifier.
+    def group(self, group_name):
+        """Fetch group data
 
-        :param topic_id: identifier of the topic to retrieve
+        :param group_name: name of the group
         """
-        params = {
-            self.PKEY: self.api_key
-        }
+        return self._fetch("group", group_name)
 
-        # http://example.com/t/8.json
-        response = self._call(self.TOPIC, topic_id,
-                              params=params)
+    def over(self, offset):
+        """Fetch messages data
 
-        return response
+        :param offset: a tuple representing the offset to retrieve
+        """
+        return self._fetch("over", offset)
 
-    def post(self, post_id):
-        """Retrieve the post whit `post_id` identifier.
+    def article(self, article_id):
+        """Fetch article data
 
-        :param post_id: identifier of the post to retrieve
+        :param article_id: id of the article to fetch
         """
-        params = {
-            self.PKEY: self.api_key
-        }
+        return self._fetch("article", article_id)
 
-        # http://example.com/posts/10.json
-        response = self._call(self.POSTS, post_id,
-                              params=params)
-
-        return response
-
-    def _call(self, res, res_id, params):
-        """Run an API command.
-
-        :param res: type of resource to fetch
-        :param res_id: identifier of the resource
-        :param params: dict with the HTTP parameters needed to run
-            the given command
+    def _fetch(self, method, args):
+        """Fetch NNTP data from the server or from the archive
+
+        :param method: the name of the command to execute
+        :param args: the arguments required by the command
         """
-        if res:
-            url = urijoin(self.base_url, res, res_id)
+        if self.from_archive:
+            data = self._fetch_from_archive(method, args)
         else:
-            url = urijoin(self.base_url, res_id)
-        url += self.TJSON
+            data = self._fetch_from_remote(method, args)
+
+        return data
 
-        logger.debug("Discourse client calls resource: %s %s params: %s",
-                     res, res_id, str(params))
+    def _fetch_article(self, article_id):
+        """Fetch article data
 
-        r = self.fetch(url, payload=params)
+        :param article_id: id of the article to fetch
+        """
+        fetched_data = self.handler.article(article_id)
+        data = {
+            'number': fetched_data[1].number,
+            'message_id': fetched_data[1].message_id,
+            'lines': fetched_data[1].lines
+        }
 
-        return r.text
+        return data
 
+    def _fetch_from_remote(self, method, args):
+        """Fetch data from NNTP
 
-class DiscourseCommand(BackendCommand):
-    """Class to run Discourse backend from the command line."""
+        :param method: the name of the command to execute
+        :param args: the arguments required by the command
+        """
+        try:
+            if method == NNTTPClient.GROUP:
+                data = self.handler.group(args)
+            elif method == NNTTPClient.OVER:
+                data = self.handler.over(args)
+            elif method == NNTTPClient.ARTICLE:
+                data = self._fetch_article(args)
+        except nntplib.NNTPTemporaryError as e:
+            data = e
+            raise e
+        finally:
+            if self.archive:
+                self.archive.store(method, args, None, data)
 
-    BACKEND = Discourse
+        return data
 
-    @staticmethod
-    def setup_cmd_parser():
-        """Returns the Discourse argument parser."""
+    def _fetch_from_archive(self, method, args):
+        """Fetch data from the archive
+
+        :param method: the name of the command to execute
+        :param args: the arguments required by the command
+        """
+        if not self.archive:
+            raise ArchiveError(cause="Archive not provided")
+
+        data = self.archive.retrieve(method, args, None)
+
+        if isinstance(data, nntplib.NNTPTemporaryError):
+            raise data
+
+        return data
+
+    def quit(self):
+        self.handler.quit()
+
+
+class NNTPCommand(BackendCommand):
+    """Class to run NNTP backend from the command line."""
+
+    BACKEND = NNTP
+
+    @classmethod
+    def setup_cmd_parser(cls):
+        """Returns the NNTP argument parser."""
 
-        parser = BackendCommandArgumentParser(from_date=True,
-                                              token_auth=True,
-                                              cache=True)
+        parser = BackendCommandArgumentParser(cls.BACKEND,
+                                              offset=True,
+                                              archive=True)
 
         # Required arguments
-        parser.parser.add_argument('url',
-                                   help="URL of the Discourse server")
+        parser.parser.add_argument('host',
+                                   help="NNTP server host")
+        parser.parser.add_argument('group',
+                                   help="Name of the NNTP group")
 
         return parser
```

### Comparing `perceval-0.9.9/perceval/backends/core/dockerhub.py` & `perceval-1.0.0rc1/perceval/backends/core/dockerhub.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2017 Bitergia
+# Copyright (C) 2015-2020 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1335, USA.
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #     Santiago Dueñas <sduenas@bitergia.com>
+#     Valerio Cosentino <valcos@bitergia.com>
+#     Jesus M. Gonzalez-Barahona <jgb@gsyc.es>
+#     Harshal Mittal <harshalmittal4@gmail.com>
 #
 
 import json
 import logging
 
-from grimoirelab.toolkit.datetime import datetime_utcnow
-from grimoirelab.toolkit.uris import urijoin
+from grimoirelab_toolkit.datetime import datetime_utcnow
+from grimoirelab_toolkit.uris import urijoin
 
 from ...backend import (Backend,
                         BackendCommand,
-                        BackendCommandArgumentParser,
-                        metadata)
+                        BackendCommandArgumentParser)
 from ...client import HttpClient
-from ...errors import CacheError
-
-
-logger = logging.getLogger(__name__)
 
+CATEGORY_DOCKERHUB_DATA = "dockerhub-data"
 
 DOCKERHUB_URL = "https://hub.docker.com/"
 DOCKERHUB_API_URL = urijoin(DOCKERHUB_URL, 'v2')
 
 DOCKER_OWNER = 'library'
 DOCKER_SHORTCUT_OWNER = '_'
 
+logger = logging.getLogger(__name__)
+
 
 class DockerHub(Backend):
     """DockerHub backend for Perceval.
 
     This class retrieves data from a repository stored
     in the Docker Hub site. To initialize this class owner
     and repositories where data will be fetched must be provided.
@@ -54,87 +54,77 @@
 
     Shortcut `_` owner for official Docker repositories will
     be replaced by its long name: `library`.
 
     :param owner: DockerHub owner
     :param repository: DockerHub repository owned by `owner`
     :param tag: label used to mark the data
-    :param cache: cache object to store raw data
+    :param archive: archive to store/retrieve items
+    :param ssl_verify: enable/disable SSL verification
     """
-    version = '0.2.0'
+    version = '1.0.0'
+
+    CATEGORIES = [CATEGORY_DOCKERHUB_DATA]
+    EXTRA_SEARCH_FIELDS = {
+        'name': ['name'],
+        'namespace': ['namespace']
+    }
 
-    def __init__(self, owner, repository,
-                 tag=None, cache=None):
+    def __init__(self, owner, repository, tag=None, archive=None, ssl_verify=True):
         if owner == DOCKER_SHORTCUT_OWNER:
             owner = DOCKER_OWNER
 
         origin = urijoin(DOCKERHUB_URL, owner, repository)
 
-        super().__init__(origin, tag=tag, cache=cache)
+        super().__init__(origin, tag=tag, archive=archive, ssl_verify=ssl_verify)
         self.owner = owner
         self.repository = repository
-        self.client = DockerHubClient()
+        self.client = None
 
-    @metadata
-    def fetch(self):
+    def fetch(self, category=CATEGORY_DOCKERHUB_DATA):
         """Fetch data from a Docker Hub repository.
 
         The method retrieves, from a repository stored in Docker Hub,
         its data which includes number of pulls, stars, description,
         among other data.
 
+        :param category: the category of items to fetch
+
         :returns: a generator of data
         """
+        kwargs = {}
+        items = super().fetch(category, **kwargs)
+
+        return items
+
+    def fetch_items(self, category, **kwargs):
+        """Fetch the Dockher Hub items
+
+        :param category: the category of items to fetch
+        :param kwargs: backend arguments
+
+        :returns: a generator of items
+        """
         logger.info("Fetching data from '%s' repository of '%s' owner",
                     self.repository, self.owner)
 
-        self._purge_cache_queue()
-
         raw_data = self.client.repository(self.owner, self.repository)
         fetched_on = datetime_utcnow().timestamp()
 
-        self._push_cache_queue(
-            {
-                'fetched_on': fetched_on,
-                'data': raw_data
-            }
-        )
-
         data = self.parse_json(raw_data)
         data['fetched_on'] = fetched_on
         yield data
 
-        self._flush_cache_queue()
-
         logger.info("Fetch process completed")
 
-    @metadata
-    def fetch_from_cache(self):
-        """Fetch items from the cache.
-
-        :returns: a generator of items
-
-        :raises CacheError: raised when an error occurs accessing the
-            cache
-        """
-        if not self.cache:
-            raise CacheError(cause="cache instance was not provided")
-
-        cache_items = self.cache.retrieve()
-
-        for raw_item in cache_items:
-            item = self.parse_json(raw_item['data'])
-            item['fetched_on'] = raw_item['fetched_on']
-            yield item
-
     @classmethod
-    def has_caching(cls):
-        """Returns whether it supports caching items on the fetch process.
+    def has_archiving(cls):
+        """Returns whether it supports archiving items on the fetch process.
 
-        :returns: this backend supports items cache
+        :returns: this backend supports items archive
         """
         return True
 
     @classmethod
     def has_resuming(cls):
         """Returns whether it supports to resume the fetch process.
 
@@ -165,15 +155,15 @@
     @staticmethod
     def metadata_category(item):
         """Extracts the category from a Docker Hub item.
 
         This backend only generates one type of item which is
         'dockerhub-data'.
         """
-        return 'dockerhub-data'
+        return CATEGORY_DOCKERHUB_DATA
 
     @staticmethod
     def parse_json(raw_json):
         """Parse a Docker Hub JSON stream.
 
         The method parses a JSON stream and returns a
         dict with the parsed data.
@@ -181,25 +171,34 @@
         :param raw_json: JSON string to parse
 
         :returns: a dict with the parsed data
         """
         result = json.loads(raw_json)
         return result
 
+    def _init_client(self, from_archive=False):
+        """Init client"""
+
+        return DockerHubClient(archive=self.archive, from_archive=from_archive, ssl_verify=self.ssl_verify)
+
 
 class DockerHubClient(HttpClient):
     """DockerHub API client.
 
     Client for fetching information from the DockerHub server
     using its REST API v2.
+
+    :param archive: an archive to store/read fetched data
+    :param from_archive: it tells whether to write/read the archive
+    :param ssl_verify: enable/disable SSL verification
     """
     RREPOSITORY = 'repositories'
 
-    def __init__(self):
-        super().__init__(DOCKERHUB_API_URL)
+    def __init__(self, archive=None, from_archive=False, ssl_verify=True):
+        super().__init__(DOCKERHUB_API_URL, archive=archive, from_archive=from_archive, ssl_verify=ssl_verify)
 
     def repository(self, owner, repository):
         """Fetch information about a repository."""
 
         url = urijoin(self.base_url, self.RREPOSITORY, owner, repository)
 
         logger.debug("DockerHub client requests: %s", url)
@@ -210,19 +209,21 @@
 
 
 class DockerHubCommand(BackendCommand):
     """Class to run DockerHub backend from the command line."""
 
     BACKEND = DockerHub
 
-    @staticmethod
-    def setup_cmd_parser():
+    @classmethod
+    def setup_cmd_parser(cls):
         """Returns the DockerHub argument parser."""
 
-        parser = BackendCommandArgumentParser(cache=True)
+        parser = BackendCommandArgumentParser(cls.BACKEND,
+                                              archive=True,
+                                              ssl_verify=True)
 
         # Required arguments
         parser.parser.add_argument('owner',
                                    help="Docker Hub owner")
         parser.parser.add_argument('repository',
                                    help="Docker Hub repository")
```

### Comparing `perceval-0.9.9/perceval/backends/core/bugzilla.py` & `perceval-1.0.0rc1/perceval/backends/core/bugzilla.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2017 Bitergia
+# Copyright (C) 2015-2020 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1335, USA.
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #     Santiago Dueñas <sduenas@bitergia.com>
 #     Alvaro del Castillo San Felix <acs@bitergia.com>
+#     Stephan Barth <stephan.barth@gmail.com>
+#     Valerio Cosentino <valcos@bitergia.com>
+#     Jesus M. Gonzalez-Barahona <jgb@gsyc.es>
+#     Harshal Mittal <harshalmittal4@gmail.com>
 #
 
 import csv
 import datetime
 import logging
 import re
 
 import bs4
 import dateutil.tz
 
-from grimoirelab.toolkit.datetime import str_to_datetime
+from grimoirelab_toolkit.datetime import str_to_datetime
 
 from ...backend import (Backend,
                         BackendCommand,
-                        BackendCommandArgumentParser,
-                        metadata)
+                        BackendCommandArgumentParser)
 from ...client import HttpClient
-from ...errors import BackendError, CacheError, ParseError
+from ...errors import BackendError, ParseError
 from ...utils import DEFAULT_DATETIME, xml_to_dict
 
-
+CATEGORY_BUG = "bug"
 MAX_BUGS = 200  # Maximum number of bugs per query
 MAX_BUGS_CSV = 10000  # Maximum number of bugs per CSV query
 
 logger = logging.getLogger(__name__)
 
 
 class Bugzilla(Backend):
@@ -55,48 +57,71 @@
     the data.
 
     :param url: Bugzilla server URL
     :param user: Bugzilla user
     :param password: Bugzilla user password
     :param max_bugs: maximum number of bugs requested on the same query
     :param tag: label used to mark the data
-    :param cache: cache object to store raw data
+    :param archive: archive to store/retrieve items
+    :param ssl_verify: enable/disable SSL verification
     """
-    version = '0.7.0'
+    version = '1.0.0'
+
+    CATEGORIES = [CATEGORY_BUG]
+    EXTRA_SEARCH_FIELDS = {
+        'product': ['product', 0, '__text__'],
+        'component': ['component', 0, '__text__']
+    }
 
     def __init__(self, url, user=None, password=None,
                  max_bugs=MAX_BUGS, max_bugs_csv=MAX_BUGS_CSV,
-                 tag=None, cache=None):
+                 tag=None, archive=None, ssl_verify=True):
         origin = url
 
-        super().__init__(origin, tag=tag, cache=cache)
+        super().__init__(origin, tag=tag, archive=archive, ssl_verify=ssl_verify)
         self.url = url
+        self.user = user
+        self.password = password
+        self.max_bugs_csv = max_bugs_csv
+        self.client = None
         self.max_bugs = max(1, max_bugs)
-        self.client = BugzillaClient(url, user=user, password=password,
-                                     max_bugs_csv=max_bugs_csv)
 
-    @metadata
-    def fetch(self, from_date=DEFAULT_DATETIME):
+    def fetch(self, category=CATEGORY_BUG, from_date=DEFAULT_DATETIME):
         """Fetch the bugs from the repository.
 
         The method retrieves, from a Bugzilla repository, the bugs
         updated since the given date.
 
+        :param category: the category of items to fetch
         :param from_date: obtain bugs updated since this date
 
         :returns: a generator of bugs
         """
         if not from_date:
             from_date = DEFAULT_DATETIME
 
+        kwargs = {"from_date": from_date}
+        items = super().fetch(category, **kwargs)
+
+        return items
+
+    def fetch_items(self, category, **kwargs):
+        """Fetch the bugs
+
+        :param category: the category of items to fetch
+        :param kwargs: backend arguments
+
+        :returns: a generator of items
+        """
+
+        from_date = kwargs['from_date']
+
         logger.info("Looking for bugs: '%s' updated from '%s'",
                     self.url, str(from_date))
 
-        self._purge_cache_queue()
-
         buglist = [bug for bug in self.__fetch_buglist(from_date)]
 
         nbugs = 0
         tbugs = len(buglist)
 
         for i in range(0, tbugs, self.max_bugs):
             chunk = buglist[i:i + self.max_bugs]
@@ -107,107 +132,22 @@
 
             for bug in bugs:
                 bug_id = bug['bug_id'][0]['__text__']
                 bug['activity'] = self.__fetch_and_parse_bug_activity(bug_id)
                 nbugs += 1
                 yield bug
 
-            self._flush_cache_queue()
-
         logger.info("Fetch process completed: %s/%s bugs fetched",
                     nbugs, tbugs)
 
-    @metadata
-    def fetch_from_cache(self):
-        """Fetch the bugs from the cache.
-
-        It returns the bugs stored in the cache object provided during
-        the initialization of the object. If this method is called but
-        no cache object was provided, the method will raise a `CacheError`
-        exception.
-
-        :returns: a generator of bugs
-
-        :raises CacheError: raised when an error occurs accesing the
-            cache
-        """
-        if not self.cache:
-            raise CacheError(cause="cache instance was not provided")
-
-        logger.info("Retrieving cached bugs: '%s'", self.url)
-
-        cache_items = self.cache.retrieve()
-
-        nbugs = 0
-
-        while True:
-            try:
-                raw_bugs = next(cache_items)
-            except StopIteration:
-                break
-
-            bugs = self.parse_bugs_details(raw_bugs)
-
-            for bug in bugs:
-                try:
-                    raw_activity = next(cache_items)
-                except StopIteration:
-                    # Fatal error. The code should not reach here.
-                    # Cache should had stored an activity item per parsed bug.
-                    cause = "cache is exhausted but more items were expected"
-                    raise CacheError(cause=cause)
-
-                activity = self.parse_bug_activity(raw_activity)
-                bug['activity'] = [event for event in activity]
-                nbugs += 1
-                yield bug
-
-        logger.info("Retrieval process completed: %s bugs retrieved from cache",
-                    nbugs)
-
-    def __fetch_buglist(self, from_date):
-        buglist = self.__fetch_and_parse_buglist_page(from_date)
-
-        while buglist:
-            bug = buglist.pop(0)
-            last_date = bug['changeddate']
-            yield bug
-
-            # Bugzilla does not support pagination. Due to this,
-            # the next list of bugs is requested adding one second
-            # to the last date obtained.
-            if not buglist:
-                from_date = str_to_datetime(last_date)
-                from_date += datetime.timedelta(seconds=1)
-                buglist = self.__fetch_and_parse_buglist_page(from_date)
-
-    def __fetch_and_parse_buglist_page(self, from_date):
-        logger.debug("Fetching and parsing buglist page from %s", str(from_date))
-        raw_csv = self.client.buglist(from_date=from_date)
-        buglist = self.parse_buglist(raw_csv)
-        return [bug for bug in buglist]
-
-    def __fetch_and_parse_bugs_details(self, *bug_ids):
-        logger.debug("Fetching and parsing bugs details")
-        raw_bugs = self.client.bugs(*bug_ids)
-        self._push_cache_queue(raw_bugs)
-        return self.parse_bugs_details(raw_bugs)
-
-    def __fetch_and_parse_bug_activity(self, bug_id):
-        logger.debug("Fetching and parsing bug #%s activity", bug_id)
-        raw_activity = self.client.bug_activity(bug_id)
-        self._push_cache_queue(raw_activity)
-        activity = self.parse_bug_activity(raw_activity)
-        return [event for event in activity]
-
     @classmethod
-    def has_caching(cls):
-        """Returns whether it supports caching items on the fetch process.
+    def has_archiving(cls):
+        """Returns whether it supports archiving items on the fetch process.
 
-        :returns: this backend supports items cache
+        :returns: this backend supports items archive
         """
         return True
 
     @classmethod
     def has_resuming(cls):
         """Returns whether it supports to resume the fetch process.
 
@@ -243,15 +183,15 @@
     @staticmethod
     def metadata_category(item):
         """Extracts the category from a Bugzilla item.
 
         This backend only generates one type of item which is
         'bug'.
         """
-        return 'bug'
+        return CATEGORY_BUG
 
     @staticmethod
     def parse_buglist(raw_csv):
         """Parse a Bugzilla CSV bug list.
 
         The method parses the CSV file and returns an iterator of
         dictionaries. Each one of this, contains the summary of a bug.
@@ -333,15 +273,15 @@
 
         def format_text(bs):
             strings = [s.strip(' \n\t') for s in bs.stripped_strings]
             s = ' '.join(strings)
             return s
 
         # Parsing starts here
-        bs = bs4.BeautifulSoup(raw_html)
+        bs = bs4.BeautifulSoup(raw_html, 'html.parser')
 
         if is_activity_empty(bs):
             fields = []
         else:
             activity_tb = find_activity_table(bs)
             remove_tags(activity_tb)
             fields = activity_tb.find_all('td')
@@ -365,27 +305,69 @@
                 event = {'Who': format_text(who),
                          'When': format_text(when),
                          'What': format_text(what),
                          'Removed': format_text(removed),
                          'Added': format_text(added)}
                 yield event
 
+    def _init_client(self, from_archive=False):
+        """Init client"""
+
+        return BugzillaClient(self.url, user=self.user, password=self.password,
+                              max_bugs_csv=self.max_bugs_csv,
+                              archive=self.archive, from_archive=from_archive, ssl_verify=self.ssl_verify)
+
+    def __fetch_buglist(self, from_date):
+        buglist = self.__fetch_and_parse_buglist_page(from_date)
+
+        while buglist:
+            bug = buglist.pop(0)
+            last_date = bug['changeddate']
+            yield bug
+
+            # Bugzilla does not support pagination. Due to this,
+            # the next list of bugs is requested adding one second
+            # to the last date obtained.
+            if not buglist:
+                from_date = str_to_datetime(last_date)
+                from_date += datetime.timedelta(seconds=1)
+                buglist = self.__fetch_and_parse_buglist_page(from_date)
+
+    def __fetch_and_parse_buglist_page(self, from_date):
+        logger.debug("Fetching and parsing buglist page from %s", str(from_date))
+        raw_csv = self.client.buglist(from_date=from_date)
+        buglist = self.parse_buglist(raw_csv)
+        return [bug for bug in buglist]
+
+    def __fetch_and_parse_bugs_details(self, *bug_ids):
+        logger.debug("Fetching and parsing bugs details")
+        raw_bugs = self.client.bugs(*bug_ids)
+        return self.parse_bugs_details(raw_bugs)
+
+    def __fetch_and_parse_bug_activity(self, bug_id):
+        logger.debug("Fetching and parsing bug #%s activity", bug_id)
+        raw_activity = self.client.bug_activity(bug_id)
+        activity = self.parse_bug_activity(raw_activity)
+        return [event for event in activity]
+
 
 class BugzillaCommand(BackendCommand):
     """Class to run Bugzilla backend from the command line."""
 
     BACKEND = Bugzilla
 
-    @staticmethod
-    def setup_cmd_parser():
+    @classmethod
+    def setup_cmd_parser(cls):
         """Returns the Bugzilla argument parser."""
 
-        parser = BackendCommandArgumentParser(from_date=True,
+        parser = BackendCommandArgumentParser(cls.BACKEND,
+                                              from_date=True,
                                               basic_auth=True,
-                                              cache=True)
+                                              archive=True,
+                                              ssl_verify=True)
 
         # Bugzilla options
         group = parser.parser.add_argument_group('Bugzilla arguments')
         group.add_argument('--max-bugs', dest='max_bugs',
                            type=int, default=MAX_BUGS,
                            help="Maximum number of bugs requested on the same query")
         group.add_argument('--max-bugs-csv', dest='max_bugs_csv',
@@ -409,16 +391,19 @@
     When it is initialized, it checks if the given Bugzilla is
     available and retrieves its version.
 
     :param base_url: URL of the Bugzilla server
     :param user: Bugzilla user
     :param password: user password
     :param max_bugs_cvs: max bugs requested per CSV query
+    :param archive: an archive to store/read fetched data
+    :param from_archive: it tells whether to write/read the archive
+    :param ssl_verify: enable/disable SSL verification
 
-    :raises BackendError: when an error occurs initilizing the
+    :raises BackendError: when an error occurs initializing the
         client
     """
     URL = "%(base)s/%(cgi)s"
 
     # Regular expression to check the Bugzilla version
     VERSION_REGEX = re.compile(r'.+bugzilla version="([^"]+)"',
                                flags=re.DOTALL)
@@ -445,17 +430,17 @@
     PEXCLUDE_FIELD = 'excludefield'
 
     # Content-type values
     CTYPE_CSV = 'csv'
     CTYPE_XML = 'xml'
 
     def __init__(self, base_url, user=None, password=None,
-                 max_bugs_csv=MAX_BUGS_CSV):
+                 max_bugs_csv=MAX_BUGS_CSV, archive=None, from_archive=False, ssl_verify=True):
         self.version = None
-        super().__init__(base_url)
+        super().__init__(base_url, archive=archive, from_archive=from_archive, ssl_verify=ssl_verify)
 
         if user is not None and password is not None:
             self.login(user, password)
 
         self.max_bugs_csv = max_bugs_csv
 
     def login(self, user, password):
@@ -577,14 +562,36 @@
         logger.debug("Bugzilla client calls command: %s params: %s",
                      cgi, str(params))
 
         req = self.fetch(url, payload=params)
 
         return req.text
 
+    @staticmethod
+    def sanitize_for_archive(url, headers, payload):
+        """Sanitize payload of a HTTP request by removing the login and password information
+        before storing/retrieving archived items
+
+        :param: url: HTTP url request
+        :param: headers: HTTP headers request
+        :param: payload: HTTP payload request
+
+        :returns url, headers and the sanitized payload
+        """
+        if BugzillaClient.PBUGZILLA_LOGIN in payload:
+            payload.pop(BugzillaClient.PBUGZILLA_LOGIN)
+
+        if BugzillaClient.PBUGZILLA_PASSWORD in payload:
+            payload.pop(BugzillaClient.PBUGZILLA_PASSWORD)
+
+        if BugzillaClient.PLOGIN in payload:
+            payload.pop(BugzillaClient.PLOGIN)
+
+        return url, headers, payload
+
     def __fetch_version(self):
         response = self.metadata()
         m = re.match(self.VERSION_REGEX, response)
 
         if m:
             version = m.group(1)
             logger.debug("Bugzilla server is online: %s (v. %s)",
```

### Comparing `perceval-0.9.9/perceval/backends/core/phabricator.py` & `perceval-1.0.0rc1/perceval/backends/core/phabricator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,226 +1,284 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2017 Bitergia
+# Copyright (C) 2015-2020 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1335, USA.
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #     Santiago Dueñas <sduenas@bitergia.com>
+#     Valerio Cosentino <valcos@bitergia.com>
+#     Jesus M. Gonzalez-Barahona <jgb@gsyc.es>
+#     Harshal Mittal <harshalmittal4@gmail.com>
 #
 
 import json
 import logging
 
-from grimoirelab.toolkit.datetime import datetime_to_utc
+from grimoirelab_toolkit.datetime import datetime_to_utc
 
 from ...backend import (Backend,
                         BackendCommand,
                         BackendCommandArgumentParser,
-                        metadata)
+                        OriginUniqueField)
 from ...client import HttpClient
-from ...errors import BaseError, CacheError
+from ...errors import BaseError
 from ...utils import DEFAULT_DATETIME
 
+CATEGORY_TASK = "task"
+
+DEFAULT_SLEEP_TIME = 1
+MAX_RETRIES = 5
+
 logger = logging.getLogger(__name__)
 
 
 class Phabricator(Backend):
     """Phabricator backend.
 
     This class allows to fetch the tasks stored on a Phabricator
     server. Initialize this class passing the URL of this server
     and the API token. The origin of the data will be set to this
     URL.
 
     :param url: URL of the server
     :param api_token: token needed to use the API
     :param tag: label used to mark the data
-    :param cache: cache object to store raw data
+    :param archive: archive to store/retrieve items
+    :param max_retries: number of max retries to a data source
+        before raising a RetryError exception
+    :param sleep_time: time (in seconds) to sleep in case
+        of connection problems
+    :param ssl_verify: enable/disable SSL verification
+    :param blacklist_ids: exclude the ids while fetching
     """
-    version = '0.6.1'
+    version = '1.0.0'
+
+    CATEGORIES = [CATEGORY_TASK]
+    ORIGIN_UNIQUE_FIELD = OriginUniqueField(name='id', type=int)
 
-    def __init__(self, url, api_token, tag=None, cache=None):
+    def __init__(self, url, api_token, tag=None, archive=None,
+                 max_retries=MAX_RETRIES, sleep_time=DEFAULT_SLEEP_TIME,
+                 ssl_verify=True, blacklist_ids=None):
         origin = url
 
-        super().__init__(origin, tag=tag, cache=cache)
+        super().__init__(origin, tag=tag, archive=archive, ssl_verify=ssl_verify, blacklist_ids=blacklist_ids)
         self.url = url
-        self.client = ConduitClient(url, api_token)
+        self.api_token = api_token
+        self.client = None
+
+        self.max_retries = max_retries
+        self.sleep_time = sleep_time
+        self.blacklist_ids = [] if not blacklist_ids else blacklist_ids
+
         self._users = {}
         self._projects = {}
 
-    @metadata
-    def fetch(self, from_date=DEFAULT_DATETIME):
+    def fetch(self, category=CATEGORY_TASK, from_date=DEFAULT_DATETIME):
         """Fetch the tasks from the server.
 
         This method fetches the tasks stored on the server that were
         updated since the given date. The transactions data related
         to each task is also included within them.
 
+        :param category: the category of items to fetch
         :param from_date: obtain tasks updated since this date
 
         :returns: a generator of tasks
         """
-        logger.info("Fetching tasks of '%s' from %s", self.url, str(from_date))
+        if not from_date:
+            from_date = DEFAULT_DATETIME
+
+        kwargs = {'from_date': from_date}
+        items = super().fetch(category, **kwargs)
+
+        return items
 
-        self._purge_cache_queue()
+    def fetch_items(self, category, **kwargs):
+        """Fetch the tasks
 
-        from_date = datetime_to_utc(from_date)
+        :param category: the category of items to fetch
+        :param kwargs: backend arguments
+
+        :returns: a generator of items
+        """
+        from_date = kwargs['from_date']
+
+        logger.info("Fetching tasks of '%s' from %s", self.url, str(from_date))
 
         ntasks = 0
 
         for task in self.__fetch_tasks(from_date):
             yield task
             ntasks += 1
 
         logger.info("Fetch process completed: %s tasks fetched", ntasks)
 
-    @metadata
-    def fetch_from_cache(self):
-        """Fetch the tasks from the cache.
-
-        It returns the tasks stored in the cache object, provided during
-        the initialization of the object. If this method is called but
-        no cache object was provided, the method will raise a `CacheError`
-        exception.
+    @classmethod
+    def has_archiving(cls):
+        """Returns whether it supports archiving items on the fetch process.
 
-        :returns: a generator of tasks
+        :returns: this backend supports items archive
+        """
+        return True
+
+    @classmethod
+    def has_resuming(cls):
+        """Returns whether it supports to resume the fetch process.
 
-        :raises CacheError: raised when an error occurs accesing the
-            cache
+        :returns: this backend supports items resuming
         """
-        if not self.cache:
-            raise CacheError(cause="cache instance was not provided")
+        return True
 
-        logger.info("Retrieving cached tasks: '%s'", self.url)
+    @staticmethod
+    def metadata_id(item):
+        """Extracts the identifier from a Phabricator item."""
 
-        ntasks = 0
+        return str(item['id'])
 
-        try:
-            for task in self.__fetch_tasks_from_cache():
-                yield task
-                ntasks += 1
-        except StopIteration:
-            # Fatal error. The code should not reach here.
-            # Cache should had stored an activity item per parsed bug.
-            cause = "cache is exhausted but more items were expected"
-            raise CacheError(cause=cause)
+    @staticmethod
+    def metadata_updated_on(item):
+        """Extracts and coverts the update time from a Phabricator item.
+
+        The timestamp is extracted from 'dateModified' field. This date is
+        in UNIX timestamp format but needs to be converted to a float
+        number.
+
+        :param item: item generated by the backend
+
+        :returns: a UNIX timestamp
+        """
+        return float(item['fields']['dateModified'])
+
+    @staticmethod
+    def metadata_category(item):
+        """Extracts the category from a Phabricator item.
+
+        This backend only generates one type of item which is
+        'task'.
+        """
+        return CATEGORY_TASK
+
+    @staticmethod
+    def parse_tasks(raw_json, blacklist_ids=[]):
+        """Parse a Phabricator tasks JSON stream.
+
+        The method parses a JSON stream and returns a list iterator.
+        Each item is a dictionary that contains the task parsed data.
+
+        :param raw_json: JSON string to parse
+        :param blacklist_ids: exclude tasks whose ids are in this list
+
+        :returns: a generator of parsed tasks
+        """
+        results = json.loads(raw_json)
+
+        tasks = results['result']['data']
+        for t in tasks:
+            if t['id'] not in blacklist_ids:
+                yield t
+
+    @staticmethod
+    def parse_tasks_transactions(raw_json):
+        """Parse a Phabricator tasks transactions JSON stream.
+
+        The method parses a JSON stream and returns a dictionary
+        with the parsed transactions.
+
+        :param raw_json: JSON string to parse
+
+        :returns: a dict with the parsed transactions
+        """
+        results = json.loads(raw_json)
+        return results['result']
+
+    @staticmethod
+    def parse_users(raw_json):
+        """Parse a Phabricator users JSON stream.
+
+        The method parses a JSON stream and returns a list iterator.
+        Each item is a dictionary that contais the user parsed data.
+
+        :param raw_json: JSON string to parse
+
+        :returns: a generator of parsed users
+        """
+        results = json.loads(raw_json)
+
+        users = results['result']
+        for u in users:
+            yield u
+
+    @staticmethod
+    def parse_phids(results):
+        """Parse a Phabicator PHIDs JSON stream.
+
+        This method parses a JSON stream and returns a list iterator.
+        Each item is a dictionary that contains the PHID parsed data.
 
-        logger.info("Retrieval process completed: %s tasks retrieved from cache",
-                    ntasks)
+        :param results: JSON to parse
+
+        :returns: a generator of parsed PHIDs
+        """
+
+        for phid in results['result'].values():
+            yield phid
+
+    def _init_client(self, from_archive=False):
+        """Init client"""
+
+        return ConduitClient(self.url, self.api_token,
+                             self.max_retries, self.sleep_time,
+                             self.archive, from_archive, self.ssl_verify,
+                             self.blacklist_ids)
 
     def __fetch_tasks(self, from_date):
+        blacklist_ids = [int(x) for x in self.blacklist_ids]
         for raw_tasks in self.client.tasks(from_date=from_date):
-            self._push_cache_queue(raw_tasks)
 
-            tasks = [t for t in self.parse_tasks(raw_tasks)]
+            tasks = [t for t in self.parse_tasks(raw_tasks, blacklist_ids)]
 
             if not tasks:
                 break
 
             tasks_ids = [t['id'] for t in tasks]
             tasks_trans = self.__fetch_and_parse_tasks_transactions(*tasks_ids)
 
             for task in tasks:
                 # Task check point
-                self._push_cache_queue('{TASK}')
 
                 tid = str(task['id'])
                 author_id = task['fields']['authorPHID']
                 owner_id = task['fields']['ownerPHID']
 
                 task['fields']['authorData'] = self.__get_or_fetch_user(author_id)
 
                 if owner_id:
                     task['fields']['ownerData'] = self.__get_or_fetch_user(owner_id)
 
-                # Users checkpoint
-                self._push_cache_queue('{ENDUSERS}')
-
                 project_ids = task['attachments']['projects']['projectPHIDs']
                 task_projects = [self.__get_or_fetch_project(project_id)
                                  for project_id in project_ids]
 
-                # Projects checkpoint
-                self._push_cache_queue('{ENDPROJECTS}')
-
                 task['transactions'] = tasks_trans[tid]
                 task['projects'] = task_projects
 
                 yield task
 
-            # Checkpoint. A tasks set finish here.
-            self._push_cache_queue('{}')
-            self._flush_cache_queue()
-
-    def __fetch_tasks_from_cache(self):
-        cache_items = self.cache.retrieve()
-        cached_users = {}
-        cached_projects = {}
-
-        while True:
-            try:
-                raw_tasks = next(cache_items)
-            except StopIteration:
-                break
-
-            tasks = [t for t in self.parse_tasks(raw_tasks)]
-
-            if not tasks:
-                break
-
-            raw_trans = next(cache_items)
-            tasks_trans = self.parse_tasks_transactions(raw_trans)
-
-            # Retrieve cached users from the transactions
-            users = self.__retrieve_cached_users(cache_items)
-            for user in users:
-                if not user:
-                    continue
-                user_id = user['phid']
-                cached_users[user_id] = user
-
-            # Retrieve cached tasks users and projects
-            raw_checkpoint = next(cache_items)
-            checkpoint = raw_checkpoint == '{}'
-
-            while not checkpoint:
-                users = self.__retrieve_cached_users(cache_items)
-                for user in users:
-                    if not user:
-                        continue
-                    user_id = user['phid']
-                    cached_users[user_id] = user
-
-                projects = self.__retrieve_cached_projects(cache_items)
-                for project in projects:
-                    project_id = project['phid']
-                    cached_projects[project_id] = project
-
-                raw_checkpoint = next(cache_items)
-                checkpoint = raw_checkpoint == '{}'
-
-            task_builder = self.__build_cached_tasks(tasks, tasks_trans,
-                                                     cached_users, cached_projects)
-
-            for task in task_builder:
-                yield task
-
     def __get_or_fetch_user(self, user_id):
         if user_id in self._users:
             return self._users[user_id]
 
         logger.debug("User %s not found on client cache; fetching it", user_id)
 
         if user_id.startswith('PHID-USER-'):
@@ -250,242 +308,143 @@
         project = None
         if phids:
             project = phids[0]
 
         self._projects[project_id] = project
         return project
 
-    def __retrieve_cached_users(self, cache_items):
-        checkpoint = False
-
-        while not checkpoint:
-            raw_item = next(cache_items)
-
-            if raw_item in ('{ENDUSERS}', '{ENDTRANS}'):
-                checkpoint = True
-            elif raw_item == '{PHID}':
-                raw_item = next(cache_items)
-                json_item = json.loads(raw_item)
-                phids = [phid for phid in self.parse_phids(json_item)]
-                yield phids[0]
-            else:
-                users = [user for user in self.parse_users(raw_item)]
-                user = users[0] if len(users) > 0 else None
-                yield user
-
-    def __retrieve_cached_projects(self, cache_items):
-        checkpoint = False
-
-        while not checkpoint:
-            raw_item = next(cache_items)
-
-            if raw_item == '{ENDPROJECTS}':
-                checkpoint = True
-            else:
-                raw_item = next(cache_items)
-                json_item = json.loads(raw_item)
-                phids = [phid for phid in self.parse_phids(json_item)]
-                yield phids[0]
-
     def __fetch_and_parse_tasks_transactions(self, *tasks_ids):
         logger.debug("Fetching and parsing tasks transactions")
 
         raw_json = self.client.transactions(*tasks_ids)
-        self._push_cache_queue(raw_json)
         tasks_trans = self.parse_tasks_transactions(raw_json)
 
         for trans in tasks_trans.values():
             for tt in trans:
                 author_id = tt['authorPHID']
                 author = self.__get_or_fetch_user(author_id)
                 tt['authorData'] = author
 
-        # Transactions checkpoint
-        self._push_cache_queue('{ENDTRANS}')
+                if tt['transactionType'] == 'reassign':
+                    tt['newValue_data'] = self.__resolve_reassign_id(tt['newValue'])
+                    tt['oldValue_data'] = self.__resolve_reassign_id(tt['oldValue'])
+
+                if tt['transactionType'] == 'core:columns':
+                    tt['newValue'] = self.__resolve_board_ids(tt['newValue'])
+                    tt['oldValue'] = self.__resolve_board_ids(tt['oldValue'])
+
+                if tt['transactionType'] == 'core:subscribers':
+                    tt['newValue_data'] = self.__resolve_subsribers_ids(tt['newValue'])
+                    tt['oldValue_data'] = self.__resolve_subsribers_ids(tt['oldValue'])
+
+                if tt['transactionType'] in ['core:edit-policy', 'core:view-policy']:
+                    tt['newValue_data'] = self.__resolve_policy_id(tt['newValue'])
+                    tt['oldValue_data'] = self.__resolve_policy_id(tt['oldValue'])
+
+                if tt['transactionType'] == 'core:edge':
+                    tt['oldValue_data'] = self.__resolve_project_ids(tt['oldValue'])
+                    tt['newValue_data'] = self.__resolve_project_ids(tt['newValue'])
 
         return tasks_trans
 
-    def __fetch_and_parse_users(self, *users_ids):
-        logger.debug("Fetching and parsing users data")
-        raw_json = self.client.users(*users_ids)
-        self._push_cache_queue(raw_json)
-        users = self.parse_users(raw_json)
-        return [user for user in users]
-
-    def __fetch_and_parse_phids(self, *phids):
-        logger.debug("Fetching and parsing phids data")
-        raw_phids = self.client.phids(*phids)
-        phids = json.loads(raw_phids)
-
-        self._push_cache_queue('{PHID}')
-        self._push_cache_queue(raw_phids)
+    def __resolve_reassign_id(self, value):
+        if not value:
+            return value
+
+        resolved = self.__get_or_fetch_user(value)
+        return resolved
+
+    def __resolve_policy_id(self, value):
+        if not value:
+            return value
 
-        result = []
-        if phids['result']:
-            # PHID checkpoint
-            result = self.parse_phids(phids)
-
-        return [phid for phid in result]
-
-    def __build_cached_tasks(self, tasks, transactions,
-                             cached_users, cached_projects):
-        for task in tasks:
-            tid = str(task['id'])
-            author_id = task['fields']['authorPHID']
-            owner_id = task['fields']['ownerPHID']
-
-            task['fields']['authorData'] = cached_users.get(author_id, None)
-
-            if owner_id:
-                task['fields']['ownerData'] = cached_users.get(owner_id, None)
-
-            # Build tasks transactions
-            task_trans = transactions[tid]
-
-            for tt in task_trans:
-                user_id = tt['authorPHID']
-                tt['authorData'] = cached_users.get(user_id, None)
-
-            # Build tasks projects
-            projects_ids = task['attachments']['projects']['projectPHIDs']
-            task_projects = [cached_projects[project_id]
-                             for project_id in projects_ids]
-
-            task['transactions'] = task_trans
-            task['projects'] = task_projects
-
-            yield task
-
-    @classmethod
-    def has_caching(cls):
-        """Returns whether it supports caching items on the fetch process.
-
-        :returns: this backend supports items cache
-        """
-        return True
-
-    @classmethod
-    def has_resuming(cls):
-        """Returns whether it supports to resume the fetch process.
-
-        :returns: this backend supports items resuming
-        """
-        return True
-
-    @staticmethod
-    def metadata_id(item):
-        """Extracts the identifier from a Phabricator item."""
-
-        return str(item['id'])
-
-    @staticmethod
-    def metadata_updated_on(item):
-        """Extracts and coverts the update time from a Phabricator item.
-
-        The timestamp is extracted from 'dateModified' field. This date is
-        in UNIX timestamp format but needs to be converted to a float
-        number.
-
-        :param item: item generated by the backend
-
-        :returns: a UNIX timestamp
-        """
-        return float(item['fields']['dateModified'])
-
-    @staticmethod
-    def metadata_category(item):
-        """Extracts the category from a Phabricator item.
-
-        This backend only generates one type of item which is
-        'task'.
-        """
-        return 'task'
-
-    @staticmethod
-    def parse_tasks(raw_json):
-        """Parse a Phabricator tasks JSON stream.
-
-        The method parses a JSON stream and returns a list iterator.
-        Each item is a dictionary that contains the task parsed data.
-
-        :param raw_json: JSON string to parse
-
-        :returns: a generator of parsed tasks
-        """
-        results = json.loads(raw_json)
+        if value.startswith('PHID-PROJ'):
+            resolved = self.__get_or_fetch_project(value)
+        else:
+            resolved = value
 
-        tasks = results['result']['data']
-        for t in tasks:
-            yield t
+        return resolved
 
-    @staticmethod
-    def parse_tasks_transactions(raw_json):
-        """Parse a Phabricator tasks transactions JSON stream.
+    def __resolve_board_ids(self, lst):
+        if not lst:
+            return lst
 
-        The method parses a JSON stream and returns a dictionary
-        with the parsed transactions.
+        for e in lst:
+            e['boardPHID_data'] = self.__get_or_fetch_project(e['boardPHID'])
 
-        :param raw_json: JSON string to parse
+        return lst
 
-        :returns: a dict with the parsed transactions
-        """
-        results = json.loads(raw_json)
-        return results['result']
+    def __resolve_subsribers_ids(self, lst):
+        if not lst:
+            return lst
 
-    @staticmethod
-    def parse_users(raw_json):
-        """Parse a Phabricator users JSON stream.
+        resolved_lst = []
+        for e in lst:
+            resolved = e
+            if not e:
+                continue
+            elif e.startswith('PHID-PROJ'):
+                resolved = self.__get_or_fetch_project(e)
+            elif e.startswith('PHID-USER'):
+                resolved = self.__get_or_fetch_user(e)
 
-        The method parses a JSON stream and returns a list iterator.
-        Each item is a dictionary that contais the user parsed data.
+            resolved_lst.append(resolved)
 
-        :param raw_json: JSON string to parse
+        return resolved_lst
 
-        :returns: a generator of parsed users
-        """
-        results = json.loads(raw_json)
+    def __resolve_project_ids(self, obj):
+        if not obj:
+            return obj
 
-        users = results['result']
-        for u in users:
-            yield u
+        if isinstance(obj, dict):
+            obj = self.__resolve_project_ids_from_dict(obj)
+        elif isinstance(obj, list):
+            obj = self.__resolve_project_ids_from_list(obj)
 
-    @staticmethod
-    def parse_phids(results):
-        """Parse a Phabicator PHIDs JSON stream.
+        return obj
 
-        This method parses a JSON stream and returns a list iterator.
-        Each item is a dictionary that contains the PHID parsed data.
+    def __resolve_project_ids_from_dict(self, dct):
+        projects = []
 
-        :param results: JSON to parse
+        for key in dct.keys():
+            content = dct.get(key)
 
-        :returns: a generator of parsed PHIDs
-        """
+            if 'dst' in content and content['dst'] and content['dst'].startswith('PHID-PROJ'):
+                project_info = self.__get_or_fetch_project(content['dst'])
+                projects.append(project_info)
 
-        for phid in results['result'].values():
-            yield phid
+        return projects
 
+    def __resolve_project_ids_from_list(self, lst):
+        projects = []
 
-class PhabricatorCommand(BackendCommand):
-    """Class to run Phabricator backend from the command line."""
+        for e in lst:
+            if e.startswith('PHID-PROJ'):
+                project_info = self.__get_or_fetch_project(e)
+                projects.append(project_info)
 
-    BACKEND = Phabricator
+        return projects
 
-    @staticmethod
-    def setup_cmd_parser():
-        """Returns the Phabricator argument parser."""
+    def __fetch_and_parse_users(self, *users_ids):
+        logger.debug("Fetching and parsing users data")
+        raw_json = self.client.users(*users_ids)
+        users = self.parse_users(raw_json)
+        return [user for user in users]
 
-        parser = BackendCommandArgumentParser(from_date=True,
-                                              token_auth=True,
-                                              cache=True)
+    def __fetch_and_parse_phids(self, *phids):
+        logger.debug("Fetching and parsing phids data")
+        raw_phids = self.client.phids(*phids)
+        phids = json.loads(raw_phids)
 
-        # Required arguments
-        parser.parser.add_argument('url',
-                                   help="URL of the Phabricator server")
+        result = []
+        if phids['result']:
+            # PHID checkpoint
+            result = self.parse_phids(phids)
 
-        return parser
+        return [phid for phid in result]
 
 
 class ConduitError(BaseError):
     """Raised when an error occurs using Conduit"""
 
     message = "%(error)s (code: %(code)s)"
 
@@ -496,15 +455,24 @@
     Phabricator uses Conduit as the Phabricator REST API.
     This class implements some of its methods to retrieve the
     contents from a Phabricator server.
 
     :param base_url: URL of the Phabricator server
     :param api_token: token to get access to restricted methods
         of the API
+    :param max_retries: number of max retries to a data source
+        before raising a RetryError exception
+    :param sleep_time: time (in seconds) to sleep in case
+        of connection problems
+    :param archive: an archive to store/read fetched data
+    :param from_archive: it tells whether to write/read the archive
+    :param ssl_verify: enable/disable SSL verification
+    :param blacklist_ids: exclude the ids of this list while fetching
     """
+    EXTRA_STATUS_FORCELIST = [429, 502, 503]
     URL = '%(base)s/api/%(method)s'
 
     # Methods
     MANIPHEST_TASKS = 'maniphest.search'
     MANIPHEST_TRANSACTIONS = 'maniphest.gettasktransactions'
     PHAB_PHIDS = 'phid.query'
     PHAB_USERS = 'user.query'
@@ -516,17 +484,21 @@
     PIDS = 'ids'
     PPROJECTS = 'projects'
     PORDER = 'order'
     PMODIFIED_START = 'modifiedStart'
 
     VOUTDATED = 'outdated'
 
-    def __init__(self, base_url, api_token):
-        super().__init__(base_url.rstrip('/'), max_retries=3, extra_status_forcelist=[502, 503])
+    def __init__(self, base_url, api_token, max_retries=MAX_RETRIES, sleep_time=DEFAULT_SLEEP_TIME,
+                 archive=None, from_archive=False, ssl_verify=True, blacklist_ids=None):
+        super().__init__(base_url.rstrip('/'), sleep_time=sleep_time, max_retries=max_retries,
+                         extra_status_forcelist=self.EXTRA_STATUS_FORCELIST,
+                         archive=archive, from_archive=from_archive, ssl_verify=ssl_verify)
         self.api_token = api_token
+        self.blacklist_ids = [] if not blacklist_ids else blacklist_ids
 
     def tasks(self, from_date=DEFAULT_DATETIME):
         """Retrieve tasks.
 
         :param from_date: retrieve tasks that where updated from that date;
             dates are converted epoch time.
         """
@@ -593,14 +565,32 @@
             self.PHIDS: phids
         }
 
         response = self._call(self.PHAB_PHIDS, params)
 
         return response
 
+    @staticmethod
+    def sanitize_for_archive(url, headers, payload):
+        """Sanitize payload of a HTTP request by removing the token information
+        before storing/retrieving archived items
+
+        :param: url: HTTP url request
+        :param: headers: HTTP headers request
+        :param: payload: HTTP payload request
+
+        :returns url, headers and the sanitized payload
+        """
+        if '__conduit__' in payload['params']:
+            params = json.loads(payload['params'])
+            params.pop('__conduit__')
+            payload['params'] = json.dumps(params, sort_keys=True)
+
+        return url, headers, payload
+
     def _call(self, method, params):
         """Call a method.
 
         :param method: method to call
         :param params: dict with the HTTP parameters needed to call
             the given method
 
@@ -608,25 +598,57 @@
         """
         url = self.URL % {'base': self.base_url, 'method': method}
 
         # Conduit and POST parameters
         params['__conduit__'] = {'token': self.api_token}
 
         data = {
-            'params': json.dumps(params),
+            'params': json.dumps(params, sort_keys=True),
             'output': 'json',
             '__conduit__': True
         }
 
         logger.debug("Phabricator Conduit client requests: %s params: %s",
                      method, str(data))
 
-        r = self.fetch(url, payload=data, method=HttpClient.POST, verify=False)
+        r = self.fetch(url, payload=data, method=HttpClient.POST)
 
         # Check for possible Conduit API errors
         result = r.json()
 
         if result['error_code']:
             raise ConduitError(error=result['error_info'],
                                code=result['error_code'])
 
         return r.text
+
+
+class PhabricatorCommand(BackendCommand):
+    """Class to run Phabricator backend from the command line."""
+
+    BACKEND = Phabricator
+
+    @classmethod
+    def setup_cmd_parser(cls):
+        """Returns the Phabricator argument parser."""
+
+        parser = BackendCommandArgumentParser(cls.BACKEND,
+                                              from_date=True,
+                                              token_auth=True,
+                                              archive=True,
+                                              ssl_verify=True,
+                                              blacklist=True)
+
+        # Phabricator options
+        group = parser.parser.add_argument_group('Phabricator arguments')
+        group.add_argument('--max-retries', dest='max_retries',
+                           default=MAX_RETRIES, type=int,
+                           help="number of API call retries")
+        group.add_argument('--sleep-time', dest='sleep_time',
+                           default=DEFAULT_SLEEP_TIME, type=int,
+                           help="sleeping time between API call retries")
+
+        # Required arguments
+        parser.parser.add_argument('url',
+                                   help="URL of the Phabricator server")
+
+        return parser
```

### Comparing `perceval-0.9.9/perceval/backends/core/git.py` & `perceval-1.0.0rc1/perceval/backends/core/git.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2017 Bitergia
+# Copyright (C) 2015-2020 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1335, USA.
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #     Santiago Dueñas <sduenas@bitergia.com>
+#     Valerio Cosentino <valcos@bitergia.com>
+#     Israel Herraiz <israel.herraiz@bbvadata.com>
+#     anveshc05 <anveshc10047@gmail.com>
+#     Jesus M. Gonzalez-Barahona <jgb@gsyc.es>
+#     Harshal Mittal <harshalmittal4@gmail.com>
+#     Victor Morales <victor.morales@intel.com>
+#     animesh <animuz111@gmail.com>
 #
 
 import collections
 import io
 import logging
 import os
 import re
 import subprocess
 import threading
 
 import dulwich.client
 import dulwich.repo
 
-from grimoirelab.toolkit.datetime import datetime_to_utc, str_to_datetime
+from grimoirelab_toolkit.datetime import datetime_to_utc, str_to_datetime
 
 from ...backend import (Backend,
                         BackendCommand,
-                        BackendCommandArgumentParser,
-                        metadata)
+                        BackendCommandArgumentParser)
 from ...errors import RepositoryError, ParseError
-from ...utils import DEFAULT_DATETIME
+from ...utils import DEFAULT_DATETIME, DEFAULT_LAST_DATETIME
 
+CATEGORY_COMMIT = 'commit'
 
 logger = logging.getLogger(__name__)
 
 
 class Git(Backend):
     """Git backend.
 
@@ -55,157 +61,154 @@
     When `gitpath` is a directory or does not exist, it will be
     considered as the place where the repository is/will be cloned;
     when `gitpath` is a file it will be considered as a Git log file.
 
     :param uri: URI of the Git repository
     :param gitpath: path to the repository or to the log file
     :param tag: label used to mark the data
-    :param cache: cache object to store raw data
+    :param archive: archive to store/retrieve items
+    :param ssl_verify: enable/disable SSL verification
 
     :raises RepositoryError: raised when there was an error cloning or
         updating the repository.
     """
-    version = '0.8.9'
+    version = '1.0.0'
 
-    def __init__(self, uri, gitpath, tag=None, cache=None):
+    CATEGORIES = [CATEGORY_COMMIT]
+
+    def __init__(self, uri, gitpath, tag=None, archive=None, ssl_verify=True):
         origin = uri
 
-        super().__init__(origin, tag=tag, cache=cache)
+        super().__init__(origin, tag=tag, archive=archive, ssl_verify=ssl_verify)
         self.uri = uri
         self.gitpath = gitpath
 
-    @metadata
-    def fetch(self, from_date=DEFAULT_DATETIME, branches=None,
-              latest_items=False):
+    def fetch(self, category=CATEGORY_COMMIT, from_date=DEFAULT_DATETIME, to_date=DEFAULT_LAST_DATETIME,
+              branches=None, latest_items=False, recovery_commit=None, no_update=False):
         """Fetch commits.
 
         The method retrieves from a Git repository or a log file
         a list of commits. Commits are returned in the same order
         they were obtained.
 
-        When `from_date` parameter is given it returns items commited
+        When `from_date` parameter is given it returns items committed
         since the given date.
 
         The list of `branches` is a list of strings, with the names of
         the branches to fetch. If the list of branches is empty, no
         commit is fetched. If the list of branches is None, all commits
         for all branches will be fetched.
 
         The parameter `latest_items` returns only those commits which
         are new since the last time this method was called.
 
+        The parameter `no_update` returns all commits without performing
+        an update of the repository before.
+
         Take into account that `from_date` and `branches` are ignored
         when the commits are fetched from a Git log file or when
         `latest_items` flag is set.
 
         The class raises a `RepositoryError` exception when an error
         occurs accessing the repository.
 
+        :param category: the category of items to fetch
         :param from_date: obtain commits newer than a specific date
             (inclusive)
+        :param to_date: obtain commits older than a specific date
         :param branches: names of branches to fetch from (default: None)
         :param latest_items: sync with the repository to fetch only the
             newest commits
+        :param recovery_commit: recover from this commit no updating the repo
+        :param no_update: if enabled, don't update the repo with the latest changes
 
         :returns: a generator of commits
         """
+        if not from_date:
+            from_date = DEFAULT_DATETIME
+        if not to_date:
+            to_date = DEFAULT_LAST_DATETIME
+
+        kwargs = {
+            'from_date': from_date,
+            'to_date': to_date,
+            'branches': branches,
+            'latest_items': latest_items,
+            'recovery_commit': recovery_commit,
+            'no_update': no_update
+        }
+        items = super().fetch(category, **kwargs)
+
+        return items
+
+    def fetch_items(self, category, **kwargs):
+        """Fetch the commits
+
+        :param category: the category of items to fetch
+        :param kwargs: backend arguments
+
+        :returns: a generator of items
+        """
+        from_date = kwargs['from_date']
+        to_date = kwargs['to_date']
+        branches = kwargs['branches']
+        latest_items = kwargs['latest_items']
+        no_update = kwargs['no_update']
+        recovery_commit = kwargs['recovery_commit']
+
         ncommits = 0
 
         try:
-            if os.path.isfile(self.gitpath):
-                commits = self.__fetch_from_log()
+            if recovery_commit:
+                commits = self._recovery(recovery_commit, from_date, to_date, branches)
+            elif os.path.isfile(self.gitpath):
+                commits = self._fetch_from_log()
             else:
-                commits = self.__fetch_from_repo(from_date, branches,
-                                                 latest_items)
+                commits = self._fetch_from_repo(from_date, to_date, branches,
+                                                latest_items, no_update)
 
             for commit in commits:
                 yield commit
                 ncommits += 1
         except EmptyRepositoryError:
             pass
 
         logger.info("Fetch process completed: %s commits fetched",
                     ncommits)
 
-    def __fetch_from_log(self):
-        logger.info("Fetching commits: '%s' git repository from log file %s",
-                    self.uri, self.gitpath)
-        return self.parse_git_log_from_file(self.gitpath)
-
-    def __fetch_from_repo(self, from_date, branches, latest_items=False):
-        # When no latest items are set or the repository has not
-        # been cloned use the default mode
-        default_mode = not latest_items or not os.path.exists(self.gitpath)
-
-        repo = self.__create_git_repository()
-
-        if default_mode:
-            commits = self.__fetch_commits_from_repo(repo, from_date, branches)
-        else:
-            commits = self.__fetch_newest_commits_from_repo(repo)
-
-        return commits
-
-    def __fetch_commits_from_repo(self, repo, from_date, branches):
-        if branches is None:
-            branches_text = "all"
-        elif len(branches) == 0:
-            branches_text = "no"
-        else:
-            branches_text = ", ".join(branches)
-
-        logger.info("Fetching commits: '%s' git repository from %s; %s branches",
-                    self.uri, str(from_date), branches_text)
-
-        # Ignore default datetime to avoid problems with git
-        # or convert to UTC
-        if from_date == DEFAULT_DATETIME:
-            from_date = None
-        else:
-            from_date = datetime_to_utc(from_date)
-
-        repo.update()
-
-        gitlog = repo.log(from_date, branches)
-        return self.parse_git_log_from_iter(gitlog)
-
-    def __fetch_newest_commits_from_repo(self, repo):
-        logger.info("Fetching latest commits: '%s' git repository",
-                    self.uri)
-
-        hashes = repo.sync()
-        if not hashes:
-            return []
-
-        gitshow = repo.show(hashes)
-        return self.parse_git_log_from_iter(gitshow)
-
-    def __create_git_repository(self):
-        if not os.path.exists(self.gitpath):
-            repo = GitRepository.clone(self.uri, self.gitpath)
-        elif os.path.isdir(self.gitpath):
-            repo = GitRepository(self.uri, self.gitpath)
-        return repo
-
     @classmethod
-    def has_caching(cls):
-        """Returns whether it supports caching items on the fetch process.
+    def has_archiving(cls):
+        """Returns whether it supports archiving items on the fetch process.
 
-        :returns: this backend does not support items cache
+        :returns: this backend does not support items archive
         """
         return False
 
     @classmethod
     def has_resuming(cls):
         """Returns whether it supports to resume the fetch process.
 
         :returns: this backend supports items resuming
         """
         return True
 
+    def metadata(self, item, filter_classified=False):
+        """Git metadata.
+
+        This method takes items, overriding `metadata` decorator,
+        to add extra information related to Git.
+
+        :param item: an item fetched by a backend
+        :param filter_classified: sets if classified fields were filtered
+        """
+        item = super().metadata(item, filter_classified=filter_classified)
+        item['offset'] = item['data']['commit']
+
+        return item
+
     @staticmethod
     def metadata_id(item):
         """Extracts the identifier from a Git item."""
 
         return item['commit']
 
     @staticmethod
@@ -228,15 +231,15 @@
     @staticmethod
     def metadata_category(item):
         """Extracts the category from a Git item.
 
         This backend only generates one type of item which is
         'commit'.
         """
-        return 'commit'
+        return CATEGORY_COMMIT
 
     @staticmethod
     def parse_git_log_from_file(filepath):
         """Parse a Git log file.
 
         The method parses the Git log file and returns an iterator of
         dictionaries. Each one of this, contains a commit.
@@ -271,55 +274,190 @@
             is invalid
         """
         parser = GitParser(iterator)
 
         for commit in parser.parse():
             yield commit
 
+    def _init_client(self, from_archive=False):
+        pass
+
+    def _fetch_from_log(self):
+        logger.info("Fetching commits: '%s' git repository from log file %s",
+                    self.uri, self.gitpath)
+        return self.parse_git_log_from_file(self.gitpath)
+
+    def _fetch_from_repo(self, from_date, to_date, branches, latest_items=False, no_update=False):
+        # When no latest items are set or the repository has not
+        # been cloned use the default mode
+        default_mode = not latest_items or not os.path.exists(self.gitpath)
+
+        repo = self._create_git_repository()
+
+        if default_mode:
+            commits = self._fetch_commits_from_repo(repo, from_date, to_date, branches, no_update)
+        else:
+            commits = self._fetch_newest_commits_from_repo(repo)
+
+        return commits
+
+    def _fetch_commits_from_repo(self, repo, from_date, to_date, branches, no_update):
+        if branches is None:
+            branches_text = "all"
+        elif len(branches) == 0:
+            branches_text = "no"
+        else:
+            branches_text = ", ".join(branches)
+
+        logger.info("Fetching commits: '%s' git repository from %s to %s; %s branches",
+                    self.uri, str(from_date), str(to_date), branches_text)
+
+        # Ignore default datetime to avoid problems with git
+        # or convert to UTC
+        if to_date == DEFAULT_LAST_DATETIME:
+            to_date = None
+        else:
+            to_date = datetime_to_utc(to_date)
+
+        if from_date == DEFAULT_DATETIME:
+            from_date = None
+        else:
+            from_date = datetime_to_utc(from_date)
+
+        if not no_update:
+            repo.update()
+
+        gitlog = repo.log(from_date, to_date, branches)
+        return self.parse_git_log_from_iter(gitlog)
+
+    def _fetch_newest_commits_from_repo(self, repo):
+        logger.info("Fetching latest commits: '%s' git repository",
+                    self.uri)
+
+        hashes = repo.sync()
+        if not hashes:
+            return []
+
+        gitshow = repo.show(hashes)
+        return self.parse_git_log_from_iter(gitshow)
+
+    def __fetch_from_packs(self, repo, packs, from_commit):
+        """Retrieve commits from packfiles starting with the pack containing from_commit"""
+
+        hashes = repo.get_commits_from_packs(packs, from_commit)
+        gitshow = repo.show(hashes)
+        commits = self.parse_git_log_from_iter(gitshow)
+
+        return commits
+
+    def _recovery(self, from_commit, from_date, to_date, branches):
+        """Recover Perceval execution from a specific commit
+
+        If the path is a Git log file, resume the execution using the
+        Git file.
+
+        When the path is a directory, there are two cases to consider:
+
+        If the repository contains only loose objects without packfiles,
+        or a single packfile without loose objects (this occurs when the
+        repository is large enough or to reduce storage space), fetch the
+        commits as it was the first execution. This involves using the
+        '__fetch_from_repository' method, which retrieves commits using the
+        log.
+
+        If the repository contains more than one packfile, or has loose
+        objects and one packfile, we can deduce that the packfile is from the
+        last execution. In this case, we will fetch the commits using the
+        '_from_packs' method.
+        """
+        if os.path.isfile(self.gitpath):
+            commits = self._fetch_from_log()
+        else:
+            repo = self._create_git_repository()
+            packs = repo.packs_by_date()
+            if not packs or (len(packs) == 1 and not repo.has_loose_objects()):
+                commits = self._fetch_from_repo(from_date=from_date, to_date=to_date,
+                                                branches=branches, no_update=True)
+            else:
+                commits = self.__fetch_from_packs(repo, packs, from_commit)
+
+        # Only commits after from_commit
+        found = False
+        for commit in commits:
+            if not found and commit['commit'] == from_commit:
+                found = True
+
+            if found:
+                yield commit
+
+    def _create_git_repository(self):
+        if not os.path.exists(self.gitpath):
+            repo = GitRepository.clone(self.uri, self.gitpath, self.ssl_verify)
+        elif os.path.isdir(self.gitpath):
+            repo = GitRepository(self.uri, self.gitpath)
+        return repo
+
 
 class GitCommand(BackendCommand):
     """Class to run Git backend from the command line."""
 
     BACKEND = Git
 
     def _pre_init(self):
         """Initialize repositories directory path"""
 
         if self.parsed_args.git_log:
             git_path = self.parsed_args.git_log
-        elif not self.parsed_args.git_path:
-            base_path = os.path.expanduser('~/.perceval/repositories/')
-            git_path = os.path.join(base_path, self.parsed_args.uri) + '-git'
-        else:
+        elif self.parsed_args.git_path:
             git_path = self.parsed_args.git_path
+        else:
+            if self.parsed_args.base_path:
+                base_path = self.parsed_args.base_path
+            else:
+                base_path = os.path.expanduser('~/.perceval/repositories/')
+
+            processed_uri = self.parsed_args.uri.lstrip('/')
+            git_path = os.path.join(base_path, processed_uri) + '-git'
 
         setattr(self.parsed_args, 'gitpath', git_path)
 
-    @staticmethod
-    def setup_cmd_parser():
+    @classmethod
+    def setup_cmd_parser(cls):
         """Returns the Git argument parser."""
 
-        parser = BackendCommandArgumentParser(from_date=True)
+        parser = BackendCommandArgumentParser(cls.BACKEND,
+                                              from_date=True,
+                                              to_date=True,
+                                              ssl_verify=True)
 
         # Optional arguments
         group = parser.parser.add_argument_group('Git arguments')
         group.add_argument('--branches', dest='branches',
                            nargs='+', type=str, default=None,
                            help="Fetch commits only from these branches")
-        group.add_argument('--latest-items', dest='latest_items',
-                           action='store_true',
-                           help="Fetch latest commits added to the repository")
 
         # Mutual exclusive parameters
         exgroup = group.add_mutually_exclusive_group()
+        exgroup.add_argument('--base-path', dest='base_path',
+                             help="Base path where the Git repositories will be cloned")
         exgroup.add_argument('--git-path', dest='git_path',
                              help="Path where the Git repository will be cloned")
         exgroup.add_argument('--git-log', dest='git_log',
                              help="Path to the Git log file")
 
+        exgroup_fetch = group.add_mutually_exclusive_group()
+        exgroup_fetch.add_argument('--latest-items', dest='latest_items',
+                                   action='store_true',
+                                   help="Fetch latest commits added to the repository")
+        exgroup_fetch.add_argument('--recovery', dest='recovery_commit',
+                                   help="Recover the last execution from a commit")
+        exgroup_fetch.add_argument('--no-update', dest='no_update',
+                                   action='store_true',
+                                   help="Fetch all commits without updating the repository")
+
         # Required arguments
         parser.parser.add_argument('uri',
                                    help="URI of the Git log repository")
 
         return parser
 
 
@@ -646,58 +784,67 @@
             return [e.strip() for e in lst]
         else:
             return []
 
     def __get_old_filepath(self, f):
         """Get the old filepath of a moved/renamed file.
 
-        Moved or renamed files can be found in the log with the next
-        patterns: '{old_prefix => new_prefix}/name' or
-        'name/{old_suffix => new_suffix}'. This method returns the
-        filepath before the file was moved or renamed.
+        Moved or renamed files can be found in the log with any of the
+        next patterns:
+          'old_name => new_name'
+          '{old_prefix => new_prefix}/name'
+          'name/{old_suffix => new_suffix}'
+
+        This method returns the filepath before the file was moved or
+        renamed.
         """
         i = f.find('{')
         j = f.find('}')
 
         if i > -1 and j > -1:
             prefix = f[0:i]
             inner = f[i + 1:f.find(' => ', i)]
             suffix = f[j + 1:]
             return prefix + inner + suffix
+        elif ' => ' in f:
+            return f.split(' => ')[0]
         else:
             return f
 
 
 class EmptyRepositoryError(RepositoryError):
     """Exception raised when a repository is empty"""
 
     message = "%(repository)s is empty"
 
 
+GitRef = collections.namedtuple('GitRef', ['hash', 'refname'])
+
+
 class _GraphWalker:
     """Commit walker needed by fetch_pack"""
 
-    def __init__(self, local_heads):
-        self.heads = set(local_heads)
+    def __init__(self, local_refs):
+        self.heads = [
+            ref.hash.encode('utf-8') for ref in local_refs
+            if ref.refname.startswith('refs/heads/')
+        ]
 
     def ack(self, sha):
         pass
 
     def next(self):
         if self.heads:
             ret = self.heads.pop()
             return ret
         return None
 
     __next__ = next
 
 
-GitRef = collections.namedtuple('GitRef', ['hash', 'refname'])
-
-
 class GitRepository:
     """Manage a Git repository.
 
     This class provides access to a Git repository running some
     common commands such as `clone`, `pull` or `log`.
     To create an instance from a remote repository, use `clone()`
     class method.
@@ -730,33 +877,39 @@
             raise RepositoryError(cause=cause)
 
         self.uri = uri
         self.dirpath = dirpath
         self.gitenv = {
             'LANG': 'C',
             'PAGER': '',
+            'HTTP_PROXY': os.getenv('HTTP_PROXY', ''),
+            'HTTPS_PROXY': os.getenv('HTTPS_PROXY', ''),
+            'NO_PROXY': os.getenv('NO_PROXY', ''),
             'HOME': os.getenv('HOME', '')
         }
 
     @classmethod
-    def clone(cls, uri, dirpath):
+    def clone(cls, uri, dirpath, ssl_verify=True):
         """Clone a Git repository.
 
         Make a bare copy of the repository stored in `uri` into `dirpath`.
         The repository would be either local or remote.
 
         :param uri: URI of the repository
-        :param dirtpath: directory where the repository will be cloned
+        :param dirpath: directory where the repository will be cloned
+        :param ssl_verify: enable/disable SSL verification
 
         :returns: a `GitRepository` class having cloned the repository
 
         :raises RepositoryError: when an error occurs cloning the given
             repository
         """
         cmd = ['git', 'clone', '--bare', uri, dirpath]
+        if not ssl_verify:
+            cmd += ['-c', 'http.sslVerify=false']
         env = {
             'LANG': 'C',
             'HOME': os.getenv('HOME', '')
         }
 
         cls._exec(cmd, env=env)
 
@@ -825,14 +978,23 @@
         this number is 0, the repositoy is empty.
 
         :raises RepositoryError: when an error occurs accessing the
             repository
         """
         return self.count_objects() == 0
 
+    def has_alternates(self):
+        """Check if the repository contains an alternates file.
+
+        The method returns if the repository borrow objects from other
+        objects stores.
+        """
+        alternates = os.path.join(self.dirpath, 'objects/info/alternates')
+        return os.path.exists(alternates)
+
     def update(self):
         """Update repository from its remote.
 
         Calling this method, the repository will be synchronized with
         the remote repository using 'fetch' command for 'heads' refs.
         Any commit stored in the local copy will be removed; refs
         will be overwritten.
@@ -874,15 +1036,55 @@
         self._update_references(refs)
 
         logger.debug("Git repository %s (%s) is synced",
                      self.uri, self.dirpath)
 
         return commits
 
-    def log(self, from_date=None, branches=None, encoding='utf-8'):
+    def rev_list(self, branches=None):
+        """Read the list commits from the repository
+
+        The list of branches is a list of strings, with the names of the
+        branches to fetch. If the list of branches is empty, no commit
+        is fetched. If the list of branches is None, all commits
+        for all branches will be fetched.
+
+        The method returns the Git rev-list of the repository using the
+        following options:
+
+            git rev-list --topo-order
+
+        :param branches: names of branches to fetch from (default: None)
+
+        :raises EmptyRepositoryError: when the repository is empty and
+            the action cannot be performed
+        :raises RepositoryError: when an error occurs executing the command
+        """
+        if self.is_empty():
+            logger.warning("Git %s repository is empty; unable to get the rev-list",
+                           self.uri)
+            raise EmptyRepositoryError(repository=self.uri)
+
+        cmd_rev_list = ['git', 'rev-list', '--topo-order']
+
+        if branches is None:
+            cmd_rev_list.extend(['--branches', '--tags', '--remotes=origin'])
+        elif len(branches) == 0:
+            cmd_rev_list.extend(['--branches', '--tags', '--max-count=0'])
+        else:
+            branches = ['refs/heads/' + branch for branch in branches]
+            cmd_rev_list.extend(branches)
+
+        for line in self._exec_nb(cmd_rev_list, cwd=self.dirpath, env=self.gitenv):
+            yield line.rstrip('\n')
+
+        logger.debug("Git rev-list fetched from %s repository (%s)",
+                     self.uri, self.dirpath)
+
+    def log(self, from_date=None, to_date=None, branches=None, encoding='utf-8'):
         """Read the commit log from the repository.
 
         The method returns the Git log of the repository using the
         following options:
 
             git log --raw --numstat --pretty=fuller --decorate=full
                 --all --reverse --topo-order --parents -M -C -c
@@ -894,35 +1096,42 @@
         The list of branches is a list of strings, with the names of the
         branches to fetch. If the list of branches is empty, no commit
         is fetched. If the list of branches is None, all commits
         for all branches will be fetched.
 
         :param from_date: fetch commits newer than a specific
             date (inclusive)
+        :param to_date: fetch commits older than a specific date
         :param branches: names of branches to fetch from (default: None)
         :param encoding: encode the log using this format
 
         :returns: a generator where each item is a line from the log
 
         :raises EmptyRepositoryError: when the repository is empty and
             the action cannot be performed
         :raises RepositoryError: when an error occurs fetching the log
         """
-        if self.is_empty():
+        if self.is_empty() and not self.has_alternates():
             logger.warning("Git %s repository is empty; unable to get the log",
                            self.uri)
             raise EmptyRepositoryError(repository=self.uri)
 
         cmd_log = ['git', 'log', '--reverse', '--topo-order']
+        if self.has_alternates():
+            cmd_log.append('--alternate-refs')
         cmd_log.extend(self.GIT_PRETTY_OUTPUT_OPTS)
 
         if from_date:
             dt = from_date.strftime("%Y-%m-%d %H:%M:%S %z")
             cmd_log.append('--since=' + dt)
 
+        if to_date:
+            dt = to_date.strftime("%Y-%m-%d %H:%M:%S %z")
+            cmd_log.append('--until=' + dt)
+
         if branches is None:
             cmd_log.extend(['--branches', '--tags', '--remotes=origin'])
         elif len(branches) == 0:
             cmd_log.append('--max-count=0')
         else:
             branches = ['refs/heads/' + branch for branch in branches]
             cmd_log.extend(branches)
@@ -951,15 +1160,15 @@
 
         :returns: a generator where each item is a line from the show output
 
         :raises EmptyRepositoryError: when the repository is empty and
             the action cannot be performed
         :raises RepositoryError: when an error occurs fetching the show output
         """
-        if self.is_empty():
+        if self.is_empty() and not self.has_alternates():
             logger.warning("Git %s repository is empty; unable to run show",
                            self.uri)
             raise EmptyRepositoryError(repository=self.uri)
 
         if commits is None:
             commits = []
 
@@ -969,14 +1178,61 @@
 
         for line in self._exec_nb(cmd_show, cwd=self.dirpath, env=self.gitenv):
             yield line
 
         logger.debug("Git show fetched from %s repository (%s)",
                      self.uri, self.dirpath)
 
+    def get_commits_from_packs(self, packs, from_commit):
+        """Get commits from a specific one using fetched packfiles"""
+
+        hashes = []
+        found = False
+
+        for pack in packs:
+            commits = self._read_commits_from_pack(pack)
+            for commit in commits:
+                if not found and from_commit == commit:
+                    found = True
+
+                if found:
+                    hashes.append(commit)
+
+        return hashes
+
+    def packs_by_date(self):
+        """Get all packs ordered by date"""
+
+        packs_dir = os.path.join(self.dirpath, 'objects/pack/')
+
+        files = os.listdir(packs_dir)
+        # Sort by date, from older to newer
+        files.sort(key=lambda x: os.path.getmtime(os.path.join(packs_dir, x)))
+        packs = [f.split('.')[0].split('-')[1]
+                 for f in files
+                 if f.endswith('.idx')]
+
+        return packs
+
+    def has_loose_objects(self):
+        """Check if the repository has loose objects"""
+
+        cmd_count_objects = ['git', 'count-objects', '-v']
+
+        outs = self._exec(cmd_count_objects, cwd=self.dirpath, env=self.gitenv)
+        outs = outs.decode('utf-8', errors='surrogateescape').rstrip()
+
+        for line in outs.split('\n'):
+            if line.startswith('count:'):
+                count = int(line.split(':')[1].strip())
+                return count > 0
+        else:
+            msg = "Unexpected output format from 'git count-objects -v'"
+            raise RepositoryError(cause=msg)
+
     def _fetch_pack(self):
         """Fetch changes and store them in a pack."""
 
         def prepare_refs(refs):
             return [ref.hash.encode('utf-8') for ref in refs
                     if not ref.refname.endswith('^{}')]
 
@@ -986,15 +1242,15 @@
             wants = [ref for ref in remote_refs if ref not in local_refs]
             return wants
 
         client, repo_path = dulwich.client.get_transport_and_path(self.uri)
         repo = dulwich.repo.Repo(self.dirpath)
         fd = io.BytesIO()
 
-        local_refs = prepare_refs(self._discover_refs())
+        local_refs = self._discover_refs()
         graph_walker = _GraphWalker(local_refs)
 
         result = client.fetch_pack(repo_path,
                                    determine_wants,
                                    graph_walker,
                                    fd.write)
         refs = [GitRef(ref_hash.decode('utf-8'), ref_name.decode('utf-8'))
```

### Comparing `perceval-0.9.9/perceval/backends/core/gmane.py` & `perceval-1.0.0rc1/perceval/backends/core/supybot.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,387 +1,417 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2017 Bitergia
+# Copyright (C) 2015-2020 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1335, USA.
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #     Santiago Dueñas <sduenas@bitergia.com>
-#     Germán Poo-Caamaño <gpoo@gnome.org>
-#
-# Note: some ot this code was based on parts of the MailingListStats project
+#     Stephan Barth <stephan.barth@gmail.com>
+#     Valerio Cosentino <valcos@bitergia.com>
+#     Jesus M. Gonzalez-Barahona <jgb@gsyc.es>
+#     Harshal Mittal <harshalmittal4@gmail.com>
 #
 
-import functools
+import datetime
 import logging
 import os
-import posixpath
+import re
 
-import requests
+import dateutil
 
-from grimoirelab.toolkit.uris import urijoin
+from grimoirelab_toolkit.datetime import datetime_to_utc, str_to_datetime
 
-from .mbox import MailingList, MBox
-from ...backend import BackendCommand, BackendCommandArgumentParser, metadata
-from ...errors import RepositoryError
+from ...backend import (Backend,
+                        BackendCommand,
+                        BackendCommandArgumentParser)
+from ...errors import ParseError
+from ...utils import DEFAULT_DATETIME
 
+CATEGORY_MESSAGE = "message"
 
 logger = logging.getLogger(__name__)
 
 
-DEFAULT_OFFSET = 0
-MAX_MESSAGES = 2000  # Maximum number of messages per query
-
-
-def gmane_metadata(func):
-    """Gmane metadata decorator.
-
-    This decorator takes items overrides `metadata` decorator to add extra
-    information related to Gmane.
-    """
-    @functools.wraps(func)
-    def decorator(self, *args, **kwargs):
-        offset = kwargs.get('offset', DEFAULT_OFFSET)
-
-        for item in func(self, *args, **kwargs):
-            item['offset'] = offset
-            offset += 1
-            yield item
-    return decorator
-
-
-class Gmane(MBox):
-    """Gmane backend.
-
-    The Gmane backend allows to fetch the email messages from a mailing
-    list stored on Gmane. Initialize this class passing the mailing list
-    address (i.e: my-mailing-list@example.com) and the directory path
-    where the mbox files will be stored.
+class Supybot(Backend):
+    """Supybot IRC log backend.
 
-    The origin of the data will be set to to the URL under Gmane stores
-    that list; usually it is similar to the next address:
-    'http://dir.gmane.org/gmane.comp.example.mylist'
-
-    :param mailing_list_address: address of the mailing list
-    :param dirpath: directory path where the mboxes are stored
+    This class fetches the messages stored by Supybot in log files.
+    Initialize this class providing the directory where those IRC
+    log files are stored.
+
+    The log filenames expected by this backend should follow the
+    pattern: #channel_YYYY-MM-DD.log (i.e #grimoirelab_2016-06-27.log).
+    This is needed to determine the date when messages were sent.
+    Other filenames might work too but the behaviour is unknown.
+
+    The format of the messages must also follow a pattern. This
+    patterns can be found in `SupybotParser` class documentation.
+
+    :param uri: URI of the IRC archives; typically, the URL of their
+        IRC channel
+    :param dirpath: directory path where the archives are stored
     :param tag: label used to mark the data
-    :param cache: cache object to store raw data
-
-    :raises  RepositoryError: when the given mailing list repository
-        is not stored by Gmane
+    :param archive: archive to store/retrieve items
     """
-    version = '0.4.1'
+    version = '1.0.0'
 
-    def __init__(self, mailing_list_address, dirpath,
-                 tag=None, cache=None):
-        self.mailing_list = GmaneMailingList(mailing_list_address, dirpath)
+    CATEGORIES = [CATEGORY_MESSAGE]
 
-        url = self.mailing_list.url
+    def __init__(self, uri, dirpath, tag=None, archive=None):
+        origin = uri
 
-        super().__init__(url, dirpath, tag=tag, cache=cache)
-        self.url = url
+        super().__init__(origin, tag=tag, archive=archive)
+        self.uri = uri
+        self.dirpath = dirpath
 
-    @gmane_metadata
-    @metadata
-    def fetch(self, offset=DEFAULT_OFFSET):
-        """Fetch the messages from Gmane.
+    def fetch(self, category=CATEGORY_MESSAGE, from_date=DEFAULT_DATETIME):
+        """Fetch the messages from the Supybot IRC logger.
 
-        The method fetches the messages stored in Gmane related
-        to the mailing list.
+        The method parsers and returns the messages saved on the
+        IRC log files and stored by Supybot in `dirpath`.
 
-        :param offset: obtain messages from this offset
+        :param category: the category of items to fetch
+        :param from_date: obtain messages since this date
 
         :returns: a generator of messages
         """
-        logger.info("Looking for messages from '%s' offset %s)",
-                    self.url, offset)
+        if not from_date:
+            from_date = DEFAULT_DATETIME
 
-        fetched = self.mailing_list.fetch(offset=offset)
-        valid_filepaths = [f[1] for f in fetched]
+        from_date = datetime_to_utc(from_date)
 
-        # Dates are converted to UTC in the next method
-        messages = self._fetch_and_parse_messages(self.mailing_list,
-                                                  valid_filepaths)
+        kwargs = {'from_date': from_date}
+        items = super().fetch(category, **kwargs)
 
-        for message in messages:
-            yield message
+        return items
 
-        logger.info("Fetch process completed")
+    def fetch_items(self, category, **kwargs):
+        """Fetch the messages
 
-    def _fetch_and_parse_messages(self, mailing_list, valid_filepaths):
-        """Overrides _fetch_and_parse_messages of MBox"""
+        :param category: the category of items to fetch
+        :param kwargs: backend arguments
 
-        nmsgs, imsgs, tmsgs = (0, 0, 0)
+        :returns: a generator of items
+        """
+        from_date = kwargs['from_date']
 
-        for mbox in mailing_list.mboxes:
-            if mbox.filepath not in valid_filepaths:
-                continue
+        logger.info("Fetching messages of '%s' from %s",
+                    self.uri, str(from_date))
 
-            try:
-                tmp_path = self._copy_mbox(mbox)
+        nmessages = 0
+        archives = self.__retrieve_archives(from_date)
 
-                for message in self.parse_mbox(tmp_path):
-                    tmsgs += 1
+        for archive in archives:
+            logger.debug("Parsing supybot archive %s", archive)
 
-                    if not self._validate_message(message):
-                        imsgs += 1
-                        continue
+            for message in self.parse_supybot_log(archive):
+                dt = str_to_datetime(message['timestamp'])
 
-                    # Convert 'CaseInsensitiveDict' to dict
-                    message = self._casedict_to_dict(message)
+                if dt < from_date:
+                    logger.debug("Message %s sent before %s; skipped",
+                                 str(dt), str(from_date))
+                    continue
 
-                    nmsgs += 1
-                    logger.debug("Message %s parsed", message['unixfrom'])
+                yield message
+                nmessages += 1
 
-                    yield message
-            except OSError as e:
-                logger.warning("Ignoring %s mbox due to: %s", mbox.filepath, str(e))
-            except Exception as e:
-                if os.path.exists(tmp_path):
-                    os.remove(tmp_path)
-                raise e
-            finally:
-                if os.path.exists(tmp_path):
-                    os.remove(tmp_path)
-
-        logger.info("Done. %s/%s messages fetched; %s ignored",
-                    nmsgs, tmsgs, imsgs)
+        logger.info("Fetch process completed: %s messages fetched",
+                    nmessages)
 
     @classmethod
-    def has_caching(cls):
-        """Returns whether it supports caching items on the fetch process.
+    def has_archiving(cls):
+        """Returns whether it supports archiving items on the fetch process.
 
-        :returns: this backend does not support items cache
+        :returns: this backend does not support items archive
         """
         return False
 
     @classmethod
     def has_resuming(cls):
         """Returns whether it supports to resume the fetch process.
 
         :returns: this backend supports items resuming
         """
         return True
 
+    @staticmethod
+    def metadata_id(item):
+        """Extracts the identifier from a Supybot item.
 
-class GmaneCommand(BackendCommand):
-    """Class to run Gmane backend from the command line."""
+        This identifier will be the mix of three fields because IRC
+        messages does not have any unique identifier. In this case,
+        'timestamp', 'nick' and 'body' values are combined because
+        there have been cases where two messages were sent by the
+        same user at the same time.
+        """
+        return item['timestamp'] + item['nick'] + item['body']
 
-    BACKEND = Gmane
+    @staticmethod
+    def metadata_updated_on(item):
+        """Extracts the update time from a Supybot item.
+
+        The timestamp used is extracted from 'timestamp' field.
+        This date is converted to UNIX timestamp format taking into
+        account the timezone of the date.
 
-    def _pre_init(self):
-        """Initialize mailing lists directory path"""
+        :param item: item generated by the backend
 
-        if not self.parsed_args.mboxes_path:
-            base_path = os.path.expanduser('~/.perceval/mailinglists/')
-            dirpath = os.path.join(base_path, self.parsed_args.mailing_list)
-        else:
-            dirpath = self.parsed_args.mboxes_path
+        :returns: a UNIX timestamp
+        """
+        ts = item['timestamp']
+        ts = str_to_datetime(ts)
 
-        setattr(self.parsed_args, 'dirpath', dirpath)
+        return ts.timestamp()
 
     @staticmethod
-    def setup_cmd_parser():
-        """Returns the Gmane argument parser."""
+    def metadata_category(item):
+        """Extracts the category from a Supybot item.
 
-        aliases = {
-            'mailing_list_address': 'mailing_list'
-        }
-        parser = BackendCommandArgumentParser(offset=True,
-                                              cache=True,
-                                              aliases=aliases)
+        This backend only generates one type of item which is
+        'message'.
+        """
+        return CATEGORY_MESSAGE
 
-        # Optional arguments
-        group = parser.parser.add_argument_group('Gmane arguments')
-        group.add_argument('--mboxes-path', dest='mboxes_path',
-                           help="Path where mbox files will be stored")
+    @staticmethod
+    def parse_supybot_log(filepath):
+        """Parse a Supybot IRC log file.
 
-        # Required arguments
-        parser.parser.add_argument('mailing_list',
-                                   help='Mailing list address on Gmane')
+        The method parses the Supybot IRC log file and returns an iterator of
+        dictionaries. Each one of this, contains a message from the file.
 
-        return parser
+        :param filepath: path to the IRC log file
 
+        :returns: a generator of parsed messages
 
-class GmaneMailingList(MailingList):
-    """Manage mailing list archives stored by Gmane.
+        :raises ParseError: raised when the format of the Supybot log file
+            is invalid
+        :raises OSError: raised when an error occurs reading the
+            given file
+        """
+        with open(filepath, 'r', errors='surrogateescape',
+                  newline=os.linesep) as f:
+            parser = SupybotParser(f)
 
-    This class gives access to remote and local messages from a
-    mailing list stored by Gmane. Due to the nature of Gmane
-    and how messages are stored, this class does not manage
-    overlaped mboxes nor duplicated messages. Messages must be
-    filtered on later stages.
-
-    :param mailing_list_address: address of the mailing list (i.e:
-        my-mailing-list@example.com)
-    :param dirpath: path to the local mboxes archives
+            try:
+                for message in parser.parse():
+                    yield message
+            except ParseError as e:
+                cause = "file: %s; reason: %s" % (filepath, str(e))
+                raise ParseError(cause=cause)
 
-    :raises  RepositoryError: when the given mailing list repository
-        is not stored by Gmane
-    """
-    def __init__(self, mailing_list_address, dirpath):
-        self.client = GmaneClient()
-        self._url = self.client.mailing_list_url(mailing_list_address)
-        super().__init__(self._url, dirpath)
-
-    def fetch(self, offset=DEFAULT_OFFSET):
-        """Fetch the messages from Gmane and store them in mbox files.
-
-        Stores the messages in mboxes files in the path given during the
-        initialization of this object. Messages are fetched from the given
-        offset.
+    def _init_client(self, from_archive=False):
+        pass
 
-        :param offset: start to fetch messages from the given index
+    def __retrieve_archives(self, from_date):
+        """Retrieve the Supybot archives after the given date"""
 
-        :returns: a list of tuples, storing the links and paths of the
-            fetched archives
-        """
-        logger.info("Downloading messages from '%s' and offset %s",
-                    self.url, str(offset))
-        logger.debug("Storing messages in '%s'", self.dirpath)
+        archives = []
 
-        if not os.path.exists(self.dirpath):
-            os.makedirs(self.dirpath)
+        candidates = self.__list_supybot_archives()
 
-        fetched = []
-        mailing_list = posixpath.basename(self.url)
+        for candidate in candidates:
+            dt = self.__parse_date_from_filepath(candidate)
 
-        while True:
-            messages = self.client.messages(mailing_list, offset,
-                                            max_messages=MAX_MESSAGES)
+            if dt.date() >= from_date.date():
+                archives.append((dt, candidate))
+            else:
+                logger.debug("Archive %s stored before %s; skipped",
+                             candidate, str(from_date))
 
-            # In Gmane, an empty page means we reached the last message.
-            if len(messages) == 0:
-                break
+        archives.sort(key=lambda x: x[0])
 
-            filepath = os.path.join(self.dirpath, str(offset))
+        return [archive[1] for archive in archives]
 
-            success = self._store_messages(filepath, offset, messages)
+    def __list_supybot_archives(self):
+        """List the filepath of the archives stored in dirpath"""
 
-            if success:
-                fetched.append((offset, filepath))
+        archives = []
 
-            offset += MAX_MESSAGES
+        for root, _, files in os.walk(self.dirpath):
+            for filename in files:
+                location = os.path.join(root, filename)
+                archives.append(location)
+
+        return archives
+
+    def __parse_date_from_filepath(self, filepath):
+        default_dt = datetime.datetime(2100, 1, 1,
+                                       tzinfo=dateutil.tz.tzutc())
 
-        logger.info("Messages from Gmane %s downloaded", self.url)
+        try:
+            name = os.path.basename(filepath)
+            dt = dateutil.parser.parse(name, default=default_dt,
+                                       fuzzy=True)
+        except (AttributeError, TypeError, ValueError) as e:
+            dt = default_dt
+            logger.debug("Date of file %s not detected due to %s",
+                         filepath, str(e))
+            logger.debug("Date set to default: %s", str(dt))
 
-        return fetched
+        return dt
 
-    @property
-    def mboxes(self):
-        """Get the mboxes managed by this mailing list.
 
-        Returns the archives sorted by offset in ascending order.
+class SupybotCommand(BackendCommand):
+    """Class to run Supybot backend from the command line."""
 
-        :returns: a list of `.MBoxArchive` objects
-        """
-        archives = []
+    BACKEND = Supybot
 
-        for mbox in super().mboxes:
-            try:
-                offset = int(os.path.basename(mbox.filepath))
-                archives.append((offset, mbox))
-            except ValueError:
-                logger.debug("Ignoring %s archive because its filename is not valid",
-                             mbox.filepath)
-                continue
+    @classmethod
+    def setup_cmd_parser(cls):
+        """Returns the Supybot argument parser."""
 
-        archives.sort(key=lambda x: x[0])
+        aliases = {
+            'dirpath': 'ircdir'
+        }
+        parser = BackendCommandArgumentParser(cls.BACKEND,
+                                              from_date=True,
+                                              aliases=aliases)
+
+        # Required arguments
+        parser.parser.add_argument('uri',
+                                   help="URI of the IRC channel")
+        parser.parser.add_argument('ircdir',
+                                   help="Path to the IRC logs directory")
 
-        return [a[1] for a in archives]
+        return parser
 
-    @property
-    def url(self):
-        """Gmane URL for this mailing list"""
-        return self._url
 
-    def _store_messages(self, filepath, offset, messages):
-        try:
-            with open(filepath, 'wb') as fd:
-                fd.write(messages)
-        except OSError as e:
-            logger.warning("Ignoring messages from %s with offset %s due to: %s",
-                           self.url, offset, str(e))
-            return False
+class SupybotParser:
+    """Supybot IRC parser.
 
-        logger.debug("%s messages with offset %s downloaded and stored in %s",
-                     self.url, offset, filepath)
-        return True
+    This class parses a Supybot IRC log stream, converting plain log
+    lines (or messages) into dict items. Each dictionary will contain
+    the date of the message, the type of message (comment or server
+    message), the nick of the sender and its body.
 
+    Each line on a log starts with a date in ISO format including its
+    timezone and it is followed by two spaces and by a message.
 
-class GmaneClient:
-    """Gmane client.
+    There are two types of valid messages in a Supybot log: comment
+    messages and server messages. First one follows any of these two
+    patterns:
 
-    This class implements a simple client to access mailing lists
-    stored in Gmane.
-    """
-    GMANE_DOMAIN = 'gmane.org'
-    GMANE_DOWNLOAD_RTYPE = 'download'
-    GMANE_LISTID_RTYPE = 'list'
+        2016-06-27T12:00:00+0000  <nick> body of the message
+        2016-06-27T12:00:00+0000  * nick waves hello
 
-    URL = "http://%(prefix)s.%(domain)s/%(resource)s"
+    While a valid server message has the next pattern:
 
-    def messages(self, mailing_list, offset, max_messages=MAX_MESSAGES):
-        """Fetch a set of messages from the given mailing list.
+        2016-06-27T12:00:00+0000  *** nick is known as new_nick
 
-        Given the mailing list identifier used by Gmane and a offset,
-        this method fetches a set of messages.
+    An exception is raised when any of the lines does not follow any
+    of the above formats.
 
-        :param mailing_list: mailing list identifier on Gmane
-        :param offset: start to fetch from here
-        :param max_messages: maximum number of messages to fetch
+    :param stream: an iterator which produces Supybot log lines
+    """
+    TIMESTAMP_PATTERN = r"""^(?P<ts>\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}[\+\-]?\d{0,4})\s\s
+                        (?P<msg>.+)$
+                        """
+    COMMENT_PATTERN = r"^<(?P<nick>(.*?)(!.*)?)>\s(?P<body>.+)$"
+    COMMENT_ACTION_PATTERN = r"^\*\s?(?P<body>(?P<nick>([^\s\*]+?)(!.*)?)\s.+)$"
+    SERVER_PATTERN = r"^\*\*\*\s(?P<body>(?P<nick>(.*?)(!.*)?)\s.+)$"
+    BOT_PATTERN = r"^-(?P<nick>(.*?)(!.*)?)-\s(?P<body>.+)$"
+    EMPTY_PATTERN = r"^\s*$"
+    EMPTY_COMMENT_PATTERN = r"^<(.*?)(!.*)?>\s*$"
+    EMPTY_COMMENT_ACTION_PATTERN = r"^\*\s?([^\s\*]+?)(!.*)?\s*$"
+    EMPTY_BOT_PATTERN = r"^-(.*?)(!.*)?-\s*$"
+
+    # Compiled patterns
+    SUPYBOT_TIMESTAMP_REGEX = re.compile(TIMESTAMP_PATTERN, re.VERBOSE)
+    SUPYBOT_COMMENT_REGEX = re.compile(COMMENT_PATTERN, re.VERBOSE)
+    SUPYBOT_COMMENT_ACTION_REGEX = re.compile(COMMENT_ACTION_PATTERN, re.VERBOSE)
+    SUPYBOT_SERVER_REGEX = re.compile(SERVER_PATTERN, re.VERBOSE)
+    SUPYBOT_BOT_REGEX = re.compile(BOT_PATTERN, re.VERBOSE)
+    SUPYBOT_EMPTY_REGEX = re.compile(EMPTY_PATTERN, re.VERBOSE)
+    SUPYBOT_EMPTY_COMMENT_REGEX = re.compile(EMPTY_COMMENT_PATTERN, re.VERBOSE)
+    SUPYBOT_EMPTY_COMMENT_ACTION_REGEX = re.compile(EMPTY_COMMENT_ACTION_PATTERN, re.VERBOSE)
+    SUPYBOT_EMPTY_BOT_REGEX = re.compile(EMPTY_BOT_PATTERN, re.VERBOSE)
+
+    # Item types
+    TCOMMENT = 'comment'
+    TSERVER = 'server'
+
+    def __init__(self, stream):
+        self.stream = stream
+        self.nline = 0
+
+    def parse(self):
+        """Parse a Supybot IRC stream.
+
+        Returns an iterator of dicts. Each dicts contains information
+        about the date, type, nick and body of a single log entry.
+
+        :returns: iterator of parsed lines
+
+        :raises ParseError: when an invalid line is found parsing the given
+            stream
         """
-        end_offset = offset + max_messages
-        resource = urijoin(mailing_list, offset, end_offset)
+        for line in self.stream:
+            line = line.rstrip('\n')
+            self.nline += 1
 
-        r = self.fetch(self.GMANE_DOWNLOAD_RTYPE, resource)
+            if self.SUPYBOT_EMPTY_REGEX.match(line):
+                continue
 
-        return r.content
+            ts, msg = self._parse_supybot_timestamp(line)
 
-    def mailing_list_url(self, mailing_list_address):
-        """Get the Gmane URL that stores the given mailing list address.
+            if self.SUPYBOT_EMPTY_COMMENT_REGEX.match(msg):
+                continue
+            elif self.SUPYBOT_EMPTY_COMMENT_ACTION_REGEX.match(msg):
+                continue
+            elif self.SUPYBOT_EMPTY_BOT_REGEX.match(msg):
+                continue
 
-        :param mailing_list_address: address of the mailing list (i.e:
-            my-mailing-list@example.com)
+            itype, nick, body = self._parse_supybot_msg(msg)
+            item = self._build_item(ts, itype, nick, body)
 
-        :raises RepositoryError: when the given mailing list repository
-            is not stored by Gmane
-        """
-        r = self.fetch(self.GMANE_LISTID_RTYPE, mailing_list_address)
+            yield item
 
-        if len(r.history) == 0:
-            cause = "%s mailing list not found in Gmane"
-            raise RepositoryError(cause=cause)
+    def _parse_supybot_timestamp(self, line):
+        """Parse timestamp section"""
 
-        return r.url
+        m = self.SUPYBOT_TIMESTAMP_REGEX.match(line)
 
-    def fetch(self, rtype, resource):
-        """Fetch the given resource.
+        if not m:
+            msg = "date expected on line %s" % (str(self.nline))
+            raise ParseError(cause=msg)
 
-        :param rtype: type of the resource
-        :param resource: resource to fetch
-        """
-        url = self.URL % {
-            'prefix': rtype,
-            'domain': self.GMANE_DOMAIN,
-            'resource': resource
-        }
+        ts = m.group('ts')
+        msg = m.group('msg')
+
+        return ts, msg
 
-        logger.debug("Gmane client requests: %s, rtype: %s resource: %s",
-                     url, rtype, resource)
+    def _parse_supybot_msg(self, line):
+        """Parse message section"""
 
-        r = requests.get(url)
-        r.raise_for_status()
+        patterns = [(self.SUPYBOT_COMMENT_REGEX, self.TCOMMENT),
+                    (self.SUPYBOT_COMMENT_ACTION_REGEX, self.TCOMMENT),
+                    (self.SUPYBOT_SERVER_REGEX, self.TSERVER),
+                    (self.SUPYBOT_BOT_REGEX, self.TCOMMENT)]
 
-        return r
+        for p in patterns:
+            m = p[0].match(line)
+            if not m:
+                continue
+            return p[1], m.group('nick'), m.group('body').strip()
+
+        msg = "invalid message on line %s" % (str(self.nline))
+        raise ParseError(cause=msg)
+
+    def _build_item(self, ts, itype, nick, body):
+        return {
+            'timestamp': ts,
+            'type': itype,
+            'nick': nick,
+            'body': body
+        }
```

### Comparing `perceval-0.9.9/perceval/backends/core/hyperkitty.py` & `perceval-1.0.0rc1/perceval/backends/core/hyperkitty.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,106 +1,130 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2017 Bitergia
+# Copyright (C) 2015-2020 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1335, USA.
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #     Santiago Dueñas <sduenas@bitergia.com>
+#     Valerio Cosentino <valcos@bitergia.com>
+#     Jesus M. Gonzalez-Barahona <jgb@gsyc.es>
+#     Harshal Mittal <harshalmittal4@gmail.com>
 #
 
 import datetime
 import logging
 import os
 
 import dateutil.parser
 import dateutil.relativedelta
 import dateutil.tz
 
-from grimoirelab.toolkit.datetime import datetime_to_utc, datetime_utcnow
-from grimoirelab.toolkit.uris import urijoin
+from grimoirelab_toolkit.datetime import datetime_to_utc, datetime_utcnow
+from grimoirelab_toolkit.uris import urijoin
 
-from .mbox import MBox, MailingList
+from .mbox import MBox, MailingList, CATEGORY_MESSAGE
 from ...backend import (BackendCommand,
-                        BackendCommandArgumentParser,
-                        metadata)
+                        BackendCommandArgumentParser)
 from ...client import HttpClient
 from ...utils import (DEFAULT_DATETIME,
+                      DEFAULT_LAST_DATETIME,
                       months_range)
 
-
 logger = logging.getLogger(__name__)
 
 
 class HyperKitty(MBox):
     """HyperKitty backend.
 
     This class allows the fetch the email messages stored on a HyperKitty
     archiver. Initialize this class passing the URL where the mailing list
     archiver is and the directory path where the mbox files will be fetched
     and stored. The origin of the data will be set to the value of `url`.
 
     :param url: URL to the HyperKitty mailing list archiver
     :param dirpath: directory path where the mboxes are stored
     :param tag: label used to mark the data
-    :param cache: cache object to store raw data
+    :param archive: archive to store/retrieve items
+    :param ssl_verify: enable/disable SSL verification
     """
-    version = '0.2.0'
+    version = '1.0.0'
+
+    CATEGORIES = [CATEGORY_MESSAGE]
 
-    def __init__(self, url, dirpath, tag=None, cache=None):
-        super().__init__(url, dirpath, tag=tag, cache=cache)
+    def __init__(self, url, dirpath, tag=None, archive=None, ssl_verify=True):
+        super().__init__(url, dirpath, tag=tag, archive=archive, ssl_verify=ssl_verify)
         self.url = url
 
-    @metadata
-    def fetch(self, from_date=DEFAULT_DATETIME):
+    def fetch(self, category=CATEGORY_MESSAGE, from_date=DEFAULT_DATETIME,
+              to_date=DEFAULT_LAST_DATETIME):
         """Fetch the messages from the HyperKitty mailing list archiver.
 
         The method fetches the mbox files from a remote HyperKitty
         mailing list archiver and retrieves the messages stored on them.
 
         Take into account that HyperKitty does not provide yet any kind
         of info to know which is the first message on the mailing list.
         For this reason, using a value in `from_date` previous to the
         date where the first message was sent will make to download
         empty mbox files.
 
+        :param category: the category of items to fetch
         :param from_date: obtain messages since this date
+        :param to_date: obtain messages until this date
 
         :returns: a generator of messages
         """
-        logger.info("Looking for messages from '%s' since %s",
-                    self.url, str(from_date))
+        if not to_date:
+            to_date = DEFAULT_LAST_DATETIME
+
+        items = super().fetch(category, from_date, to_date)
+
+        return items
+
+    def fetch_items(self, category, **kwargs):
+        """Fetch the messages
+
+        :param category: the category of items to fetch
+        :param kwargs: backend arguments
+
+        :returns: a generator of items
+        """
+        from_date = kwargs['from_date']
+        to_date = kwargs['to_date']
+
+        logger.info("Looking for messages from '%s' since %s until %s",
+                    self.url, str(from_date), str(to_date))
 
         mailing_list = HyperKittyList(self.url, self.dirpath)
-        mailing_list.fetch(from_date=from_date)
+        mailing_list.fetch(from_date=from_date, to_date=to_date)
 
-        messages = self._fetch_and_parse_messages(mailing_list, from_date)
+        messages = self._fetch_and_parse_messages(mailing_list, from_date, to_date)
 
         for message in messages:
             yield message
 
         logger.info("Fetch process completed")
 
     @classmethod
-    def has_caching(cls):
-        """Returns whether it supports caching items on the fetch process.
+    def has_archiving(cls):
+        """Returns whether it supports archiving items on the fetch process.
 
-        :returns: this backend dooes not support items cache
+        :returns: this backend does not support items archive
         """
         return False
 
     @classmethod
     def has_resuming(cls):
         """Returns whether it supports to resume the fetch process.
 
@@ -118,45 +142,59 @@
 
     Notice that this class only works with HyperKitty version 1.0.4
     or greater. Previous versions do not export messages in MBox
     format.
 
     :param url: URL to the HyperKitty archiver for this list
     :param dirpath: path to the local mboxes archives
+    :param ssl_verify: enable/disable SSL verification
     """
-    def __init__(self, url, dirpath):
+    # API resources
+    REXPORT = 'export'
+
+    # Resource parameters
+    PSTART = 'start'
+    PEND = 'end'
+
+    def __init__(self, url, dirpath, ssl_verify=True):
         super().__init__(url, dirpath)
-        self.client = HttpClient(url)
+        self.client = HttpClient(url, ssl_verify=ssl_verify)
 
-    def fetch(self, from_date=DEFAULT_DATETIME):
+    def fetch(self, from_date=DEFAULT_DATETIME, to_date=DEFAULT_LAST_DATETIME):
         """Fetch the mbox files from the remote archiver.
 
         This method stores the archives in the path given during the
         initialization of this object.
 
         HyperKitty archives are accessed month by month and stored following
         the schema year-month. Archives are fetched from the given month
         till the current month.
 
         :param from_date: fetch archives that store messages
             equal or after the given date; only year and month values
             are compared
+        :param to_date: fetch archives that store messages
+            equal or before the given date; only year and month values
+            are compared
 
         :returns: a list of tuples, storing the links and paths of the
             fetched archives
         """
-        logger.info("Downloading mboxes from '%s' to since %s",
-                    self.client.base_url, str(from_date))
+        logger.info("Downloading mboxes from '%s' to since %s until %s",
+                    self.client.base_url, str(from_date), str(to_date))
         logger.debug("Storing mboxes in '%s'", self.dirpath)
 
         self.client.fetch(self.client.base_url)
 
         from_date = datetime_to_utc(from_date)
-        to_end = datetime_utcnow()
-        to_end += dateutil.relativedelta.relativedelta(months=1)
+        if to_date != DEFAULT_LAST_DATETIME:
+            to_end = datetime_to_utc(to_date)
+        else:
+            to_end = datetime_utcnow()
+            to_end += dateutil.relativedelta.relativedelta(months=1)
 
         months = months_range(from_date, to_end)
 
         fetched = []
 
         if not os.path.exists(self.dirpath):
             os.makedirs(self.dirpath)
@@ -165,19 +203,19 @@
 
         for dts in months:
             tmbox += 1
             start, end = dts[0], dts[1]
             filename = start.strftime("%Y-%m.mbox.gz")
             filepath = os.path.join(self.dirpath, filename)
 
-            url = urijoin(self.client.base_url, 'export', filename)
+            url = urijoin(self.client.base_url, self.REXPORT, filename)
 
             params = {
-                'start': start.strftime("%Y-%m-%d"),
-                'end': end.strftime("%Y-%m-%d")
+                self.PSTART: start.strftime("%Y-%m-%d"),
+                self.PEND: end.strftime("%Y-%m-%d")
             }
 
             success = self._download_archive(url, params, filepath)
 
             if success:
                 fetched.append((url, filepath))
 
@@ -246,20 +284,22 @@
             base_path = os.path.expanduser('~/.perceval/mailinglists/')
             dirpath = os.path.join(base_path, self.parsed_args.url)
         else:
             dirpath = self.parsed_args.mboxes_path
 
         setattr(self.parsed_args, 'dirpath', dirpath)
 
-    @staticmethod
-    def setup_cmd_parser():
+    @classmethod
+    def setup_cmd_parser(cls):
         """Returns the HyperKitty argument parser."""
 
-        parser = BackendCommandArgumentParser(from_date=True,
-                                              cache=False)
+        parser = BackendCommandArgumentParser(cls.BACKEND,
+                                              from_date=True,
+                                              to_date=True,
+                                              ssl_verify=True)
 
         # Optional arguments
         group = parser.parser.add_argument_group('HyperKitty arguments')
         group.add_argument('--mboxes-path', dest='mboxes_path',
                            help="Path where mbox files will be stored")
 
         # Required arguments
```

### Comparing `perceval-0.9.9/perceval/backends/core/gerrit.py` & `perceval-1.0.0rc1/perceval/backends/core/gerrit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,126 +1,202 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2017 Bitergia
+# Copyright (C) 2015-2020 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1335, USA.
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
-#     Alvaro del Castillo San Felix <acs@bitergia.com>
 #     Santiago Dueñas <sduenas@bitergia.com>
+#     Alvaro del Castillo <acs@bitergia.com>
+#     Valerio Cosentino <valcos@bitergia.com>
+#     Prabhat <prabhatsharma7298@gmail.com>
+#     Jesus M. Gonzalez-Barahona <jgb@gsyc.es>
+#     Harshal Mittal <harshalmittal4@gmail.com>
 #
 
 import json
 import logging
 import re
 import subprocess
 import time
 
-from grimoirelab.toolkit.datetime import datetime_to_utc
+from grimoirelab_toolkit.datetime import datetime_to_utc
 
 from ...backend import (Backend,
                         BackendCommand,
                         BackendCommandArgumentParser,
-                        metadata)
-from ...errors import BackendError, CacheError
+                        OriginUniqueField)
+from ...errors import BackendError
 from ...utils import DEFAULT_DATETIME
 
+CATEGORY_REVIEW = "review"
 
 MAX_REVIEWS = 500  # Maximum number of reviews per query
 PORT = '29418'
 
 logger = logging.getLogger(__name__)
 
 
 class Gerrit(Backend):
     """Gerrit backend.
 
     Class to fetch the reviews from a Gerrit server. To initialize
-    this class the URL of the server must be provided. The `url`
+    this class the Hostname of the server must be provided. The `hostname`
     will be set as the origin of the data.
 
-    :param url: Gerrit server URL
+    :param hostname: Gerrit server Hostname
     :param user: SSH user used to connect to the Gerrit server
+    :param port: SSH port
     :param max_reviews: maximum number of reviews requested on the same query
-    :param blacklist_reviews: exclude the reviews of this list while fetching
+    :param disable_host_key_check: disable host key controls
     :param tag: label used to mark the data
-    :param cache: cache object to store raw data
+    :param archive: archive to store/retrieve items
+    :param blacklist_ids: exclude the reviews while fetching
+    :param id_filepath: path to SSH private key
     """
-    version = '0.7.4'
+    version = '1.0.0'
 
-    def __init__(self, url,
-                 user=None, port=PORT, max_reviews=MAX_REVIEWS,
-                 blacklist_reviews=None,
-                 disable_host_key_check=False,
-                 tag=None, cache=None):
-        origin = url
+    CATEGORIES = [CATEGORY_REVIEW]
+    EXTRA_SEARCH_FIELDS = {
+        'project_name': ['project'],
+        'review_hash': ['id']
+    }
+    ORIGIN_UNIQUE_FIELD = OriginUniqueField(name='number', type=str)
 
-        super().__init__(origin, tag=tag, cache=cache)
-        self.url = url
+    def __init__(self, hostname,
+                 user=None, port=PORT, max_reviews=MAX_REVIEWS,
+                 disable_host_key_check=False, id_filepath=None,
+                 tag=None, archive=None, blacklist_ids=None):
+        origin = hostname
+
+        super().__init__(origin, tag=tag, archive=archive, blacklist_ids=blacklist_ids)
+        self.hostname = hostname
+        self.user = user
+        self.port = port
+        self.id_filepath = id_filepath
         self.max_reviews = max(1, max_reviews)
-        self.blacklist_reviews = blacklist_reviews
-        self.client = GerritClient(self.url, user, max_reviews,
-                                   blacklist_reviews, disable_host_key_check, port=port)
+        self.blacklist_ids = blacklist_ids
+        self.disable_host_key_check = disable_host_key_check
+        self.archive = archive
+        self.client = None
 
-    @metadata
-    def fetch(self, from_date=DEFAULT_DATETIME):
+    def fetch(self, category=CATEGORY_REVIEW, from_date=DEFAULT_DATETIME):
         """Fetch the reviews from the repository.
 
         The method retrieves, from a Gerrit repository, the reviews
         updated since the given date.
 
+        :param category: the category of items to fetch
         :param from_date: obtain reviews updated since this date
 
         :returns: a generator of reviews
         """
-        self._purge_cache_queue()
+        if not from_date:
+            from_date = DEFAULT_DATETIME
+
+        kwargs = {'from_date': from_date}
+        items = super().fetch(category, **kwargs)
+
+        return items
+
+    def fetch_items(self, category, **kwargs):
+        """Fetch the reviews
+
+        :param category: the category of items to fetch
+        :param kwargs: backend arguments
+
+        :returns: a generator of items
+        """
+        from_date = kwargs['from_date']
 
         if self.client.version[0] == 2 and self.client.version[1] == 8:
             fetcher = self._fetch_gerrit28(from_date)
         else:
             fetcher = self._fetch_gerrit(from_date)
 
         for review in fetcher:
             yield review
 
-    @metadata
-    def fetch_from_cache(self):
-        """Fetch reviews from the cache.
-
-        It returns the reviews stored in the cache object provided during
-        the initialization of the object. If this method is called but
-        no cache object was provided, the method will raise a `CacheError`
-        exception.
+    @classmethod
+    def has_archiving(cls):
+        """Returns whether it supports archiving items on the fetch process.
 
-        :returns: a generator of items
+        :returns: this backend supports items archive
+        """
+        return True
 
-        :raises CacheError: raised when an error occurs accesing the
-            cache
+    @classmethod
+    def has_resuming(cls):
+        """Returns whether it supports to resume the fetch process.
+
+        :returns: this backend does not support items resuming
         """
-        if not self.cache:
-            raise CacheError(cause="cache instance was not provided")
+        return False
 
-        cache_items = self.cache.retrieve()
+    @staticmethod
+    def metadata_id(item):
+        """Extracts the identifier from a Gerrit item."""
 
-        for raw_items in cache_items:
-            reviews = self.parse_reviews(raw_items)
-            for review in reviews:
-                yield review
+        return str(item['number'])
+
+    @staticmethod
+    def metadata_updated_on(item):
+        """Extracts and converts the update time from a Gerrit item.
+
+        The timestamp is extracted from 'lastUpdated' field. This date is
+        a UNIX timestamp but needs to be converted to a float value.
+
+        :param item: item generated by the backend
+
+        :returns: a UNIX timestamp
+        """
+        return float(item['lastUpdated'])
+
+    @staticmethod
+    def metadata_category(item):
+        """Extracts the category from a Gerrit item.
+
+        This backend only generates one type of item which is
+        'review'.
+        """
+        return CATEGORY_REVIEW
+
+    @staticmethod
+    def parse_reviews(raw_data):
+        """Parse a Gerrit reviews list."""
+
+        # Join isolated reviews in JSON in array for parsing
+        items_raw = "[" + raw_data.replace("\n", ",") + "]"
+        items_raw = items_raw.replace(",]", "]")
+        items = json.loads(items_raw)
+        reviews = []
+
+        for item in items:
+            if 'project' in item.keys():
+                reviews.append(item)
+
+        return reviews
+
+    def _init_client(self, from_archive=False):
+
+        return GerritClient(self.hostname, self.user, self.max_reviews,
+                            self.blacklist_ids, self.disable_host_key_check,
+                            self.port, self.id_filepath, self.archive,
+                            from_archive)
 
     def _fetch_gerrit28(self, from_date=DEFAULT_DATETIME):
         """ Specific fetch for gerrit 2.8 version.
 
         Get open and closed reviews in different queries.
         Take the newer review from both lists and iterate.
         """
@@ -152,15 +228,15 @@
                 review = review_closed
             else:
                 review_open = reviews_open.pop(0)
                 review = review_open
 
             updated = review['lastUpdated']
             if updated <= from_ut:
-                logger.debug("No more updates for %s" % (self.url))
+                logger.debug("No more updates for %s" % (self.hostname))
                 break
             else:
                 yield review
 
             if not reviews_open and last_nreviews_open >= self.max_reviews:
                 last_item_open = self.client.next_retrieve_group_item(last_item_open, review_open)
                 reviews_open = self._get_reviews(last_item_open, filter_open)
@@ -183,161 +259,93 @@
             review = reviews.pop(0)
             try:
                 last_item += 1
             except Exception:
                 pass  # last_item is a string in old gerrits
             updated = review['lastUpdated']
             if updated <= from_ut:
-                logger.debug("No more updates for %s" % (self.url))
+                logger.debug("No more updates for %s" % (self.hostname))
                 break
             else:
                 yield review
 
             if not reviews and last_nreviews >= self.max_reviews:
                 logger.debug("GETTING MORE REVIEWS %i >= %i " % (last_nreviews, self.max_reviews))
                 last_item = self.client.next_retrieve_group_item(last_item, review)
                 reviews = self._get_reviews(last_item)
                 last_nreviews = len(reviews)
 
     def _get_reviews(self, last_item, filter_=None):
         task_init = time.time()
         raw_data = self.client.reviews(last_item, filter_)
-        self._push_cache_queue(raw_data)
-        self._flush_cache_queue()
         reviews = self.parse_reviews(raw_data)
         logger.info("Received %i reviews in %.2fs" % (len(reviews),
                                                       time.time() - task_init))
         return reviews
 
-    @classmethod
-    def has_caching(cls):
-        """Returns whether it supports caching items on the fetch process.
-
-        :returns: this backend supports items cache
-        """
-        return True
-
-    @classmethod
-    def has_resuming(cls):
-        """Returns whether it supports to resume the fetch process.
-
-        :returns: this backend does not support items resuming
-        """
-        return False
-
-    @staticmethod
-    def metadata_id(item):
-        """Extracts the identifier from a Gerrit item."""
-
-        return str(item['number'])
-
-    @staticmethod
-    def metadata_updated_on(item):
-        """Extracts and converts the update time from a Gerrit item.
-
-        The timestamp is extracted from 'lastUpdated' field. This date is
-        a UNIX timestamp but needs to be converted to a float value.
-
-        :param item: item generated by the backend
-
-        :returns: a UNIX timestamp
-        """
-        return float(item['lastUpdated'])
-
-    @staticmethod
-    def metadata_category(item):
-        """Extracts the category from a Gerrit item.
-
-        This backend only generates one type of item which is
-        'review'.
-        """
-        return 'review'
-
-    @staticmethod
-    def parse_reviews(raw_data):
-        """Parse a Gerrit reviews list."""
-
-        # Join isolated reviews in JSON in array for parsing
-        items_raw = "[" + raw_data.replace("\n", ",") + "]"
-        items_raw = items_raw.replace(",]", "]")
-        items = json.loads(items_raw)
-        reviews = []
-
-        for item in items:
-            if 'project' in item.keys():
-                reviews.append(item)
-
-        return reviews
-
 
 class GerritClient():
     """Gerrit API client.
 
     This class implements a client to retrieve reviews from a Gerrit
     repository using the ssh API. Currently it supports <2.8 and >=2.9
     versions in incremental mode.
 
     Check the next link for more info:
     https://gerrit-documentation.storage.googleapis.com/Documentation/2.12/cmd-query.html
 
-    :param repository: URL of the Gerrit server
+    :param repository: Hostname of the Gerrit server
     :param user: SSH user to be used to connect to gerrit server
     :param max_reviews: max number of reviews per query
+    :param blacklist_reviews: exclude the reviews of this list while fetching
+    :param disable_host_key_check: disable host key controls
+    :param port: SSH port
+    :param id_filepath: SSH private key path
+    :param archive: collect issues already retrieved from an archive
+    :param from_archive: it tells whether to write/read the archive
     """
     VERSION_REGEX = re.compile(r'gerrit version (\d+)\.(\d+).*')
     CMD_GERRIT = 'gerrit'
     CMD_VERSION = 'version'
     MAX_RETRIES = 3  # max number of retries when a command fails
     RETRY_WAIT = 60  # number of seconds when retrying a ssh command
 
-    def __init__(self, repository, user, max_reviews, blacklist_reviews=[],
-                 disable_host_key_check=False, port=PORT):
+    def __init__(self, repository, user=None, max_reviews=MAX_REVIEWS, blacklist_reviews=None,
+                 disable_host_key_check=False, port=PORT, id_filepath=None,
+                 archive=None, from_archive=False):
         self.gerrit_user = user
         self.max_reviews = max_reviews
-        self.blacklist_reviews = blacklist_reviews
+
+        self.blacklist_reviews = [] if not blacklist_reviews else blacklist_reviews
         self.repository = repository
         self.project = None
         self._version = None
         self.port = port
+        self.id_filepath = id_filepath
+        self.archive = archive
+        self.from_archive = from_archive
+
         ssh_opts = ''
         if disable_host_key_check:
             ssh_opts += "-o StrictHostKeyChecking=no "
 
+        if self.id_filepath:
+            ssh_opts += "-i %s " % self.id_filepath
+
         if self.port:
             self.gerrit_cmd = "ssh %s -p %s %s@%s" % (ssh_opts, self.port,
                                                       self.gerrit_user, self.repository)
         else:
             self.gerrit_cmd = "ssh %s %s@%s" % (ssh_opts, self.gerrit_user, self.repository)
 
         self.gerrit_cmd += " %s " % (GerritClient.CMD_GERRIT)
 
-    def __execute(self, cmd):
-        """ Execute gerrit command with retry if it fails """
-
-        data = None  # data result from the cmd execution
-
-        retries = 0
-
-        while retries < self.MAX_RETRIES:
-            try:
-                data = subprocess.check_output(cmd, shell=True)
-                break
-            except subprocess.CalledProcessError as ex:
-                logger.error("gerrit cmd %s failed: %s", cmd, ex)
-                time.sleep(self.RETRY_WAIT * retries)
-                retries += 1
-
-        if data is None:
-            raise RuntimeError(cmd + " failed " + str(self.MAX_RETRIES) + " times. Giving up!")
-
-        return data
-
     @property
     def version(self):
-        """ Return the Gerrit server version."""
+        """Return the Gerrit server version."""
 
         if self._version:
             return self._version
 
         cmd = self.gerrit_cmd + " %s " % (GerritClient.CMD_VERSION)
 
         logger.debug("Getting version: %s" % (cmd))
@@ -376,29 +384,90 @@
     def next_retrieve_group_item(self, last_item=None, entry=None):
         """Return the item to start from in next reviews group."""
 
         next_item = None
 
         gerrit_version = self.version
 
-        if gerrit_version[0] == 2 and gerrit_version[1] >= 9:
+        if (gerrit_version[0] == 2 and gerrit_version[1] > 9) or gerrit_version[0] == 3:
             if last_item is None:
                 next_item = 0
             else:
                 next_item = last_item
-        elif gerrit_version[0] == 2 and gerrit_version == 9:
+        elif gerrit_version[0] == 2 and gerrit_version[1] == 9:
             # https://groups.google.com/forum/#!topic/repo-discuss/yQgRR5hlS3E
             cause = "Gerrit 2.9.0 does not support pagination"
             raise BackendError(cause=cause)
         else:
             if entry is not None:
                 next_item = entry['sortKey']
 
         return next_item
 
+    @staticmethod
+    def sanitize_for_archive(cmd):
+        """Sanitize the Gerrit command by removing username information
+        before storing/retrieving archived items
+
+        :param: cmd: Gerrit command
+
+        :returns the sanitized cmd
+        """
+        sanitized_cmd = re.sub(r" \S*@", ' xxxxx@', cmd)
+
+        return sanitized_cmd
+
+    def __execute(self, cmd):
+        """Execute gerrit command"""
+
+        if self.from_archive:
+            response = self.__execute_from_archive(cmd)
+        else:
+            response = self.__execute_from_remote(cmd)
+
+        return response
+
+    def __execute_from_archive(self, cmd):
+        """Execute gerrit command against the archive"""
+
+        cmd = self.sanitize_for_archive(cmd)
+        response = self.archive.retrieve(cmd, None, None)
+
+        if isinstance(response, RuntimeError):
+            raise response
+
+        return response
+
+    def __execute_from_remote(self, cmd):
+        """Execute gerrit command with retry if it fails"""
+
+        result = None  # data result from the cmd execution
+        retries = 0
+
+        while retries < self.MAX_RETRIES:
+            try:
+                result = subprocess.check_output(cmd, shell=True)
+                break
+            except subprocess.CalledProcessError as ex:
+                logger.error("gerrit cmd %s failed: %s", cmd, ex)
+                time.sleep(self.RETRY_WAIT * retries)
+                retries += 1
+
+        if result is None:
+            result = RuntimeError(cmd + " failed " + str(self.MAX_RETRIES) + " times. Giving up!")
+
+        if self.archive:
+            cmd = self.sanitize_for_archive(cmd)
+            self.archive.store(cmd, None, None, result)
+
+        if isinstance(result, RuntimeError):
+            raise result
+
+        return result
+
     def _get_gerrit_cmd(self, last_item, filter_=None):
 
         if filter_ and filter_ not in ['status:open', 'status:closed']:
             cause = "Filter not supported in gerrit %s" % (filter_)
             raise BackendError(cause=cause)
 
         cmd = self.gerrit_cmd + " query "
@@ -421,48 +490,48 @@
                 cmd += " %s " % (filter_)
 
         cmd += " --all-approvals --comments --format=JSON"
 
         gerrit_version = self.version
 
         if last_item is not None:
-            if gerrit_version[0] == 2 and gerrit_version[1] >= 9:
+            if (gerrit_version[0] == 2 and gerrit_version[1] >= 9) or gerrit_version[0] == 3:
                 cmd += " --start=" + str(last_item)
             else:
                 cmd += " resume_sortkey:" + last_item
 
         return cmd
 
 
 class GerritCommand(BackendCommand):
     """Class to run Gerrit backend from the command line."""
 
     BACKEND = Gerrit
 
-    @staticmethod
-    def setup_cmd_parser():
+    @classmethod
+    def setup_cmd_parser(cls):
         """Returns the Gerrit argument parser."""
 
-        parser = BackendCommandArgumentParser(from_date=True,
-                                              cache=True)
+        parser = BackendCommandArgumentParser(cls.BACKEND,
+                                              from_date=True,
+                                              archive=True,
+                                              blacklist=True)
 
         # Gerrit options
         group = parser.parser.add_argument_group('Gerrit arguments')
         group.add_argument('--user', dest='user',
                            help="Gerrit ssh user")
         group.add_argument('--max-reviews', dest='max_reviews',
                            type=int, default=MAX_REVIEWS,
                            help="Max number of reviews per ssh query.")
-        group.add_argument('--blacklist-reviews', dest='blacklist_reviews',
-                           nargs='*',
-                           help="Wrong reviews that must not be retrieved.")
         group.add_argument('--disable-host-key-check', dest='disable_host_key_check', action='store_true',
                            help="Don't check remote host identity")
         group.add_argument('--ssh-port', dest='port',
-                           default=PORT,
+                           default=PORT, type=int,
                            help="Set SSH port of the Gerrit server")
+        group.add_argument('--ssh-id-filepath', dest='id_filepath', help="Set SSH private key path")
 
         # Required arguments
-        parser.parser.add_argument('url',
-                                   help="URL of the Gerrit server")
+        parser.parser.add_argument('hostname',
+                                   help="Hostname of the Gerrit server")
 
         return parser
```

### Comparing `perceval-0.9.9/perceval/backends/core/redmine.py` & `perceval-1.0.0rc1/perceval/backends/core/redmine.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,98 +1,123 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2017 Bitergia
+# Copyright (C) 2015-2020 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1335, USA.
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #     Santiago Dueñas <sduenas@bitergia.com>
+#     Stephan Barth <stephan.barth@gmail.com>
+#     Valerio Cosentino <valcos@bitergia.com>
+#     Jesus M. Gonzalez-Barahona <jgb@gsyc.es>
+#     Harshal Mittal <harshalmittal4@gmail.com>
 #
 
 import json
 import logging
 
 import requests
 
-from grimoirelab.toolkit.datetime import datetime_to_utc, str_to_datetime
-from grimoirelab.toolkit.uris import urijoin
+from grimoirelab_toolkit.datetime import datetime_to_utc, str_to_datetime
+from grimoirelab_toolkit.uris import urijoin
 
 from ...backend import (Backend,
                         BackendCommand,
-                        BackendCommandArgumentParser,
-                        metadata)
+                        BackendCommandArgumentParser)
 from ...client import HttpClient
-from ...errors import CacheError
 from ...utils import DEFAULT_DATETIME
 
-
-logger = logging.getLogger(__name__)
-
+CATEGORY_ISSUE = "issue"
 
 MAX_ISSUES = 100  # Maximum number of issues per query
 USER_FIELDS = ['assigned_to', 'author']
 
+logger = logging.getLogger(__name__)
+
 
 class Redmine(Backend):
     """Redmine backend.
 
     This class allows to fetch the issues stored on a Redmine
     server. Initialize this class passing the URL of this server.
     Some servers require authentication to get access to some
     data, if this is the case, pass the API token to `api_token`
     parameter.
 
     :param url: URL of the server
     :param api_token: token needed to use the API
     :param max_issues:  maximum number of issues requested on the same query
     :param tag: label used to mark the data
-    :param cache: cache object to store raw data
+    :param archive: archive to store/retrieve items
+    :param ssl_verify: enable/disable SSL verification
     """
-    version = '0.6.0'
+    version = '1.0.0'
+
+    CATEGORIES = [CATEGORY_ISSUE]
+    EXTRA_SEARCH_FIELDS = {
+        'project_name': ['project', 'name'],
+        'project_id': ['project', 'id']
+    }
 
     def __init__(self, url, api_token=None, max_issues=MAX_ISSUES,
-                 tag=None, cache=None):
+                 tag=None, archive=None, ssl_verify=True):
         origin = url
 
-        super().__init__(origin, tag=tag, cache=cache)
+        super().__init__(origin, tag=tag, archive=archive, ssl_verify=ssl_verify)
         self.url = url
+        self.api_token = api_token
         self.max_issues = max_issues
-        self.client = RedmineClient(url, api_token=api_token)
+        self.client = None
+
         self._users = {}
 
-    @metadata
-    def fetch(self, from_date=DEFAULT_DATETIME):
+    def fetch(self, category=CATEGORY_ISSUE, from_date=DEFAULT_DATETIME):
         """Fetch the issues from the server.
 
         This method fetches the issues stored on the server that were
         updated since the given date. Data about attachments, journals
         and watchers (among others) are included within each issue.
 
+        :param category: the category of items to fetch
         :param from_date: obtain issues updated since this date
 
         :returns: a generator of issues
         """
-        logger.info("Fetching issues of '%s' from %s",
-                    self.url, str(from_date))
-
-        self._purge_cache_queue()
+        if not from_date:
+            from_date = DEFAULT_DATETIME
 
         from_date = datetime_to_utc(from_date)
+        kwargs = {'from_date': from_date}
+        items = super().fetch(category, **kwargs)
+
+        return items
+
+    def fetch_items(self, category, **kwargs):
+        """Fetch the issues
+
+        :param category: the category of items to fetch
+        :param kwargs: backend arguments
+
+        :returns: a generator of items
+        """
+        from_date = kwargs['from_date']
+
+        logger.info("Fetching issues of '%s' from %s",
+                    self.url, str(from_date))
 
         nissues = 0
 
         for issue_id in self.__fetch_issues_ids(from_date):
             issue = self.__fetch_and_parse_issue(issue_id)
 
             for key in USER_FIELDS:
@@ -105,171 +130,24 @@
             for journal in issue['journals']:
                 if 'user' not in journal:
                     continue
 
                 user = self.__get_or_fetch_user(journal['user']['id'])
                 journal['user_data'] = user
 
-            # Checkpoint
-            self._push_cache_queue('{}')
-
             yield issue
             nissues += 1
-            self._flush_cache_queue()
 
         logger.info("Fetch process completed: %s issues fetched", nissues)
 
-    @metadata
-    def fetch_from_cache(self):
-        """Fetch the issues from the cache.
-
-        It returns the issues stored in the cache object, provided during
-        the initialization of the object. If this method is called but
-        no cache object was provided, the method will raise a `CacheError`
-        exception.
-
-        :returns: a generator of issues
-
-        :raises CacheError: raised when an error occurs accesing the
-            cache
-        """
-        if not self.cache:
-            raise CacheError(cause="cache instance was not provided")
-
-        logger.info("Retrieving cached tasks: '%s'", self.url)
-
-        nissues = 0
-
-        for issue in self.__fetch_from_cache():
-            yield issue
-            nissues += 1
-
-        logger.info("Retrieval process completed: %s bugs retrieved from cache",
-                    nissues)
-
-    def __fetch_issues_ids(self, from_date):
-        offset = 0
-        issues = self.__fetch_and_parse_issues_page(from_date, offset,
-                                                    self.max_issues)
-
-        while issues:
-            issue = issues.pop(0)
-            issue_id = issue['id']
-            yield issue_id
-
-            if not issues:
-                offset += self.max_issues
-                issues = self.__fetch_and_parse_issues_page(from_date, offset,
-                                                            self.max_issues)
-
-    def __get_or_fetch_user(self, user_id):
-        if user_id in self._users:
-            return self._users[user_id]
-
-        logger.debug("User %s not found on client cache; fetching it", user_id)
-
-        try:
-            user = self.__fetch_and_parse_user(user_id)
-        except requests.exceptions.HTTPError as e:
-            if e.response.status_code == 404:
-                logger.warning("User %s not found on the server; skipping it",
-                               user_id)
-                user = {}
-            else:
-                raise e
-
-        self._users[user_id] = user
-
-        return user
-
-    def __fetch_from_cache(self):
-        cache_items = self.cache.retrieve()
-
-        while True:
-            try:
-                raw_issue = next(cache_items)
-            except StopIteration:
-                break
-
-            issue = self.parse_issue_data(raw_issue)
-
-            for cache_user in self.__fetch_users_from_cache(cache_items):
-                self._users[cache_user['id']] = cache_user
-
-            for key in USER_FIELDS:
-                if key not in issue:
-                    continue
-
-                user_id = issue[key]['id']
-
-                try:
-                    issue[key + '_data'] = self._users.get(user_id, {})
-                except KeyError:
-                    # Fatal error. Keys must exist.
-                    cause = "invalid cached data, user id %s not found" % user_id
-                    raise CacheError(cause=cause)
-
-            for journal in issue['journals']:
-                if 'user' not in journal:
-                    continue
-
-                user_id = journal['user']['id']
-
-                try:
-                    journal['user_data'] = self._users.get(user_id, {})
-                except KeyError:
-                    # Fatal error. Keys must exist.
-                    cause = "invalid cached data, user id %s not found" % user_id
-                    raise CacheError(cause=cause)
-
-            yield issue
-
-    def __fetch_users_from_cache(self, cache_items):
-        fetch_user = True
-
-        while fetch_user:
-            try:
-                raw_user = next(cache_items)
-            except StopIteration:
-                # Fatal error. The code should not reach here.
-                # Cache should had reaeched a checkpoint
-                cause = "cache is exhausted but more items were expected"
-                raise CacheError(cause=cause)
-
-            if raw_user == '{}':
-                fetch_user = False
-            else:
-                user = self.parse_user_data(raw_user)
-                yield user
-
-    def __fetch_and_parse_issues_page(self, from_date, offset, max_issues):
-        logger.debug("Fetching and parsing issues page from %s (offset: %s)",
-                     str(from_date), str(offset))
-        raw_json = self.client.issues(from_date=from_date, offset=offset,
-                                      max_issues=max_issues)
-        issues = self.parse_issues(raw_json)
-        return [issue for issue in issues]
-
-    def __fetch_and_parse_issue(self, issue_id):
-        logger.debug("Fetching and parsing issue #%s", issue_id)
-        raw_issue = self.client.issue(issue_id)
-        self._push_cache_queue(raw_issue)
-        return self.parse_issue_data(raw_issue)
-
-    def __fetch_and_parse_user(self, user_id):
-        logger.debug("Fetching and parsing user #%s", user_id)
-        raw_user = self.client.user(user_id)
-        self._push_cache_queue(raw_user)
-        return self.parse_user_data(raw_user)
-
     @classmethod
-    def has_caching(cls):
-        """Returns whether it supports caching items on the fetch process.
+    def has_archiving(cls):
+        """Returns whether it supports archiving items on the fetch process.
 
-        :returns: this backend supports items cache
+        :returns: this backend supports items archive
         """
         return True
 
     @classmethod
     def has_resuming(cls):
         """Returns whether it supports to resume the fetch process.
 
@@ -302,15 +180,15 @@
     @staticmethod
     def metadata_category(item):
         """Extracts the category from a Redmine item.
 
         This backend only generates one type of item which is
         'issue'.
         """
-        return 'issue'
+        return CATEGORY_ISSUE
 
     @staticmethod
     def parse_issues(raw_json):
         """Parse a Redmine issues JSON stream.
 
         The method parses a JSON stream and returns a list iterator.
         Each item is a dictionary that contains the issue parsed data.
@@ -349,27 +227,87 @@
         :param raw_json: JSON string to parse
 
         :returns: a dictionary with the parsed user data
         """
         result = json.loads(raw_json)
         return result['user']
 
+    def _init_client(self, from_archive=False):
+        """Init client"""
+
+        return RedmineClient(self.url, self.api_token, self.archive, from_archive, self.ssl_verify)
+
+    def __fetch_issues_ids(self, from_date):
+        offset = 0
+        issues = self.__fetch_and_parse_issues_page(from_date, offset,
+                                                    self.max_issues)
+
+        while issues:
+            issue = issues.pop(0)
+            issue_id = issue['id']
+            yield issue_id
+
+            if not issues:
+                offset += self.max_issues
+                issues = self.__fetch_and_parse_issues_page(from_date, offset,
+                                                            self.max_issues)
+
+    def __get_or_fetch_user(self, user_id):
+        if user_id in self._users:
+            return self._users[user_id]
+
+        logger.debug("User %s not found on client cache; fetching it", user_id)
+
+        try:
+            user = self.__fetch_and_parse_user(user_id)
+        except requests.exceptions.HTTPError as e:
+            if e.response.status_code == 404:
+                logger.warning("User %s not found on the server; skipping it",
+                               user_id)
+                user = {}
+            else:
+                raise e
+
+        self._users[user_id] = user
+
+        return user
+
+    def __fetch_and_parse_issues_page(self, from_date, offset, max_issues):
+        logger.debug("Fetching and parsing issues page from %s (offset: %s)",
+                     str(from_date), str(offset))
+        raw_json = self.client.issues(from_date=from_date, offset=offset,
+                                      max_issues=max_issues)
+        issues = self.parse_issues(raw_json)
+        return [issue for issue in issues]
+
+    def __fetch_and_parse_issue(self, issue_id):
+        logger.debug("Fetching and parsing issue #%s", issue_id)
+        raw_issue = self.client.issue(issue_id)
+        return self.parse_issue_data(raw_issue)
+
+    def __fetch_and_parse_user(self, user_id):
+        logger.debug("Fetching and parsing user #%s", user_id)
+        raw_user = self.client.user(user_id)
+        return self.parse_user_data(raw_user)
+
 
 class RedmineCommand(BackendCommand):
     """Class to run Redmine backend from the command line."""
 
     BACKEND = Redmine
 
-    @staticmethod
-    def setup_cmd_parser():
+    @classmethod
+    def setup_cmd_parser(cls):
         """Returns the Redmine argument parser."""
 
-        parser = BackendCommandArgumentParser(from_date=True,
+        parser = BackendCommandArgumentParser(cls.BACKEND,
+                                              from_date=True,
                                               token_auth=True,
-                                              cache=True)
+                                              archive=True,
+                                              ssl_verify=True)
 
         # Redmine options
         group = parser.parser.add_argument_group('Redmine arguments')
         group.add_argument('--max-issues', dest='max_issues',
                            type=int, default=MAX_ISSUES,
                            help="Maximum number of issues requested on the same query")
 
@@ -386,14 +324,17 @@
     This class implements a client that retrieves issues from
     a Redmine server. Remine servers provides a REST API that
     returns its results in JSON format.
 
     :param base_url: URL of the Phabricator server
     :param api_token: token to get access to restricted data
         stored in the server
+    :param archive: an archive to store/read fetched data
+    :param from_archive: it tells whether to write/read the archive
+    :param ssl_verify: enable/disable SSL verification
     """
     URL = '%(base)s/%(resource)s'
 
     RISSUES = 'issues'
     RUSERS = 'users'
 
     PINCLUDE = 'include'
@@ -408,16 +349,16 @@
     CATTACHMENTS = 'attachments'
     CCHANGESETS = 'changesets'
     CCHILDREN = 'children'
     CJOURNALS = 'journals'
     CRELATIONS = 'relations'
     CWATCHERS = 'watchers'
 
-    def __init__(self, base_url, api_token=None):
-        super().__init__(base_url.rstrip('/'))
+    def __init__(self, base_url, api_token=None, archive=None, from_archive=False, ssl_verify=True):
+        super().__init__(base_url.rstrip('/'), archive=archive, from_archive=from_archive, ssl_verify=ssl_verify)
         self.api_token = api_token
 
     def issues(self, from_date=DEFAULT_DATETIME,
                offset=None, max_issues=MAX_ISSUES):
         """Get the information of a list of issues.
 
         :param from_date: retrieve issues that where updated from that date;
@@ -472,14 +413,30 @@
 
         params = {}
 
         response = self._call(resource, params)
 
         return response
 
+    @staticmethod
+    def sanitize_for_archive(url, headers, payload):
+        """Sanitize payload of a HTTP request by removing the token information
+        before storing/retrieving archived items
+
+        :param: url: HTTP url request
+        :param: headers: HTTP headers request
+        :param: payload: HTTP payload request
+
+        :returns url, headers and the sanitized payload
+        """
+        if RedmineClient.PKEY in payload:
+            payload.pop(RedmineClient.PKEY)
+
+        return url, headers, payload
+
     def _call(self, resource, params):
         """Call to get a resource.
 
         :param method: resource to get
         :param params: dict with the HTTP parameters needed to get
             the given resource
         """
@@ -487,10 +444,10 @@
 
         if self.api_token:
             params[self.PKEY] = self.api_token
 
         logger.debug("Redmine client requests: %s params: %s",
                      resource, str(params))
 
-        r = self.fetch(url, payload=params, verify=False)
+        r = self.fetch(url, payload=params)
 
         return r.text
```

### Comparing `perceval-0.9.9/perceval/backends/core/mediawiki.py` & `perceval-1.0.0rc1/perceval/backends/core/mediawiki.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2016-2017 Bitergia
+# Copyright (C) 2015-2020 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1335, USA.
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
+#     Santiago Dueñas <sduenas@bitergia.com>
+#     Stephan Barth <stephan.barth@gmail.com>
 #     Alvaro del Castillo <acs@bitergia.com>
+#     Valerio Cosentino <valcos@bitergia.com>
+#     Jesus M. Gonzalez-Barahona <jgb@gsyc.es>
+#     Harshal Mittal <harshalmittal4@gmail.com>
 #
 
-import datetime
 import json
 import logging
 
 import dateutil
 
-from grimoirelab.toolkit.datetime import datetime_to_utc, str_to_datetime
-from grimoirelab.toolkit.uris import urijoin
+from grimoirelab_toolkit.datetime import (datetime_to_utc,
+                                          datetime_utcnow,
+                                          str_to_datetime)
+from grimoirelab_toolkit.uris import urijoin
 
 from ...backend import (Backend,
                         BackendCommand,
-                        BackendCommandArgumentParser,
-                        metadata)
+                        BackendCommandArgumentParser)
 from ...client import HttpClient
-from ...errors import BackendError, CacheError
+from ...errors import BackendError
 from ...utils import DEFAULT_DATETIME
 
+CATEGORY_PAGE = 'page'
 
 logger = logging.getLogger(__name__)
 
 MAX_RECENT_DAYS = 30  # max number of days included in MediaWiki recent changes
 
 
 class MediaWiki(Backend):
@@ -64,113 +69,82 @@
     The page and revisions data downloaded are the standard. More data could
     be gathered using additional properties.
 
     Deleted pages are not analyzed.
 
     :param url: MediaWiki url
     :param tag: label used to mark the data
-    :param cache: cache object to store raw data
+    :param archive: archive to store/retrieve items
+    :param ssl_verify: enable/disable SSL verification
     """
-    version = '0.6.0'
+    version = '1.0.0'
 
-    def __init__(self, url, tag=None, cache=None):
+    CATEGORIES = [CATEGORY_PAGE]
+
+    def __init__(self, url, tag=None, archive=None, ssl_verify=True):
         origin = url
 
-        super().__init__(origin, tag=tag, cache=cache)
+        super().__init__(origin, tag=tag, archive=archive, ssl_verify=ssl_verify)
         self.url = url
-        self.client = MediaWikiClient(url)
-        self._test_mode = False
+        self.client = None
 
-    @metadata
-    def fetch(self, from_date=DEFAULT_DATETIME, reviews_api=False):
+    def fetch(self, category=CATEGORY_PAGE, from_date=DEFAULT_DATETIME, reviews_api=False):
         """Fetch the pages from the backend url.
 
         The method retrieves, from a MediaWiki url, the
         wiki pages.
 
+        :param category: the category of items to fetch
+        :param from_date: obtain pages updated since this date
         :param reviews_api: use the reviews API available in MediaWiki >= 1.27
 
-
         :returns: a generator of pages
         """
-
-        self._purge_cache_queue()
-
         if from_date == DEFAULT_DATETIME:
             from_date = None
         else:
             from_date = datetime_to_utc(from_date)
 
+        kwargs = {"from_date": from_date, "reviews_api": reviews_api}
+        items = super().fetch(category, **kwargs)
+
+        return items
+
+    def fetch_items(self, category, **kwargs):
+        """Fetch the pages
+
+        :param category: the category of items to fetch
+        :param kwargs: backend arguments
+
+        :returns: a generator of items
+        """
+        from_date = kwargs['from_date']
+        reviews_api = kwargs['reviews_api']
+
         mediawiki_version = self.client.get_version()
         logger.info("MediaWiki version: %s", mediawiki_version)
-        self._push_cache_queue(json.dumps({"reviews_api": reviews_api}))
-        self._flush_cache_queue()
 
         if reviews_api:
-            if ((mediawiki_version[0] == 1 and mediawiki_version[1] >= 27) or
-                mediawiki_version[0] > 1):
+            if (mediawiki_version[0] == 1 and mediawiki_version[1] >= 27) or mediawiki_version[0] > 1:
                 fetcher = self.__fetch_1_27(from_date)
             else:
                 logger.warning("Reviews API only available in MediaWiki >= 1.27")
                 logger.warning("Using the Pages API instead")
                 fetcher = self.__fetch_pre1_27(from_date)
         else:
             fetcher = self.__fetch_pre1_27(from_date)
 
         for page_reviews in fetcher:
             yield page_reviews
 
-    @metadata
-    def fetch_from_cache(self):
-        """Fetch the pages from the cache.
-
-        :returns: a generator of pages
-
-        :raises CacheError: raised when an error occurs accessing the
-            cache
-        """
-        if not self.cache:
-            raise CacheError(cause="cache instance was not provided")
-
-        cache_items = self.cache.retrieve()
-
-        pages_dicts = ['allrevisions', 'allpages', 'recentchanges']
-        pages_done = []  # pages already retrieved in reviews API
-        reviews_api_json = json.loads(next(cache_items))
-        if 'reviews_api' not in reviews_api_json:
-            raise CacheError(cause="reviews_api not found at cache file start.")
-        reviews_api = reviews_api_json['reviews_api']
-
-        # pages -> revisions
-        for items in cache_items:
-            data_json = json.loads(items)
-            if 'reviews_api' in data_json:
-                # New perceval execution
-                reviews_api = data_json['reviews_api']
-                pages_done = []
-                continue
-            for pages_dict in pages_dicts:
-                if pages_dict in data_json['query']:
-                    pages_json = data_json['query'][pages_dict]
-                    for page in pages_json:
-                        if reviews_api:
-                            if page['pageid'] in pages_done:
-                                # The page was already returned for previous revisions
-                                continue
-                            pages_done.append(page['pageid'])
-                        page_reviews = self.__build_page_reviews(page, json.loads(next(cache_items)))
-                        if not page_reviews:
-                            continue
-                        yield page_reviews
-
     @classmethod
-    def has_caching(cls):
-        """Returns whether it supports caching items on the fetch process.
+    def has_archiving(cls):
+        """Returns whether it supports archiving items on the fetch process.
 
-        :returns: this backend supports items cache
+        :returns: this backend supports items archive
         """
         return True
 
     @classmethod
     def has_resuming(cls):
         """Returns whether it supports to resume the fetch process.
 
@@ -200,15 +174,20 @@
     @staticmethod
     def metadata_category(item):
         """Extracts the category from a MediaWiki item.
 
         This backend only generates one type of item which is
         'page'.
         """
-        return 'page'
+        return CATEGORY_PAGE
+
+    def _init_client(self, from_archive=False):
+        """Init client"""
+
+        return MediaWikiClient(self.url, self.archive, from_archive, self.ssl_verify)
 
     def __get_max_date(self, reviews):
         """"Get the max date in unixtime format from reviews."""
         max_ts = 0
         for review in reviews:
             ts = str_to_datetime(review['timestamp'])
             ts = datetime_to_utc(ts)
@@ -232,45 +211,48 @@
         wiki pages.
 
         :returns: a generator of pages
         """
 
         logger.info("Looking for pages at url '%s'", self.url)
 
-        self._purge_cache_queue()
         npages = 0  # number of pages processed
+        tpages = 0  # number of total pages
         pages_done = []  # pages already retrieved in reviews API
 
         namespaces_contents = self.__get_namespaces_contents()
 
         arvcontinue = ''  # pagination for getting revisions and their pages
         while arvcontinue is not None:
             raw_pages = self.client.get_pages_from_allrevisions(namespaces_contents, from_date, arvcontinue)
-            self._push_cache_queue(raw_pages)
             data_json = json.loads(raw_pages)
-            if 'continue' in data_json:
-                arvcontinue = data_json['continue']['arvcontinue']
-            else:
-                arvcontinue = None
+            arvcontinue = data_json['continue']['arvcontinue'] if 'continue' in data_json else None
             pages_json = data_json['query']['allrevisions']
             for page in pages_json:
+
                 if page['pageid'] in pages_done:
-                    # The page was already returned for previous revisions
+                    logger.debug("Page %s already processed; skipped", page['pageid'])
                     continue
+
+                tpages += 1
                 pages_done.append(page['pageid'])
-                yield self.__get_page_reviews(page)
+                page_reviews = self.__get_page_reviews(page)
+
+                if not page_reviews:
+                    logger.warning("Revisions not found in %s [page id: %s], page skipped",
+                                   page['title'], page['pageid'])
+                    continue
+
+                yield page_reviews
                 npages += 1
-            self._flush_cache_queue()
 
-        logger.info("Total number of pages: %i", npages)
+        logger.info("Total number of pages: %i, skipped %i", tpages, tpages - npages)
 
     def __get_page_reviews(self, page):
-        revisions_raw = self.client.get_revisions(page['title'])
-        self._push_cache_queue(revisions_raw)
-        self._flush_cache_queue()
+        revisions_raw = self.client.get_revisions(page['pageid'])
         page_reviews = self.__build_page_reviews(page, json.loads(revisions_raw))
         return page_reviews
 
     def __fetch_pre1_27(self, from_date=None):
         """Fetch the pages from the backend url.
 
         The method retrieves, from a MediaWiki url, the
@@ -278,87 +260,115 @@
 
         :returns: a generator of pages
         """
 
         def fetch_incremental_changes(namespaces_contents):
             # Use recent changes API to get the pages from date
             npages = 0  # number of pages processed
+            tpages = 0  # number of total pages
+            pages_done = []  # pages already retrieved in reviews API
+
             rccontinue = ''
             hole_created = True  # To detect that incremental is not complete
             while rccontinue is not None:
                 raw_pages = self.client.get_recent_pages(namespaces_contents, rccontinue)
-                self._push_cache_queue(raw_pages)
-                self._flush_cache_queue()
                 data_json = json.loads(raw_pages)
+
                 if 'query-continue' in data_json:
                     # < 1.27
                     rccontinue = data_json['query-continue']['recentchanges']['rccontinue']
                 elif 'continue' in data_json:
                     # >= 1.27
                     rccontinue = data_json['continue']['rccontinue']
                 else:
                     rccontinue = None
+
                 pages_json = data_json['query']['recentchanges']
                 for page in pages_json:
+
                     page_ts = dateutil.parser.parse(page['timestamp'])
                     if from_date >= page_ts:
                         # The rest of recent changes are older than from_date
                         logger.debug("All recent changes newer than %s processed.", from_date)
                         rccontinue = None
                         hole_created = False
                         break
+
+                    if 'pageid' not in page:
+                        logger.warning("Missing pageid in page %s; skipped", page)
+                        continue
+
+                    if page['pageid'] in pages_done:
+                        logger.debug("Page %s already processed; skipped", page['pageid'])
+                        continue
+
+                    tpages += 1
+                    pages_done.append(page['pageid'])
                     page_reviews = self.__get_page_reviews(page)
+
                     if not page_reviews:
-                        # Page without reviews are not managed
+                        logger.warning("Revisions not found in %s [page id: %s], page skipped",
+                                       page['title'], page['pageid'])
                         continue
+
                     yield page_reviews
                     npages += 1
             if hole_created:
                 logger.error("Incremental update NOT completed. Hole in history created.")
-            logger.info("Total number of pages: %i", npages)
+            logger.info("Total number of pages: %i, skipped %i", tpages, tpages - npages)
 
         def fetch_all_pages(namespaces_contents):
             # Use get all pages API to get pages
             npages = 0  # number of pages processed
+            tpages = 0  # number of total pages
+            pages_done = []  # pages already retrieved in reviews API
 
             for ns in namespaces_contents:
                 apcontinue = ''  # pagination for getting pages
                 logger.debug("Getting pages for namespace: %s", ns)
                 while apcontinue is not None:
                     raw_pages = self.client.get_pages(ns, apcontinue)
-                    self._push_cache_queue(raw_pages)
-                    self._flush_cache_queue()
                     data_json = json.loads(raw_pages)
                     if 'query-continue' in data_json:
                         # < 1.27
                         apcontinue = data_json['query-continue']['allpages']['apcontinue']
                     elif 'continue' in data_json:
                         # >= 1.27
                         apcontinue = data_json['continue']['apcontinue']
                     else:
                         apcontinue = None
                     pages_json = data_json['query']['allpages']
                     for page in pages_json:
-                        yield self.__get_page_reviews(page)
+
+                        if page['pageid'] in pages_done:
+                            logger.debug("Page %s already processed; skipped", page['pageid'])
+                            continue
+
+                        tpages += 1
+                        pages_done.append(page['pageid'])
+                        page_reviews = self.__get_page_reviews(page)
+
+                        if not page_reviews:
+                            logger.warning("Revisions not found in %s [page id: %s], page skipped",
+                                           page['title'], page['pageid'])
+                            continue
+
+                        yield page_reviews
                         npages += 1
-            logger.info("Total number of pages: %i", npages)
+            logger.info("Total number of pages: %i, skipped %i", tpages, tpages - npages)
 
         logger.info("Looking for pages at url '%s'", self.url)
 
         # from_date can not be older than MAX_RECENT_DAYS days ago
         if from_date:
-            if self._test_mode:
-                logger.warning("Test mode active; MAX_RECENT_DAYS limit ignored")
-            elif (datetime.datetime.now(dateutil.tz.tzlocal()) - from_date).days >= MAX_RECENT_DAYS:
+            if (datetime_utcnow() - from_date).days >= MAX_RECENT_DAYS:
                 cause = "Can't get incremental pages older than %i days." % MAX_RECENT_DAYS
                 cause += " Do a complete analysis without from_date for older changes."
                 raise BackendError(cause=cause)
 
-        self._purge_cache_queue()
-
         namespaces_contents = self.__get_namespaces_contents()
 
         if not from_date:
             return fetch_all_pages(namespaces_contents)
         else:
             return fetch_incremental_changes(namespaces_contents)
 
@@ -366,34 +376,76 @@
         page['revisions'] = None
         page['update'] = None
         if str(page["pageid"]) in reviews["query"]["pages"]:
             reviews_json = reviews["query"]["pages"][str(page["pageid"])]
             if 'revisions' in reviews_json:
                 page["revisions"] = reviews_json['revisions']
                 page['update'] = self.__get_max_date(page['revisions'])
+            else:
+                page = None
         else:
-            logger.warning("Revisions not found in %s", reviews["query"]["pages"])
-            logger.warning("for page: %s", page)
+            logger.warning("Revisions not found in %s [page id: %s], page skipped",
+                           page['title'], page['pageid'])
             page = None
         return page
 
 
 class MediaWikiClient(HttpClient):
     """MediaWiki API client.
 
     This class implements a simple client to retrieve pages from
     projects in a MediaWiki node.
 
     :param url: URL of mediawiki site: https://wiki.mozilla.org
+    :param archive: an archive to store/retrieved the fetched data
+    :param from_archive: define whether the archive is used to store/read data
+    :param ssl_verify: enable/disable SSL verification
 
     :raises HTTPError: when an error occurs doing the request
     """
+    # Resource parameters
+    PACTION = "action"
+    PMETA = "meta"
+    PSIPROP = "siprop"
+    PFORMAT = "format"
+    PLIST = "list"
+    PAP_LIMIT = "aplimit"
+    PAP_NAMESPACE = "apnamespace"
+    PAP_CONTINUE = "apcontinue"
+    PRC_LIMIT = "rclimit"
+    PRC_NAMESPACE = "rcnamespace"
+    PRC_PROP = "rcprop"
+    PRC_CONTINUE = "rccontinue"
+    PPROP = "prop"
+    PPAGE_IDS = "pageids"
+    PRV_DIR = "rvdir"
+    PRV_LIMIT = "rvlimit"
+    PRV_START = "rvstart"
+    PARV_NAMESPACE = "arvnamespace"
+    PARV_DIR = "arvdir"
+    PARV_LIMIT = "arvlimit"
+    PARV_PROP = "arvprop"
+    PARV_CONTINUE = "arvcontinue"
+    PARV_START = "arvstart"
+
+    # Predefined values
+    VQUERY = "query"
+    VSITE_INFO = "siteinfo"
+    VNAMESPACES = "namespaces"
+    VJSON = "json"
+    VALL_PAGES = "allpages"
+    VRECENT_CHANGES = "recentchanges"
+    VRC_PROP = "title|timestamp|ids"
+    VREVISIONS = "revisions"
+    VNEWER = "newer"
+    VALL_REVISIONS = "allrevisions"
+    VIDS = "ids"
 
-    def __init__(self, url):
-        super().__init__(urijoin(url, "api.php"))
+    def __init__(self, url, archive=None, from_archive=False, ssl_verify=True):
+        super().__init__(urijoin(url, "api.php"), archive=archive, from_archive=from_archive, ssl_verify=ssl_verify)
         self.limit = "max"  # Always get the max number of items
 
     def call(self, params):
         """Run an API command.
         :param cgi: cgi command to run on the server
         :param params: dict with the HTTP parameters needed to run
             the given command
@@ -404,133 +456,137 @@
         req = self.fetch(self.base_url, payload=params)
         return req.text
 
     def get_namespaces(self):
         """ Retrieve all contents namespaces."""
 
         params = {
-            "action": "query",
-            "meta": "siteinfo",
-            "siprop": "namespaces",
-            "format": "json"
+            self.PACTION: self.VQUERY,
+            self.PMETA: self.VSITE_INFO,
+            self.PSIPROP: self.VNAMESPACES,
+            self.PFORMAT: self.VJSON
         }
 
         return self.call(params)
 
     def get_version(self):
         params = {
-            "action": "query",
-            "meta": "siteinfo",
-            "format": "json"
+            self.PACTION: self.VQUERY,
+            self.PMETA: self.VSITE_INFO,
+            self.PFORMAT: self.VJSON
         }
 
         try:
             res = self.call(params)
             siteinfo = json.loads(res)
             siteinfo = siteinfo["query"]["general"]
-        except Exception:
-            logger.error(res)
+        except Exception as ex:
+            logger.error(ex)
             cause = "Wrong MediaWiki API: " + self.base_url
             raise BackendError(cause=cause)
 
         version = siteinfo['generator']
         # MediaWiki 1.28.0-wmf.7, MediaWiki 1.19alpha
         version = version.split(" ")[1]  # Removes MediaWiki
         version_major = int(version.split(".")[0])
         version_minor = int(version.split(".")[1][0:2])
 
         return [version_major, version_minor]
 
     def get_pages(self, namespace, apcontinue=''):
         """Retrieve all pages from a namespace starting from apcontinue."""
         params = {
-            "action": "query",
-            "list": "allpages",
-            "aplimit": self.limit,
-            "apnamespace": namespace,
-            "format": "json"
+            self.PACTION: self.VQUERY,
+            self.PLIST: self.VALL_PAGES,
+            self.PAP_LIMIT: self.limit,
+            self.PAP_NAMESPACE: namespace,
+            self.PFORMAT: self.VJSON
         }
         if apcontinue:
-            params['apcontinue'] = apcontinue
+            params[self.PAP_CONTINUE] = apcontinue
 
         return self.call(params)
 
     def get_recent_pages(self, namespaces, rccontinue=''):
         """Retrieve recent pages from all namespaces starting from rccontinue."""
 
+        namespaces.sort()
         params = {
-            "action": "query",
-            "list": "recentchanges",
-            "rclimit": self.limit,
-            "rcnamespace": "|".join(namespaces),
-            "rcprop": "title|timestamp|ids",
-            "format": "json"
+            self.PACTION: self.VQUERY,
+            self.PLIST: self.VRECENT_CHANGES,
+            self.PRC_LIMIT: self.limit,
+            self.PRC_NAMESPACE: "|".join(namespaces),
+            self.PRC_PROP: self.VRC_PROP,
+            self.PFORMAT: self.VJSON
         }
         if rccontinue:
-            params['rccontinue'] = rccontinue
+            params[self.PRC_CONTINUE] = rccontinue
 
         return self.call(params)
 
-    def get_revisions(self, title, last_date=None):
+    def get_revisions(self, pageid, last_date=None):
         # TODO: Iterate if more than self.max reviews (500)
 
         if last_date:
             last_date_str = last_date.isoformat()
 
         params = {
-            "action": "query",
-            "prop": "revisions",
-            "titles": title,
-            "rvdir": "newer",
-            "rvlimit": self.limit,
-            "format": "json"
+            self.PACTION: self.VQUERY,
+            self.PPROP: self.VREVISIONS,
+            self.PPAGE_IDS: pageid,
+            self.PRV_DIR: self.VNEWER,
+            self.PRV_LIMIT: self.limit,
+            self.PFORMAT: self.VJSON
         }
         if last_date:
-            params['rvstart'] = last_date_str
+            params[self.PRV_START] = last_date_str
 
         return self.call(params)
 
     def get_pages_from_allrevisions(self, namespaces, from_date=None, arvcontinue=None):
 
         if from_date:
             if from_date.tzinfo != dateutil.tz.tzutc():
                 raise ValueError("Datetime is not in UTC timezone")
 
             from_date_str = from_date.strftime("%Y-%m-%dT%H:%M:%SZ")
 
+        namespaces.sort()
         params = {
-            "action": "query",
-            "list": "allrevisions",
-            "arvnamespace": "|".join(namespaces),
-            "arvdir": "newer",
-            "arvlimit": self.limit,
-            "arvprop": "ids",
-            "format": "json"
+            self.PACTION: self.VQUERY,
+            self.PLIST: self.VALL_REVISIONS,
+            self.PARV_NAMESPACE: "|".join(namespaces),
+            self.PARV_DIR: self.VNEWER,
+            self.PARV_LIMIT: self.limit,
+            self.PARV_PROP: self.VIDS,
+            self.PFORMAT: self.VJSON
         }
 
         if arvcontinue:
-            params['arvcontinue'] = arvcontinue
+            params[self.PARV_CONTINUE] = arvcontinue
         else:
             if from_date:
-                params['arvstart'] = from_date_str
+                params[self.PARV_START] = from_date_str
 
         return self.call(params)
 
 
 class MediaWikiCommand(BackendCommand):
     """Class to run MediaWiki backend from the command line."""
 
     BACKEND = MediaWiki
 
-    @staticmethod
-    def setup_cmd_parser():
+    @classmethod
+    def setup_cmd_parser(cls):
         """Returns the MediaWiki argument parser."""
 
-        parser = BackendCommandArgumentParser(from_date=True,
-                                              cache=True)
+        parser = BackendCommandArgumentParser(cls.BACKEND,
+                                              from_date=True,
+                                              archive=True,
+                                              ssl_verify=True)
 
         # MediaWiki options
         group = parser.parser.add_argument_group('MediaWiki arguments')
         group.add_argument('--reviews-api', action='store_true',
                            help="Use the experimental Reviews API in MediaWiki >= 1.27")
 
         # Required arguments
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `perceval-0.9.9/perceval/backends/__init__.py` & `perceval-1.0.0rc1/perceval/backends/core/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2017 Bitergia
+# Copyright (C) 2015-2020 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1335, USA.
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #     Santiago Dueñas <sduenas@bitergia.com>
+#     Jesus M. Gonzalez-Barahona <jgb@gsyc.es>
+#     Valerio Cosentino <valcos@bitergia.com>
 #
 
-__import__('pkg_resources').declare_namespace(__name__)
+from ..._version import __version__
+
+__version__ = __version__
```

### Comparing `perceval-0.9.9/perceval/client.py` & `perceval-1.0.0rc1/perceval/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2017 Bitergia
+# Copyright (C) 2015-2020 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1335, USA.
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #     Valerio Cosentino <valcos@bitergia.com>
+#     Santiago Dueñas <sduenas@bitergia.com>
 #
 
 import logging
 import time
 
 import requests
 import urllib3.util
@@ -46,18 +46,28 @@
     To track which version of the client was used during
     the fetching process, this class provides a `version`
     attribute that each client may override.
 
     :param base_url: base URL of the data source
     :param max_retries: number of max retries to a data source
         before raising a RetryError exception
-    :param default_sleep_time: default time to sleep in case
+    :param sleep_time: time (in seconds) to sleep in case
         of connection problems
+    :param extra_headers: extra headers to be included in
+        the requests
+    :param extra_status_forcelist: a set of HTTP status codes that will
+        force a retry on
+    :param extra_retry_after_status: a set of HTTP status codes that will
+        perform a retry respecting the Retry-After header
+    :param archive: archive to store/retrieve items
+    :param from_archive: if `True` the data is fetched
+        from an archive
+    :param ssl_verify: enable/disable SSL verification
     """
-    version = '0.1.1'
+    version = '0.3.0'
 
     DEFAULT_SLEEP_TIME = 1
 
     MAX_RETRIES = 5
     MAX_RETRIES_ON_CONNECT = 5
     MAX_RETRIES_ON_READ = 5
     MAX_RETRIES_ON_REDIRECT = 5
@@ -72,18 +82,20 @@
     DEFAULT_STATUS_FORCE_LIST = [408, 423, 504]
 
     DEFAULT_HEADERS = {'User-Agent': 'Perceval/' + __version__}
 
     GET = "GET"
     POST = "POST"
 
-    def __init__(self, base_url, max_retries=MAX_RETRIES, default_sleep_time=DEFAULT_SLEEP_TIME,
-                 extra_headers=None, extra_status_forcelist=None, extra_retry_after_status=None):
+    def __init__(self, base_url, max_retries=MAX_RETRIES, sleep_time=DEFAULT_SLEEP_TIME,
+                 extra_headers=None, extra_status_forcelist=None, extra_retry_after_status=None,
+                 archive=None, from_archive=False, ssl_verify=True):
 
         self.base_url = base_url
+        self.ssl_verify = ssl_verify
 
         self.headers = dict(self.DEFAULT_HEADERS)
         if extra_headers:
             self.headers.update(extra_headers)
 
         self.status_forcelist = list(self.DEFAULT_STATUS_FORCE_LIST)
         if extra_status_forcelist:
@@ -99,41 +111,87 @@
         self.max_retries_on_redirect = self.MAX_RETRIES_ON_REDIRECT
         self.max_retries_on_status = self.MAX_RETRIES_ON_STATUS
 
         self.method_whitelist = self.DEFAULT_METHOD_WHITELIST
         self.raise_on_redirect = self.DEFAULT_RAISE_ON_REDIRECT
         self.raise_on_status = self.DEFAULT_RAISE_ON_STATUS
         self.respect_retry_after_header = self.DEFAULT_RESPECT_RETRY_AFTER_HEADER
-        self.default_sleep_time = default_sleep_time
+        self.sleep_time = sleep_time
+
+        self.archive = archive
+        self.from_archive = from_archive
 
         self._create_http_session()
 
     def __del__(self):
         self._close_http_session()
 
-    def fetch(self, url, payload=None, headers=None, method=GET, stream=False, verify=True):
+    def fetch(self, url, payload=None, headers=None, method=GET, stream=False, auth=None):
         """Fetch the data from a given URL.
 
         :param url: link to the resource
         :param payload: payload of the request
         :param headers: headers of the request
         :param method: type of request call (GET or POST)
         :param stream: defer downloading the response body until the response content is available
-        :param verify: verifying the SSL certificate
+        :param auth: auth of the request
 
         :returns a response object
         """
+        if self.from_archive:
+            response = self._fetch_from_archive(url, payload, headers)
+        else:
+            response = self._fetch_from_remote(url, payload, headers, method, stream, auth)
+
+        return response
+
+    @staticmethod
+    def sanitize_for_archive(url, headers, payload):
+        """Sanitize the URL, headers and payload of a HTTP request before storing/retrieving items.
+        By default, this method does not modify url, headers and payload. The modifications take
+        place within the specific backends that redefine the sanitize_for_archive.
+
+        :param: url: HTTP url request
+        :param: headers: HTTP headers request
+        :param: payload: HTTP payload request
+
+        :returns url, headers and payload sanitized
+        """
+        return url, headers, payload
+
+    def _fetch_from_archive(self, url, payload, headers):
+
+        url, headers, payload = self.sanitize_for_archive(url, headers, payload)
+        response = self.archive.retrieve(url, payload, headers)
+
+        if not isinstance(response, requests.Response):
+            raise response
+
+        return response
+
+    def _fetch_from_remote(self, url, payload, headers, method, stream, auth):
 
         if method == self.GET:
-            response = self.session.get(url, params=payload, headers=headers, stream=stream, verify=verify)
+            response = self.session.get(url, params=payload, headers=headers, stream=stream,
+                                        verify=self.ssl_verify, auth=auth)
         else:
-            response = self.session.post(url, data=payload, headers=headers, stream=stream, verify=verify)
-
-        response.raise_for_status()
+            response = self.session.post(url, data=payload, headers=headers, stream=stream,
+                                         verify=self.ssl_verify, auth=auth)
 
+        try:
+            response.raise_for_status()
+        except Exception as e:
+            if self.archive:
+                url, headers, payload = self.sanitize_for_archive(url, headers, payload)
+                self.archive.store(url, payload, headers, e)
+            raise e
+
+        if self.archive:
+            url, headers, payload = self.sanitize_for_archive(url, headers, payload)
+            self.archive.store(url, payload, headers, response)
         return response
 
     def _create_http_session(self):
         """Create a http session and initialize the retry object."""
 
         self.session = requests.Session()
 
@@ -141,17 +199,17 @@
             self.session.headers.update(self.headers)
 
         retries = urllib3.util.Retry(total=self.max_retries,
                                      connect=self.max_retries_on_connect,
                                      read=self.max_retries_on_read,
                                      redirect=self.max_retries_on_redirect,
                                      status=self.max_retries_on_status,
-                                     method_whitelist=self.method_whitelist,
+                                     allowed_methods=self.method_whitelist,
                                      status_forcelist=self.status_forcelist,
-                                     backoff_factor=self.default_sleep_time,
+                                     backoff_factor=self.sleep_time,
                                      raise_on_redirect=self.raise_on_redirect,
                                      raise_on_status=self.raise_on_status,
                                      respect_retry_after_header=self.respect_retry_after_header)
 
         self.session.mount('http://', requests.adapters.HTTPAdapter(max_retries=retries))
         self.session.mount('https://', requests.adapters.HTTPAdapter(max_retries=retries))
 
@@ -166,15 +224,15 @@
     """Class to handle rate limit for HTTP clients.
 
     :param sleep_for_rate: sleep until rate limit is reset
     :param min_rate_to_sleep: minimun rate needed to sleep until it will be rese
     :param rate_limit_header: header to know the current rate limit
     :param rate_limit_reset_header: header to know the next rate limit reset
     """
-    version = '0.1'
+    version = '0.2'
 
     MIN_RATE_LIMIT = 10
     MAX_RATE_LIMIT = 500
     RATE_LIMIT_HEADER = "X-RateLimit-Remaining"
     RATE_LIMIT_RESET_HEADER = "X-RateLimit-Reset"
 
     def setup_rate_limit_handler(self, sleep_for_rate=False, min_rate_to_sleep=MIN_RATE_LIMIT,
@@ -204,36 +262,41 @@
 
     def sleep_for_rate_limit(self):
         """The fetching process sleeps until the rate limit is restored or
            raises a RateLimitError exception if sleep_for_rate flag is disabled.
         """
         if self.rate_limit is not None and self.rate_limit <= self.min_rate_to_sleep:
             seconds_to_reset = self.calculate_time_to_reset()
+
+            if seconds_to_reset < 0:
+                logger.warning("Value of sleep for rate limit is negative, reset it to 0")
+                seconds_to_reset = 0
+
             cause = "Rate limit exhausted."
             if self.sleep_for_rate:
                 logger.info("%s Waiting %i secs for rate limit reset.", cause, seconds_to_reset)
                 time.sleep(seconds_to_reset)
             else:
                 raise RateLimitError(cause=cause, seconds_to_reset=seconds_to_reset)
 
     def calculate_time_to_reset(self):
         """Calculate the seconds to reset the token requests."""
 
         raise NotImplementedError
 
     def update_rate_limit(self, response):
-        """Update the rate limit and the time to reset the rate limit
-           from the response headers.
+        """Update the rate limit and the time to reset
+        from the response headers.
 
         :param: response: the response object
         """
         if self.rate_limit_header in response.headers:
             self.rate_limit = int(response.headers[self.rate_limit_header])
             logger.debug("Rate limit: %s", self.rate_limit)
         else:
             self.rate_limit = None
 
         if self.rate_limit_reset_header in response.headers:
             self.rate_limit_reset_ts = int(response.headers[self.rate_limit_reset_header])
-            logger.debug("Rate limit reset: %s", self.rate_limit_reset_ts)
+            logger.debug("Rate limit reset: %s", self.calculate_time_to_reset())
         else:
             self.rate_limit_reset_ts = None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `perceval-0.9.9/perceval/errors.py` & `perceval-1.0.0rc1/perceval/errors.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2017 Bitergia
+# Copyright (C) 2015-2020 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1335, USA.
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #     Santiago Dueñas <sduenas@bitergia.com>
+#     Stephan Barth <stephan.barth@gmail.com>
+#     Valerio Cosentino <valcos@bitergia.com>
 #
 
 
 class BaseError(Exception):
     """Base class for Perceval exceptions.
 
     Derived classes can overwrite the error message declaring ``message``
@@ -33,22 +34,28 @@
         super().__init__()
         self.msg = self.message % kwargs
 
     def __str__(self):
         return self.msg
 
 
-class BackendError(BaseError):
-    """Generic error for backends"""
+class ArchiveError(BaseError):
+    """Generic error for archive objects"""
+
+    message = "%(cause)s"
+
+
+class ArchiveManagerError(BaseError):
+    """Generic error for archive manager"""
 
     message = "%(cause)s"
 
 
-class CacheError(BaseError):
-    """Generic error for cache objects"""
+class BackendError(BaseError):
+    """Generic error for backends"""
 
     message = "%(cause)s"
 
 
 class HttpClientError(BaseError):
     """Generic error for HTTP Cient"""
 
@@ -75,7 +82,13 @@
         return self._seconds_to_reset
 
 
 class ParseError(BaseError):
     """Exception raised a parsing errors occurs"""
 
     message = "%(cause)s"
+
+
+class BackendCommandArgumentParserError(BaseError):
+    """Generic error for BackendCommandArgumentParser"""
+
+    message = "%(cause)s"
```

### Comparing `perceval-0.9.9/perceval/backend.py` & `perceval-1.0.0rc1/perceval/archive.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,455 +1,465 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2017 Bitergia
+# Copyright (C) 2015-2020 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1335, USA.
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
+#     Valerio Cosentino <valcos@bitergia.com>
 #     Santiago Dueñas <sduenas@bitergia.com>
+#     Jesus M. Gonzalez-Barahona <jgb@gsyc.es>
 #
 
-import argparse
-import functools
 import hashlib
-import importlib
 import json
-import pkgutil
-import sys
+import logging
+import os
+import pickle
+import sqlite3
+import uuid
 
-from datetime import datetime as dt
+from grimoirelab_toolkit.datetime import (datetime_utcnow,
+                                          datetime_to_utc,
+                                          str_to_datetime)
 
-from grimoirelab.toolkit.introspect import find_signature_parameters
-from grimoirelab.toolkit.datetime import str_to_datetime
+from .errors import ArchiveError, ArchiveManagerError
 
-from ._version import __version__
-from .cache import Cache, setup_cache
-from .utils import DEFAULT_DATETIME
 
+logger = logging.getLogger(__name__)
 
-class Backend:
-    """Abstract class for backends.
 
-    Base class to fetch data from a repository. This repository
-    will be named as 'origin'. During the initialization, a `Cache`
-    object can be provided for caching raw data from the repositories.
+class Archive:
+    """Basic class for archiving raw items fetched by Perceval.
 
-    Derivated classes have to implement `fetch`, `fetch_from_cache`,
-    `has_caching` and `has_resuming` methods. Otherwise, `NotImplementedError`
-    exception will be raised. Metadata decorator can be used together with
-    fetch methods but requires the implementation of `metadata_id`,
-    `metadata_updated_on` and `metadata_category` static methods.
+    This class allows to archive raw items - usually HTML pages or
+    JSON documents - for a further recovery. These raw items will
+    be fetched, stored and retrieved back by a backend.
 
-    The fetched items can be tagged using the `tag` parameter. It will
-    be useful to trace data. When it is set to `None` or to an empty
-    string, the tag will be the same that the `origin` attribute.
+    Each stored item will have a hash code used as unique identifier.
+    Hash codes are generated using URIs and other parameters needed
+    to fetch raw items.
 
-    To track which version of the backend was used during the fetching
-    process, this class provides a `version` attribute that each backend
-    may override.
+    When an instance of `Archive` is initialized it will expect
+    to access an existing archive file. To create a new and empty
+    archive used `create` class method instead. Metadata must be
+    initialized calling to `init_metadata` method after creating
+    a new archive.
 
-    :param origin: identifier of the repository
-    :param tag: tag items using this label
-    :param cache: object to cache raw data
+    :param archive_path: path where this archive is stored
 
-    :raises ValueError: raised when `cache` is not an instance of
-        `Cache` class
+    :raises ArchiveError: when the archive does not exist or is invalid
     """
-    version = '0.5'
 
-    def __init__(self, origin, tag=None, cache=None):
-        self._origin = origin
-        self.tag = tag if tag else origin
-        self.cache = cache or None
-        self.cache_queue = []
-
-    @property
-    def origin(self):
-        return self._origin
-
-    @property
-    def cache(self):
-        return self._cache
-
-    @cache.setter
-    def cache(self, obj):
-        if obj and not isinstance(obj, Cache):
-            msg = "obj is not an instance of Cache. %s object given" \
-                % (str(type(obj)))
-            raise ValueError(msg)
+    ARCHIVE_TABLE = "archive"
+    METADATA_TABLE = "metadata"
 
-        self._cache = obj
+    # Table structure
+    ARCHIVE_CREATE_STMT = "CREATE TABLE " + ARCHIVE_TABLE + " ( " \
+                          "id INTEGER PRIMARY KEY AUTOINCREMENT, " \
+                          "hashcode VARCHAR(256) UNIQUE NOT NULL, " \
+                          "uri TEXT, " \
+                          "payload BLOB, " \
+                          "headers BLOB, " \
+                          "data BLOB)"
+
+    METADATA_CREATE_STMT = "CREATE TABLE " + METADATA_TABLE + " ( " \
+                           "origin TEXT, " \
+                           "backend_name TEXT, " \
+                           "backend_version TEXT, " \
+                           "category TEXT, " \
+                           "backend_params BLOB, " \
+                           "created_on TEXT)"
+
+    def __init__(self, archive_path):
+        if not os.path.exists(archive_path):
+            raise ArchiveError(cause="archive %s does not exist" % (archive_path))
+
+        self.archive_path = archive_path
+        self.origin = None
+        self.backend_name = None
+        self.backend_version = None
+        self.category = None
+        self.backend_params = None
+        self.created_on = None
+
+        self._db = sqlite3.connect(self.archive_path)
+
+        self._verify_archive()
+        self._load_metadata()
+
+    def __del__(self):
+        conn = getattr(self, '_db', None)
+        if conn:
+            conn.close()
+
+    def init_metadata(self, origin, backend_name, backend_version,
+                      category, backend_params):
+        """Init metadata information.
+
+        Metatada is composed by basic information needed to identify
+        where archived data came from and how it can be retrieved
+        and built into Perceval items.
+
+        :param: origin: identifier of the repository
+        :param: backend_name: name of the backend
+        :param: backend_version: version of the backend
+        :param: category: category of the items fetched
+        :param: backend_params: dict representation of the fetch parameters
 
-    def fetch(self, from_date=DEFAULT_DATETIME):
-        raise NotImplementedError
-
-    def fetch_from_cache(self):
-        raise NotImplementedError
-
-    @classmethod
-    def has_caching(cls):
-        raise NotImplementedError
-
-    @classmethod
-    def has_resuming(cls):
-        raise NotImplementedError
-
-    @staticmethod
-    def metadata_id(item):
-        raise NotImplementedError
+        raises ArchiveError: when an error occurs initializing the metadata
+        """
+        created_on = datetime_to_utc(datetime_utcnow())
+        created_on_dumped = created_on.isoformat()
+        backend_params_dumped = pickle.dumps(backend_params, 0)
 
-    @staticmethod
-    def metadata_updated_on(item):
-        raise NotImplementedError
+        metadata = (origin, backend_name, backend_version, category,
+                    backend_params_dumped, created_on_dumped,)
 
-    @staticmethod
-    def metadata_category(item):
-        raise NotImplementedError
+        try:
+            cursor = self._db.cursor()
+            insert_stmt = "INSERT INTO " + self.METADATA_TABLE + " "\
+                          "(origin, backend_name, backend_version, " \
+                          "category, backend_params, created_on) " \
+                          "VALUES (?, ?, ?, ?, ?, ?)"
+            cursor.execute(insert_stmt, metadata)
+
+            self._db.commit()
+            cursor.close()
+        except sqlite3.DatabaseError as e:
+            msg = "metadata initialization error; cause: %s" % str(e)
+            raise ArchiveError(cause=msg)
+
+        self.origin = origin
+        self.backend_name = backend_name
+        self.backend_version = backend_version
+        self.category = category
+        self.backend_params = backend_params
+        self.created_on = created_on
+
+        logger.debug("Metadata of archive %s initialized to %s",
+                     self.archive_path, metadata)
+
+    def store(self, uri, payload, headers, data):
+        """Store a raw item in this archive.
+
+        The method will store `data` content in this archive. The unique
+        identifier for that item will be generated using the rest of the
+        parameters.
+
+        :param uri: request URI
+        :param payload: request payload
+        :param headers: request headers
+        :param data: data to store in this archive
 
-    def _purge_cache_queue(self):
-        self.cache_queue = []
+        :raises ArchiveError: when an error occurs storing the given data
+        """
+        hashcode = self.make_hashcode(uri, payload, headers)
+        payload_dump = pickle.dumps(payload, 0)
+        headers_dump = pickle.dumps(headers, 0)
+        data_dump = pickle.dumps(data, 0)
 
-    def _flush_cache_queue(self):
-        if not self.cache:
-            return
-        self.cache.store(*self.cache_queue)
-        self._purge_cache_queue()
-
-    def _push_cache_queue(self, item):
-        if not self.cache:
-            return
-        self.cache_queue.append(item)
-
-
-class BackendCommandArgumentParser:
-    """Manage and parse backend command arguments.
-
-    This class defines and parses a set of arguments common to
-    backends commands. Some parameters like cache or the different
-    types of authentication can be set during the initialization
-    of the instance.
-
-    :param from_date: set from_date argument
-    :param to_date: set to_date argument
-    :param offset: set offset argument
-    :param basic_auth: set basic authentication arguments
-    :param token_auth: set token/key authentication arguments
-    :param cache: set caching arguments
-    :param aliases: define aliases for parsed arguments
+        logger.debug("Archiving %s with %s %s %s in %s",
+                     hashcode, uri, payload, headers, self.archive_path)
 
-    :raises AttributeArror: when both `from_date` and `offset` are set
-        to `True`
-    """
-    def __init__(self, from_date=False, to_date=False, offset=False,
-                 basic_auth=False, token_auth=False,
-                 cache=False, aliases=None):
-        self._from_date = from_date
-        self._to_date = to_date
-        self._cache = cache
-
-        self.aliases = aliases or {}
-        self.parser = argparse.ArgumentParser()
-
-        group = self.parser.add_argument_group('general arguments')
-        group.add_argument('--tag', dest='tag',
-                           help="tag the items generated during the fetching process")
-
-        if (from_date or to_date) and offset:
-            raise AttributeError("date and offset parameters are incompatible")
-
-        if from_date:
-            group.add_argument('--from-date', dest='from_date',
-                               default='1970-01-01',
-                               help="fetch items updated since this date")
-        if to_date:
-            group.add_argument('--to-date', dest='to_date',
-                               help="fetch items updated before this date")
-        if offset:
-            group.add_argument('--offset', dest='offset',
-                               type=int, default=0,
-                               help="offset to start fetching items")
-
-        if basic_auth or token_auth:
-            self._set_auth_arguments(basic_auth=basic_auth,
-                                     token_auth=token_auth)
-
-        if cache:
-            self._set_cache_arguments()
-
-        self._set_output_arguments()
-
-    def parse(self, *args):
-        """Parse a list of arguments.
-
-        Parse argument strings needed to run a backend command. The result
-        will be a `argparse.Namespace` object populated with the values
-        obtained after the validation of the parameters.
+        try:
+            cursor = self._db.cursor()
+            insert_stmt = "INSERT INTO " + self.ARCHIVE_TABLE + " (" \
+                          "id, hashcode, uri, payload, headers, data) " \
+                          "VALUES(?,?,?,?,?,?)"
+            cursor.execute(insert_stmt, (None, hashcode, uri,
+                                         payload_dump, headers_dump, data_dump))
+            self._db.commit()
+            cursor.close()
+        except sqlite3.IntegrityError as e:
+            msg = "data storage error; cause: duplicated entry %s" % hashcode
+            raise ArchiveError(cause=msg)
+        except sqlite3.DatabaseError as e:
+            msg = "data storage error; cause: %s" % str(e)
+            raise ArchiveError(cause=msg)
+
+        logger.debug("%s data archived in %s", hashcode, self.archive_path)
+
+    def retrieve(self, uri, payload, headers):
+        """Retrieve a raw item from the archive.
+
+        The method will return the `data` content corresponding to the
+        hascode derived from the given parameters.
+
+        :param uri: request URI
+        :param payload: request payload
+        :param headers: request headers
 
-        :param args: argument strings
+        :returns: the archived data
 
-        :result: an object with the parsed values
+        :raises ArchiveError: when an error occurs retrieving data
         """
-        parsed_args = self.parser.parse_args(args)
+        hashcode = self.make_hashcode(uri, payload, headers)
 
-        if self._from_date:
-            parsed_args.from_date = str_to_datetime(parsed_args.from_date)
-        if self._to_date and parsed_args.to_date:
-            parsed_args.to_date = str_to_datetime(parsed_args.to_date)
-
-        if self._cache and parsed_args.fetch_cache and parsed_args.no_cache:
-            raise AttributeError("fetch-cache and no-cache arguments are not compatible")
-
-        # Set aliases
-        for alias, arg in self.aliases.items():
-            if (alias not in parsed_args) and (arg in parsed_args):
-                value = getattr(parsed_args, arg, None)
-                setattr(parsed_args, alias, value)
-
-        return parsed_args
-
-    def _set_auth_arguments(self, basic_auth=True, token_auth=False):
-        """Activate authentication arguments parsing"""
-
-        group = self.parser.add_argument_group('authentication arguments')
-
-        if basic_auth:
-            group.add_argument('-u', '--backend-user', dest='user',
-                               help="backend user")
-            group.add_argument('-p', '--backend-password', dest='password',
-                               help="backend password")
-        if token_auth:
-            group.add_argument('-t', '--api-token', dest='api_token',
-                               help="backend authentication token / API key")
-
-    def _set_cache_arguments(self):
-        """Activate cache arguments parsing"""
-
-        group = self.parser.add_argument_group('cache arguments')
-        group.add_argument('--cache-path', dest='cache_path', default=None,
-                           help="directory path to the cache")
-        group.add_argument('--clean-cache', dest='clean_cache', action='store_true',
-                           help="clean the cache before the fetching process")
-        group.add_argument('--no-cache', dest='no_cache', action='store_true',
-                           help="do not store data in the cache")
-        group.add_argument('--fetch-cache', dest='fetch_cache', action='store_true',
-                           help="fetch data from the cache")
-
-    def _set_output_arguments(self):
-        """Activate output arguments parsing"""
-
-        group = self.parser.add_argument_group('output arguments')
-        group.add_argument('-o', '--output', type=argparse.FileType('w'),
-                           dest='outfile', default=sys.stdout,
-                           help="output file")
-
-
-class BackendCommand:
-    """Abstract class to run backends from the command line.
-
-    When the class is initialized, it parses the given arguments using
-    the defined argument parser on `setump_cmd_parser` method. Those
-    arguments will be stored in the attribute `parsed_args`.
-
-    The arguments will be used to inizialize and run the `Backend` object
-    assigned to this command. The backend used to run the command is stored
-    under `BACKEND` class attributed. Any class derived from this and must
-    set its own `Backend` class.
+        logger.debug("Retrieving entry %s with %s %s %s in %s",
+                     hashcode, uri, payload, headers, self.archive_path)
 
-    Moreover, the method `setup_cmd_parser` must be implemented to exectute
-    the backend.
-    """
-    BACKEND = None
-
-    def __init__(self, *args):
-        parser = self.setup_cmd_parser()
-        self.parsed_args = parser.parse(*args)
+        self._db.row_factory = sqlite3.Row
 
-        self._pre_init()
+        try:
+            cursor = self._db.cursor()
+            select_stmt = "SELECT data " \
+                          "FROM " + self.ARCHIVE_TABLE + " " \
+                          "WHERE hashcode = ?"
+            cursor.execute(select_stmt, (hashcode,))
+            row = cursor.fetchone()
+            cursor.close()
+        except sqlite3.DatabaseError as e:
+            msg = "data retrieval error; cause: %s" % str(e)
+            raise ArchiveError(cause=msg)
 
-        parsed_args = vars(self.parsed_args)
-        kw = find_signature_parameters(self.BACKEND.__init__, parsed_args)
-        self.backend = self.BACKEND(**kw)
-        self.backend.cache = self._initialize_cache()
+        if row:
+            found = pickle.loads(row['data'])
+        else:
+            msg = "entry %s not found in archive %s" % (hashcode, self.archive_path)
+            raise ArchiveError(cause=msg)
 
-        self._post_init()
+        return found
 
-        self.outfile = self.parsed_args.outfile
+    @classmethod
+    def create(cls, archive_path):
+        """Create a brand new archive.
 
-    def run(self):
-        """Fetch and write items.
+         Call this method to create a new and empty archive. It will initialize
+         the storage file in the path defined by `archive_path`.
 
-        This method runs the backend to fetch the items from the given
-        origin. Items are converted to JSON objects and written to the
-        defined output.
+        :param archive_path: absolute path where the archive file will be created
 
-        If `fetch-cache` parameter was given as an argument during
-        the inizialization of the instance, the items will be retrieved
-        from the cache.
+        :raises ArchiveError: when the archive file already exists
         """
-        if self.backend.cache and self.parsed_args.fetch_cache:
-            fetch = self.backend.fetch_from_cache
-        else:
-            fetch = self.backend.fetch
+        if os.path.exists(archive_path):
+            msg = "archive %s already exists; remove it before creating a new one"
+            raise ArchiveError(cause=msg % (archive_path))
 
-        parsed_args = vars(self.parsed_args)
-        kw = find_signature_parameters(fetch, parsed_args)
-        items = fetch(**kw)
+        conn = sqlite3.connect(archive_path)
 
-        try:
-            for item in items:
-                obj = json.dumps(item, indent=4, sort_keys=True)
-                self.outfile.write(obj)
-                self.outfile.write('\n')
-        except IOError as e:
-            raise RuntimeError(str(e))
-        except Exception as e:
-            if self.backend.cache:
-                self.backend.cache.recover()
-            raise RuntimeError(str(e))
-
-    def _pre_init(self):
-        """Override to execute before backend is initialized."""
-        pass
-
-    def _post_init(self):
-        """Override to execute after backend is initialized."""
-        pass
-
-    def _initialize_cache(self):
-        """Initialize cache based on the parsed parameters"""
-
-        if 'cache_path' not in self.parsed_args:
-            return None
-
-        if self.parsed_args.no_cache:
-            return None
-
-        return setup_cache(self.backend.origin,
-                           cache_path=self.parsed_args.cache_path,
-                           clean_cache=self.parsed_args.clean_cache)
+        cursor = conn.cursor()
+        cursor.execute(cls.METADATA_CREATE_STMT)
+        cursor.execute(cls.ARCHIVE_CREATE_STMT)
+        conn.commit()
 
-    @staticmethod
-    def setup_cmd_parser():
-        raise NotImplementedError
+        cursor.close()
+        conn.close()
 
+        logger.debug("Creating archive %s", archive_path)
+        archive = cls(archive_path)
+        logger.debug("Achive %s was created", archive_path)
 
-def metadata(func):
-    """Add metadata to an item.
+        return archive
 
-    Decorator that adds metadata to a given item such as how and
-    when it was fetched. The contents from the original item will
-    be stored under the 'data' keyword.
+    @staticmethod
+    def make_hashcode(uri, payload, headers):
+        """Generate a SHA1 based on the given arguments.
 
-    Take into account that this decorator can only be called from a
-    'Backend' class due it needs access to some of the attributes
-    and methods of this class.
-    """
-    @functools.wraps(func)
-    def decorator(self, *args, **kwargs):
-        for data in func(self, *args, **kwargs):
-            item = {
-                'backend_name': self.__class__.__name__,
-                'backend_version': self.version,
-                'perceval_version': __version__,
-                'timestamp': dt.utcnow().timestamp(),
-                'origin': self.origin,
-                'uuid': uuid(self.origin, self.metadata_id(data)),
-                'updated_on': self.metadata_updated_on(data),
-                'category': self.metadata_category(data),
-                'tag': self.tag,
-                'data': data,
-            }
-            yield item
-    return decorator
-
-
-def uuid(*args):
-    """Generate a UUID based on the given parameters.
-
-    The UUID will be the SHA1 of the concatenation of the values
-    from the list. The separator bewteedn these values is ':'.
-    Each value must be a non-empty string, otherwise, the function
-    will raise an exception.
+        Hashcodes created by this method will used as unique identifiers
+        for the raw items or resources stored by this archive.
 
-    :param *args: list of arguments used to generate the UUID
+        :param uri: URI to the resource
+        :param payload: payload of the request needed to fetch the resource
+        :param headers: headers of the request needed to fetch the resource
 
-    :returns: a universal unique identifier
+        :returns: a SHA1 hash code
+        """
+        def dict_to_json_str(data):
+            return json.dumps(data, sort_keys=True)
 
-    :raises ValueError: when anyone of the values is not a string,
-        is empty or `None`.
-    """
-    def check_value(v):
-        if not isinstance(v, str):
-            raise ValueError("%s value is not a string instance" % str(v))
-        elif not v:
-            raise ValueError("value cannot be None or empty")
-        else:
-            return v
+        content = ':'.join([uri, dict_to_json_str(payload), dict_to_json_str(headers)])
+        hashcode = hashlib.sha1(content.encode('utf-8'))
+        return hashcode.hexdigest()
 
-    s = ':'.join(map(check_value, args))
+    def _verify_archive(self):
+        """Check whether the archive is valid or not.
 
-    sha1 = hashlib.sha1(s.encode('utf-8', errors='surrogateescape'))
-    uuid_sha1 = sha1.hexdigest()
+        This method will check if tables were created and if they
+        contain valid data.
+        """
+        nentries = self._count_table_rows(self.ARCHIVE_TABLE)
+        nmetadata = self._count_table_rows(self.METADATA_TABLE)
 
-    return uuid_sha1
+        if nmetadata > 1:
+            msg = "archive %s metadata corrupted; multiple metadata entries" % (self.archive_path)
+            raise ArchiveError(cause=msg)
+        if nmetadata == 0 and nentries > 0:
+            msg = "archive %s metadata is empty but %s entries were achived" % (self.archive_path)
+            raise ArchiveError(cause=msg)
+
+        logger.debug("Integrity of archive %s OK; entries: %s rows, metadata: %s rows",
+                     self.archive_path, nentries, nmetadata)
+
+    def _load_metadata(self):
+        """Load metadata from the archive file"""
+
+        logger.debug("Loading metadata infomation of archive %s", self.archive_path)
+
+        cursor = self._db.cursor()
+        select_stmt = "SELECT origin, backend_name, backend_version, " \
+                      "category, backend_params, created_on " \
+                      "FROM " + self.METADATA_TABLE + " " \
+                      "LIMIT 1"
+        cursor.execute(select_stmt)
+        row = cursor.fetchone()
+        cursor.close()
+
+        if row:
+            self.origin = row[0]
+            self.backend_name = row[1]
+            self.backend_version = row[2]
+            self.category = row[3]
+            self.backend_params = pickle.loads(row[4])
+            self.created_on = str_to_datetime(row[5])
+        else:
+            logger.debug("Metadata of archive %s was empty", self.archive_path)
 
+        logger.debug("Metadata of archive %s loaded", self.archive_path)
 
-def find_backends(top_package):
-    """Find available backends.
+    def _count_table_rows(self, table_name):
+        """Fetch the number of rows in a table"""
 
-    Look for the Perceval backends and commands under `top_package`
-    and its sub-packages. When `top_package` defines a namespace,
-    backends under that same namespace will be found too.
+        cursor = self._db.cursor()
+        select_stmt = "SELECT COUNT(*) FROM " + table_name
 
-    :param top_package: package storing backends
+        try:
+            cursor.execute(select_stmt)
+            row = cursor.fetchone()
+        except sqlite3.DatabaseError as e:
+            msg = "invalid archive file; cause: %s" % str(e)
+            raise ArchiveError(cause=msg)
+        finally:
+            cursor.close()
+
+        return row[0]
+
+
+class ArchiveManager:
+    """Manager for handling archives in Perceval.
+
+    This class manages the creation, deletion and access of `Archive`
+    objects. Archives are stored under `dirpath` directory, using
+    a random SHA1 for each file. The first byte of the hashcode will
+    be the name of the subdirectory; the remaining bytes, the archive
+    name.
 
-    :returns: a tuple with two dicts: one with `Backend` classes and one
-        with `BackendCommand` classes
+    :param: dirpath: path where the archives are stored
     """
-    candidates = pkgutil.walk_packages(top_package.__path__,
-                                       prefix=top_package.__name__ + '.')
 
-    modules = [name for _, name, is_pkg in candidates if not is_pkg]
+    STORAGE_EXT = '.sqlite3'
 
-    return _import_backends(modules)
+    def __init__(self, dirpath):
+        self.dirpath = dirpath
 
+        if not os.path.exists(self.dirpath):
+            os.makedirs(self.dirpath)
 
-def _import_backends(modules):
-    for module in modules:
-        importlib.import_module(module)
+    def create_archive(self):
+        """Create a new archive.
 
-    bkls = _find_classes(Backend, modules)
-    ckls = _find_classes(BackendCommand, modules)
+        The method creates in the filesystem a brand new archive with
+        a random SHA1 as its name. The first byte of the hashcode will
+        be the name of the subdirectory; the remaining bytes, the
+        archive name.
 
-    backends = {name: kls for name, kls in bkls}
-    commands = {name: klass for name, klass in ckls}
+        :returns: a new `Archive` object
 
-    return backends, commands
+        :raises ArchiveManagerError: when an error occurs creating the
+            new archive
+        """
+        hashcode = uuid.uuid4().hex
+        archive_dir = os.path.join(self.dirpath, hashcode[0:2])
+        archive_name = hashcode[2:] + self.STORAGE_EXT
+        archive_path = os.path.join(archive_dir, archive_name)
 
+        if not os.path.exists(archive_dir):
+            os.makedirs(archive_dir)
 
-def _find_classes(parent, modules):
-    parents = parent.__subclasses__()
+        try:
+            archive = Archive.create(archive_path)
+        except ArchiveError as e:
+            raise ArchiveManagerError(cause=str(e))
 
-    while parents:
-        kls = parents.pop()
+        return archive
 
-        m = kls.__module__
+    def remove_archive(self, archive_path):
+        """Remove an archive.
 
-        if m not in modules:
-            continue
+        This method deletes from the filesystem the archive stored
+        in `archive_path`.
 
-        name = m.split('.')[-1]
-        parents.extend(kls.__subclasses__())
+        :param archive_path: path to the archive
 
-        yield name, kls
+        :raises ArchiveManangerError: when an error occurs removing the
+            archive
+        """
+        try:
+            Archive(archive_path)
+        except ArchiveError as e:
+            raise ArchiveManagerError(cause=str(e))
+
+        os.remove(archive_path)
+
+    def search(self, origin, backend_name, category, archived_after):
+        """Search archives.
+
+        Get the archives which store data based on the given parameters.
+        These parameters define which the origin was (`origin`), how data
+        was fetched (`backend_name`) and data type ('category').
+        Only those archives created on or after `archived_after` will be
+        returned.
+
+        The method returns a list with the file paths to those archives.
+        The list is sorted by the date of creation of each archive.
+
+        :param origin: data origin
+        :param backend_name: backed used to fetch data
+        :param category: type of the items fetched by the backend
+        :param archived_after: get archives created on or after this date
+
+        :returns: a list with archive names which match the search criteria
+        """
+        archives = self._search_archives(origin, backend_name,
+                                         category, archived_after)
+        archives = [(fp, date) for fp, date in archives]
+        archives = [fp for fp, _ in sorted(archives, key=lambda x: x[1])]
+
+        return archives
+
+    def _search_archives(self, origin, backend_name, category, archived_after):
+        """Search archives using filters."""
+
+        for archive_path in self._search_files():
+            try:
+                archive = Archive(archive_path)
+            except ArchiveError:
+                continue
+
+            match = archive.origin == origin and \
+                archive.backend_name == backend_name and \
+                archive.category == category and \
+                archive.created_on >= archived_after
+
+            if not match:
+                continue
+
+            yield archive_path, archive.created_on
+
+    def _search_files(self):
+        """Retrieve the file paths stored under the base path."""
+
+        for root, _, files in os.walk(self.dirpath):
+            for filename in files:
+                location = os.path.join(root, filename)
+                yield location
```

