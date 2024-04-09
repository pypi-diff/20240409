# Comparing `tmp/grimoire-elk-0.99.0.tar.gz` & `tmp/grimoire_elk-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/dist/grimoire-elk-0.99.0.tar", last modified: Thu Jan 27 11:03:58 2022, max compression
+gzip compressed data, was "grimoire_elk-1.0.0rc1.tar", max compression
```

## Comparing `grimoire-elk-0.99.0.tar` & `grimoire_elk-1.0.0rc1.tar`

### file list

```diff
@@ -1,146 +1,248 @@
-drwxrwxr-x   0 quan      (1001) quan      (1001)        0 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/
--rw-rw-r--   0 quan      (1001) quan      (1001)      204 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/setup.cfg
--rw-rw-r--   0 quan      (1001) quan      (1001)     2421 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/pyproject.toml
-drwxrwxr-x   0 quan      (1001) quan      (1001)        0 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/grimoire_elk.egg-info/
--rw-rw-r--   0 quan      (1001) quan      (1001)        1 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/grimoire_elk.egg-info/dependency_links.txt
--rw-rw-r--   0 quan      (1001) quan      (1001)     4275 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/grimoire_elk.egg-info/SOURCES.txt
--rw-rw-r--   0 quan      (1001) quan      (1001)        1 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/grimoire_elk.egg-info/not-zip-safe
--rw-rw-r--   0 quan      (1001) quan      (1001)      411 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/grimoire_elk.egg-info/requires.txt
--rw-rw-r--   0 quan      (1001) quan      (1001)    13847 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/grimoire_elk.egg-info/PKG-INFO
--rw-rw-r--   0 quan      (1001) quan      (1001)       13 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/grimoire_elk.egg-info/top_level.txt
--rw-rw-r--   0 quan      (1001) quan      (1001)    13847 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/PKG-INFO
-drwxrwxr-x   0 quan      (1001) quan      (1001)        0 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/utils/
--rwxrwxr-x   0 quan      (1001) quan      (1001)     5183 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/utils/gelk_mapping.py
--rwxrwxr-x   0 quan      (1001) quan      (1001)     3963 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/utils/p2o.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    35147 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/LICENSE
--rw-rw-r--   0 quan      (1001) quan      (1001)    13009 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/README.md
--rw-rw-r--   0 quan      (1001) quan      (1001)       18 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/MANIFEST.in
-drwxrwxr-x   0 quan      (1001) quan      (1001)        0 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/grimoire_elk/
--rw-rw-r--   0 quan      (1001) quan      (1001)       23 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/_version.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1309 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/errors.py
-drwxrwxr-x   0 quan      (1001) quan      (1001)        0 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/
--rw-rw-r--   0 quan      (1001) quan      (1001)     5209 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/sortinghat_gelk.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    13610 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/meetup.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     6687 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/puppetforge.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    16209 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/gitlab.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    36434 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/github.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    12332 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/discourse.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     6172 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/mozillaclub.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     6144 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/dockerhub.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     8696 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/study_ceres_aoc.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    45718 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/git.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     8036 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/remo.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     6787 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/rocketchat.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     9130 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/mediawiki.py
--rw-rw-r--   0 quan      (1001) quan      (1001)      897 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/groupsio.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     8747 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/kitsune.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    12673 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/ceres_base.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    16606 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/mbox_study_kip.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     5566 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/redmine.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     3481 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/rss.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     5408 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/gitter.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    10011 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/stackexchange.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    18578 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/jira.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    32205 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/gerrit.py
--rw-rw-r--   0 quan      (1001) quan      (1001)      907 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/pipermail.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    12855 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/pagure.py
--rw-rw-r--   0 quan      (1001) quan      (1001)        0 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/__init__.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    33027 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/githubql.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1670 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/google_hits.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     5431 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/twitter.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     4691 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/dockerdeps.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    14023 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/askbot.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     7284 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/bugzilla.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    15829 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/study_ceres_onion.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1052 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/nntp.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    23552 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/slack.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    92030 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/enrich.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     6067 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/bugzillarest.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     5408 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/github_study_evolution.py
--rw-rw-r--   0 quan      (1001) quan      (1001)      908 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/hyperkitty.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     5141 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/confluence.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     8339 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/mattermost.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     5328 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/telegram.py
--rwxrwxr-x   0 quan      (1001) quan      (1001)     7997 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/utils.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     3747 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/finosmeetings.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     3362 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/supybot.py
-drwxrwxr-x   0 quan      (1001) quan      (1001)        0 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/mappings/
--rw-rw-r--   0 quan      (1001) quan      (1001)      981 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/mappings/onion.json
--rw-rw-r--   0 quan      (1001) quan      (1001)      961 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/mappings/onion_es7.json
--rw-rw-r--   0 quan      (1001) quan      (1001)     2552 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/mappings/git_aoc.json
--rw-rw-r--   0 quan      (1001) quan      (1001)     2295 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/mappings/git_aoc_es7.json
--rw-rw-r--   0 quan      (1001) quan      (1001)     8144 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/mbox.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    27867 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/github2.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    15340 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/cocom.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     5296 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/crates.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     6286 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/weblate.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     5648 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/graal_study_evolution.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     6242 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/functest.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    16216 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/colic.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     4922 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/dockersmells.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     7797 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/launchpad.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2233 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/database.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    15732 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/phabricator.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     8332 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/jenkins.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    14188 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/elastic_items.py
-drwxrwxr-x   0 quan      (1001) quan      (1001)        0 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/grimoire_elk/raw/
--rw-rw-r--   0 quan      (1001) quan      (1001)     2666 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/meetup.py
--rw-rw-r--   0 quan      (1001) quan      (1001)      874 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/puppetforge.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2074 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/graal.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     3448 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/gitlab.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     4828 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/github.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     3488 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/discourse.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1882 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/mozillaclub.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2036 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/dockerhub.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2178 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/git.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1788 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/remo.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1863 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/rocketchat.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2128 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/mediawiki.py
--rw-rw-r--   0 quan      (1001) quan      (1001)      882 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/groupsio.py
--rw-rw-r--   0 quan      (1001) quan      (1001)      875 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/kitsune.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2088 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/redmine.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2023 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/rss.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1831 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/gitter.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2613 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/stackexchange.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     3442 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/jira.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     3017 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/gerrit.py
--rw-rw-r--   0 quan      (1001) quan      (1001)      892 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/pipermail.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1921 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/pagure.py
--rw-rw-r--   0 quan      (1001) quan      (1001)        0 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/__init__.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1853 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/githubql.py
--rw-rw-r--   0 quan      (1001) quan      (1001)      903 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/google_hits.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     3815 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/twitter.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2181 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/askbot.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2450 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/bugzilla.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2113 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/nntp.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2900 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/slack.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     4458 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/bugzillarest.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1831 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/hyperkitty.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2288 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/confluence.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     5204 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/mattermost.py
--rw-rw-r--   0 quan      (1001) quan      (1001)      877 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/telegram.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1594 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/finosmeetings.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1044 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/supybot.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    11043 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/elastic.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2249 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/mbox.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1836 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/crates.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1899 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/weblate.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2341 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/functest.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1870 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/launchpad.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     3052 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/phabricator.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     5603 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/jenkins.py
--rwxrwxr-x   0 quan      (1001) quan      (1001)    33930 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/elk.py
-drwxrwxr-x   0 quan      (1001) quan      (1001)        0 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/grimoire_elk/identities/
--rw-rw-r--   0 quan      (1001) quan      (1001)     1835 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/identities/meetup.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1237 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/identities/identities.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1722 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/identities/gitlab.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2712 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/identities/github.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1732 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/identities/git.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1916 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/identities/stackexchange.py
--rw-rw-r--   0 quan      (1001) quan      (1001)        0 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/identities/__init__.py
--rw-rw-r--   0 quan      (1001) quan      (1001)      894 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/__init__.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1637 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/elastic_analyzer.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1653 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/elastic_mapping.py
--rwxrwxr-x   0 quan      (1001) quan      (1001)    19994 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/utils.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    22450 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/elastic.py
--rwxrwxr-x   0 quan      (1001) quan      (1001)     3397 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/setup.py
+-rw-r--r--   0        0        0      468 2024-04-09 16:28:32.315883 grimoire_elk-1.0.0rc1/AUTHORS
+-rw-r--r--   0        0        0    35147 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0    27832 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/NEWS
+-rw-r--r--   0        0        0    14186 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/README.md
+-rw-r--r--   0        0        0      894 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/_version.py
+-rw-r--r--   0        0        0    23287 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/elastic.py
+-rw-r--r--   0        0        0     1642 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/elastic_analyzer.py
+-rw-r--r--   0        0        0    15494 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/elastic_items.py
+-rw-r--r--   0        0        0     1653 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/elastic_mapping.py
+-rwxr-xr-x   0        0        0    36859 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/elk.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/__init__.py
+-rw-r--r--   0        0        0    14023 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/askbot.py
+-rw-r--r--   0        0        0     7751 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/bugzilla.py
+-rw-r--r--   0        0        0     6067 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/bugzillarest.py
+-rw-r--r--   0        0        0    12774 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/ceres_base.py
+-rw-r--r--   0        0        0    15605 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/cocom.py
+-rw-r--r--   0        0        0    16481 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/colic.py
+-rw-r--r--   0        0        0     5141 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/confluence.py
+-rw-r--r--   0        0        0     5296 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/crates.py
+-rw-r--r--   0        0        0    12597 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/discourse.py
+-rw-r--r--   0        0        0     4956 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/dockerdeps.py
+-rw-r--r--   0        0        0     6144 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/dockerhub.py
+-rw-r--r--   0        0        0     5187 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/dockersmells.py
+-rw-r--r--   0        0        0    97698 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/enrich.py
+-rw-r--r--   0        0        0     6242 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/functest.py
+-rw-r--r--   0        0        0    32547 2024-04-09 16:28:32.319883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/gerrit.py
+-rw-r--r--   0        0        0    46730 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/git.py
+-rw-r--r--   0        0        0    36818 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/github.py
+-rw-r--r--   0        0        0    28496 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/github2.py
+-rw-r--r--   0        0        0     5505 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/github_study_evolution.py
+-rw-r--r--   0        0        0    33292 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/githubql.py
+-rw-r--r--   0        0        0    16523 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/gitlab.py
+-rw-r--r--   0        0        0     5673 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/gitter.py
+-rw-r--r--   0        0        0     1670 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/google_hits.py
+-rw-r--r--   0        0        0     5648 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/graal_study_evolution.py
+-rw-r--r--   0        0        0      897 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/groupsio.py
+-rw-r--r--   0        0        0      908 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/hyperkitty.py
+-rw-r--r--   0        0        0     8614 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/jenkins.py
+-rw-r--r--   0        0        0    18534 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/jira.py
+-rw-r--r--   0        0        0     9440 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/kitsune.py
+-rw-r--r--   0        0        0     8062 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/launchpad.py
+-rw-r--r--   0        0        0     2552 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mappings/git_aoc.json
+-rw-r--r--   0        0        0     2295 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mappings/git_aoc_es7.json
+-rw-r--r--   0        0        0      981 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mappings/onion.json
+-rw-r--r--   0        0        0      961 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mappings/onion_es7.json
+-rw-r--r--   0        0        0     9237 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mattermost.py
+-rw-r--r--   0        0        0     8409 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mbox.py
+-rw-r--r--   0        0        0    16606 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mbox_study_kip.py
+-rw-r--r--   0        0        0     9113 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mediawiki.py
+-rw-r--r--   0        0        0    13622 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/meetup.py
+-rw-r--r--   0        0        0     6172 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mozillaclub.py
+-rw-r--r--   0        0        0     1052 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/nntp.py
+-rw-r--r--   0        0        0    13120 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/pagure.py
+-rw-r--r--   0        0        0    16022 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/phabricator.py
+-rw-r--r--   0        0        0      907 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/pipermail.py
+-rw-r--r--   0        0        0     6687 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/puppetforge.py
+-rw-r--r--   0        0        0     5566 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/redmine.py
+-rw-r--r--   0        0        0     8301 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/remo.py
+-rw-r--r--   0        0        0     6787 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/rocketchat.py
+-rw-r--r--   0        0        0     3481 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/rss.py
+-rw-r--r--   0        0        0    23552 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/slack.py
+-rw-r--r--   0        0        0    19794 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/sortinghat_gelk.py
+-rw-r--r--   0        0        0    10011 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/stackexchange.py
+-rw-r--r--   0        0        0     8795 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/study_ceres_aoc.py
+-rw-r--r--   0        0        0    16420 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/study_ceres_onion.py
+-rw-r--r--   0        0        0     3362 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/supybot.py
+-rw-r--r--   0        0        0     5328 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/telegram.py
+-rw-r--r--   0        0        0     5431 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/twitter.py
+-rwxr-xr-x   0        0        0     8567 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/utils.py
+-rw-r--r--   0        0        0     6565 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/enriched/weblate.py
+-rw-r--r--   0        0        0     1309 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/errors.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/identities/__init__.py
+-rw-r--r--   0        0        0     1732 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/identities/git.py
+-rw-r--r--   0        0        0     2712 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/identities/github.py
+-rw-r--r--   0        0        0     1722 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/identities/gitlab.py
+-rw-r--r--   0        0        0     1237 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/identities/identities.py
+-rw-r--r--   0        0        0     1835 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/identities/meetup.py
+-rw-r--r--   0        0        0     1916 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/identities/stackexchange.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/__init__.py
+-rw-r--r--   0        0        0     2181 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/askbot.py
+-rw-r--r--   0        0        0     2450 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/bugzilla.py
+-rw-r--r--   0        0        0     4458 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/bugzillarest.py
+-rw-r--r--   0        0        0     2831 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/confluence.py
+-rw-r--r--   0        0        0     1836 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/crates.py
+-rw-r--r--   0        0        0     3488 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/discourse.py
+-rw-r--r--   0        0        0     2036 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/dockerhub.py
+-rw-r--r--   0        0        0    11185 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/elastic.py
+-rw-r--r--   0        0        0     2341 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/functest.py
+-rw-r--r--   0        0        0     3017 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/gerrit.py
+-rw-r--r--   0        0        0     2728 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/git.py
+-rw-r--r--   0        0        0     4828 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/github.py
+-rw-r--r--   0        0        0     1853 2024-04-09 16:28:32.323883 grimoire_elk-1.0.0rc1/grimoire_elk/raw/githubql.py
+-rw-r--r--   0        0        0     3448 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/gitlab.py
+-rw-r--r--   0        0        0     1831 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/gitter.py
+-rw-r--r--   0        0        0      903 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/google_hits.py
+-rw-r--r--   0        0        0     2327 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/graal.py
+-rw-r--r--   0        0        0      882 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/groupsio.py
+-rw-r--r--   0        0        0     1831 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/hyperkitty.py
+-rw-r--r--   0        0        0     5603 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/jenkins.py
+-rw-r--r--   0        0        0     3442 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/jira.py
+-rw-r--r--   0        0        0     2407 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/kitsune.py
+-rw-r--r--   0        0        0     1870 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/launchpad.py
+-rw-r--r--   0        0        0     5204 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/mattermost.py
+-rw-r--r--   0        0        0     2249 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/mbox.py
+-rw-r--r--   0        0        0     2128 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/mediawiki.py
+-rw-r--r--   0        0        0     2666 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/meetup.py
+-rw-r--r--   0        0        0     1882 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/mozillaclub.py
+-rw-r--r--   0        0        0     2113 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/nntp.py
+-rw-r--r--   0        0        0     1921 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/pagure.py
+-rw-r--r--   0        0        0     3052 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/phabricator.py
+-rw-r--r--   0        0        0      892 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/pipermail.py
+-rw-r--r--   0        0        0      874 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/puppetforge.py
+-rw-r--r--   0        0        0     2088 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/redmine.py
+-rw-r--r--   0        0        0     1788 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/remo.py
+-rw-r--r--   0        0        0     1863 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/rocketchat.py
+-rw-r--r--   0        0        0     2023 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/rss.py
+-rw-r--r--   0        0        0     3084 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/slack.py
+-rw-r--r--   0        0        0     2613 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/stackexchange.py
+-rw-r--r--   0        0        0     1044 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/supybot.py
+-rw-r--r--   0        0        0      877 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/telegram.py
+-rw-r--r--   0        0        0     3815 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/twitter.py
+-rw-r--r--   0        0        0     1899 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/raw/weblate.py
+-rwxr-xr-x   0        0        0    20183 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/grimoire_elk/utils.py
+-rw-r--r--   0        0        0     2144 2024-04-09 16:28:32.327884 grimoire_elk-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      775 2024-04-09 16:28:32.331884 grimoire_elk-1.0.0rc1/tests/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 16:28:32.331884 grimoire_elk-1.0.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0    16169 2024-04-09 16:28:32.331884 grimoire_elk-1.0.0rc1/tests/base.py
+-rw-r--r--   0        0        0   317579 2024-04-09 16:28:32.331884 grimoire_elk-1.0.0rc1/tests/data/askbot.json
+-rw-r--r--   0        0        0     1262 2024-04-09 16:28:32.331884 grimoire_elk-1.0.0rc1/tests/data/author_min_max_dates_1.json
+-rw-r--r--   0        0        0     1262 2024-04-09 16:28:32.335883 grimoire_elk-1.0.0rc1/tests/data/author_min_max_dates_2.json
+-rw-r--r--   0        0        0      282 2024-04-09 16:28:32.335883 grimoire_elk-1.0.0rc1/tests/data/author_min_max_dates_empty.json
+-rw-r--r--   0        0        0   123043 2024-04-09 16:28:32.335883 grimoire_elk-1.0.0rc1/tests/data/bugzilla.json
+-rw-r--r--   0        0        0    13208 2024-04-09 16:28:32.335883 grimoire_elk-1.0.0rc1/tests/data/bugzillarest-item-bulgarian.json
+-rw-r--r--   0        0        0      189 2024-04-09 16:28:32.335883 grimoire_elk-1.0.0rc1/tests/data/bugzillarest-projects.json
+-rw-r--r--   0        0        0   742238 2024-04-09 16:28:32.335883 grimoire_elk-1.0.0rc1/tests/data/bugzillarest.json
+-rw-r--r--   0        0        0    12691 2024-04-09 16:28:32.335883 grimoire_elk-1.0.0rc1/tests/data/cocom.json
+-rw-r--r--   0        0        0    16260 2024-04-09 16:28:32.335883 grimoire_elk-1.0.0rc1/tests/data/colic.json
+-rw-r--r--   0        0        0    66663 2024-04-09 16:28:32.335883 grimoire_elk-1.0.0rc1/tests/data/confluence.json
+-rw-r--r--   0        0        0     8772 2024-04-09 16:28:32.335883 grimoire_elk-1.0.0rc1/tests/data/confluence_with_credentials.json
+-rw-r--r--   0        0        0   155992 2024-04-09 16:28:32.335883 grimoire_elk-1.0.0rc1/tests/data/crates.json
+-rw-r--r--   0        0        0   544021 2024-04-09 16:28:32.339884 grimoire_elk-1.0.0rc1/tests/data/discourse.json
+-rw-r--r--   0        0        0    37574 2024-04-09 16:28:32.339884 grimoire_elk-1.0.0rc1/tests/data/dockerdeps.json
+-rw-r--r--   0        0        0   115251 2024-04-09 16:28:32.339884 grimoire_elk-1.0.0rc1/tests/data/dockerhub.json
+-rw-r--r--   0        0        0    11347 2024-04-09 16:28:32.339884 grimoire_elk-1.0.0rc1/tests/data/dockersmells.json
+-rw-r--r--   0        0        0    53387 2024-04-09 16:28:32.339884 grimoire_elk-1.0.0rc1/tests/data/functest.json
+-rw-r--r--   0        0        0   279521 2024-04-09 16:28:32.339884 grimoire_elk-1.0.0rc1/tests/data/functest_wrong.json
+-rw-r--r--   0        0        0   843001 2024-04-09 16:28:32.343884 grimoire_elk-1.0.0rc1/tests/data/gerrit.json
+-rw-r--r--   0        0        0    15713 2024-04-09 16:28:32.343884 grimoire_elk-1.0.0rc1/tests/data/git.json
+-rw-r--r--   0        0        0   244775 2024-04-09 16:28:32.343884 grimoire_elk-1.0.0rc1/tests/data/github.json
+-rw-r--r--   0        0        0   234447 2024-04-09 16:28:32.343884 grimoire_elk-1.0.0rc1/tests/data/github2.json
+-rw-r--r--   0        0        0    75664 2024-04-09 16:28:32.343884 grimoire_elk-1.0.0rc1/tests/data/githubql.json
+-rw-r--r--   0        0        0   672068 2024-04-09 16:28:32.343884 grimoire_elk-1.0.0rc1/tests/data/gitlab.json
+-rw-r--r--   0        0        0    12297 2024-04-09 16:28:32.343884 grimoire_elk-1.0.0rc1/tests/data/gitter.json
+-rw-r--r--   0        0        0   330892 2024-04-09 16:28:32.347884 grimoire_elk-1.0.0rc1/tests/data/gmane.json
+-rw-r--r--   0        0        0     2025 2024-04-09 16:28:32.347884 grimoire_elk-1.0.0rc1/tests/data/google_hits.json
+-rw-r--r--   0        0        0   346405 2024-04-09 16:28:32.347884 grimoire_elk-1.0.0rc1/tests/data/groupsio.json
+-rw-r--r--   0        0        0     8313 2024-04-09 16:28:32.347884 grimoire_elk-1.0.0rc1/tests/data/hyperkitty.json
+-rw-r--r--   0        0        0   384247 2024-04-09 16:28:32.347884 grimoire_elk-1.0.0rc1/tests/data/jenkins.json
+-rw-r--r--   0        0        0   185733 2024-04-09 16:28:32.347884 grimoire_elk-1.0.0rc1/tests/data/jira.json
+-rw-r--r--   0        0        0      649 2024-04-09 16:28:32.347884 grimoire_elk-1.0.0rc1/tests/data/jira_enriched_fields.json
+-rw-r--r--   0        0        0    20498 2024-04-09 16:28:32.347884 grimoire_elk-1.0.0rc1/tests/data/jira_new.json
+-rw-r--r--   0        0        0   378857 2024-04-09 16:28:32.351884 grimoire_elk-1.0.0rc1/tests/data/jira_raw_fields.json
+-rw-r--r--   0        0        0    17761 2024-04-09 16:28:32.351884 grimoire_elk-1.0.0rc1/tests/data/kitsune.json
+-rw-r--r--   0        0        0    79536 2024-04-09 16:28:32.351884 grimoire_elk-1.0.0rc1/tests/data/launchpad.json
+-rw-r--r--   0        0        0   210275 2024-04-09 16:28:32.351884 grimoire_elk-1.0.0rc1/tests/data/mattermost.json
+-rw-r--r--   0        0        0   269992 2024-04-09 16:28:32.351884 grimoire_elk-1.0.0rc1/tests/data/mbox.json
+-rw-r--r--   0        0        0    57533 2024-04-09 16:28:32.351884 grimoire_elk-1.0.0rc1/tests/data/mediawiki.json
+-rw-r--r--   0        0        0   324979 2024-04-09 16:28:32.351884 grimoire_elk-1.0.0rc1/tests/data/meetup.json
+-rw-r--r--   0        0        0   296278 2024-04-09 16:28:32.351884 grimoire_elk-1.0.0rc1/tests/data/mozillaclub.json
+-rw-r--r--   0        0        0   115901 2024-04-09 16:28:32.351884 grimoire_elk-1.0.0rc1/tests/data/nntp.json
+-rw-r--r--   0        0        0    54714 2024-04-09 16:28:32.351884 grimoire_elk-1.0.0rc1/tests/data/pagure.json
+-rw-r--r--   0        0        0   112410 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/phabricator.json
+-rw-r--r--   0        0        0   298460 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/pipermail.json
+-rw-r--r--   0        0        0      101 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/projects-release-mediawiki-uc2.json
+-rw-r--r--   0        0        0     3760 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/projects-release.json
+-rw-r--r--   0        0        0    44809 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/puppetforge.json
+-rw-r--r--   0        0        0   103516 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/redmine.json
+-rw-r--r--   0        0        0   105975 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/remo.json
+-rw-r--r--   0        0        0    50742 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/rocketchat.json
+-rw-r--r--   0        0        0   131368 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/rss.json
+-rw-r--r--   0        0        0    43442 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/slack.json
+-rw-r--r--   0        0        0    92013 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/stackexchange.json
+-rw-r--r--   0        0        0     8311 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/supybot.json
+-rw-r--r--   0        0        0     2032 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/task-identities-data.json
+-rw-r--r--   0        0        0    12597 2024-04-09 16:28:32.355884 grimoire_elk-1.0.0rc1/tests/data/telegram.json
+-rw-r--r--   0        0        0    44540 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/data/twitter.json
+-rw-r--r--   0        0        0     8339 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/data/weblate.json
+-rw-r--r--   0        0        0    11214 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/model.py
+-rwxr-xr-x   0        0        0      992 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/run_tests.py
+-rw-r--r--   0        0        0     4180 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_askbot.py
+-rw-r--r--   0        0        0     4678 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_bugzilla.py
+-rw-r--r--   0        0        0     5330 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_bugzillarest.py
+-rw-r--r--   0        0        0     7455 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_cocom.py
+-rw-r--r--   0        0        0     6691 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_colic.py
+-rw-r--r--   0        0        0     9722 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_confluence.py
+-rw-r--r--   0        0        0     4466 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_crates.py
+-rw-r--r--   0        0        0    10044 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_discourse.py
+-rw-r--r--   0        0        0     4687 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_dockerdeps.py
+-rw-r--r--   0        0        0     4082 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_dockerhub.py
+-rw-r--r--   0        0        0     5813 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_dockersmells.py
+-rw-r--r--   0        0        0    32434 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_elastic.py
+-rw-r--r--   0        0        0    20552 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_elastic_items.py
+-rw-r--r--   0        0        0     2791 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_elastic_ocean.py
+-rw-r--r--   0        0        0     4636 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_elk.py
+-rw-r--r--   0        0        0    34090 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_enrich.py
+-rw-r--r--   0        0        0     1906 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_enrich_jira.py
+-rw-r--r--   0        0        0     2451 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_errors.py
+-rw-r--r--   0        0        0     4776 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_functest.py
+-rw-r--r--   0        0        0    17512 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_gerrit.py
+-rw-r--r--   0        0        0    41064 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_git.py
+-rw-r--r--   0        0        0    21320 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_github.py
+-rw-r--r--   0        0        0    15209 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_github2.py
+-rw-r--r--   0        0        0    23121 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_githubql.py
+-rw-r--r--   0        0        0    15573 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_gitlab.py
+-rw-r--r--   0        0        0    10355 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_gitter.py
+-rw-r--r--   0        0        0     3353 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_google_hits.py
+-rw-r--r--   0        0        0     4398 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_groupsio.py
+-rw-r--r--   0        0        0     4700 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_hyperkitty.py
+-rw-r--r--   0        0        0     5747 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_jenkins.py
+-rw-r--r--   0        0        0     8950 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_jira.py
+-rw-r--r--   0        0        0     5503 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_kitsune.py
+-rw-r--r--   0        0        0    15777 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_launchpad.py
+-rw-r--r--   0        0        0     4677 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_load_identities.py
+-rw-r--r--   0        0        0    10822 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_mattermost.py
+-rw-r--r--   0        0        0     8469 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_mbox.py
+-rw-r--r--   0        0        0    12014 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_mediawiki.py
+-rw-r--r--   0        0        0     7827 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_meetup.py
+-rw-r--r--   0        0        0     4818 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_mozillaclub.py
+-rw-r--r--   0        0        0     5533 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_nntp.py
+-rw-r--r--   0        0        0    11163 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_pagure.py
+-rw-r--r--   0        0        0     4439 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_phabricator.py
+-rw-r--r--   0        0        0     4549 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_pipermail.py
+-rw-r--r--   0        0        0     4950 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_projects.sql
+-rw-r--r--   0        0        0     4189 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_puppetforge.py
+-rw-r--r--   0        0        0     5116 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_redmine.py
+-rw-r--r--   0        0        0     4170 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_remo.py
+-rw-r--r--   0        0        0     5900 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_rocketchat.py
+-rw-r--r--   0        0        0     4173 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_rss.py
+-rw-r--r--   0        0        0     5681 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_slack.py
+-rw-r--r--   0        0        0    14524 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_sortinghat_gelk.py
+-rw-r--r--   0        0        0     6478 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_stackexchange.py
+-rw-r--r--   0        0        0     4697 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_supybot.py
+-rw-r--r--   0        0        0     5967 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_telegram.py
+-rw-r--r--   0        0        0     4178 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_twitter.py
+-rw-r--r--   0        0        0    11146 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/test_weblate.py
+-rw-r--r--   0        0        0      137 2024-04-09 16:28:32.359884 grimoire_elk-1.0.0rc1/tests/tests.conf
+-rw-r--r--   0        0        0    15901 1970-01-01 00:00:00.000000 grimoire_elk-1.0.0rc1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk.egg-info/PKG-INFO` & `grimoire_elk-1.0.0rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,13 @@
-Metadata-Version: 2.1
-Name: grimoire-elk
-Version: 0.99.0
-Summary: GrimoireLab library to produce indexes for ElasticSearch
-Home-page: https://github.com/grimoirelab/GrimoireELK
-Author: Bitergia
-Author-email: metrics-grimoire@lists.libresoft.info
-License: GPLv3
-Keywords: development repositories analytics
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Requires-Python: >=3.4
-Description-Content-Type: text/markdown
-Provides-Extra: sortinghat
-Provides-Extra: mysql
-License-File: LICENSE
+# Welcome to GrimoireELK [![Build Status](https://github.com/chaoss/grimoirelab-elk/workflows/tests/badge.svg)](https://github.com/chaoss/grimoirelab-elk/actions?query=workflow:tests+branch:master+event:push) [![Coverage Status](https://coveralls.io/repos/github/chaoss/grimoirelab-elk/badge.svg?branch=master)](https://coveralls.io/github/chaoss/grimoirelab-elk?branch=master) [![PyPI version](https://badge.fury.io/py/grimoire-elk.svg)](https://badge.fury.io/py/grimoire-elk) 
 
-# Welcome to GrimoireELK [![Build Status](https://github.com/chaoss/grimoirelab-elk/workflows/tests/badge.svg)](https://github.com/chaoss/grimoirelab-elk/actions?query=workflow:tests+branch:master+event:push) [![Coverage Status](https://coveralls.io/repos/github/chaoss/grimoirelab-elk/badge.svg?branch=master)](https://coveralls.io/github/chaoss/grimoirelab-elk?branch=master)
-
-GrimoireELK is the component that interacts with the ElasticSearch database. Its goal is two-fold, first it aims at offering a convenient
+GrimoireELK is the component of [GrimoireLab](https://github.com/chaoss/grimoirelab) that interacts with the ElasticSearch database. Its goal is two-fold, first it aims at offering a convenient
 way to store the data coming from Perceval, second it processes and enriches the data in a format that can be consumed by Kibiter.
 
-The Perceval data is stored in ElasticSearch indexes as raw documents (one per item extracted by Perceval). Those raw documents, which will be referred to as "raw data" in
+The [Perceval](https://github.com/chaoss/grimoirelab-perceval) data is stored in ElasticSearch indexes as raw documents (one per item extracted by Perceval). Those raw documents, which will be referred to as "raw data" in
 this documentation, include all information coming from the original data source which grants the platform to perform multiple analysis without the need of downloading the
 same data over and over again. Once raw data is retrieved, a new phase starts where data is enriched according to the data source from where it was collected and stored
 in ElasticSearch indexes. The enrichment removes information not needed by Kibiter and includes additional information which is not directly available within the raw data.
 For instance, pair programming information for Git data, time to solve (i.e., close or merge) issues and pull requests for GitHub data, and identities and organization
 information coming from [SortingHat](https://github.com/chaoss/grimoirelab-sortinghat) . The enriched data is stored as JSON documents, which embed information linked to
 the corresponding raw documents to ease debugging and guarantee traceability.
 
@@ -136,23 +113,68 @@
 
 #### Extra fields:
 - **extra_** (anything): Extra fields added using the `enrich_extra_data` study.
 
 #### Data source specific fields
 Details of the fields of each data source is available in the [Schema](https://github.com/chaoss/grimoirelab-elk/tree/master/schema) folder.
 
+## Installation
+
+There are several ways to install GrimoireELK on your system: packages or source 
+code using Poetry or pip.
+
+### PyPI
+
+GrimoireELK can be installed using pip, a tool for installing Python packages. 
+To do it, run the next command:
+```
+$ pip install grimoire-elk
+```
+
+### Source code
+
+To install from the source code you will need to clone the repository first:
+```
+$ git clone https://github.com/chaoss/grimoirelab-elk
+$ cd grimoirelab-elk
+```
+
+Then use pip or Poetry to install the package along with its dependencies.
+
+#### Pip
+To install the package from local directory run the following command:
+```
+$ pip install .
+```
+In case you are a developer, you should install GrimoireELK in editable mode:
+```
+$ pip install -e .
+```
+
+#### Poetry
+We use [poetry](https://python-poetry.org/) for dependency management and 
+packaging. You can install it following its [documentation](https://python-poetry.org/docs/#installation).
+Once you have installed it, you can install GrimoireELK and the dependencies in 
+a project isolated environment using:
+```
+$ poetry install
+```
+To spaw a new shell within the virtual environment use:
+```
+$ poetry shell
+```
+
 ## Running tests
 
-Tests are located in the folder [tests](https://github.com/chaoss/grimoirelab-elk/tree/master/tests). In order to run them, you need to have in your machine:
-- instances (or Docker containers) of ElasticSearch and MySQL
-- the [dependencies](https://github.com/chaoss/grimoirelab-elk/blob/master/requirements.txt) installed or available (the latter applies to the dependencies with the other GrimoireLab repositories).
+Tests are located in the folder [tests](https://github.com/chaoss/grimoirelab-elk/tree/master/tests). 
+In order to run them, you need to have in your machine instances (or Docker containers) of ElasticSearch and MySQL
 
 Then you need to:
 - update the file [tests.conf](https://github.com/chaoss/grimoirelab-elk/blob/master/tests/tests.conf) file:
-  - in case your ElasticSearch instance isn't available at http://localhost:9200. For example, if you are using the secure edition of elasticsearch, it will be located at https://admin:admin@localhost:9200
+  - in case your ElasticSearch instance isn't available at `http://localhost:9200`. For example, if you are using the secure edition of elasticsearch, it will be located at `https://admin:admin@localhost:9200`
   - in case you are using non-default credentials for your SortingHat database, you will need to include the `[Database]` section of the file with both `user` and `password` parameters
 - create the databases `test_sh` and `test_projects` in your MySQL instance (e.g., `mysql -u root -e "create database test_sh"`, if you are running mysql in a container use `docker exec -i <container id> mysql -u root -e "create database test_sh"`)
 - populate the database `test_projects` with the SQL file [test_projects.sql](https://github.com/chaoss/grimoirelab-elk/blob/master/tests/test_projects.sql) (e.g., `mysql -u root test_projects < tests/test_projects.sql`)
 
 The full battery of tests can be executed with [run_tests.py](https://github.com/chaoss/grimoirelab-elk/blob/master/tests/run_tests.py). However, it is also possible to execute
 a sub-set of tests by running the single test files (`test_*` files in the [tests folder](https://github.com/chaoss/grimoirelab-elk/tree/master/tests))
 
@@ -176,9 +198,7 @@
 The output will be similar to the following one:
 ```buildoutcfg
 Name                                                                                                                Stmts   Miss  Cover   Missing
 --------------------------------------------------------------------------------------------------------------------------------------------------
 .../ELK/grimoire_elk/__init__.py                                                                                       4      0   100%
 .../ELK/grimoire_elk/_version.py                                                                                       1      0   100%
 ```
-
-
```

### Comparing `grimoire-elk-0.99.0/PKG-INFO` & `grimoire_elk-1.0.0rc1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,54 @@
 Metadata-Version: 2.1
 Name: grimoire-elk
-Version: 0.99.0
-Summary: GrimoireLab library to produce indexes for ElasticSearch
-Home-page: https://github.com/grimoirelab/GrimoireELK
-Author: Bitergia
-Author-email: metrics-grimoire@lists.libresoft.info
-License: GPLv3
+Version: 1.0.0rc1
+Summary: GrimoireELK processes and stores software development data to ElasticSearch
+Home-page: https://github.com/chaoss/grimoirelab-elk
+License: GPL-3.0-or-later
 Keywords: development repositories analytics
-Platform: UNKNOWN
+Author: Bitergia
+Author-email: grimoirelab-discussions@lists.linuxfoundation.org
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Requires-Python: >=3.4
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Requires-Dist: cereslib (>=0.3)
+Requires-Dist: elasticsearch (==6.3.1)
+Requires-Dist: elasticsearch-dsl (==6.3.1)
+Requires-Dist: geopy (>=2.0.0,<3.0.0)
+Requires-Dist: graal (>=0.3)
+Requires-Dist: grimoirelab-toolkit (>=0.3)
+Requires-Dist: numpy (>=1.21.0,<2.0.0)
+Requires-Dist: pandas (>=1.3.5,<2.0.0)
+Requires-Dist: perceval (>=0.19)
+Requires-Dist: perceval-mozilla (>=0.3)
+Requires-Dist: perceval-opnfv (>=0.2)
+Requires-Dist: perceval-puppet (>=0.2)
+Requires-Dist: perceval-weblate (>=0.2)
+Requires-Dist: requests (>=2.7.0,<3.0.0)
+Requires-Dist: scipy (>=1.7.0)
+Requires-Dist: sortinghat (>=0.7.20)
+Requires-Dist: statsmodels (>=0.9.0)
+Requires-Dist: urllib3 (>=1.26,<2.0)
+Project-URL: Bug Tracker, https://github.com/chaoss/grimoirelab-elk/issues
+Project-URL: Repository, https://github.com/chaoss/grimoirelab-elk
 Description-Content-Type: text/markdown
-Provides-Extra: sortinghat
-Provides-Extra: mysql
-License-File: LICENSE
 
-# Welcome to GrimoireELK [![Build Status](https://github.com/chaoss/grimoirelab-elk/workflows/tests/badge.svg)](https://github.com/chaoss/grimoirelab-elk/actions?query=workflow:tests+branch:master+event:push) [![Coverage Status](https://coveralls.io/repos/github/chaoss/grimoirelab-elk/badge.svg?branch=master)](https://coveralls.io/github/chaoss/grimoirelab-elk?branch=master)
+# Welcome to GrimoireELK [![Build Status](https://github.com/chaoss/grimoirelab-elk/workflows/tests/badge.svg)](https://github.com/chaoss/grimoirelab-elk/actions?query=workflow:tests+branch:master+event:push) [![Coverage Status](https://coveralls.io/repos/github/chaoss/grimoirelab-elk/badge.svg?branch=master)](https://coveralls.io/github/chaoss/grimoirelab-elk?branch=master) [![PyPI version](https://badge.fury.io/py/grimoire-elk.svg)](https://badge.fury.io/py/grimoire-elk) 
 
-GrimoireELK is the component that interacts with the ElasticSearch database. Its goal is two-fold, first it aims at offering a convenient
+GrimoireELK is the component of [GrimoireLab](https://github.com/chaoss/grimoirelab) that interacts with the ElasticSearch database. Its goal is two-fold, first it aims at offering a convenient
 way to store the data coming from Perceval, second it processes and enriches the data in a format that can be consumed by Kibiter.
 
-The Perceval data is stored in ElasticSearch indexes as raw documents (one per item extracted by Perceval). Those raw documents, which will be referred to as "raw data" in
+The [Perceval](https://github.com/chaoss/grimoirelab-perceval) data is stored in ElasticSearch indexes as raw documents (one per item extracted by Perceval). Those raw documents, which will be referred to as "raw data" in
 this documentation, include all information coming from the original data source which grants the platform to perform multiple analysis without the need of downloading the
 same data over and over again. Once raw data is retrieved, a new phase starts where data is enriched according to the data source from where it was collected and stored
 in ElasticSearch indexes. The enrichment removes information not needed by Kibiter and includes additional information which is not directly available within the raw data.
 For instance, pair programming information for Git data, time to solve (i.e., close or merge) issues and pull requests for GitHub data, and identities and organization
 information coming from [SortingHat](https://github.com/chaoss/grimoirelab-sortinghat) . The enriched data is stored as JSON documents, which embed information linked to
 the corresponding raw documents to ease debugging and guarantee traceability.
 
@@ -136,23 +154,68 @@
 
 #### Extra fields:
 - **extra_** (anything): Extra fields added using the `enrich_extra_data` study.
 
 #### Data source specific fields
 Details of the fields of each data source is available in the [Schema](https://github.com/chaoss/grimoirelab-elk/tree/master/schema) folder.
 
+## Installation
+
+There are several ways to install GrimoireELK on your system: packages or source 
+code using Poetry or pip.
+
+### PyPI
+
+GrimoireELK can be installed using pip, a tool for installing Python packages. 
+To do it, run the next command:
+```
+$ pip install grimoire-elk
+```
+
+### Source code
+
+To install from the source code you will need to clone the repository first:
+```
+$ git clone https://github.com/chaoss/grimoirelab-elk
+$ cd grimoirelab-elk
+```
+
+Then use pip or Poetry to install the package along with its dependencies.
+
+#### Pip
+To install the package from local directory run the following command:
+```
+$ pip install .
+```
+In case you are a developer, you should install GrimoireELK in editable mode:
+```
+$ pip install -e .
+```
+
+#### Poetry
+We use [poetry](https://python-poetry.org/) for dependency management and 
+packaging. You can install it following its [documentation](https://python-poetry.org/docs/#installation).
+Once you have installed it, you can install GrimoireELK and the dependencies in 
+a project isolated environment using:
+```
+$ poetry install
+```
+To spaw a new shell within the virtual environment use:
+```
+$ poetry shell
+```
+
 ## Running tests
 
-Tests are located in the folder [tests](https://github.com/chaoss/grimoirelab-elk/tree/master/tests). In order to run them, you need to have in your machine:
-- instances (or Docker containers) of ElasticSearch and MySQL
-- the [dependencies](https://github.com/chaoss/grimoirelab-elk/blob/master/requirements.txt) installed or available (the latter applies to the dependencies with the other GrimoireLab repositories).
+Tests are located in the folder [tests](https://github.com/chaoss/grimoirelab-elk/tree/master/tests). 
+In order to run them, you need to have in your machine instances (or Docker containers) of ElasticSearch and MySQL
 
 Then you need to:
 - update the file [tests.conf](https://github.com/chaoss/grimoirelab-elk/blob/master/tests/tests.conf) file:
-  - in case your ElasticSearch instance isn't available at http://localhost:9200. For example, if you are using the secure edition of elasticsearch, it will be located at https://admin:admin@localhost:9200
+  - in case your ElasticSearch instance isn't available at `http://localhost:9200`. For example, if you are using the secure edition of elasticsearch, it will be located at `https://admin:admin@localhost:9200`
   - in case you are using non-default credentials for your SortingHat database, you will need to include the `[Database]` section of the file with both `user` and `password` parameters
 - create the databases `test_sh` and `test_projects` in your MySQL instance (e.g., `mysql -u root -e "create database test_sh"`, if you are running mysql in a container use `docker exec -i <container id> mysql -u root -e "create database test_sh"`)
 - populate the database `test_projects` with the SQL file [test_projects.sql](https://github.com/chaoss/grimoirelab-elk/blob/master/tests/test_projects.sql) (e.g., `mysql -u root test_projects < tests/test_projects.sql`)
 
 The full battery of tests can be executed with [run_tests.py](https://github.com/chaoss/grimoirelab-elk/blob/master/tests/run_tests.py). However, it is also possible to execute
 a sub-set of tests by running the single test files (`test_*` files in the [tests folder](https://github.com/chaoss/grimoirelab-elk/tree/master/tests))
 
@@ -177,8 +240,7 @@
 ```buildoutcfg
 Name                                                                                                                Stmts   Miss  Cover   Missing
 --------------------------------------------------------------------------------------------------------------------------------------------------
 .../ELK/grimoire_elk/__init__.py                                                                                       4      0   100%
 .../ELK/grimoire_elk/_version.py                                                                                       1      0   100%
 ```
 
-
```

### Comparing `grimoire-elk-0.99.0/LICENSE` & `grimoire_elk-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.99.0/grimoire_elk/errors.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/meetup.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/meetup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -273,15 +273,15 @@
             identity = self.get_sh_identity(item['member'])
         elif 'event_hosts' in item:
             # meetup event
             identity = self.get_sh_identity(item['event_hosts'][0])
         else:
             return sh_fields
 
-        created = unixtime_to_datetime(item['created'] / 1000)
+        created = unixtime_to_datetime(item['created'] / 1000).isoformat()
         if self.sortinghat:
             sh_fields = self.get_item_sh_fields(identity, created)
         else:
             sh_fields = self.get_item_no_sh_fields(identity, 'author')
 
         return sh_fields
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/puppetforge.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/puppetforge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/gitlab.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/gitlab.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -70,18 +70,21 @@
 class GitLabEnrich(Enrich):
 
     mapping = Mapping
 
     issue_roles = ['author', 'assignee']
     merge_roles = ['author']
 
-    def __init__(self, db_sortinghat=None, db_projects_map=None, json_projects_map=None,
-                 db_user='', db_password='', db_host=''):
-        super().__init__(db_sortinghat, db_projects_map, json_projects_map,
-                         db_user, db_password, db_host)
+    def __init__(self, db_sortinghat=None, json_projects_map=None,
+                 db_user='', db_password='', db_host='', db_path=None,
+                 db_port=None, db_ssl=False, db_verify_ssl=True, db_tenant=None):
+        super().__init__(db_sortinghat=db_sortinghat, json_projects_map=json_projects_map,
+                         db_user=db_user, db_password=db_password, db_host=db_host,
+                         db_port=db_port, db_path=db_path, db_ssl=db_ssl, db_verify_ssl=db_verify_ssl,
+                         db_tenant=db_tenant)
 
         self.users = {}  # cache users
         self.studies = []
         self.studies.append(self.enrich_onion)
 
     def set_elastic(self, elastic):
         self.elastic = elastic
@@ -372,29 +375,30 @@
 
             if start_date_str:
                 eitem['milestone_start_date'] = str_to_datetime(start_date_str).replace(tzinfo=None).isoformat()
 
             if due_date_str:
                 eitem['milestone_due_date'] = str_to_datetime(due_date_str).replace(tzinfo=None).isoformat()
 
-    def enrich_onion(self, ocean_backend, enrich_backend,
+    def enrich_onion(self, ocean_backend, enrich_backend, alias,
                      in_index, out_index, data_source=None, no_incremental=False,
                      contribs_field='uuid',
                      timeframe_field='grimoire_creation_date',
                      sort_on_field='metadata__timestamp',
                      seconds=Enrich.ONION_INTERVAL):
 
         if not data_source:
             raise ELKError(cause="Missing data_source attribute")
 
         if data_source not in [GITLAB_MERGES, GITLAB_ISSUES]:
             logger.warning("[gitlab] data source value {} should be: {} or {}".format(
                            data_source, GITLAB_ISSUES, GITLAB_MERGES))
 
         super().enrich_onion(enrich_backend=enrich_backend,
+                             alias=alias,
                              in_index=in_index,
                              out_index=out_index,
                              data_source=data_source,
                              contribs_field=contribs_field,
                              timeframe_field=timeframe_field,
                              sort_on_field=sort_on_field,
                              no_incremental=no_incremental,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/github.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/github.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2020 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -100,18 +100,21 @@
 
     mapping = Mapping
 
     issue_roles = ['assignee_data', 'user_data']
     pr_roles = ['merged_by_data', 'user_data']
     roles = ['assignee_data', 'merged_by_data', 'user_data']
 
-    def __init__(self, db_sortinghat=None, db_projects_map=None, json_projects_map=None,
-                 db_user='', db_password='', db_host=''):
-        super().__init__(db_sortinghat, db_projects_map, json_projects_map,
-                         db_user, db_password, db_host)
+    def __init__(self, db_sortinghat=None, json_projects_map=None,
+                 db_user='', db_password='', db_host='', db_path=None,
+                 db_port=None, db_ssl=False, db_verify_ssl=True, db_tenant=None):
+        super().__init__(db_sortinghat=db_sortinghat, json_projects_map=json_projects_map,
+                         db_user=db_user, db_password=db_password, db_host=db_host,
+                         db_port=db_port, db_path=db_path, db_ssl=db_ssl, db_verify_ssl=db_verify_ssl,
+                         db_tenant=db_tenant)
 
         self.studies = []
         self.studies.append(self.enrich_onion)
         self.studies.append(self.enrich_pull_requests)
         self.studies.append(self.enrich_geolocation)
         self.studies.append(self.enrich_extra_data)
         self.studies.append(self.enrich_backlog_analysis)
@@ -231,43 +234,45 @@
             logger.error("[github] rich item not defined for GitHub category {}".format(
                          item['category']))
 
         self.add_repository_labels(rich_item)
         self.add_metadata_filter_raw(rich_item)
         return rich_item
 
-    def enrich_demography(self, ocean_backend, enrich_backend, date_field="grimoire_creation_date",
+    def enrich_demography(self, ocean_backend, enrich_backend, alias, date_field="grimoire_creation_date",
                           author_field="author_uuid"):
 
-        super().enrich_demography(ocean_backend, enrich_backend, date_field, author_field=author_field)
+        super().enrich_demography(ocean_backend, enrich_backend, alias, date_field, author_field=author_field)
 
-    def enrich_onion(self, ocean_backend, enrich_backend,
+    def enrich_onion(self, ocean_backend, enrich_backend, alias,
                      no_incremental=False,
                      in_index_iss='github_issues_onion-src',
                      in_index_prs='github_prs_onion-src',
                      out_index_iss='github_issues_onion-enriched',
                      out_index_prs='github_prs_onion-enriched',
                      data_source_iss='github-issues',
                      data_source_prs='github-prs',
                      contribs_field='uuid',
                      timeframe_field='grimoire_creation_date',
                      sort_on_field='metadata__timestamp',
                      seconds=Enrich.ONION_INTERVAL):
 
         super().enrich_onion(enrich_backend=enrich_backend,
+                             alias=alias,
                              in_index=in_index_iss,
                              out_index=out_index_iss,
                              data_source=data_source_iss,
                              contribs_field=contribs_field,
                              timeframe_field=timeframe_field,
                              sort_on_field=sort_on_field,
                              no_incremental=no_incremental,
                              seconds=seconds)
 
         super().enrich_onion(enrich_backend=enrich_backend,
+                             alias=alias,
                              in_index=in_index_prs,
                              out_index=out_index_prs,
                              data_source=data_source_prs,
                              contribs_field=contribs_field,
                              timeframe_field=timeframe_field,
                              sort_on_field=sort_on_field,
                              no_incremental=no_incremental,
@@ -783,15 +788,15 @@
             repository_name = repository_url.split("/")[-1]
 
             logger.debug("[enrich-backlog-analysis] Start analysis for {}".format(repository_url))
 
             # get each day since repository creation
             dates = es_in.search(
                 index=in_index,
-                body=get_issues_dates(interval_days, repository_url)
+                body=get_issues_dates(self.elastic, interval_days, repository_url)
             )['aggregations']['created_per_interval'].get("buckets", [])
 
             # for each selected label + others labels
             for label, other in [("", True)] + [(label, False) for label in reduced_labels]:
                 # compute metrics for each day (ES request for each day)
                 evolution_items = []
                 for date in map(lambda i: i['key_as_string'], dates):
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/discourse.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/discourse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -58,18 +58,21 @@
         return {"items": mapping}
 
 
 class DiscourseEnrich(Enrich):
 
     mapping = Mapping
 
-    def __init__(self, db_sortinghat=None, db_projects_map=None, json_projects_map=None,
-                 db_user='', db_password='', db_host=''):
-        super().__init__(db_sortinghat, db_projects_map, json_projects_map,
-                         db_user, db_password, db_host)
+    def __init__(self, db_sortinghat=None, json_projects_map=None,
+                 db_user='', db_password='', db_host='', db_path=None,
+                 db_port=None, db_ssl=False, db_verify_ssl=True, db_tenant=None):
+        super().__init__(db_sortinghat=db_sortinghat, json_projects_map=json_projects_map,
+                         db_user=db_user, db_password=db_password, db_host=db_host,
+                         db_port=db_port, db_path=db_path, db_ssl=db_ssl, db_verify_ssl=db_verify_ssl,
+                         db_tenant=db_tenant)
         self.categories = {}  # Map from category_id to category_name
         self.categories_tree = {}  # Categories with subcategories
 
     def get_identities(self, item):
         """ Return the identities from an item """
 
         # All identities are in the post stream
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/mozillaclub.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mozillaclub.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/dockerhub.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/dockerhub.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/study_ceres_aoc.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/study_ceres_aoc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -24,14 +24,15 @@
 from elasticsearch import helpers
 
 from cereslib.dfutils.filter import FilterRows
 from cereslib.enrich.enrich import FileType, FilePath, ToUTF8
 from cereslib.events.events import Git, Events
 
 from grimoire_elk.enriched.ceres_base import ESConnector, CeresBase
+from grimoire_elk.elastic import ElasticSearch
 
 
 logger = logging.getLogger(__name__)
 
 
 class ESPandasConnector(ESConnector):
     """ElasticSearch connector to ease data management with Pandas library.
@@ -128,15 +129,15 @@
             doc = {
                 "_index": self._es_index,
                 "_type": "items",
                 "_id": item_id,
                 "_source": row
             }
 
-            if self._es_major == '7':
+            if not ElasticSearch.is_legacy_static(self._es_major, self._es_distribution):
                 doc.pop('_type')
 
             docs.append(doc)
         # TODO exception and error handling
         chunk_size = 2000
         chunks = [docs[i:i + chunk_size] for i in range(0, len(docs), chunk_size)]
         for chunk in chunks:
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/git.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/git.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -34,23 +34,21 @@
                                           str_to_datetime,
                                           datetime_utcnow)
 from perceval.backends.core.git import (GitCommand,
                                         GitRepository,
                                         EmptyRepositoryError,
                                         RepositoryError)
 from .enrich import Enrich, metadata
-from .sortinghat_gelk import SortingHat
 from .study_ceres_aoc import areas_of_code, ESPandasConnector
 from ..elastic_mapping import Mapping as BaseMapping
 from ..elastic_items import HEADER_JSON, MAX_BULK_UPDATE_SIZE
 from .utils import anonymize_url
 
 GITHUB = 'https://github.com/'
 DEMOGRAPHY_COMMIT_MIN_DATE = '1980-01-01'
-AREAS_OF_CODE_ALIAS = 'git_areas_of_code'
 logger = logging.getLogger(__name__)
 
 
 class Mapping(BaseMapping):
 
     @staticmethod
     def get_elastic_mappings(es_major):
@@ -75,32 +73,37 @@
 
 class GitEnrich(Enrich):
 
     mapping = Mapping
 
     # REGEX to extract authors from a multi author commit: several authors present
     # in the Author field in the commit. Used if self.pair_programming is True
-    AUTHOR_P2P_REGEX = re.compile(r'(?P<first_authors>.* .*) and (?P<last_author>.* .*) (?P<email>.*)')
+    AUTHOR_P2P_REGEX = re.compile(r'(?P<first_authors>.* .*) ([aA][nN][dD]|&|\+) (?P<last_author>.* .*) (?P<email>.*)')
     AUTHOR_P2P_NEW_REGEX = re.compile(r"Co-authored-by:(?P<first_authors>.* .*)<(?P<email>.*)>\n?")
 
     # REGEX to extract authors from the commit
     AUTHOR_REGEX = re.compile(r'^\s*(?P<field>.*): (?P<author>.* <.*>)$')
 
     GIT_AOC_ENRICHED = "git_aoc-enriched"
 
     roles = ['Author', 'Commit']
-    meta_fields = ['acked_by_multi', 'co_developed_by_multi', 'reported_by_multi', 'reviewed_by_multi',
-                   'signed_off_by_multi', 'suggested_by_multi', 'tested_by_multi']
+    meta_fields = ['acked_by_multi', 'approved_by_multi', 'co_authored_by_multi', 'co_developed_by_multi',
+                   'merged_by_multi', 'reported_by_multi', 'reviewed_by_multi', 'signed_off_by_multi',
+                   'suggested_by_multi', 'tested_by_multi']
     meta_fields_suffixes = ['_bots', '_domains', '_names', '_org_names', '_uuids']
     meta_non_authored_prefix = 'non_authored_'
 
-    def __init__(self, db_sortinghat=None, db_projects_map=None, json_projects_map=None,
-                 db_user='', db_password='', db_host='', pair_programming=False):
-        super().__init__(db_sortinghat, db_projects_map, json_projects_map,
-                         db_user, db_password, db_host)
+    def __init__(self, db_sortinghat=None, json_projects_map=None,
+                 db_user='', db_password='', db_host='', db_path=None,
+                 db_port=None, db_ssl=False, db_verify_ssl=True, db_tenant=None,
+                 pair_programming=False):
+        super().__init__(db_sortinghat=db_sortinghat, json_projects_map=json_projects_map,
+                         db_user=db_user, db_password=db_password, db_host=db_host,
+                         db_port=db_port, db_path=db_path, db_ssl=db_ssl, db_verify_ssl=db_verify_ssl,
+                         db_tenant=db_tenant)
 
         self.studies = []
         self.studies.append(self.enrich_demography)
         self.studies.append(self.enrich_areas_of_code)
         self.studies.append(self.enrich_onion)
         self.studies.append(self.enrich_git_branches)
         self.studies.append(self.enrich_forecast_activity)
@@ -204,17 +207,14 @@
         eitem = {}
         self.copy_raw_fields(self.RAW_FIELDS_COPY, item, eitem)
         # For pair programming uuid is not a unique field. Use git_uuid in general as unique field.
         eitem['git_uuid'] = eitem['uuid']
         # The real data
         commit = item['data']
 
-        self.__fix_field_date(commit, 'AuthorDate')
-        self.__fix_field_date(commit, 'CommitDate')
-
         # data fields to copy
         copy_fields = ["message"]
         for f in copy_fields:
             if f in commit:
                 eitem[f] = commit[f]
             else:
                 eitem[f] = None
@@ -230,16 +230,17 @@
             eitem['message'] = commit['message'][:self.KEYWORD_MAX_LENGTH]
 
         if 'refs' in commit:
             eitem["commit_tags"] = list(filter(lambda r: "tag: " in r, commit['refs']))
 
         eitem['hash_short'] = eitem['hash'][0:6]
         # Enrich dates
-        author_date = str_to_datetime(commit["AuthorDate"])
-        commit_date = str_to_datetime(commit["CommitDate"])
+
+        author_date = self.__cast_str_to_datetime(commit, 'AuthorDate')
+        commit_date = self.__cast_str_to_datetime(commit, 'CommitDate')
 
         eitem["author_date"] = author_date.replace(tzinfo=None).isoformat()
         eitem["commit_date"] = commit_date.replace(tzinfo=None).isoformat()
 
         eitem["author_date_weekday"] = author_date.replace(tzinfo=None).isoweekday()
         eitem["author_date_hour"] = author_date.replace(tzinfo=None).hour
 
@@ -317,42 +318,44 @@
         if 'project' in item:
             eitem['project'] = item['project']
 
         # Adding the git author domain
         author_domain = self.get_identity_domain(self.get_sh_identity(item, 'Author'))
         eitem['git_author_domain'] = author_domain
 
-        eitem.update(self.get_grimoire_fields(commit["AuthorDate"], "commit"))
+        grimoire_fields = self.get_grimoire_fields(author_date, "commit")
+        eitem.update(grimoire_fields)
 
         # grimoire_creation_date is needed in the item
-        item.update(self.get_grimoire_fields(commit["AuthorDate"], "commit"))
+        item.update(grimoire_fields)
         eitem.update(self.get_item_sh(item, self.roles))
 
         if self.prjs_map:
             eitem.update(self.get_item_project(eitem))
 
         if self.pair_programming:
             eitem = self.__add_pair_programming_metrics(commit, eitem)
 
         self.add_repository_labels(eitem)
         self.add_metadata_filter_raw(eitem)
         self.__add_commit_meta_fields(eitem, commit)
         return eitem
 
-    def __fix_field_date(self, item, attribute):
-        """Fix possible errors in the field date"""
+    def __cast_str_to_datetime(self, item, attribute):
+        """Convert str to datetime fixing possible errors"""
 
         field_date = str_to_datetime(item[attribute])
 
         try:
             _ = int(field_date.strftime("%z")[0:3])
         except ValueError:
             logger.warning("[git] {} in commit {} has a wrong format".format(
                            attribute, item['commit']))
-            item[attribute] = field_date.replace(tzinfo=None).isoformat()
+            return field_date.replace(tzinfo=None).isoformat()
+        return field_date
 
     def __add_commit_meta_fields(self, eitem, commit):
         """Add commit meta fields as signed_off_by, reviwed_by, tested_by, etc."""
         non_authored = []
         if self.meta_non_authored_prefix:
             non_authored = [self.meta_non_authored_prefix + field for field in self.meta_fields]
         all_meta_fields = self.meta_fields + non_authored
@@ -375,16 +378,25 @@
                 continue
 
             author = m.group('author')
             identity = self.get_sh_identity(author)
 
             if self.sortinghat:
                 # Create SH identity if it does not exist
-                SortingHat.add_identity(self.sh_db, identity, self.get_connector_name())
-                item_date = str_to_datetime(eitem[self.get_field_date()])
+                backend_name = self.get_sh_backend_name()
+                identity_id = self.generate_uuid(backend_name,
+                                                 email=identity['email'],
+                                                 name=identity['name'],
+                                                 username=identity['username'])
+                individual = self.get_entity(identity_id)
+                if not individual:
+                    identity_tuple = tuple(identity.items())
+                    self.add_sh_identity_cache(identity_tuple)
+                    logger.debug("Create a new individual {} in commit_meta_fields".format(identity_id))
+                item_date = eitem[self.get_field_date()]
                 sh_fields = self.get_item_sh_fields(identity, item_date, rol=meta_field)
             else:
                 sh_fields = self.get_item_no_sh_fields(identity, rol=meta_field)
 
             uuid = sh_fields[meta_field + '_uuid']
             self.add_meta_fields(eitem, meta_eitem, sh_fields, meta_field, uuid, self.meta_fields_suffixes,
                                  self.meta_non_authored_prefix)
@@ -485,14 +497,15 @@
                 m = self.AUTHOR_P2P_REGEX.match(item['data']['Author'])
                 n = self.AUTHOR_P2P_NEW_REGEX.match(item['data']['Author'])
                 if m or n:
                     logger.debug("[git] Multiauthor detected. Creating one commit "
                                  "per author: {}".format(item['data']['Author']))
                     item['data']['authors'] = self.__get_authors(item['data']['Author'])
                     item['data']['Author'] = item['data']['authors'][0]
+                    item['data']['is_git_commit_multi_author'] = 1
                 m = self.AUTHOR_P2P_REGEX.match(item['data']['Commit'])
                 n = self.AUTHOR_P2P_NEW_REGEX.match(item['data']['Author'])
                 if m or n:
                     logger.debug("[git] Multicommitter detected: using just the first committer")
                     item['data']['committers'] = self.__get_authors(item['data']['Commit'])
                     item['data']['Commit'] = item['data']['committers'][0]
                 # Add the authors list using the original Author and the Signed-off list
@@ -527,18 +540,17 @@
                     # First author already added in the above commit
                     authors = item['data']['authors']
                     for i in range(1, len(authors)):
                         # logger.debug('Adding a new commit for %s', authors[i])
                         item['data']['Author'] = authors[i]
                         item['data']['is_git_commit_multi_author'] = 1
                         rich_item = self.get_rich_item(item)
-                        item['data']['is_git_commit_multi_author'] = 1
-                        data_json = json.dumps(rich_item)
                         commit_id = item["uuid"] + "_" + str(i - 1)
                         rich_item['git_uuid'] = commit_id
+                        data_json = json.dumps(rich_item)
                         bulk_json += '{"index" : {"_id" : "%s" } }\n' % rich_item['git_uuid']
                         bulk_json += data_json + "\n"  # Bulk document
                         current += 1
                         total_multi_author += 1
 
                 if rich_item['Signed-off-by_number'] > 0:
                     nsg = 0
@@ -571,20 +583,20 @@
 
         if self.pair_programming:
             logger.info("[git] Signed-off commits generated: {}".format(total_signed_off))
             logger.info("[git] Multi author commits generated: {}".format(total_multi_author))
 
         return total
 
-    def enrich_demography(self, ocean_backend, enrich_backend, date_field="grimoire_creation_date",
+    def enrich_demography(self, ocean_backend, enrich_backend, alias, date_field="grimoire_creation_date",
                           author_field="author_uuid"):
 
-        super().enrich_demography(ocean_backend, enrich_backend, date_field, author_field=author_field)
+        super().enrich_demography(ocean_backend, enrich_backend, alias, date_field, author_field=author_field)
 
-    def enrich_areas_of_code(self, ocean_backend, enrich_backend, no_incremental=False,
+    def enrich_areas_of_code(self, ocean_backend, enrich_backend, alias, no_incremental=False,
                              in_index="git-raw",
                              out_index=GIT_AOC_ENRICHED,
                              sort_on_field='metadata__timestamp'):
 
         log_prefix = "[git] study areas_of_code"
 
         logger.info("{} Starting study - Input: {} Output: {}".format(log_prefix, in_index, out_index))
@@ -600,15 +612,15 @@
         out_conn = ESPandasConnector(es_conn=es_out, es_index=out_index, sort_on_field=sort_on_field, read_only=False)
 
         exists_index = out_conn.exists()
         if no_incremental or not exists_index:
             logger.info("{} Creating out ES index".format(log_prefix))
             # Initialize out index
 
-            if self.elastic.major == '7':
+            if not self.elastic.is_legacy():
                 filename = pkg_resources.resource_filename('grimoire_elk', 'enriched/mappings/git_aoc_es7.json')
             else:
                 filename = pkg_resources.resource_filename('grimoire_elk', 'enriched/mappings/git_aoc.json')
             out_conn.create_index(filename, delete=exists_index)
 
         repos = []
         for source in self.json_projects.values():
@@ -626,20 +638,20 @@
 
             # delete the documents in the AOC index which correspond to commits that don't exist in the raw index
             if out_conn.exists():
                 self.update_items_aoc(ocean_backend, es_out, out_index, repo_name)
 
         # Create alias if output index exists and alias does not
         if out_conn.exists():
-            if not out_conn.exists_alias(AREAS_OF_CODE_ALIAS) \
-                    and not enrich_backend.elastic.alias_in_use(AREAS_OF_CODE_ALIAS):
-                logger.info("{} creating alias: {}".format(log_prefix, AREAS_OF_CODE_ALIAS))
-                out_conn.create_alias(AREAS_OF_CODE_ALIAS)
+            if not out_conn.exists_alias(alias) \
+                    and not enrich_backend.elastic.alias_in_use(alias):
+                logger.info("{} creating alias: {}".format(log_prefix, alias))
+                out_conn.create_alias(alias)
             else:
-                logger.warning("{} alias already exists: {}.".format(log_prefix, AREAS_OF_CODE_ALIAS))
+                logger.warning("{} alias already exists: {}.".format(log_prefix, alias))
 
         logger.info("{} end".format(log_prefix))
 
     def get_unique_hashes_aoc(self, es_aoc, index_aoc, repository):
         """Retrieve the unique commit hashes in the AOC index
 
         :param es_aoc: the ES object to access AOC data
@@ -768,25 +780,26 @@
         if to_process:
             # delete documents from the AOC index
             self.remove_commits(to_process, aoc_index_url, 'hash', repository)
 
         logger.debug("[git] study areas_of_code {} commits deleted from {} with origin {}.".format(
             len(hashes_to_delete), anonymize_url(aoc_index_url), repository))
 
-    def enrich_onion(self, ocean_backend, enrich_backend,
+    def enrich_onion(self, ocean_backend, enrich_backend, alias,
                      no_incremental=False,
                      in_index='git_onion-src',
                      out_index='git_onion-enriched',
                      data_source='git',
                      contribs_field='hash',
                      timeframe_field='grimoire_creation_date',
                      sort_on_field='metadata__timestamp',
                      seconds=Enrich.ONION_INTERVAL):
 
         super().enrich_onion(enrich_backend=enrich_backend,
+                             alias=alias,
                              in_index=in_index,
                              out_index=out_index,
                              data_source=data_source,
                              contribs_field=contribs_field,
                              timeframe_field=timeframe_field,
                              sort_on_field=sort_on_field,
                              no_incremental=no_incremental,
@@ -935,16 +948,19 @@
 
             for url in urls:
                 if '--filter-no-collection=true' in url:
                     # Skip study when --filter-no-collection is present
                     logger.info("[git] study git-branches skipping repo {}".format(anonymize_url(url)))
                     continue
                 cmd = GitCommand(*[url])
-
-                git_repo = GitRepository(cmd.parsed_args.uri, cmd.parsed_args.gitpath)
+                try:
+                    git_repo = GitRepository(cmd.parsed_args.uri, cmd.parsed_args.gitpath)
+                except RepositoryError:
+                    logger.error("[git] study git-branches skipping not cloned repo {}".format(anonymize_url(url)))
+                    continue
 
                 logger.debug("[git] study git-branches delete branch info for repo {} in index {}".format(
                              git_repo.uri, anonymize_url(enrich_backend.elastic.index_url)))
                 self.delete_commit_branches(git_repo, enrich_backend)
 
                 logger.debug("[git] study git-branches add branch info for repo {} in index {}".format(
                              git_repo.uri, anonymize_url(enrich_backend.elastic.index_url)))
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/remo.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/remo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -54,18 +54,21 @@
         return {"items": mapping}
 
 
 class ReMoEnrich(Enrich):
 
     mapping = Mapping
 
-    def __init__(self, db_sortinghat=None, db_projects_map=None, json_projects_map=None,
-                 db_user='', db_password='', db_host=''):
-        super().__init__(db_sortinghat, db_projects_map, json_projects_map,
-                         db_user, db_password, db_host)
+    def __init__(self, db_sortinghat=None, json_projects_map=None,
+                 db_user='', db_password='', db_host='', db_path=None,
+                 db_port=None, db_ssl=False, db_verify_ssl=True, db_tenant=None):
+        super().__init__(db_sortinghat=db_sortinghat, json_projects_map=json_projects_map,
+                         db_user=db_user, db_password=db_password, db_host=db_host,
+                         db_port=db_port, db_path=db_path, db_ssl=db_ssl, db_verify_ssl=db_verify_ssl,
+                         db_tenant=db_tenant)
         self.author = "user"  # changes if we are generating events
 
     def get_field_author(self):
         return self.author
 
     def get_identities(self, item):
         """Return the identities from an item"""
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/rocketchat.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/rocketchat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2020 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/mediawiki.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mediawiki.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -111,15 +111,15 @@
 
         return identity
 
     def get_review_sh(self, revision, item):
         """ Add sorting hat enrichment fields for the author of the revision """
 
         identity = self.get_sh_identity(revision)
-        update = str_to_datetime(item[self.get_field_date()])
+        update = item[self.get_field_date()]
         erevision = self.get_item_sh_fields(identity, update)
 
         return erevision
 
     def get_rich_item_reviews(self, item):
         erevisions = []
         eitem = {}
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/groupsio.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/groupsio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/kitsune.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/kitsune.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -47,28 +47,40 @@
                 "content_analyzed": {
                   "type": "text",
                   "index": true
                 },
                 "tags_analyzed": {
                   "type": "text",
                   "index": true
+                },
+                "id": {
+                  "type": "keyword"
                 }
            }
         } """
 
         return {"items": mapping}
 
 
 class KitsuneEnrich(Enrich):
 
-    mappping = Mapping
+    mapping = Mapping
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        self.studies = []
+        self.studies.append(self.enrich_demography)
 
     def get_field_author(self):
         return "creator"
 
+    def get_field_unique_id(self):
+        return "id"
+
     def get_sh_identity(self, item, identity_field=None):
         identity = {}
 
         user = item
         if isinstance(item, dict) and 'data' in item:
             user = item['data'][identity_field]
         elif identity_field in item:
@@ -142,14 +154,16 @@
             # Enrich dates
             eitem["creation_date"] = str_to_datetime(question["created"]).isoformat()
             eitem["last_activity_date"] = str_to_datetime(question["updated"]).isoformat()
 
             eitem['lifetime_days'] = \
                 get_time_diff_days(question['created'], question['updated'])
 
+            # Add id info to allow to coexistence of items of different types in the same index
+            eitem['id'] = 'question_{}'.format(question['id'])
             eitem.update(self.get_grimoire_fields(question['created'], "question"))
 
             eitem['author'] = question['creator']['username']
             if question['creator']['display_name']:
                 eitem['author'] = question['creator']['display_name']
 
             if self.sortinghat:
@@ -190,14 +204,16 @@
             # Enrich dates
             eitem["creation_date"] = str_to_datetime(answer["created"]).isoformat()
             eitem["last_activity_date"] = str_to_datetime(answer["updated"]).isoformat()
 
             eitem['lifetime_days'] = \
                 get_time_diff_days(answer['created'], answer['updated'])
 
+            # Add id info to allow to coexistence of items of different types in the same index
+            eitem['id'] = 'question_{}_answer_{}'.format(answer['question'], answer['id'])
             eitem.update(self.get_grimoire_fields(answer['created'], "answer"))
 
             eitem['author'] = answer['creator']['username']
             if answer['creator']['display_name']:
                 eitem['author'] = answer['creator']['display_name']
 
             if self.sortinghat:
@@ -227,30 +243,31 @@
                 total += self.elastic.safe_put_bulk(url, bulk_json)
                 bulk_json = ""
                 current = 0
 
             rich_item = self.get_rich_item(item)
             data_json = json.dumps(rich_item)
             bulk_json += '{"index" : {"_id" : "%s" } }\n' % \
-                (item[self.get_field_unique_id()])
+                (rich_item[self.get_field_unique_id()])
             bulk_json += data_json + "\n"  # Bulk document
             current += 1
             # Time to enrich also de answers
             if 'answers_data' in item['data']:
                 for answer in item['data']['answers_data']:
                     # Add question title in answers
                     answer['title'] = item['data']['title']
                     answer['solution'] = 0
                     if answer['id'] == item['data']['solution']:
                         answer['solution'] = 1
                     rich_answer = self.get_rich_item(answer, kind='answer')
+                    self.copy_raw_fields(self.RAW_FIELDS_COPY, item, rich_answer)
+
                     data_json = json.dumps(rich_answer)
-                    bulk_json += '{"index" : {"_id" : "%s_%i" } }\n' % \
-                        (item[self.get_field_unique_id()],
-                         rich_answer['answer_id'])
+                    bulk_json += '{"index" : {"_id" : "%s" } }\n' % \
+                                 (rich_answer[self.get_field_unique_id()])
                     bulk_json += data_json + "\n"  # Bulk document
                     current += 1
 
         if current > 0:
             total += self.elastic.safe_put_bulk(url, bulk_json)
 
         return total
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/ceres_base.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/ceres_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -151,14 +151,15 @@
         self._es_index = es_index
         self._sort_on_field = sort_on_field
         self._repo = repo
         self._read_only = read_only
         self.__log_prefix = "[" + es_index + "] study "
 
         self._es_major = self._es_conn.info()['version']['number'].split('.')[0]
+        self._es_distribution = self._es_conn.info()['version'].get('distribution', 'elasticsearch')
 
     def update_repo(self, repo):
         self._repo = repo
 
     def read_item(self, from_date=None):
         """Read items and return them one by one.
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/mbox_study_kip.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mbox_study_kip.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/redmine.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/redmine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/rss.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/rss.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/gitter.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/gitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2020 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -59,18 +59,21 @@
 class GitterEnrich(Enrich):
 
     mapping = Mapping
 
     # REGEX to extract links from HTML text
     HTML_LINK_REGEX = re.compile("href=[\"\'](.*?)[\"\']")
 
-    def __init__(self, db_sortinghat=None, db_projects_map=None, json_projects_map=None,
-                 db_user='', db_password='', db_host=''):
-        super().__init__(db_sortinghat, db_projects_map, json_projects_map,
-                         db_user, db_password, db_host)
+    def __init__(self, db_sortinghat=None, json_projects_map=None,
+                 db_user='', db_password='', db_host='', db_path=None,
+                 db_port=None, db_ssl=False, db_verify_ssl=True, db_tenant=None):
+        super().__init__(db_sortinghat=db_sortinghat, json_projects_map=json_projects_map,
+                         db_user=db_user, db_password=db_password, db_host=db_host,
+                         db_port=db_port, db_path=db_path, db_ssl=db_ssl, db_verify_ssl=db_verify_ssl,
+                         db_tenant=db_tenant)
 
     def get_field_author(self):
         return "fromUser"
 
     def get_sh_identity(self, item, identity_field=None):
         # email not available for gitter
         identity = {
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/stackexchange.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/stackexchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/jira.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/jira.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -110,20 +110,18 @@
         """Add sorting hat enrichment fields"""
 
         eitem_sh = {}
 
         if not self.sortinghat:
             return eitem_sh
 
-        created = str_to_datetime(date_field)
-
         for rol in roles:
             identity = self.get_sh_identity(item, rol)
 
-            eitem_sh.update(self.get_item_sh_fields(identity, created, rol=rol))
+            eitem_sh.update(self.get_item_sh_fields(identity, date_field, rol=rol))
 
             if not eitem_sh[rol + '_org_name']:
                 eitem_sh[rol + '_org_name'] = SH_UNKNOWN_VALUE
 
             if not eitem_sh[rol + '_name']:
                 eitem_sh[rol + '_name'] = SH_UNKNOWN_VALUE
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/gerrit.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/gerrit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2020 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -83,18 +83,21 @@
         return {"items": mapping}
 
 
 class GerritEnrich(Enrich):
 
     mapping = Mapping
 
-    def __init__(self, db_sortinghat=None, db_projects_map=None, json_projects_map=None,
-                 db_user='', db_password='', db_host=''):
-        super().__init__(db_sortinghat, db_projects_map, json_projects_map,
-                         db_user, db_password, db_host)
+    def __init__(self, db_sortinghat=None, json_projects_map=None,
+                 db_user='', db_password='', db_host='', db_path=None,
+                 db_port=None, db_ssl=False, db_verify_ssl=True, db_tenant=None):
+        super().__init__(db_sortinghat=db_sortinghat, json_projects_map=json_projects_map,
+                         db_user=db_user, db_password=db_password, db_host=db_host,
+                         db_port=db_port, db_path=db_path, db_ssl=db_ssl, db_verify_ssl=db_verify_ssl,
+                         db_tenant=db_tenant)
 
         self.studies = []
         self.studies.append(self.enrich_demography)
         self.studies.append(self.enrich_demography_contribution)
         self.studies.append(self.enrich_onion)
 
     roles = ["author", "by", "changeset_author", "reviewer", "uploader"]
@@ -703,35 +706,36 @@
             missing = num_items - ins_items
             logger.error("[gerrit] {}/{} missing items".format(missing, num_items))
         else:
             logger.info("[gerrit] {} items inserted".format(num_items))
 
         return num_items
 
-    def enrich_demography(self, ocean_backend, enrich_backend, date_field="grimoire_creation_date",
+    def enrich_demography(self, ocean_backend, enrich_backend, alias, date_field="grimoire_creation_date",
                           author_field="author_uuid"):
 
-        super().enrich_demography(ocean_backend, enrich_backend, date_field, author_field=author_field)
+        super().enrich_demography(ocean_backend, enrich_backend, alias, date_field, author_field=author_field)
 
-    def enrich_demography_contribution(self, ocean_backend, enrich_backend, date_field="grimoire_creation_date",
+    def enrich_demography_contribution(self, ocean_backend, enrich_backend, alias, date_field="grimoire_creation_date",
                                        author_field="author_uuid"):
 
-        super().enrich_demography_contribution(ocean_backend, enrich_backend, date_field, author_field=author_field)
+        super().enrich_demography_contribution(ocean_backend, enrich_backend, alias, date_field, author_field=author_field)
 
-    def enrich_onion(self, ocean_backend, enrich_backend,
+    def enrich_onion(self, ocean_backend, enrich_backend, alias,
                      no_incremental=False,
                      in_index='gerrit_onion-src',
                      out_index='gerrit_onion-enriched',
                      data_source='gerrit',
                      contribs_field='uuid',
                      timeframe_field='grimoire_creation_date',
                      sort_on_field='metadata__timestamp',
                      seconds=Enrich.ONION_INTERVAL):
 
         super().enrich_onion(enrich_backend=enrich_backend,
+                             alias=alias,
                              in_index=in_index,
                              out_index=out_index,
                              data_source=data_source,
                              contribs_field=contribs_field,
                              timeframe_field=timeframe_field,
                              sort_on_field=sort_on_field,
                              no_incremental=no_incremental,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/pipermail.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/pipermail.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/pagure.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/pagure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2020 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -68,18 +68,21 @@
 
 class PagureEnrich(Enrich):
     mapping = Mapping
 
     comment_roles = ['user']
     issue_roles = ['user', 'assignee']
 
-    def __init__(self, db_sortinghat=None, db_projects_map=None, json_projects_map=None,
-                 db_user='', db_password='', db_host=''):
-        super().__init__(db_sortinghat, db_projects_map, json_projects_map,
-                         db_user, db_password, db_host)
+    def __init__(self, db_sortinghat=None, json_projects_map=None,
+                 db_user='', db_password='', db_host='', db_path=None,
+                 db_port=None, db_ssl=False, db_verify_ssl=True, db_tenant=None):
+        super().__init__(db_sortinghat=db_sortinghat, json_projects_map=json_projects_map,
+                         db_user=db_user, db_password=db_password, db_host=db_host,
+                         db_port=db_port, db_path=db_path, db_ssl=db_ssl, db_verify_ssl=db_verify_ssl,
+                         db_tenant=db_tenant)
 
     def set_elastic(self, elastic):
         self.elastic = elastic
 
     def get_field_author(self):
         return "user"
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/githubql.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/githubql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2020 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -72,18 +72,21 @@
 
 class GitHubQLEnrich(Enrich):
 
     mapping = Mapping
 
     event_roles = ['actor', 'reporter', 'submitter']
 
-    def __init__(self, db_sortinghat=None, db_projects_map=None, json_projects_map=None,
-                 db_user='', db_password='', db_host=''):
-        super().__init__(db_sortinghat, db_projects_map, json_projects_map,
-                         db_user, db_password, db_host)
+    def __init__(self, db_sortinghat=None, json_projects_map=None,
+                 db_user='', db_password='', db_host='', db_path=None,
+                 db_port=None, db_ssl=False, db_verify_ssl=True, db_tenant=None):
+        super().__init__(db_sortinghat=db_sortinghat, json_projects_map=json_projects_map,
+                         db_user=db_user, db_password=db_password, db_host=db_host,
+                         db_port=db_port, db_path=db_path, db_ssl=db_ssl, db_verify_ssl=db_verify_ssl,
+                         db_tenant=db_tenant)
 
         self.studies = [self.enrich_duration_analysis, self.enrich_reference_analysis]
 
     def set_elastic(self, elastic):
         self.elastic = elastic
 
     def get_field_author(self):
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/google_hits.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/google_hits.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/twitter.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/twitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/dockerdeps.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/dockerdeps.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -68,18 +68,21 @@
         '''
 
         return {"items": mapping}
 
 
 class Dockerdeps(Enrich):
 
-    def __init__(self, db_sortinghat=None, db_projects_map=None, json_projects_map=None,
-                 db_user='', db_password='', db_host=''):
-        super().__init__(db_sortinghat, db_projects_map, json_projects_map,
-                         db_user, db_password, db_host)
+    def __init__(self, db_sortinghat=None, json_projects_map=None,
+                 db_user='', db_password='', db_host='', db_path=None,
+                 db_port=None, db_ssl=False, db_verify_ssl=True, db_tenant=None):
+        super().__init__(db_sortinghat=db_sortinghat, json_projects_map=json_projects_map,
+                         db_user=db_user, db_password=db_password, db_host=db_host,
+                         db_port=db_port, db_path=db_path, db_ssl=db_ssl, db_verify_ssl=db_verify_ssl,
+                         db_tenant=db_tenant)
 
         self.studies = []
 
     def get_identities(self, item):
         """ Return the identities from an item """
         identities = []
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/askbot.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/askbot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/bugzilla.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/bugzilla.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2020 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -49,14 +49,18 @@
                "main_description_analyzed": {
                     "type": "text",
                     "index": true
                },
                "summary_analyzed": {
                     "type": "text",
                     "index": true
+               },
+               "description_analyzed": {
+                    "type": "text",
+                    "index": true
                }
            }
         }"""
 
         return {"items": mapping}
 
 
@@ -167,14 +171,20 @@
             if "__text__" in issue["short_desc"][0]:
                 eitem["main_description"] = issue['short_desc'][0]['__text__'][:self.KEYWORD_MAX_LENGTH]
                 eitem["main_description_analyzed"] = issue['short_desc'][0]['__text__']
         if "summary" in issue:
             if "__text__" in issue["summary"][0]:
                 eitem["summary"] = issue['summary'][0]['__text__'][:self.KEYWORD_MAX_LENGTH]
                 eitem["summary_analyzed"] = issue['summary'][0]['__text__']
+        try:
+            eitem['description'] = issue['long_desc'][0]['thetext'][0]['__text__'][:self.KEYWORD_MAX_LENGTH]
+            eitem['description_analyzed'] = issue['long_desc'][0]['thetext'][0]['__text__']
+        except (KeyError, IndexError):
+            eitem['description'] = ""
+            eitem['description_analyzed'] = ""
 
         # Fix dates
         date_ts = str_to_datetime(issue['delta_ts'][0]['__text__'])
         eitem['changeddate_date'] = date_ts.isoformat()
         eitem['delta_ts'] = date_ts.strftime('%Y-%m-%dT%H:%M:%S')
 
         # Add extra JSON fields used in Kibana (enriched fields)
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/study_ceres_onion.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/study_ceres_onion.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -25,14 +25,15 @@
 import pandas
 from elasticsearch import helpers, NotFoundError
 from elasticsearch_dsl import Search, Q
 
 from cereslib.enrich.enrich import Onion
 from grimoirelab_toolkit import datetime as gl_dt
 from grimoire_elk.enriched.ceres_base import ESConnector, CeresBase
+from grimoire_elk.elastic import ElasticSearch
 
 
 logger = logging.getLogger(__name__)
 
 
 class ESOnionConnector(ESConnector):
     """ElasticSearch connector to ease data management related to Onion metric.
@@ -119,15 +120,15 @@
                 for timing in response.aggregations[self.TIMEFRAME].buckets:
                     yield self.__build_dataframe(timing, org_name=org_name).copy()
 
             # Get project specific data
             for project in projects:
 
                 logger.debug("{} Quarter: {}  Project: {}".format(
-                             self.__log_prefix, quarter, project))
+                    self.__log_prefix, quarter, project))
 
                 # Global project
                 s = self.__build_search(date_range, project_name=project)
                 response = s.execute()
 
                 for timing in response.aggregations[self.TIMEFRAME].buckets:
                     yield self.__build_dataframe(timing, project_name=project).copy()
@@ -168,15 +169,15 @@
             doc = {
                 "_index": self._es_index,
                 "_type": "item",
                 "_id": item_id,
                 "_source": row
             }
 
-            if self._es_major == '7':
+            if not ElasticSearch.is_legacy_static(self._es_major, self._es_distribution):
                 doc.pop('_type')
 
             docs.append(doc)
 
         # TODO uncomment following lines for incremental version
         # # Delete old data if exists to ensure refreshing in case of deleted commits
         # timeframe = docs[0]['_source']['timeframe']
@@ -242,16 +243,20 @@
             q = Q('range')
             q.__setattr__(self._sort_on_field, {'gte': from_date})
             s = s.filter(q)
 
         # from:to parameters (=> from: 0, size: 0)
         s = s[0:0]
 
-        s.aggs.bucket(self.TIMEFRAME, 'date_histogram', field=self._timeframe_field,
-                      interval='quarter', min_doc_count=1)
+        if ElasticSearch.is_legacy_static(self._es_major, self._es_distribution):
+            s.aggs.bucket(self.TIMEFRAME, 'date_histogram', field=self._timeframe_field,
+                          interval='quarter', min_doc_count=1)
+        else:
+            s.aggs.bucket(self.TIMEFRAME, 'date_histogram', field=self._timeframe_field,
+                          calendar_interval='quarter', min_doc_count=1)
         response = s.execute()
 
         quarters = []
         for quarter in response.aggregations[self.TIMEFRAME].buckets:
             period = pandas.Period(quarter.key_as_string, 'Q')
             quarters.append(period)
 
@@ -295,20 +300,22 @@
         s = s[0:0]
 
         # Get author_name and most recent metadata__timestamp for quarter (should be enough per quarter,
         # computing it by user probably is not needed as we are going to recalculate the whole quarter)
 
         # We are not keeping all metadata__* fields because we are grouping commits by author, so we can only
         # store one value per author.
-        s.aggs.bucket(self.TIMEFRAME, 'date_histogram', field=self._timeframe_field, interval='quarter') \
-            .metric(self.LATEST_TS, 'max', field=self._sort_on_field)\
+        if ElasticSearch.is_legacy_static(self._es_major, self._es_distribution):
+            bucket = s.aggs.bucket(self.TIMEFRAME, 'date_histogram', field=self._timeframe_field, interval='quarter')
+        else:
+            bucket = s.aggs.bucket(self.TIMEFRAME, 'date_histogram', field=self._timeframe_field, calendar_interval='quarter')
+        bucket.metric(self.LATEST_TS, 'max', field=self._sort_on_field) \
             .bucket(self.AUTHOR_UUID, 'terms', field=self.AUTHOR_UUID, size=1000) \
             .metric(self.CONTRIBUTIONS, 'cardinality', field=self.contribs_field, precision_threshold=40000)\
             .bucket(self.AUTHOR_NAME, 'terms', field=self.AUTHOR_NAME, size=1)
-
         return s
 
     def __build_dataframe(self, timing, project_name=None, org_name=None):
         """Build a DataFrame from a time bucket.
 
         :param timing:
         :param project_name:
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/nntp.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/nntp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/slack.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/slack.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/enrich.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/enrich.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2020 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -16,15 +16,15 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #   Alvaro del Castillo San Felix <acs@bitergia.com>
 #   Quan Zhou <quan@bitergia.com>
 #   Miguel Ángel Fernández <mafesan@bitergia.com>
 #
-
+import datetime
 import json
 import functools
 import logging
 import requests
 import sys
 import time
 
@@ -34,15 +34,15 @@
 import pkg_resources
 from functools import lru_cache
 
 from elasticsearch import Elasticsearch as ES, RequestsHttpConnection
 from geopy.geocoders import Nominatim
 
 from perceval.backend import find_signature_parameters
-from grimoirelab_toolkit.datetime import (datetime_utcnow, str_to_datetime)
+from grimoirelab_toolkit.datetime import datetime_utcnow, str_to_datetime
 
 from ..elastic import ElasticSearch
 from ..elastic_analyzer import Analyzer
 from ..elastic_items import (ElasticItems,
                              HEADER_JSON)
 from .study_ceres_onion import ESOnionConnector, onion_study
 from .sortinghat_gelk import MULTI_ORG_NAMES
@@ -52,105 +52,98 @@
 
 from .utils import grimoire_con, METADATA_FILTER_RAW, REPO_LABELS, anonymize_url
 from .. import __version__
 
 logger = logging.getLogger(__name__)
 
 try:
-    import pymysql
-    MYSQL_LIBS = True
-except ImportError:
-    logger.info("MySQL not available")
-    MYSQL_LIBS = False
-
-try:
-    from sortinghat.db.database import Database
-    from sortinghat import api, utils
-    from sortinghat.exceptions import NotFoundError, InvalidValueError
+    from sortinghat.cli.client import (SortingHatClient,
+                                       SortingHatClientError)
+    from sortinghat.utils import generate_uuid
 
     from .sortinghat_gelk import SortingHat
 
     SORTINGHAT_LIBS = True
 except ImportError:
     logger.info("SortingHat not available")
     SORTINGHAT_LIBS = False
 
-
 UNKNOWN_PROJECT = 'unknown'
 DEFAULT_PROJECT = 'Main'
 DEFAULT_DB_USER = 'root'
 CUSTOM_META_PREFIX = 'cm'
 EXTRA_PREFIX = 'extra'
 SH_UNKNOWN_VALUE = 'Unknown'
-DEMOGRAPHICS_ALIAS = 'demographics'
-DEMOGRAPHICS_CONTRIBUTION_ALIAS = 'demographics_contribution'
-ONION_ALIAS = 'all_onion'
 
 
 def metadata(func):
     """Add metadata to an item.
 
     Decorator that adds metadata to a given item such as
     the gelk revision used.
 
     """
+
     @functools.wraps(func)
     def decorator(self, *args, **kwargs):
         eitem = func(self, *args, **kwargs)
         metadata = {
             'metadata__gelk_version': self.gelk_version,
             'metadata__gelk_backend_name': self.__class__.__name__,
             'metadata__enriched_on': datetime_utcnow().isoformat()
         }
         eitem.update(metadata)
         return eitem
+
     return decorator
 
 
 class Enrich(ElasticItems):
     analyzer = Analyzer
     sh_db = None
     kibiter_version = None
     RAW_FIELDS_COPY = ["metadata__updated_on", "metadata__timestamp",
                        "offset", "origin", "tag", "uuid"]
     KEYWORD_MAX_LENGTH = 1000  # this control allows to avoid max_bytes_length_exceeded_exception
 
     ONION_INTERVAL = seconds = 3600 * 24 * 7
 
-    def __init__(self, db_sortinghat=None, db_projects_map=None, json_projects_map=None,
-                 db_user='', db_password='', db_host='', insecure=True):
+    def __init__(self, db_sortinghat=None, json_projects_map=None, db_user='',
+                 db_password='', db_host='', insecure=True, db_port=None, db_path=None,
+                 db_ssl=False, db_verify_ssl=True, db_tenant=None):
+
         perceval_backend = None
         super().__init__(perceval_backend, insecure=insecure)
-
+        self._connector_name = None
         self.sortinghat = False
         if db_user == '':
             db_user = DEFAULT_DB_USER
         if db_sortinghat and not SORTINGHAT_LIBS:
             raise RuntimeError("Sorting hat configured but libraries not available.")
         if db_sortinghat:
-            # self.sh_db = Database("root", "", db_sortinghat, "mariadb")
             if not Enrich.sh_db:
-                Enrich.sh_db = Database(db_user, db_password, db_sortinghat, db_host)
+                client = SortingHatClient(host=db_host, port=db_port,
+                                          path=db_path, ssl=db_ssl,
+                                          verify_ssl=db_verify_ssl,
+                                          user=db_user, password=db_password,
+                                          tenant=db_tenant)
+                client.connect()
+                client.gqlc.logger.setLevel(logging.CRITICAL)
+                Enrich.sh_db = client
+
             self.sortinghat = True
 
         self.prjs_map = None  # mapping beetween repositories and projects
         self.json_projects = None
 
         if json_projects_map:
             with open(json_projects_map) as data_file:
                 self.json_projects = json.load(data_file)
                 # If we have JSON projects always use them for mapping
                 self.prjs_map = self.__convert_json_to_projects_map(self.json_projects)
-        if not self.json_projects:
-            if db_projects_map and not MYSQL_LIBS:
-                raise RuntimeError("Projects configured but MySQL libraries not available.")
-            if db_projects_map and not self.json_projects:
-                self.prjs_map = self.__get_projects_map(db_projects_map,
-                                                        db_user, db_password,
-                                                        db_host)
 
         if self.prjs_map and self.json_projects:
             # logger.info("Comparing db and json projects")
             # self.__compare_projects_map(self.prjs_map, self.json_projects)
             pass
 
         self.studies = []
@@ -228,15 +221,15 @@
             for ds in json[project]:
                 if ds == "meta":
                     continue  # not a real data source
                 if ds not in ds_repo_to_prj:
                     if ds not in ds_repo_to_prj:
                         ds_repo_to_prj[ds] = {}
                 for repo in json[project][ds]:
-                    repo, _ = self.extract_repo_labels(repo)
+                    repo, _ = self.extract_repo_tags(repo)
                     if repo in ds_repo_to_prj[ds]:
                         if project == ds_repo_to_prj[ds][repo]:
                             logger.debug("Duplicated repo: {} {} {}".format(ds, repo, project))
                         else:
                             if len(project.split(".")) > len(ds_repo_to_prj[ds][repo].split(".")):
                                 logger.debug("Changed repo project because we found a leaf: {} leaf vs "
                                              "{} ({}, {})".format(project, ds_repo_to_prj[ds][repo], repo, ds))
@@ -265,15 +258,15 @@
             for repository in db[ds]:
                 # A repository could be in more than one project. But we get only one.
                 project = db[ds][repository]
                 if project not in db_projects:
                     db_projects.append(project)
                 if project not in json:
                     logger.error("Project not found in JSON {}".format(project))
-                    raise NotFoundError("Project not found in JSON {}".format(project))
+                    raise Exception("Project not found in JSON {}".format(project))
                 else:
                     if ds == 'mls':
                         repo_mls = repository.split("/")[-1]
                         repo_mls = repo_mls.replace(".mbox", "")
                         repository = 'https://dev.eclipse.org/mailman/listinfo/' + repo_mls
                     if ds_map_db[ds] not in json[project]:
                         logger.error("db repository not found in json {}".format(repository))
@@ -299,40 +292,14 @@
                         pass
                     else:
                         logger.debug("Not found repository in db {} {}".format(repo, ds))
 
         logger.debug("Number of db projects: {}".format(db_projects))
         logger.debug("Number of json projects: {} (>={})".format(json.keys(), db_projects))
 
-    def __get_projects_map(self, db_projects_map, db_user=None, db_password=None, db_host=None):
-        # Read the repo to project mapping from a database
-        ds_repo_to_prj = {}
-
-        db = pymysql.connect(user=db_user, passwd=db_password, host=db_host,
-                             db=db_projects_map)
-        cursor = db.cursor()
-
-        query = """
-            SELECT data_source, p.id, pr.repository_name
-            FROM projects p
-            JOIN project_repositories pr ON p.project_id=pr.project_id
-        """
-
-        res = int(cursor.execute(query))
-        if res > 0:
-            rows = cursor.fetchall()
-            for row in rows:
-                [ds, name, repo] = row
-                if ds not in ds_repo_to_prj:
-                    ds_repo_to_prj[ds] = {}
-                ds_repo_to_prj[ds][repo] = name
-        else:
-            raise RuntimeError("Can't find projects mapping in {}".format(db_projects_map))
-        return ds_repo_to_prj
-
     def get_field_unique_id(self):
         """ Field in the raw item with the unique id """
         return "uuid"
 
     def get_field_event_unique_id(self):
         """ Field in the rich event with the unique id """
         raise NotImplementedError
@@ -389,24 +356,24 @@
                 bulk_json = ""
                 current = 0
 
             if not events:
                 rich_item = self.get_rich_item(item)
                 data_json = json.dumps(rich_item)
                 bulk_json += '{"index" : {"_id" : "%s" } }\n' % \
-                    (item[self.get_field_unique_id()])
+                             (item[self.get_field_unique_id()])
                 bulk_json += data_json + "\n"  # Bulk document
                 current += 1
             else:
                 rich_events = self.get_rich_events(item)
                 for rich_event in rich_events:
                     data_json = json.dumps(rich_event)
                     bulk_json += '{"index" : {"_id" : "%s_%s" } }\n' % \
-                        (item[self.get_field_unique_id()],
-                         rich_event[self.get_field_event_unique_id()])
+                                 (item[self.get_field_unique_id()],
+                                  rich_event[self.get_field_event_unique_id()])
                     bulk_json += data_json + "\n"  # Bulk document
                     current += 1
 
         if current > 0:
             total += self.elastic.safe_put_bulk(url, bulk_json)
 
         return total
@@ -420,15 +387,22 @@
         """Add filter raw information to the enriched item"""
 
         eitem[METADATA_FILTER_RAW] = self.filter_raw
 
     def get_connector_name(self):
         """ Find the name for the current connector """
         from ..utils import get_connector_name
-        return get_connector_name(type(self))
+        if not self._connector_name:
+            self._connector_name = get_connector_name(type(self))
+        return self._connector_name
+
+    def get_sh_backend_name(self):
+        """Retrieve the backend name for SortingHat identities."""
+
+        return self.get_connector_name()
 
     def get_field_author(self):
         """ Field with the author information """
         raise NotImplementedError
 
     def get_field_date(self):
         """ Field with the date in the JSON enriched items """
@@ -450,15 +424,15 @@
         except (IndexError, AttributeError):
             # logger.warning("Bad email format: %s" % (identity['email']))
             pass
         return domain
 
     def get_identity_domain(self, identity):
         domain = None
-        if identity['email']:
+        if 'email' in identity and identity['email']:
             domain = self.get_email_domain(identity['email'])
         return domain
 
     def get_item_id(self, eitem):
         """ Return the item_id linked to this enriched eitem """
 
         # If possible, enriched_item and item will have the same id
@@ -472,35 +446,38 @@
 
     def get_last_offset_from_es(self, _filters=[]):
         # offset is always the field name from perceval
         last_update = self.elastic.get_last_offset("offset", _filters)
 
         return last_update
 
-#    def get_elastic_mappings(self):
-#        """ Mappings for enriched indexes """
-#
-#        mapping = '{}'
-#        return {"items": mapping}
+    # def get_elastic_mappings(self):
+    #     """ Mappings for enriched indexes """
+    #
+    #     mapping = '{}'
+    #     return {"items": mapping}
 
     def get_elastic_analyzers(self):
         """ Custom analyzers for our indexes  """
 
         analyzers = '{}'
 
         return analyzers
 
     def get_grimoire_fields(self, creation_date, item_name):
         """ Return common grimoire fields for all data sources """
 
         grimoire_date = None
-        try:
-            grimoire_date = str_to_datetime(creation_date).isoformat()
-        except Exception as ex:
-            pass
+        if isinstance(creation_date, datetime.datetime):
+            grimoire_date = creation_date.isoformat()
+        else:
+            try:
+                grimoire_date = str_to_datetime(creation_date).isoformat()
+            except Exception as ex:
+                pass
 
         name = "is_" + self.get_connector_name() + "_" + item_name
 
         return {
             "grimoire_creation_date": grimoire_date,
             name: 1
         }
@@ -646,73 +623,14 @@
     def get_sh_identity(self, item, identity_field):
         """ Empty identity. Real implementation in each data source. """
         identity = {}
         for field in ['name', 'email', 'username']:
             identity[field] = None
         return identity
 
-    def get_domain(self, identity):
-        """ Get the domain from a SH identity """
-        domain = None
-        if identity['email']:
-            try:
-                domain = identity['email'].split("@")[1]
-            except IndexError:
-                # logger.warning("Bad email format: %s" % (identity['email']))
-                pass
-        return domain
-
-    def is_bot(self, uuid):
-        bot = False
-        u = self.get_unique_identity(uuid)
-        if u.profile:
-            bot = u.profile.is_bot
-        return bot
-
-    def get_enrollment(self, uuid, item_date):
-        """ Get the enrollment for the uuid when the item was done """
-        # item_date must be offset-naive (utc)
-        if item_date and item_date.tzinfo:
-            item_date = (item_date - item_date.utcoffset()).replace(tzinfo=None)
-
-        enrollments = self.get_enrollments(uuid)
-        enroll = self.unaffiliated_group
-        if enrollments:
-            for enrollment in enrollments:
-                if not item_date:
-                    enroll = enrollment.organization.name
-                    break
-                elif item_date >= enrollment.start and item_date <= enrollment.end:
-                    enroll = enrollment.organization.name
-                    break
-        return enroll
-
-    def get_multi_enrollment(self, uuid, item_date):
-        """ Get the enrollments for the uuid when the item was done """
-
-        enrolls = []
-
-        # item_date must be offset-naive (utc)
-        if item_date and item_date.tzinfo:
-            item_date = (item_date - item_date.utcoffset()).replace(tzinfo=None)
-
-        enrollments = self.get_enrollments(uuid)
-
-        if enrollments:
-            for enrollment in enrollments:
-                if not item_date:
-                    enrolls.append(enrollment.organization.name)
-                elif enrollment.start <= item_date <= enrollment.end:
-                    enrolls.append(enrollment.organization.name)
-
-        if not enrolls:
-            enrolls.append(self.unaffiliated_group)
-
-        return enrolls
-
     @staticmethod
     def get_main_enrollments(enrollments):
         """ Get the main enrollment given a list of enrollments.
         If the enrollment contains :: the main one is the first part.
 
         For example:
         - Enrollment: Chaoss::Eng
@@ -721,14 +639,27 @@
         If there is more than one, it will return ordered alphabetically.
         """
         main_orgs = list(map(lambda x: x.split("::")[0], enrollments))
         main_orgs = sorted(list(set(main_orgs)))
 
         return main_orgs
 
+    @staticmethod
+    def remove_prefix_enrollments(enrollments):
+        """ Remove the prefix `::` of the enrollments.
+
+        :param enrollments: list of enrollments
+        :return: list of enrollments without prefix
+        """
+        enrolls = [enroll.split("::")[1] if "::" in enroll else
+                   enroll for enroll in enrollments]
+        enrolls_unique = sorted(list(set(enrolls)))
+
+        return enrolls_unique
+
     def __get_item_sh_fields_empty(self, rol, undefined=False):
         """ Return a SH identity with all fields to empty_field """
         # If empty_field is None, the fields do not appear in index patterns
         empty_field = '' if not undefined else '-- UNDEFINED --'
         return {
             rol + "_id": empty_field,
             rol + "_uuid": empty_field,
@@ -744,160 +675,322 @@
 
     def get_item_no_sh_fields(self, identity, rol):
         """ Create an item with reasonable data when SH is not enabled """
 
         username = identity.get('username', '')
         email = identity.get('email', '')
         name = identity.get('name', '')
-        backend_name = self.get_connector_name()
+        backend_name = self.get_sh_backend_name()
 
         if not (username or email or name):
             return self.__get_item_sh_fields_empty(rol)
 
-        uuid = utils.uuid(backend_name, email=email,
-                          name=name, username=username)
+        uuid = self.generate_uuid(backend_name, email=email,
+                                  name=name, username=username)
         return {
             rol + "_id": uuid,
             rol + "_uuid": uuid,
             rol + "_name": name,
             rol + "_user_name": username,
             rol + "_domain": self.get_identity_domain(identity),
             rol + "_gender": self.unknown_gender,
             rol + "_gender_acc": None,
             rol + "_org_name": self.unaffiliated_group,
             rol + "_bot": False,
             rol + MULTI_ORG_NAMES: [self.unaffiliated_group]
         }
 
+    def get_individual_fields(self, individual, sh_id=None, item_date=None, rol='author'):
+        """ Get standard SH fields from a SH identity """
+
+        eitem_sh = self.__get_item_sh_fields_empty(rol)
+
+        eitem_sh[rol + "_id"] = sh_id
+        eitem_sh[rol + "_uuid"] = individual['mk']
+
+        profile = individual['profile']
+        eitem_sh[rol + "_name"] = profile.get('name', eitem_sh[rol + "_name"])
+        email = profile.get('email', None)
+        eitem_sh[rol + "_domain"] = self.get_email_domain(email)
+        eitem_sh[rol + "_gender"] = profile.get('gender', self.unknown_gender)
+        eitem_sh[rol + "_gender_acc"] = profile.get('genderAcc', 0)
+        eitem_sh[rol + "_bot"] = profile.get('isBot', False)
+
+        multi_enrolls = self.get_sh_item_multi_enrollments(individual['enrollments'], item_date)
+        main_enrolls = self.get_main_enrollments(multi_enrolls)
+        all_enrolls = list(set(main_enrolls + multi_enrolls))
+        eitem_sh[rol + MULTI_ORG_NAMES] = self.remove_prefix_enrollments(all_enrolls)
+        eitem_sh[rol + "_org_name"] = main_enrolls[0]
+
+        return eitem_sh
+
     def get_item_sh_fields(self, identity=None, item_date=None, sh_id=None,
                            rol='author'):
         """ Get standard SH fields from a SH identity """
+
         eitem_sh = self.__get_item_sh_fields_empty(rol)
 
         if identity:
-            # Use the identity to get the SortingHat identity
-            sh_ids = self.get_sh_ids(identity, self.get_connector_name())
-            eitem_sh[rol + "_id"] = sh_ids.get('id', '')
-            eitem_sh[rol + "_uuid"] = sh_ids.get('uuid', '')
+            sh_item = self.get_sh_item_from_identity(identity, self.get_sh_backend_name())
+            eitem_sh[rol + "_id"] = sh_item.get('id', '')
+            eitem_sh[rol + "_uuid"] = sh_item.get('uuid', '')
             eitem_sh[rol + "_name"] = identity.get('name', '')
             eitem_sh[rol + "_user_name"] = identity.get('username', '')
             eitem_sh[rol + "_domain"] = self.get_identity_domain(identity)
         elif sh_id:
             # Use the SortingHat id to get the identity
+            sh_item = self.get_sh_item_from_id(sh_id)
             eitem_sh[rol + "_id"] = sh_id
-            eitem_sh[rol + "_uuid"] = self.get_uuid_from_id(sh_id)
+            eitem_sh[rol + "_uuid"] = sh_item.get('uuid', '')
         else:
             # No data to get a SH identity. Return an empty one.
             return eitem_sh
 
-        # If the identity does not exists return and empty identity
+        # If the identity does not exist return an empty identity
         if rol + "_uuid" not in eitem_sh or not eitem_sh[rol + "_uuid"]:
             return self.__get_item_sh_fields_empty(rol, undefined=True)
 
-        # Get the SH profile to use first this data
-        profile = self.get_profile_sh(eitem_sh[rol + "_uuid"])
-
-        if profile:
+        if 'profile' in sh_item and sh_item['profile']:
+            profile = sh_item['profile']
             # If name not in profile, keep its old value (should be empty or identity's name field value)
             eitem_sh[rol + "_name"] = profile.get('name', eitem_sh[rol + "_name"])
 
             email = profile.get('email', None)
             eitem_sh[rol + "_domain"] = self.get_email_domain(email)
 
             eitem_sh[rol + "_gender"] = profile.get('gender', self.unknown_gender)
-            eitem_sh[rol + "_gender_acc"] = profile.get('gender_acc', 0)
-
-        elif not profile and sh_id:
-            logger.warning("Can't find SH identity profile: {}".format(sh_id))
+            eitem_sh[rol + "_gender_acc"] = profile.get('genderAcc', 0)
+            eitem_sh[rol + "_bot"] = profile.get('isBot', False)
 
         # Ensure we always write gender fields
         if not eitem_sh.get(rol + "_gender"):
             eitem_sh[rol + "_gender"] = self.unknown_gender
             eitem_sh[rol + "_gender_acc"] = 0
 
-        eitem_sh[rol + "_bot"] = self.is_bot(eitem_sh[rol + '_uuid'])
-
-        multi_enrolls = self.get_multi_enrollment(eitem_sh[rol + "_uuid"], item_date)
+        multi_enrolls = self.get_sh_item_multi_enrollments(sh_item['enrollments'], item_date)
         main_enrolls = self.get_main_enrollments(multi_enrolls)
         all_enrolls = list(set(main_enrolls + multi_enrolls))
-        eitem_sh[rol + MULTI_ORG_NAMES] = all_enrolls
+        eitem_sh[rol + MULTI_ORG_NAMES] = self.remove_prefix_enrollments(all_enrolls)
         eitem_sh[rol + "_org_name"] = main_enrolls[0]
 
         return eitem_sh
 
-    def get_profile_sh(self, uuid):
-        profile = {}
+    @lru_cache(4096)
+    def get_sh_item_from_id(self, sh_id):
+        """Get all the identity information from SortingHat using the individual id"""
+
+        sh_item = {}
+
+        try:
+            individual = self.get_entity(sh_id)
+            if not individual:
+                msg = "Individual not found given the following id: {}".format(sh_id)
+                logger.debug(msg)
+                return sh_item
+            uuid = individual['mk']
+        except Exception as ex:
+            msg = "Error getting individual {} from SortingHat: {}".format(sh_id, ex)
+            logger.error(msg)
+            return sh_item
+
+        # Fill the information needed with the identity, individual and profile
+        sh_item['id'] = sh_id
+        sh_item['uuid'] = uuid
+        sh_item['profile'] = individual['profile']
+        sh_item['enrollments'] = individual['enrollments']
+
+        return sh_item
+
+    def get_sh_item_from_identity(self, identity, backend_name):
+        identity_tuple = tuple(identity.items())
+        sh_item = self.get_sh_item_from_identity_cache(identity_tuple, backend_name)
+        return sh_item
+
+    @lru_cache(4096)
+    def get_sh_item_from_identity_cache(self, identity_tuple, backend_name):
+        """Get a SortingHat item with all the information related with an identity"""
+        sh_item = {}
+        iden = {}
+
+        # Convert the identity to dict again
+        identity = dict((x, y) for x, y in identity_tuple)
+
+        for field in ['email', 'name', 'username']:
+            iden[field] = identity.get(field)
+
+        if not iden['name'] and not iden['email'] and not iden['username']:
+            logger.warning("Name, email and username are none in {}".format(backend_name))
+            return sh_item
+
+        identity_id = self.generate_uuid(backend_name,
+                                         email=iden['email'],
+                                         name=iden['name'],
+                                         username=iden['username'])
+
+        try:
+            individual = self.get_entity(identity_id)
+            if not individual:
+                msg = "Individual not found given the following identity: {}".format(identity_id)
+                logger.debug(msg)
+                return sh_item
+
+            for indv_identity in individual['identities']:
+                if indv_identity['uuid'] == identity_id:
+                    identity_sh = indv_identity
+                    break
+            else:
+                msg = "Identity {} not found in individual returned by SortingHat.".format(identity)
+                logger.error(msg)
+                return sh_item
+        except SortingHatClientError:
+            msg = "None Identity found {}, identity: {}".format(backend_name, identity)
+            logger.debug(msg)
+            return sh_item
+        except UnicodeEncodeError:
+            msg = "UnicodeEncodeError {}, identity: {}".format(backend_name, identity)
+            logger.error(msg)
+            return sh_item
+        except Exception as ex:
+            msg = "Unknown error getting identity from SortingHat, {}, {}, {}".format(ex, backend_name, identity)
+            logger.error(msg)
+            return sh_item
+
+        # Fill the information needed with the identity, individual and profile
+        sh_item['id'] = identity_sh['uuid']
+        sh_item['uuid'] = individual['mk']
+        sh_item['name'] = identity_sh['name']
+        sh_item['username'] = identity_sh['username']
+        sh_item['email'] = identity_sh['email']
+        sh_item['profile'] = individual['profile']
+        sh_item['enrollments'] = individual['enrollments']
+
+        return sh_item
+
+    def get_sh_item_multi_enrollments(self, enrollments, item_date_str):
+        """ Get the enrollments for the uuid when the item was done """
+
+        enrolls = []
+        enrollments = enrollments if enrollments else []
+
+        if enrollments:
+            if item_date_str:
+                item_date = str_to_datetime(item_date_str)
+            else:
+                item_date = None
 
-        u = self.get_unique_identity(uuid)
-        if u.profile:
-            profile['name'] = u.profile.name
-            profile['email'] = u.profile.email
-            profile['gender'] = u.profile.gender
-            profile['gender_acc'] = u.profile.gender_acc
+            # item_date must be offset-naive (utc)
+            if item_date and item_date.tzinfo:
+                item_date = (item_date - item_date.utcoffset()).replace(tzinfo=None)
+
+        for enrollment in enrollments:
+            group = enrollment['group']
+            if not item_date:
+                if group['type'] == 'team' and group['parentOrg']:
+                    name = "{}::{}".format(group['parentOrg']['name'], group['name'])
+                else:
+                    name = group['name']
+                enrolls.append(name)
+            elif str_to_datetime(enrollment['start']).isoformat() <= item_date.isoformat() \
+                    <= str_to_datetime(enrollment['end']).isoformat():
+                if group['type'] == 'team' and group['parentOrg']:
+                    name = "{}::{}".format(group['parentOrg']['name'], group['name'])
+                else:
+                    name = group['name']
+                enrolls.append(name)
+        if not enrolls:
+            enrolls.append(self.unaffiliated_group)
 
-        return profile
+        return enrolls
 
-    def get_item_sh_from_id(self, eitem, roles=None):
+    def get_item_sh_from_id(self, eitem, roles=None, individuals=None):
         # Get the SH fields from the data in the enriched item
 
         eitem_sh = {}  # Item enriched
 
         author_field = self.get_field_author()
         if not author_field:
             return eitem_sh
         sh_id_author = None
 
         if not roles:
             roles = [author_field]
 
-        date = str_to_datetime(eitem[self.get_field_date()])
-
+        date = eitem[self.get_field_date()]
         for rol in roles:
             if rol + "_id" not in eitem:
                 # For example assignee in github it is usual that it does not appears
                 logger.debug("Enriched index does not include SH ids for {}_id. Can not refresh it.".format(rol))
                 continue
             sh_id = eitem[rol + "_id"]
             if not sh_id:
                 logger.debug("{}_id is None".format(rol))
                 continue
             if rol == author_field:
                 sh_id_author = sh_id
-            eitem_sh.update(self.get_item_sh_fields(sh_id=sh_id, item_date=date,
-                                                    rol=rol))
+            individual = self.find_individual(individuals, sh_id)
+            if not individual:
+                logger.debug(f"Individual {sh_id} not found.")
+                continue
+            eitem_sh.update(self.get_individual_fields(individual=individual,
+                                                       sh_id=sh_id,
+                                                       item_date=date,
+                                                       rol=rol))
 
         # Add the author field common in all data sources
         rol_author = 'author'
         if sh_id_author and author_field != rol_author:
-            eitem_sh.update(self.get_item_sh_fields(sh_id=sh_id_author,
-                                                    item_date=date, rol=rol_author))
+            individual = self.find_individual(individuals, sh_id_author)
+            if individual:
+                eitem_sh.update(self.get_individual_fields(individual=individual,
+                                                           sh_id=sh_id_author,
+                                                           item_date=date,
+                                                           rol=rol_author))
+            else:
+                logger.debug(f"Individual {sh_id_author} not found.")
+
         return eitem_sh
 
-    def get_item_sh_meta_fields(self, eitem, roles=None, suffixes=None, non_authored_prefix=None):
+    def get_item_sh_meta_fields(self, eitem, roles=None, suffixes=None, non_authored_prefix=None, individuals=None):
         """Get the SH meta fields from the data in the enriched item."""
 
         eitem_meta_sh = {}  # Item enriched
 
-        date = str_to_datetime(eitem[self.get_field_date()])
+        date = eitem[self.get_field_date()]
 
         for rol in roles:
             if rol + "_uuids" not in eitem:
                 continue
             sh_uuids = eitem[rol + "_uuids"]
             if not sh_uuids:
                 logger.debug("{}_uuids is None".format(rol))
                 continue
 
             for sh_uuid in sh_uuids:
-                sh_fields = self.get_item_sh_fields(sh_id=sh_uuid, item_date=date, rol=rol)
+                individual = self.find_individual(individuals, sh_uuid)
+                if not individual:
+                    logger.debug(f"Individual {sh_uuid} not found.")
+                    continue
+                sh_fields = self.get_individual_fields(individual=individual, sh_id=sh_uuid, item_date=date, rol=rol)
 
                 self.add_meta_fields(eitem, eitem_meta_sh, sh_fields, rol, sh_uuid, suffixes, non_authored_prefix)
 
         return eitem_meta_sh
 
+    @staticmethod
+    def find_individual(individuals, sh_id):
+        if not individuals:
+            return None
+        for indiv in individuals:
+            if sh_id == indiv['mk']:
+                return indiv
+            for identity in indiv['identities']:
+                if sh_id == identity['uuid']:
+                    return indiv
+        return None
+
     def add_meta_fields(self, eitem, meta_eitem, sh_fields, rol, uuid, suffixes, non_authored_prefix):
         def add_non_authored_fields(author_uuid, uuid, new_eitem, new_list, non_authored_field):
             if author_uuid == uuid:
                 non_authored = []
             else:
                 non_authored = new_list
             new_eitem[non_authored_field] = non_authored
@@ -943,17 +1036,17 @@
 
         author_field = self.get_field_author()
 
         if not roles:
             roles = [author_field]
 
         if not date_field:
-            item_date = str_to_datetime(item[self.get_field_date()])
+            item_date = item[self.get_field_date()]
         else:
-            item_date = str_to_datetime(item[date_field])
+            item_date = item[date_field]
 
         users_data = self.get_users_data(item)
 
         for rol in roles:
             if rol in users_data:
                 identity = self.get_sh_identity(item, rol)
                 if self.sortinghat:
@@ -989,98 +1082,74 @@
                 eitem_sh['author_name'] = SH_UNKNOWN_VALUE
 
             if not eitem_sh['author_user_name']:
                 eitem_sh['author_user_name'] = SH_UNKNOWN_VALUE
 
         return eitem_sh
 
-    @lru_cache()
+    def generate_uuid(self, source, email=None, name=None, username=None):
+        """
+        Generate UUID from identity fields.
+        Force empty fields to None, the same way add_identity works.
+        """
+        args = {
+            "email": email,
+            "name": name,
+            "source": source,
+            "username": username
+        }
+        args_without_empty = {k: v for k, v in args.items() if v}
+        return generate_uuid(**args_without_empty)
+
+    @lru_cache(4096)
+    def get_entity(self, id):
+        return SortingHat.get_entity(self.sh_db, id)
+
+    @lru_cache(4096)
+    def is_bot(self, uuid):
+        return SortingHat.is_bot(self.sh_db, uuid)
+
+    @lru_cache(4096)
     def get_enrollments(self, uuid):
-        return api.enrollments(self.sh_db, uuid)
+        return SortingHat.get_enrollments(self.sh_db, uuid)
 
-    @lru_cache()
+    @lru_cache(4096)
     def get_unique_identity(self, uuid):
-        return api.unique_identities(self.sh_db, uuid)[0]
+        return SortingHat.get_unique_identity(self.sh_db, uuid)
 
-    @lru_cache()
+    @lru_cache(4096)
     def get_uuid_from_id(self, sh_id):
         """ Get the SH identity uuid from the id """
         return SortingHat.get_uuid_from_id(self.sh_db, sh_id)
 
-    def get_sh_ids(self, identity, backend_name):
-        """ Return the Sorting Hat id and uuid for an identity """
-        # Convert the dict to tuple so it is hashable
-        identity_tuple = tuple(identity.items())
-        sh_ids = self.__get_sh_ids_cache(identity_tuple, backend_name)
-        return sh_ids
-
-    @lru_cache()
-    def __get_sh_ids_cache(self, identity_tuple, backend_name):
+    def add_sh_identities(self, identities):
+        SortingHat.add_identities(self.sh_db, identities,
+                                  self.get_sh_backend_name())
+
+    @lru_cache(4096)
+    def add_sh_identity_cache(self, identity_tuple):
+        """Cache add_sh_identity calls. Identity must be in tuple format"""
 
-        # Convert tuple to the original dict
         identity = dict((x, y) for x, y in identity_tuple)
+        self.add_sh_identity(identity)
 
-        if not self.sortinghat:
-            raise RuntimeError("Sorting Hat not active during enrich")
-
-        iden = {}
-        sh_ids = {"id": None, "uuid": None}
-
-        for field in ['email', 'name', 'username']:
-            iden[field] = None
-            if field in identity:
-                iden[field] = identity[field]
-
-        if not iden['name'] and not iden['email'] and not iden['username']:
-            logger.warning("Name, email and username are none in {}".format(backend_name))
-            return sh_ids
-
-        try:
-            # Find the uuid for a given id.
-            id = utils.uuid(backend_name, email=iden['email'],
-                            name=iden['name'], username=iden['username'])
-
-            if not id:
-                logger.warning("Id not found in SortingHat for name: {}, email: {} and username: {} in {}".format(
-                               iden['name'], iden['email'], iden['username'], backend_name))
-                return sh_ids
-
-            with self.sh_db.connect() as session:
-                identity_found = api.find_identity(session, id)
-
-                if not identity_found:
-                    return sh_ids
-
-                sh_ids['id'] = identity_found.id
-                sh_ids['uuid'] = identity_found.uuid
-        except InvalidValueError:
-            msg = "None Identity found {}".format(backend_name)
-            logger.debug(msg)
-        except NotFoundError:
-            msg = "Identity not found in SortingHat {}".format(backend_name)
-            logger.debug(msg)
-        except UnicodeEncodeError:
-            msg = "UnicodeEncodeError {}, identity: {}".format(backend_name, identity)
-            logger.error(msg)
-        except Exception as ex:
-            msg = "Unknown error adding identity in SortingHat, {}, {}, {}".format(ex, backend_name, identity)
-            logger.error(msg)
-
-        return sh_ids
+    def add_sh_identity(self, identity):
+        SortingHat.add_identity(self.sh_db, identity,
+                                self.get_sh_backend_name())
 
     def copy_raw_fields(self, copy_fields, source, target):
         """Copy fields from item to enriched item."""
 
         for f in copy_fields:
             if f in source:
                 target[f] = source[f]
             else:
                 target[f] = None
 
-    def enrich_onion(self, enrich_backend, in_index, out_index, data_source,
+    def enrich_onion(self, enrich_backend, alias, in_index, out_index, data_source,
                      contribs_field, timeframe_field, sort_on_field,
                      seconds=ONION_INTERVAL, no_incremental=False):
 
         log_prefix = "[" + data_source + "] study onion"
 
         logger.info("{}  starting study - Input: {} Output: {}".format(log_prefix, in_index, out_index))
 
@@ -1115,28 +1184,28 @@
                 logger.info("{} too soon to update. Next update will be at {}".format(
                             log_prefix, update_after.isoformat()))
                 return
 
         # Onion currently does not support incremental option
         logger.info("{} Creating out ES index".format(log_prefix))
         # Initialize out index
-        if self.elastic.major == '7':
+        if not self.elastic.is_legacy():
             filename = pkg_resources.resource_filename('grimoire_elk', 'enriched/mappings/onion_es7.json')
         else:
             filename = pkg_resources.resource_filename('grimoire_elk', 'enriched/mappings/onion.json')
 
         out_conn.create_index(filename, delete=out_conn.exists())
 
         onion_study(in_conn=in_conn, out_conn=out_conn, data_source=data_source)
 
         # Create alias if output index exists (index is always created from scratch, so
         # alias need to be created each time)
-        if out_conn.exists() and not out_conn.exists_alias(out_index, ONION_ALIAS):
-            logger.info("{} Creating alias: {}".format(log_prefix, ONION_ALIAS))
-            out_conn.create_alias(ONION_ALIAS)
+        if out_conn.exists() and not out_conn.exists_alias(out_index, alias):
+            logger.info("{} Creating alias: {}".format(log_prefix, alias))
+            out_conn.create_alias(alias)
 
         logger.info("{} end".format(log_prefix))
 
     def enrich_extra_data(self, ocean_backend, enrich_backend, json_url, target_index=None):
         """
         This study enables setting/removing extra fields on/from a target index. For example if a use case
         requires tagging specific documents in an index with extra fields, like tagging all kernel
@@ -1760,27 +1829,28 @@
                     ]
                 }
                 """ % (date_field, repository_url, date_field, min_date, max_date,
                        author_field, author_value, date_field)
 
         return es_query
 
-    def enrich_demography_contribution(self, ocean_backend, enrich_backend, date_field="grimoire_creation_date",
+    def enrich_demography_contribution(self, ocean_backend, enrich_backend, alias, date_field="grimoire_creation_date",
                                        author_field="author_uuid"):
         """
         Run demography study for the different types of the author activities and add the resulting enriched items.
 
         The resulting min and max dates are updated in all items including attributes following the pattern
         <contribution_type>_min_date and <contribution_type>_max_date.
 
         The different contribution types available are obtained with a query asking for unique "type" elements
         within the contributions from all authors.
 
         :param ocean_backend: backend from which to read the raw items
         :param enrich_backend:  backend from which to read the enriched items
+        :poram alias: name of the study alias
         :param date_field: field used to find the mix and max dates for the author's activity
         :param author_field: field of the author
 
         :return: None
         """
         data_source = enrich_backend.__class__.__name__.split("Enrich")[0].lower()
         log_prefix = "[{}] Demography Contribution".format(data_source)
@@ -1803,41 +1873,42 @@
             type_fields.append(type_field['key'])
 
         # Run demography study for each contribution type
         type_fields.sort()
         for field in type_fields:
             Enrich.run_demography(self, date_field, author_field, log_prefix, contribution_type=field)
 
-        if not self.elastic.alias_in_use(DEMOGRAPHICS_CONTRIBUTION_ALIAS):
-            logger.info("{} Creating alias: {}".format(log_prefix, DEMOGRAPHICS_CONTRIBUTION_ALIAS))
-            self.elastic.add_alias(DEMOGRAPHICS_CONTRIBUTION_ALIAS)
+        if not self.elastic.alias_in_use(alias):
+            logger.info("{} Creating alias: {}".format(log_prefix, alias))
+            self.elastic.add_alias(alias)
 
         logger.info("{} end {}".format(log_prefix, anonymize_url(self.elastic.index_url)))
 
-    def enrich_demography(self, ocean_backend, enrich_backend, date_field="grimoire_creation_date",
+    def enrich_demography(self, ocean_backend, enrich_backend, alias, date_field="grimoire_creation_date",
                           author_field="author_uuid"):
         """
         Run demography study for all of the author activities and add the resulting enriched items.
 
         :param ocean_backend: backend from which to read the raw items
         :param enrich_backend:  backend from which to read the enriched items
+        :poram alias: name of the study alias
         :param date_field: field used to find the mix and max dates for the author's activity
         :param author_field: field of the author
 
         :return: None
         """
         data_source = enrich_backend.__class__.__name__.split("Enrich")[0].lower()
         log_prefix = "[{}] Demography".format(data_source)
         logger.info("{} starting study {}".format(log_prefix, anonymize_url(self.elastic.index_url)))
 
         Enrich.run_demography(self, date_field, author_field, log_prefix)
 
-        if not self.elastic.alias_in_use(DEMOGRAPHICS_ALIAS):
-            logger.info("{} Creating alias: {}".format(log_prefix, DEMOGRAPHICS_ALIAS))
-            self.elastic.add_alias(DEMOGRAPHICS_ALIAS)
+        if not self.elastic.alias_in_use(alias):
+            logger.info("{} Creating alias: {}".format(log_prefix, alias))
+            self.elastic.add_alias(alias)
 
         logger.info("{} end {}".format(log_prefix, anonymize_url(self.elastic.index_url)))
 
     def run_demography(self, date_field, author_field, log_prefix, contribution_type=None):
         """
         The goal of the algorithm is to add to all enriched items the first and last date
         of all the activities or an specific contribution type of the author activities.
@@ -1853,62 +1924,85 @@
         :param date_field: field used to find the mix and max dates for the author's activity
         :param author_field: field of the author
         :param log_prefix: log prefix used on logger
         :param contribution_type: name of the contribution type (if any) which the dates are computed for.
             In case there is no specific contribution type, by default all contributions will be considered.
         """
         # The first step is to find the current min and max date for all the authors
-        authors_min_max_data = {}
-
-        es_query = Enrich.authors_min_max_dates(date_field,
-                                                author_field=author_field,
-                                                contribution_type=contribution_type)
-        r = self.requests.post(self.elastic.index_url + "/_search",
-                               data=es_query, headers=HEADER_JSON,
-                               verify=False)
-        try:
-            r.raise_for_status()
-        except requests.exceptions.HTTPError as ex:
-            logger.error("{} error getting authors mix and max date. Aborted.".format(log_prefix))
-            logger.error(ex)
-            return
-
-        for author in r.json()['aggregations']['author']['buckets']:
-            authors_min_max_data[author['key']] = author
+        authors_min_max_data = self.fetch_authors_min_max_dates(log_prefix, author_field, contribution_type, date_field)
 
         # Then we update the min max dates of all authors
-        for author_key in authors_min_max_data:
-            author_min_date = authors_min_max_data[author_key]['min']['value_as_string']
-            author_max_date = authors_min_max_data[author_key]['max']['value_as_string']
-
+        for author in authors_min_max_data:
+            author_min_date = author['min']['value_as_string']
+            author_max_date = author['max']['value_as_string']
+            author_key = author['key']['author_uuid']
             field_name = contribution_type if contribution_type else 'demography'
             es_update = Enrich.update_author_min_max_date(author_min_date, author_max_date,
                                                           author_key, field_name, author_field=author_field)
 
             try:
                 r = self.requests.post(
                     self.elastic.index_url + "/_update_by_query?wait_for_completion=true&conflicts=proceed",
                     data=es_update, headers=HEADER_JSON,
                     verify=False
                 )
-                self.check_version_conflicts(es_update, r.json()['version_conflicts'], log_prefix)
+                self.check_version_conflicts(es_update, r.json().get('version_conflicts', None), log_prefix)
 
             except requests.exceptions.RetryError:
                 logger.warning("{} retry exceeded while executing demography."
                                " The following query is skipped {}".format(log_prefix, es_update))
                 continue
 
             try:
                 r.raise_for_status()
             except requests.exceptions.HTTPError as ex:
                 logger.error("{} error updating mix and max date for author {}. Aborted.".format(
                              log_prefix, author_key))
                 logger.error(ex)
                 return
 
+    def fetch_authors_min_max_dates(self, log_prefix, author_field, contribution_type, date_field):
+        """ Fetch all authors with their first and last date of activity.
+
+        :param log_prefix: log prefix used on logger.
+        :param author_field: field of the author.
+        :param contribution_type: name of the contribution type (if any) which the dates are computed for.
+            In case there is no specific contribution type, by default all contributions will be considered.
+        :param date_field: field used to find the mix and max dates for the author's activity.
+
+        :return: dictionary of authors with min and max dates.
+        """
+        after = None
+
+        while True:
+            es_query = Enrich.authors_min_max_dates(date_field,
+                                                    author_field=author_field,
+                                                    contribution_type=contribution_type,
+                                                    after=after)
+            r = self.requests.post(self.elastic.index_url + "/_search",
+                                   data=es_query, headers=HEADER_JSON,
+                                   verify=False)
+            try:
+                r.raise_for_status()
+            except requests.exceptions.HTTPError as ex:
+                logger.error("{} error getting authors mix and max date. Aborted.".format(log_prefix))
+                logger.error(ex)
+                return
+
+            aggregations_author = r.json()['aggregations']['author']
+
+            # When there are no more elements, it will return an empty list of buckets
+            if not aggregations_author['buckets']:
+                return
+
+            after = aggregations_author['after_key'][author_field]
+
+            for author in aggregations_author['buckets']:
+                yield author
+
     def check_version_conflicts(self, es_update, version_conflicts, log_prefix, max_retries=5):
         """
         Check if there are version conflicts within a query response and retries the request.
         The time between requests is 0.5 second. This method will perform the retries until there are no
         more version conflicts.
 
         :param es_update: ES update query
@@ -1927,51 +2021,79 @@
         r = self.requests.post(
             self.elastic.index_url + "/_update_by_query?wait_for_completion=true&conflicts=proceed",
             data=es_update, headers=HEADER_JSON,
             verify=False
         )
         r.raise_for_status()
         retries = max_retries - 1
-        self.check_version_conflicts(es_update, r.json()['version_conflicts'], log_prefix, max_retries=retries)
+        self.check_version_conflicts(es_update, r.json().get('version_conflicts', None), log_prefix, max_retries=retries)
 
     @staticmethod
-    def authors_min_max_dates(date_field, author_field="author_uuid", contribution_type=None):
+    def authors_min_max_dates(date_field, author_field="author_uuid", contribution_type=None, after=None):
         """
         Get the aggregation of author with their min and max activity dates
 
         :param date_field: field used to find the mix and max dates for the author's activity
         :param author_field: field of the author
         :param contribution_type: name of the contribution type (if any) which the dates are computed for.
             In case there is no specific contribution type, by default all contributions will be considered.
+        :param after: value used for pagination
 
         :return: the query to be executed to get the authors min and max aggregation data
         """
 
-        # Limit aggregations: https://github.com/elastic/elasticsearch/issues/18838
-        # 30000 seems to be a sensible number of the number of people in git
+        # Limit aggregations:
+        # - OpenSearch: 10000
+        #   - https://opensearch.org/docs/latest/opensearch/bucket-agg/
+        # - ElasticSearch: 10000
+        #   - https://discuss.elastic.co/t/increasing-max-buckets-for-specific-visualizations/187390/4
+        #   - When you try to fetch more than 10000 it will return this error message:
+        #     {
+        #       "type": "too_many_buckets_exception",
+        #       "reason": "Trying to create too many buckets. Must be less than or equal to: [10000] but was [20000].
+        #                 This limit can be set by changing the [search.max_buckets] cluster level setting.",
+        #       "max_buckets": 10000
+        #     }
+
         query_type = ""
         if contribution_type:
             query_type = """"query": {
             "bool" : {
               "must" : {
                 "term" : {
                   "type" : "%s"
                 }
               }
             }
           },""" % contribution_type
+
+        query_after = ""
+        if after:
+            query_after = """"after": {
+                  "%s": "%s"
+                },""" % (author_field, after)
+
         es_query = """
         {
           "size": 0,
           %s
           "aggs": {
             "author": {
-              "terms": {
-                "field": "%s",
-                "size": 30000
+              "composite": {
+                "sources": [
+                  {
+                    "%s": {
+                      "terms": {
+                        "field": "%s"
+                      }
+                    }
+                  }
+                ],
+                %s
+                "size": 10000
               },
               "aggs": {
                 "min": {
                   "min": {
                     "field": "%s"
                   }
                 },
@@ -1980,15 +2102,15 @@
                     "field": "%s"
                   }
                 }
               }
             }
           }
         }
-        """ % (query_type, author_field, date_field, date_field)
+        """ % (query_type, author_field, author_field, query_after, date_field, date_field)
 
         return es_query
 
     @staticmethod
     def fetch_contribution_types():
         query = '''
         {
@@ -2080,19 +2202,19 @@
                                 }
                             }
                         ]
                     }
                 },
                 "sort": [
                     {
-                      "%s": {
-                        "order": "asc"
-                      }
+                        "%s": {
+                           "order": "asc"
+                        }
                     }
-                  ]
+                ]
             }
             """ % date_field
 
         logger.info("[enrich-feelings] Start study on {} with data from {}".format(
             anonymize_url(self.elastic.index_url), nlp_rest_url))
 
         es = ES([self.elastic_url], timeout=3600, max_retries=50, retry_on_timeout=True,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/bugzillarest.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/bugzillarest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2020 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/github_study_evolution.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/github_study_evolution.py`

 * *Files 4% similar despite different names*

```diff
@@ -171,24 +171,24 @@
     }
     """ % (str(exclude_labels).replace("'", "\""),
            repository_url, to_date, to_date)
 
     return issues_open_at
 
 
-def get_issues_dates(interval, repository_url):
-
+def get_issues_dates(elastic, interval, repository_url):
+    interval_string = "interval" if elastic.is_legacy() else "fixed_interval"
     query_issues_dates = """
 {
     "size": 0,
     "aggs" : {
         "created_per_interval" : {
             "date_histogram" : {
                 "field" : "metadata__updated_on",
-                "interval" : "%dd"
+                "%s" : "%dd"
             },
             "aggs": {
                 "created": {
                   "value_count": {
                         "field": "created_at"
                     }
                 },
@@ -206,10 +206,10 @@
                     "term": {
                         "origin": "%s"
                     }
                 }]
             }
         }
     }
-    """ % (interval, repository_url)
+    """ % (interval_string, interval, repository_url)
 
     return query_issues_dates
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/hyperkitty.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/hyperkitty.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/confluence.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/confluence.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/mattermost.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mattermost.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -54,14 +54,25 @@
 
 
 class MattermostEnrich(Enrich):
     # This enricher must compatible with the Slack enricher to reuse the Kibiter panel
 
     mapping = Mapping
 
+    def __init__(self, db_sortinghat=None, json_projects_map=None,
+                 db_user='', db_password='', db_host='', db_path=None,
+                 db_port=None, db_ssl=False, db_verify_ssl=True, db_tenant=None):
+        super().__init__(db_sortinghat=db_sortinghat, json_projects_map=json_projects_map,
+                         db_user=db_user, db_password=db_password, db_host=db_host,
+                         db_port=db_port, db_path=db_path, db_ssl=db_ssl, db_verify_ssl=db_verify_ssl,
+                         db_tenant=db_tenant)
+
+        self.studies = []
+        self.studies.append(self.enrich_demography)
+
     def get_field_author(self):
         return "user_data"
 
     def get_sh_identity(self, item, identity_field=None):
         identity = {
             'username': None,
             'name': None,
@@ -178,14 +189,18 @@
 
         eitem.update(self.get_grimoire_fields(item["metadata__updated_on"], "message"))
 
         self.add_repository_labels(eitem)
         self.add_metadata_filter_raw(eitem)
         return eitem
 
+    def enrich_demography(self, ocean_backend, enrich_backend, alias, date_field="grimoire_creation_date",
+                          author_field="author_uuid"):
+        super().enrich_demography(ocean_backend, enrich_backend, alias, date_field, author_field=author_field)
+
     @staticmethod
     def __get_files(message):
         files = []
         for file in message:
             new_file = {
                 'file_user_id': file['user_id'],
                 'file_post_id': file['post_id'],
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/telegram.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/telegram.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/utils.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -52,15 +52,15 @@
 
     if not perceval_backend:
         return filter_
 
     field = 'origin'
     value = anonymize_url(perceval_backend.origin)
 
-    if perceval_backend_name in ["meetup", "nntp", "stackexchange", "jira"]:
+    if perceval_backend_name in ["meetup", "nntp", "stackexchange", "jira", "hyperkitty"]:
         # Until tag is supported in all raw and enriched indexes
         # we should use origin. But stackexchange and meetup won't work with origin
         # because the tag must be included in the filter.
         # For nntp we have a common group server as origin, so we need to use also the tag.
         # And in jira we can filter by product, and the origin is the same jira server.
         field = 'tag'
         value = perceval_backend.tag
@@ -83,14 +83,39 @@
         # In GitHub we receive GITHUB + '/', the site url without org and repo
         # In Meetup we receive https://meetup.com/ as the tag
         filter_ = {}
 
     return filter_
 
 
+def get_confluence_spaces_filter(repo_spaces, perceval_backend_name):
+    """ Get the spaces needed for get the items in a confluence instance """
+
+    filter_ = {}
+
+    if not repo_spaces or perceval_backend_name != "confluence":
+        return filter_
+
+    field = 'data._expandable.space'
+    value_path = "/rest/api/space/"
+    values = repo_spaces
+
+    filter_ = {
+        "should": []
+    }
+
+    for value in values:
+        new = {
+            "term": {field: value_path + value}
+        }
+        filter_["should"].append(new)
+
+    return filter_
+
+
 def anonymize_url(url):
     """Remove credentials from the url
 
     :param url: target url
     """
     anonymized = re.sub('://.*@', '://', url)
 
@@ -119,15 +144,15 @@
     conn = requests.Session()
     # {backoff factor} * (2 ^ ({number of total retries} - 1))
     # conn_retries = 21  # 209715.2 = 2.4d
     # total covers issues like 'ProtocolError('Connection aborted.')
     # Retry when there are errors in HTTP connections
     retries = urllib3.util.Retry(total=total, connect=conn_retries, read=MAX_RETRIES_ON_READ,
                                  redirect=MAX_RETRIES_ON_REDIRECT, backoff_factor=BACKOFF_FACTOR,
-                                 method_whitelist=False, status_forcelist=STATUS_FORCE_LIST)
+                                 allowed_methods=False, status_forcelist=STATUS_FORCE_LIST)
     adapter = requests.adapters.HTTPAdapter(max_retries=retries)
     conn.mount('http://', adapter)
     conn.mount('https://', adapter)
 
     if insecure:
         urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
         conn.verify = False
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/finosmeetings.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/supybot.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -12,130 +12,108 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
-#   Valerio Cosentino <valcos@bitergia.com>
+#   Alvaro del Castillo San Felix <acs@bitergia.com>
 #
 
 import logging
 
 from .enrich import Enrich, metadata
 from ..elastic_mapping import Mapping as BaseMapping
-from .sortinghat_gelk import SortingHat
-
+from grimoirelab_toolkit.datetime import str_to_datetime
 
 logger = logging.getLogger(__name__)
 
-GITHUB_BACKEND = "github"
-
 
 class Mapping(BaseMapping):
 
     @staticmethod
     def get_elastic_mappings(es_major):
         """Get Elasticsearch mapping.
 
         :param es_major: major version of Elasticsearch, as string
         :returns:        dictionary with a key, 'items', with the mapping
         """
 
-        mapping = '''
-         {
-            "dynamic":true,
+        mapping = """
+        {
             "properties": {
-                "date": {
-                    "type": "keyword"
+                "body_analyzed": {
+                  "type": "text",
+                  "fielddata": true,
+                  "index": true
                 }
-            }
-        }
-        '''
+           }
+        } """
 
         return {"items": mapping}
 
 
-class FinosMeetingsEnrich(Enrich):
+class SupybotEnrich(Enrich):
 
     mapping = Mapping
 
-    def get_sh_identity(self, item, identity_field=None):
-        identity = {}
-        for field in ['name', 'email', 'username']:
-            identity[field] = None
-
-        user = item['data'] if isinstance(item, dict) and 'data' in item else item
-
-        if 'name' in user and user['name']:
-            identity['name'] = user['name']
-        if 'email' in user and user['email']:
-            identity['email'] = user['email']
-        if 'githubid' in user and user['githubid']:
-            identity['username'] = user['githubid']
-
-        return identity
-
     def get_field_author(self):
-        return 'email'
-
-    def add_sh_github_identity(self, github_login):
-        identity = {
-            'username': github_login,
-            'email': None,
-            'name': None
-        }
-
-        SortingHat.add_identity(self.sh_db, identity, GITHUB_BACKEND)
+        return "nick"
 
     def get_identities(self, item):
         """ Return the identities from an item """
 
-        data = item['data']
-        identity = self.get_sh_identity(data)
-
-        if identity['username']:
-            self.add_sh_github_identity(identity['username'])
+        user = self.get_sh_identity(item['data']['nick'])
+        yield user
 
-        yield identity
+    def get_sh_identity(self, item, identity_field=None):
+        identity = {}
+        identity['username'] = None
+        identity['email'] = None
+        identity['name'] = None
+
+        if not item:
+            return identity
+
+        nick = item
+        if isinstance(item, dict) and 'data' in item:
+            nick = item['data'][identity_field]
 
-    def has_identities(self):
-        """ Return whether the enriched items contains identities """
+        identity['username'] = nick
+        identity['name'] = nick
 
-        return True
+        return identity
 
     @metadata
     def get_rich_item(self, item):
         eitem = {}
 
         self.copy_raw_fields(self.RAW_FIELDS_COPY, item, eitem)
+        # The real data
+        message = item['data']
 
-        entry = item['data']
-
-        for e in entry.keys():
-            if e == '_id_columns':
-                continue
-            elif e == 'org':
-                eitem['csv_org'] = entry[e]
+        # data fields to copy
+        copy_fields = ["nick", "body", "type"]
+        for f in copy_fields:
+            if f in message:
+                eitem[f] = message[f]
             else:
-                eitem[e] = entry[e]
+                eitem[f] = None
+        # Fields which names are translated
+        map_fields = {"body": "body_analyzed", "timestamp": "sent_date"}
+        for fn in map_fields:
+            eitem[map_fields[fn]] = message[fn]
+
+        # Enrich dates
+        eitem["update_date"] = str_to_datetime(item["metadata__updated_on"]).isoformat()
+        eitem["channel"] = eitem["origin"]
 
+        eitem.update(self.get_grimoire_fields(eitem["update_date"], "message"))
         if self.sortinghat:
             eitem.update(self.get_item_sh(item))
 
         if self.prjs_map:
             eitem.update(self.get_item_project(eitem))
 
-        eitem.update(self.get_grimoire_fields(item["metadata__updated_on"], "entry"))
-
         self.add_repository_labels(eitem)
         self.add_metadata_filter_raw(eitem)
         return eitem
-
-    def get_item_project(self, eitem):
-
-        project_info = {
-            "project": eitem['cm_title'],
-            "project_1": eitem['cm_title']
-        }
-
-        return project_info
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/supybot.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/phabricator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -15,105 +15,76 @@
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #   Alvaro del Castillo San Felix <acs@bitergia.com>
 #
 
-import logging
-
-from .enrich import Enrich, metadata
+from .elastic import ElasticOcean
 from ..elastic_mapping import Mapping as BaseMapping
-from grimoirelab_toolkit.datetime import str_to_datetime
-
-logger = logging.getLogger(__name__)
 
 
 class Mapping(BaseMapping):
 
     @staticmethod
     def get_elastic_mappings(es_major):
         """Get Elasticsearch mapping.
 
+        Non dynamic discovery of type for:
+            * data.transaction: has string arrays and dicts arrays
+        Specific type for:
+            * data.fields.priority.subpriority (float)
+
         :param es_major: major version of Elasticsearch, as string
         :returns:        dictionary with a key, 'items', with the mapping
         """
 
-        mapping = """
+        mapping = '''
         {
+            "dynamic":true,
             "properties": {
-                "body_analyzed": {
-                  "type": "text",
-                  "fielddata": true,
-                  "index": true
+                "data": {
+                    "properties": {
+                        "transactions": {
+                            "dynamic":false,
+                            "properties": {}
+                        },
+                        "fields": {
+                            "properties": {
+                                "priority" : {
+                                    "properties": {
+                                        "subpriority" : {"type": "float"}
+                                    }
+                                },
+                                "description": {
+                                    "dynamic":false,
+                                    "properties": {}
+                                },
+                                "custom_error_stack": {
+                                    "type": "text",
+                                    "index": true
+                                }
+                            }
+                        }
+                    }
                 }
-           }
-        } """
+            }
+        }
+        '''
 
         return {"items": mapping}
 
 
-class SupybotEnrich(Enrich):
+class PhabricatorOcean(ElasticOcean):
+    """Phabricator Ocean feeder"""
 
     mapping = Mapping
 
-    def get_field_author(self):
-        return "nick"
-
-    def get_identities(self, item):
-        """ Return the identities from an item """
-
-        user = self.get_sh_identity(item['data']['nick'])
-        yield user
-
-    def get_sh_identity(self, item, identity_field=None):
-        identity = {}
-        identity['username'] = None
-        identity['email'] = None
-        identity['name'] = None
-
-        if not item:
-            return identity
-
-        nick = item
-        if isinstance(item, dict) and 'data' in item:
-            nick = item['data'][identity_field]
-
-        identity['username'] = nick
-        identity['name'] = nick
-
-        return identity
-
-    @metadata
-    def get_rich_item(self, item):
-        eitem = {}
-
-        self.copy_raw_fields(self.RAW_FIELDS_COPY, item, eitem)
-        # The real data
-        message = item['data']
-
-        # data fields to copy
-        copy_fields = ["nick", "body", "type"]
-        for f in copy_fields:
-            if f in message:
-                eitem[f] = message[f]
-            else:
-                eitem[f] = None
-        # Fields which names are translated
-        map_fields = {"body": "body_analyzed", "timestamp": "sent_date"}
-        for fn in map_fields:
-            eitem[map_fields[fn]] = message[fn]
-
-        # Enrich dates
-        eitem["update_date"] = str_to_datetime(item["metadata__updated_on"]).isoformat()
-        eitem["channel"] = eitem["origin"]
-
-        eitem.update(self.get_grimoire_fields(eitem["update_date"], "message"))
-        if self.sortinghat:
-            eitem.update(self.get_item_sh(item))
-
-        if self.prjs_map:
-            eitem.update(self.get_item_project(eitem))
-
-        self.add_repository_labels(eitem)
-        self.add_metadata_filter_raw(eitem)
-        return eitem
+    def _fix_item(self, item):
+        # fields cannot contain dots in ES 2.2. For consistency reason, this fix is applied also
+        # to more recent versions of ES
+
+        for field in list(item["data"]["fields"]):
+            if '.' in field:
+                undotted_field = field.replace('.', '_')
+                item["data"]["fields"][undotted_field] = item["data"]["fields"][field]
+                item["data"]['fields'].pop(field)
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/mappings/onion.json` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mappings/onion.json`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/mappings/onion_es7.json` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mappings/onion_es7.json`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/mappings/git_aoc.json` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mappings/git_aoc.json`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/mappings/git_aoc_es7.json` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mappings/git_aoc_es7.json`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/mbox.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/mbox.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -61,18 +61,21 @@
         return {"items": mapping}
 
 
 class MBoxEnrich(Enrich):
 
     mapping = Mapping
 
-    def __init__(self, db_sortinghat=None, db_projects_map=None, json_projects_map=None,
-                 db_user='', db_password='', db_host=''):
-        super().__init__(db_sortinghat, db_projects_map, json_projects_map,
-                         db_user, db_password, db_host)
+    def __init__(self, db_sortinghat=None, json_projects_map=None,
+                 db_user='', db_password='', db_host='', db_path=None,
+                 db_port=None, db_ssl=False, db_verify_ssl=True, db_tenant=None):
+        super().__init__(db_sortinghat=db_sortinghat, json_projects_map=json_projects_map,
+                         db_user=db_user, db_password=db_password, db_host=db_host,
+                         db_port=db_port, db_path=db_path, db_ssl=db_ssl, db_verify_ssl=db_verify_ssl,
+                         db_tenant=db_tenant)
 
         self.studies = [self.kafka_kip]
 
     def get_field_author(self):
         return "From"
 
     def get_identities(self, item):
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/github2.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/github2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -101,80 +101,93 @@
     mapping = Mapping
 
     comment_roles = ['user_data']
     issue_roles = ['assignee_data', 'user_data']
     pr_roles = ['merged_by_data', 'user_data']
     roles = ['assignee_data', 'merged_by_data', 'user_data']
 
-    def __init__(self, db_sortinghat=None, db_projects_map=None, json_projects_map=None,
-                 db_user='', db_password='', db_host=''):
-        super().__init__(db_sortinghat, db_projects_map, json_projects_map,
-                         db_user, db_password, db_host)
+    def __init__(self, db_sortinghat=None, json_projects_map=None,
+                 db_user='', db_password='', db_host='', db_path=None,
+                 db_port=None, db_ssl=False, db_verify_ssl=True, db_tenant=None):
+        super().__init__(db_sortinghat=db_sortinghat, json_projects_map=json_projects_map,
+                         db_user=db_user, db_password=db_password, db_host=db_host,
+                         db_port=db_port, db_path=db_path, db_ssl=db_ssl, db_verify_ssl=db_verify_ssl,
+                         db_tenant=db_tenant)
 
         self.studies = []
         self.studies.append(self.enrich_geolocation)
         self.studies.append(self.enrich_feelings)
         self.studies.append(self.enrich_extra_data)
         self.studies.append(self.enrich_demography)
 
     def set_elastic(self, elastic):
         self.elastic = elastic
 
+    def get_sh_backend_name(self):
+        """Retrieve the backend name for SortingHat identities."""
+
+        return "github"
+
     def get_field_author(self):
         return "user_data"
 
     def get_field_date(self):
         """ Field with the date in the JSON enriched items """
         return "grimoire_creation_date"
 
     def get_identities(self, item):
         """Return the identities from an item"""
 
         category = item['category']
         item = item['data']
-        comments_attr = None
         if category == "issue":
             identity_types = ['user', 'assignee']
-            comments_attr = 'comments_data'
+            comments_attrs = ['comments_data']
         elif category == "pull_request":
             identity_types = ['user', 'merged_by']
-            comments_attr = 'review_comments_data'
+            comments_attrs = ['review_comments_data', 'reviews_data']
         else:
             identity_types = []
+            comments_attrs = []
 
         for identity in identity_types:
             identity_attr = identity + "_data"
             if item[identity] and identity_attr in item:
                 # In user_data we have the full user data
                 user = self.get_sh_identity(item[identity_attr])
                 if user:
                     yield user
 
-        comments = item.get(comments_attr, [])
-        for comment in comments:
-            user = self.get_sh_identity(comment['user_data'])
-            if user:
-                yield user
+        for comments_attr in comments_attrs:
+            comments = item.get(comments_attr, [])
+            for comment in comments:
+                user = self.get_sh_identity(comment['user_data'])
+                if user:
+                    yield user
 
     def get_sh_identity(self, item, identity_field=None):
         identity = {}
 
         user = item  # by default a specific user dict is expected
 
         if isinstance(item, dict) and 'data' in item:
             user = item['data'][identity_field]
         elif identity_field:
             user = item[identity_field]
 
         if not user:
             return identity
 
-        identity['name'] = user.get('name', user.get('login', None))
         identity['email'] = user.get('email', None)
-        identity['username'] = user.get('username', user.get('login', None))
+        identity['name'] = user.get('name', None)
+        if not identity['name']:
+            identity['name'] = user.get('login', None)
+        identity['username'] = user.get('username', None)
+        if not identity['username']:
+            identity['username'] = user.get('login', None)
 
         return identity
 
     def get_project_repository(self, eitem):
         repo = eitem['origin']
         return repo
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/cocom.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/cocom.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -144,18 +144,21 @@
 
         return {"items": mapping}
 
 
 class CocomEnrich(Enrich):
     metrics = ["ccn", "num_funs", "tokens", "loc", "comments", "blanks"]
 
-    def __init__(self, db_sortinghat=None, db_projects_map=None, json_projects_map=None,
-                 db_user='', db_password='', db_host=''):
-        super().__init__(db_sortinghat, db_projects_map, json_projects_map,
-                         db_user, db_password, db_host)
+    def __init__(self, db_sortinghat=None, json_projects_map=None,
+                 db_user='', db_password='', db_host='', db_path=None,
+                 db_port=None, db_ssl=False, db_verify_ssl=True, db_tenant=None):
+        super().__init__(db_sortinghat=db_sortinghat, json_projects_map=json_projects_map,
+                         db_user=db_user, db_password=db_password, db_host=db_host,
+                         db_port=db_port, db_path=db_path, db_ssl=db_ssl, db_verify_ssl=db_verify_ssl,
+                         db_tenant=db_tenant)
 
         self.studies = []
         self.studies.append(self.enrich_cocom_analysis)
 
     def get_identities(self, item):
         """ Return the identities from an item """
         identities = []
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/crates.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/crates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/weblate.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/weblate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2020 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -55,18 +55,21 @@
         return {"items": mapping}
 
 
 class WeblateEnrich(Enrich):
 
     mapping = Mapping
 
-    def __init__(self, db_sortinghat=None, db_projects_map=None, json_projects_map=None,
-                 db_user='', db_password='', db_host=''):
-        super().__init__(db_sortinghat, db_projects_map, json_projects_map,
-                         db_user, db_password, db_host)
+    def __init__(self, db_sortinghat=None, json_projects_map=None,
+                 db_user='', db_password='', db_host='', db_path=None,
+                 db_port=None, db_ssl=False, db_verify_ssl=True, db_tenant=None):
+        super().__init__(db_sortinghat=db_sortinghat, json_projects_map=json_projects_map,
+                         db_user=db_user, db_password=db_password, db_host=db_host,
+                         db_port=db_port, db_path=db_path, db_ssl=db_ssl, db_verify_ssl=db_verify_ssl,
+                         db_tenant=db_tenant)
 
         self.studies = []
         self.studies.append(self.enrich_demography)
 
     def get_field_author(self):
         return "author_data"
 
@@ -170,11 +173,11 @@
 
         eitem.update(self.get_grimoire_fields(item["metadata__updated_on"], "message"))
 
         self.add_repository_labels(eitem)
         self.add_metadata_filter_raw(eitem)
         return eitem
 
-    def enrich_demography(self, ocean_backend, enrich_backend, date_field="grimoire_creation_date",
+    def enrich_demography(self, ocean_backend, enrich_backend, alias, date_field="grimoire_creation_date",
                           author_field="author_uuid"):
 
-        super().enrich_demography(ocean_backend, enrich_backend, date_field, author_field=author_field)
+        super().enrich_demography(ocean_backend, enrich_backend, alias, date_field, author_field=author_field)
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/graal_study_evolution.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/graal_study_evolution.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/functest.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/functest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/colic.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/colic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -80,18 +80,21 @@
         '''
 
         return {"items": mapping}
 
 
 class ColicEnrich(Enrich):
 
-    def __init__(self, db_sortinghat=None, db_projects_map=None, json_projects_map=None,
-                 db_user='', db_password='', db_host=''):
-        super().__init__(db_sortinghat, db_projects_map, json_projects_map,
-                         db_user, db_password, db_host)
+    def __init__(self, db_sortinghat=None, json_projects_map=None,
+                 db_user='', db_password='', db_host='', db_path=None,
+                 db_port=None, db_ssl=False, db_verify_ssl=True, db_tenant=None):
+        super().__init__(db_sortinghat=db_sortinghat, json_projects_map=json_projects_map,
+                         db_user=db_user, db_password=db_password, db_host=db_host,
+                         db_port=db_port, db_path=db_path, db_ssl=db_ssl, db_verify_ssl=db_verify_ssl,
+                         db_tenant=db_tenant)
 
         self.studies = []
         self.studies.append(self.enrich_colic_analysis)
 
     def get_identities(self, item):
         """ Return the identities from an item """
         identities = []
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/dockersmells.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/dockersmells.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -68,18 +68,21 @@
         '''
 
         return {"items": mapping}
 
 
 class Dockersmells(Enrich):
 
-    def __init__(self, db_sortinghat=None, db_projects_map=None, json_projects_map=None,
-                 db_user='', db_password='', db_host=''):
-        super().__init__(db_sortinghat, db_projects_map, json_projects_map,
-                         db_user, db_password, db_host)
+    def __init__(self, db_sortinghat=None, json_projects_map=None,
+                 db_user='', db_password='', db_host='', db_path=None,
+                 db_port=None, db_ssl=False, db_verify_ssl=True, db_tenant=None):
+        super().__init__(db_sortinghat=db_sortinghat, json_projects_map=json_projects_map,
+                         db_user=db_user, db_password=db_password, db_host=db_host,
+                         db_port=db_port, db_path=db_path, db_ssl=db_ssl, db_verify_ssl=db_verify_ssl,
+                         db_tenant=db_tenant)
 
         self.studies = []
 
     def get_identities(self, item):
         """ Return the identities from an item """
         identities = []
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/launchpad.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/launchpad.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2020 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -57,18 +57,21 @@
 
 
 class LaunchpadEnrich(Enrich):
 
     mapping = Mapping
     roles = ['assignee_data', 'owner_data']
 
-    def __init__(self, db_sortinghat=None, db_projects_map=None, json_projects_map=None,
-                 db_user='', db_password='', db_host=''):
-        super().__init__(db_sortinghat, db_projects_map, json_projects_map,
-                         db_user, db_password, db_host)
+    def __init__(self, db_sortinghat=None, json_projects_map=None,
+                 db_user='', db_password='', db_host='', db_path=None,
+                 db_port=None, db_ssl=False, db_verify_ssl=True, db_tenant=None):
+        super().__init__(db_sortinghat=db_sortinghat, json_projects_map=json_projects_map,
+                         db_user=db_user, db_password=db_password, db_host=db_host,
+                         db_port=db_port, db_path=db_path, db_ssl=db_ssl, db_verify_ssl=db_verify_ssl,
+                         db_tenant=db_tenant)
 
     def get_field_author(self):
         return "owner_data"
 
     def set_elastic(self, elastic):
         self.elastic = elastic
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/phabricator.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/phabricator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -71,17 +71,21 @@
 
 class PhabricatorEnrich(Enrich):
 
     mapping = Mapping
 
     roles = ['authorData', 'ownerData']
 
-    def __init__(self, db_sortinghat=None, db_projects_map=None, json_projects_map=None,
-                 db_user='', db_password='', db_host=''):
-        super().__init__(db_sortinghat, db_projects_map, json_projects_map, db_user, db_password, db_host)
+    def __init__(self, db_sortinghat=None, json_projects_map=None,
+                 db_user='', db_password='', db_host='', db_path=None,
+                 db_port=None, db_ssl=False, db_verify_ssl=True, db_tenant=None):
+        super().__init__(db_sortinghat=db_sortinghat, json_projects_map=json_projects_map,
+                         db_user=db_user, db_password=db_password, db_host=db_host,
+                         db_port=db_port, db_path=db_path, db_ssl=db_ssl, db_verify_ssl=db_verify_ssl,
+                         db_tenant=db_tenant)
 
         self.phab_ids_names = {}  # To convert from phab ids to phab names
 
     def get_field_event_unique_id(self):
         return "transactionID"
 
     def get_field_author(self):
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/enriched/jenkins.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/enriched/jenkins.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -55,18 +55,22 @@
 
 class JenkinsEnrich(Enrich):
 
     mapping = Mapping
 
     MAIN_NODE_NAME = "main"
 
-    def __init__(self, db_sortinghat=None, db_projects_map=None, json_projects_map=None,
-                 db_user='', db_password='', db_host='', node_regex=None):
-        super().__init__(db_sortinghat, db_projects_map, json_projects_map,
-                         db_user, db_password, db_host)
+    def __init__(self, db_sortinghat=None, json_projects_map=None,
+                 db_user='', db_password='', db_host='', db_path=None,
+                 db_port=None, db_ssl=False, db_verify_ssl=True, db_tenant=None,
+                 node_regex=None):
+        super().__init__(db_sortinghat=db_sortinghat, json_projects_map=json_projects_map,
+                         db_user=db_user, db_password=db_password, db_host=db_host,
+                         db_port=db_port, db_path=db_path, db_ssl=db_ssl, db_verify_ssl=db_verify_ssl,
+                         db_tenant=db_tenant)
         self.nodes_rename_file = None
         self.nodes_rename = {}
         self.node_regex = node_regex
 
     def set_jenkins_rename_file(self, nodes_rename_file):
         """ File with nodes renaming mapping:
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/elastic_items.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/elastic_items.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -23,65 +23,76 @@
 
 
 import json
 import logging
 import re
 import time
 
-from .enriched.utils import get_repository_filter, grimoire_con, anonymize_url
+from .enriched.utils import get_repository_filter, get_confluence_spaces_filter, grimoire_con, anonymize_url
 from .elastic_mapping import Mapping
 
 HEADER_JSON = {"Content-Type": "application/json"}
 MAX_BULK_UPDATE_SIZE = 1000
 
 FILTER_DATA_ATTR = 'data.'
 FILTER_SEPARATOR = r",\s*%s" % FILTER_DATA_ATTR
 PROJECTS_JSON_LABELS_PATTERN = r".*(--labels=\[(.*)\]).*"
+PROJECTS_JSON_SPACES_PATTERN = r".*(--spaces=\[(.*)\]).*"
 
 logger = logging.getLogger(__name__)
 
 
 class ElasticItems:
 
     mapping = Mapping
 
     # In large projects like Eclipse commits, 100 is too much
     # Change it from p2o command line or mordred config
     scroll_size = 100
     scroll_wait = 900
 
-    def __init__(self, perceval_backend, from_date=None, insecure=True, offset=None):
+    def __init__(self, perceval_backend, from_date=None, insecure=True, offset=None, to_date=None):
         """Class to perform operations over the items stored in a ES index.
 
         :param perceval_backend: Perceval backend object
         :param from_date: Date obj used to extract the items in an ES index after a given date
         :param insecure: support https with invalid certificates
         :param offset: Offset number used to extract the items in an ES index after a given offset ID
+        :param to_date: Date obj used to extract the items in an ES index before a given date
         """
         self.perceval_backend = perceval_backend
         self.last_update = None  # Last update in ocean items index for feed
         self.from_date = from_date  # fetch from_date
+        self.to_date = to_date  # fetch to_date
         self.offset = offset  # fetch from offset
         self.filter_raw = None  # to filter raw items from Ocean
         self.filter_raw_dict = []
         self.projects_json_repo = None
         self.repo_labels = None
+        self.repo_spaces = None
 
         self.requests = grimoire_con(insecure)
         self.elastic = None
         self.elastic_url = None
         self.cfg_section_name = None
 
     def get_repository_filter_raw(self, term=False):
         """Returns the filter to be used in queries in a repository items"""
 
         perceval_backend_name = self.get_connector_name()
         filter_ = get_repository_filter(self.perceval_backend, perceval_backend_name, term)
         return filter_
 
+    def get_confluence_spaces(self, repo_spaces):
+        """Returns the spaces to be used in queries in a confluence items"""
+
+        perceval_backend_name = self.get_connector_name()
+        filter_ = get_confluence_spaces_filter(repo_spaces, perceval_backend_name)
+        return filter_
+
     def get_field_date(self):
         """Field with the update in the JSON items. Now the same in all."""
 
         return "metadata__updated_on"
 
     def get_incremental_date(self):
         """Field with the date used for incremental analysis."""
@@ -98,34 +109,45 @@
     def set_repo_labels(self, labels):
         """Set the labels of the repo
 
         :param labels: list of labels (str)
         """
         self.repo_labels = labels
 
+    def set_repo_spaces(self, spaces):
+        """Set the spaces of the repo
+
+        :param spaces: list of labels (str)
+        """
+        self.repo_spaces = spaces
+
     @staticmethod
-    def extract_repo_labels(repo):
-        """Extract the labels declared in the repositories within the projects.json, and
+    def extract_repo_tags(repo, tag="labels"):
+        """Extract the tags declared in the repositories within the projects.json, and
         remove them to avoid breaking already existing functionalities.
 
         :param repo: repo url in projects.json
+        :param tag: labels | spaces
         """
         processed_repo = repo
-        labels_lst = []
+        tags_lst = []
 
-        pattern = re.compile(PROJECTS_JSON_LABELS_PATTERN)
+        tag_pattern = PROJECTS_JSON_LABELS_PATTERN
+        if tag == "spaces":
+            tag_pattern = PROJECTS_JSON_SPACES_PATTERN
+        pattern = re.compile(tag_pattern)
         matchObj = pattern.match(repo)
 
         if matchObj:
             labels_info = matchObj.group(1)
             labels = matchObj.group(2)
-            labels_lst = [label.strip() for label in labels.split(',')]
+            tags_lst = [label.strip() for label in labels.split(',')]
             processed_repo = processed_repo.replace(labels_info, '').strip()
 
-        return processed_repo, labels_lst
+        return processed_repo, tags_lst
 
     @staticmethod
     def __process_filter(fltr_raw):
         fltr = fltr_raw
 
         if not fltr_raw.startswith(FILTER_DATA_ATTR):
             fltr = FILTER_DATA_ATTR + fltr_raw
@@ -302,14 +324,21 @@
                         { "%s": %s }
                     }
                 ''' % (_filter['name'], _filter['value'])
                 # List to string conversion uses ' that are not allowed in JSON
                 filter_str = filter_str.replace("'", "\"")
                 filters += filter_str
 
+            filters_spaces_dict = self.get_confluence_spaces(self.repo_spaces)
+            if filters_spaces_dict:
+                filters_spaces = json.dumps(filters_spaces_dict)
+                filters += '''
+                    , {"bool":%s}
+                ''' % (filters_spaces)
+
             # The code below performs the incremental enrichment based on the last value of `metadata__timestamp`
             # in the enriched index, which is calculated in the TaskEnrich before enriching the single repos that
             # belong to a given data source. The old implementation of the incremental enrichment, which consisted in
             # collecting the last value of `metadata__timestamp` in the enriched index for each repo, didn't work
             # for global data source (which are collected globally and only partially enriched).
             if self.from_date and not ignore_incremental:
                 date_field = self.get_incremental_date()
@@ -355,15 +384,17 @@
 
         rjson = None
         try:
             res = self.requests.post(url, data=query_data, headers=headers)
             if self.too_many_scrolls(res):
                 return {'too_many_scrolls': True}
             res.raise_for_status()
-            rjson = res.json()
+            rjson = json.loads(json.dumps(res.json(), ensure_ascii=False)
+                               .encode('utf-8', errors='ignore').decode('utf-8'))
+
         except Exception:
             # The index could not exists yet or it could be empty
             logger.debug("No results found from {}".format(anonymize_url(url)))
 
         return rjson
 
     def too_many_scrolls(self, res):
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/meetup.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/meetup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/puppetforge.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/puppetforge.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/graal.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/crates.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -12,62 +12,54 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
-#   Nishchith Shetty <inishchith@gmail.com>
+#   Alvaro del Castillo San Felix <acs@bitergia.com>
 #
 
 from .elastic import ElasticOcean
 from ..elastic_mapping import Mapping as BaseMapping
 
 
 class Mapping(BaseMapping):
 
     @staticmethod
     def get_elastic_mappings(es_major):
         """Get Elasticsearch mapping.
 
-        Ensure data.message is string, since it can be very large
-
         :param es_major: major version of Elasticsearch, as string
         :returns:        dictionary with a key, 'items', with the mapping
         """
 
         mapping = '''
-        {
+         {
             "dynamic":true,
-            "properties": {
-                "data": {
-                    "properties": {
-                        "message": {
-                            "type": "text",
-                            "index": true
-                        },
-                        "analysis": {
-                            "dynamic":false,
-                            "properties": {}
+                "properties": {
+                    "data": {
+                        "properties": {
+                            "versions_data": {
+                                "dynamic":false,
+                                "properties": {}
+                            }
                         }
                     }
                 }
-            }
         }
         '''
 
         return {"items": mapping}
 
 
-class GraalOcean(ElasticOcean):
-    """Graal Ocean feeder"""
+class CratesOcean(ElasticOcean):
+    """Confluence Ocean feeder"""
 
     mapping = Mapping
 
     @classmethod
     def get_perceval_params_from_url(cls, url):
+        # crates does not need any param
         params = []
-        tokens = url.split(' ', 1)  # Just split the URL not the filter
-        url = tokens[0]
-        params.append(url)
 
         return params
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/gitlab.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/gitlab.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/github.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/github.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/discourse.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/discourse.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/mozillaclub.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/redmine.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -15,48 +15,55 @@
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #   Alvaro del Castillo San Felix <acs@bitergia.com>
 #
 
-from grimoire_elk.raw.elastic import ElasticOcean
+from .elastic import ElasticOcean
 from ..elastic_mapping import Mapping as BaseMapping
 
 
 class Mapping(BaseMapping):
 
     @staticmethod
     def get_elastic_mappings(es_major):
         """Get Elasticsearch mapping.
 
+        Non dynamic discovery of type for:
+            * data.journals
+
         :param es_major: major version of Elasticsearch, as string
         :returns:        dictionary with a key, 'items', with the mapping
         """
 
         mapping = '''
          {
             "dynamic":true,
                 "properties": {
                     "data": {
                         "properties": {
-                            "Event Creations": {
+                            "journals": {
+                                "dynamic": false,
+                                "properties": {}
+                            },
+                            "subject": {
                                 "type": "text",
                                 "index": true
                             },
-                            "Event Description": {
+                            "description": {
                                 "type": "text",
                                 "index": true
                             }
                         }
                     }
                 }
         }
         '''
 
         return {"items": mapping}
 
 
-class MozillaClubOcean(ElasticOcean):
-    """MozillaClub Ocean feeder"""
+class RedmineOcean(ElasticOcean):
+    """Redmine Ocean feeder"""
 
     mapping = Mapping
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/dockerhub.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/dockerhub.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/git.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/graal.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -12,15 +12,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
-#   Alvaro del Castillo San Felix <acs@bitergia.com>
+#   Nishchith Shetty <inishchith@gmail.com>
 #
 
 from .elastic import ElasticOcean
 from ..elastic_mapping import Mapping as BaseMapping
 from ..identities.git import GitIdentities
 from ..enriched.utils import anonymize_url
 
@@ -34,34 +34,38 @@
         Ensure data.message is string, since it can be very large
 
         :param es_major: major version of Elasticsearch, as string
         :returns:        dictionary with a key, 'items', with the mapping
         """
 
         mapping = '''
-         {
+        {
             "dynamic":true,
             "properties": {
                 "data": {
                     "properties": {
                         "message": {
                             "type": "text",
                             "index": true
+                        },
+                        "analysis": {
+                            "dynamic":false,
+                            "properties": {}
                         }
                     }
                 }
             }
         }
         '''
 
         return {"items": mapping}
 
 
-class GitOcean(ElasticOcean):
-    """Git Ocean feeder"""
+class GraalOcean(ElasticOcean):
+    """Graal Ocean feeder"""
 
     mapping = Mapping
     identities = GitIdentities
 
     def _fix_item(self, item):
         item['origin'] = anonymize_url(item['origin'])
         item['tag'] = anonymize_url(item['tag'])
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/remo.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/remo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/rocketchat.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/rocketchat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2020 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/mediawiki.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/mediawiki.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/groupsio.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/groupsio.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/kitsune.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/telegram.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -18,11 +18,11 @@
 # Authors:
 #   Alvaro del Castillo San Felix <acs@bitergia.com>
 #
 
 from .elastic import ElasticOcean
 
 
-class KitsuneOcean(ElasticOcean):
-    """Kitsune Ocean feeder"""
+class TelegramOcean(ElasticOcean):
+    """Telegram Ocean feeder"""
 
     pass
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/redmine.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/kitsune.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -16,54 +16,62 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #   Alvaro del Castillo San Felix <acs@bitergia.com>
 #
 
 from .elastic import ElasticOcean
-from ..elastic_mapping import Mapping as BaseMapping
+from grimoire_elk.elastic_mapping import Mapping as BaseMapping
 
 
 class Mapping(BaseMapping):
 
     @staticmethod
     def get_elastic_mappings(es_major):
         """Get Elasticsearch mapping.
 
-        Non dynamic discovery of type for:
-            * data.journals
-
         :param es_major: major version of Elasticsearch, as string
-        :returns:        dictionary with a key, 'items', with the mapping
+        :returns: dictionary with a key, 'items', with the mapping
         """
 
         mapping = '''
          {
             "dynamic":true,
-                "properties": {
-                    "data": {
-                        "properties": {
-                            "journals": {
-                                "dynamic": false,
-                                "properties": {}
-                            },
-                            "subject": {
-                                "type": "text",
-                                "index": true
-                            },
-                            "description": {
-                                "type": "text",
-                                "index": true
+            "properties": {
+                "data": {
+                    "dynamic":false,
+                    "properties": {
+                        "metadata": {
+                            "dynamic":false,
+                            "properties": {
+                                "value": {
+                                    "type": "text",
+                                    "index": true
+                                }
+                            }
+                        },
+                        "answers_data": {
+                            "dynamic":false,
+                            "properties": {
+                                "content": {
+                                    "type": "text",
+                                    "index": true
+                                }
                             }
+                        },
+                        "content": {
+                            "type": "text",
+                            "index": true
                         }
                     }
                 }
+            }
         }
         '''
 
         return {"items": mapping}
 
 
-class RedmineOcean(ElasticOcean):
-    """Redmine Ocean feeder"""
+class KitsuneOcean(ElasticOcean):
+    """Kitsune Ocean feeder"""
 
     mapping = Mapping
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/rss.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/mozillaclub.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -15,15 +15,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #   Alvaro del Castillo San Felix <acs@bitergia.com>
 #
 
-from .elastic import ElasticOcean
+from grimoire_elk.raw.elastic import ElasticOcean
 from ..elastic_mapping import Mapping as BaseMapping
 
 
 class Mapping(BaseMapping):
 
     @staticmethod
     def get_elastic_mappings(es_major):
@@ -35,34 +35,28 @@
 
         mapping = '''
          {
             "dynamic":true,
                 "properties": {
                     "data": {
                         "properties": {
-                            "content": {
-                                "dynamic":false,
-                                "properties": {}
-                            },
-                            "summary_detail": {
-                                "dynamic":false,
-                                "properties": {}
+                            "Event Creations": {
+                                "type": "text",
+                                "index": true
                             },
-                            "summary": {
+                            "Event Description": {
                                 "type": "text",
                                 "index": true
                             }
                         }
                     }
                 }
         }
         '''
 
         return {"items": mapping}
 
 
-class RSSOcean(ElasticOcean):
-    """RSS Ocean feeder"""
+class MozillaClubOcean(ElasticOcean):
+    """MozillaClub Ocean feeder"""
 
     mapping = Mapping
-
-    pass
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/gitter.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/gitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2020 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/stackexchange.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/stackexchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/jira.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/jira.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/gerrit.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/gerrit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/pipermail.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/pipermail.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/pagure.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/pagure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2020 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/githubql.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/githubql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/google_hits.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -12,19 +12,17 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
-#   Valerio Cosentino <valcos@bitergia.com>
+#     Alvaro del Castillo <acs@bitergia.com>
 #
 
-"""GoogleHits Ocean feeder"""
+import logging
 
-from .elastic import ElasticOcean
+from ._version import __version__
 
+__all__ = [__version__]
 
-class GoogleHitsOcean(ElasticOcean):
-    """GoogleHits Ocean feeder"""
-
-    pass
+logging.getLogger(__name__).addHandler(logging.NullHandler())
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/twitter.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/twitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/askbot.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/askbot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/bugzilla.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/bugzilla.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/nntp.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/nntp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/slack.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/slack.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -54,14 +54,18 @@
                                     "properties": {
                                         "latest": {
                                             "dynamic": false,
                                             "properties": {}
                                         }
                                     }
                                 },
+                                "file": {
+                                    "dynamic": false,
+                                    "properties": {}
+                                },
                                 "files": {
                                     "dynamic": false,
                                     "properties": {}
                                 },
                                 "root": {
                                    "dynamic":false,
                                     "properties": {}
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/bugzillarest.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/bugzillarest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/hyperkitty.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/hyperkitty.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/mattermost.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/mattermost.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/telegram.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/google_hits.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -12,17 +12,19 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
-#   Alvaro del Castillo San Felix <acs@bitergia.com>
+#   Valerio Cosentino <valcos@bitergia.com>
 #
 
+"""GoogleHits Ocean feeder"""
+
 from .elastic import ElasticOcean
 
 
-class TelegramOcean(ElasticOcean):
-    """Telegram Ocean feeder"""
+class GoogleHitsOcean(ElasticOcean):
+    """GoogleHits Ocean feeder"""
 
     pass
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/finosmeetings.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/launchpad.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -12,15 +12,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
-#   Valerio Cosentino <valcos@bitergia.com>
+#   Nitish Gupta <imnitish.ng@gmail.com>
 #
 
 from .elastic import ElasticOcean
 from ..elastic_mapping import Mapping as BaseMapping
 
 
 class Mapping(BaseMapping):
@@ -30,28 +30,38 @@
         """Get Elasticsearch mapping.
 
         :param es_major: major version of Elasticsearch, as string
         :returns:        dictionary with a key, 'items', with the mapping
         """
 
         mapping = '''
-         {
-            "dynamic":true,
-            "properties": {
-                "data": {
-                    "properties": {
-                        "date": {
-                            "type": "keyword"
-                        }
+             {
+                "dynamic":true,
+                "properties": {
+                    "data": {
+                        "dynamic":false,
+                        "properties": {}
                     }
                 }
             }
-        }
-        '''
+            '''
 
         return {"items": mapping}
 
 
-class FinosMeetingsOcean(ElasticOcean):
-    """FinosMeetings Ocean feeder"""
+class LaunchpadOcean(ElasticOcean):
+    """Launchpad Ocean feeder"""
 
     mapping = Mapping
+
+    @classmethod
+    def get_perceval_params_from_url(cls, url):
+        params = []
+        splits = url.split('/')
+        if '+source' in url:
+            params.append(splits[-3])
+            params.append('--package')
+            params.append(splits[-1])
+        else:
+            params.append(splits[-1])
+
+        return params
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/supybot.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/supybot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/elastic.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/elastic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -55,17 +55,18 @@
 
         parser.add_argument("-e", "--elastic_url", default="http://127.0.0.1:9200",
                             help="Host with elastic search (default: http://127.0.0.1:9200)")
         parser.add_argument("--elastic_url-enrich",
                             help="Host with elastic search and enriched indexes")
 
     def __init__(self, perceval_backend, from_date=None, fetch_archive=False,
-                 project=None, insecure=True, offset=None, anonymize=False):
+                 project=None, insecure=True, offset=None, anonymize=False,
+                 to_date=None):
 
-        super().__init__(perceval_backend, from_date, insecure, offset)
+        super().__init__(perceval_backend, from_date, insecure, offset, to_date)
 
         self.fetch_archive = fetch_archive  # fetch from archive
         self.project = project  # project to be used for this data source
         self.anonymize = anonymize
 
     def set_elastic_url(self, url):
         """ Elastic URL """
@@ -149,15 +150,15 @@
         updated = unixtime_to_datetime(item['updated_on'])
         timestamp = unixtime_to_datetime(item['timestamp'])
         item['metadata__updated_on'] = updated.isoformat()
         # Also add timestamp used in incremental enrichment
         item['metadata__timestamp'] = timestamp.isoformat()
 
     def feed(self, from_date=None, from_offset=None, category=None, branches=None,
-             latest_items=None, filter_classified=None, no_update=None):
+             latest_items=None, filter_classified=None, no_update=None, to_date=None):
         """Feed data in Elastic from Perceval"""
 
         if self.fetch_archive:
             items = self.perceval_backend.fetch_from_archive()
             self.feed_items(items)
             return
 
@@ -176,17 +177,17 @@
         if 'from_date' in signature.parameters:
             if from_date:
                 last_update = from_date
             else:
                 self.last_update = self.get_last_update_from_es(filters_=filters_)
                 last_update = self.last_update
 
-            logger.info("[{}] Incremental from: {} for {}".format(
+            logger.info("[{}] Incremental from: {} until {} for {}".format(
                         self.perceval_backend.__class__.__name__.lower(),
-                        last_update, anonymize_url(self.perceval_backend.origin)))
+                        last_update, to_date, anonymize_url(self.perceval_backend.origin)))
 
         offset = None
         if 'offset' in signature.parameters:
             if from_offset:
                 offset = from_offset
             else:
                 offset = self.elastic.get_last_offset("offset", filters_=filters_)
@@ -196,22 +197,24 @@
                             self.perceval_backend.__class__.__name__.lower(),
                             offset, anonymize_url(self.perceval_backend.origin)))
             else:
                 logger.info("[{}] Not incremental".format(
                             self.perceval_backend.__class__.__name__.lower()))
 
         params = {}
-        # category and filter_classified params are shared
+        # category, filter_classified, and to_date params are shared
         # by all Perceval backends
         if category is not None:
             params['category'] = category
         if branches is not None:
             params['branches'] = branches
         if filter_classified is not None:
             params['filter_classified'] = filter_classified
+        if to_date:
+            params['to_date'] = to_date
 
         # no_update, latest_items, from_date and offset cannot be used together,
         # thus, the params dictionary is filled with the param available
         # and Perceval is executed
         if no_update:
             params['no_update'] = no_update
             items = self.perceval_backend.fetch(**params)
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/mbox.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/mbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/crates.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/rss.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -35,31 +35,34 @@
 
         mapping = '''
          {
             "dynamic":true,
                 "properties": {
                     "data": {
                         "properties": {
-                            "versions_data": {
+                            "content": {
                                 "dynamic":false,
                                 "properties": {}
+                            },
+                            "summary_detail": {
+                                "dynamic":false,
+                                "properties": {}
+                            },
+                            "summary": {
+                                "type": "text",
+                                "index": true
                             }
                         }
                     }
                 }
         }
         '''
 
         return {"items": mapping}
 
 
-class CratesOcean(ElasticOcean):
-    """Confluence Ocean feeder"""
+class RSSOcean(ElasticOcean):
+    """RSS Ocean feeder"""
 
     mapping = Mapping
 
-    @classmethod
-    def get_perceval_params_from_url(cls, url):
-        # crates does not need any param
-        params = []
-
-        return params
+    pass
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/weblate.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/weblate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2020 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/functest.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/functest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/launchpad.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/elastic_mapping.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2020 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -12,56 +12,38 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
-#   Nitish Gupta <imnitish.ng@gmail.com>
+#   Jesus M. Gonzalez-Barahona <jgb@bitergia.com>
 #
 
-from .elastic import ElasticOcean
-from ..elastic_mapping import Mapping as BaseMapping
 
+class Mapping:
+    """Class for Elasticsearch mappings.
 
-class Mapping(BaseMapping):
+    This class will be subclassed by backends,
+    which will provide specific mappings.
+    """
 
     @staticmethod
     def get_elastic_mappings(es_major):
         """Get Elasticsearch mapping.
 
+        Different versions of Elasticsearch may need specific versions
+        of the mapping, thus using es_major to potentially provide
+        different mappings.
+
+        When the mapping depends on the version of Kibiter/Kibana,
+        we will use the Elasticsearch version anyway, since they should
+        be paired (same major version for 5 and larger, ES major version 2
+        for Kibiter/Kibana major version 4).
+
         :param es_major: major version of Elasticsearch, as string
         :returns:        dictionary with a key, 'items', with the mapping
         """
 
-        mapping = '''
-             {
-                "dynamic":true,
-                "properties": {
-                    "data": {
-                        "dynamic":false,
-                        "properties": {}
-                    }
-                }
-            }
-            '''
+        mapping = '{}'
 
         return {"items": mapping}
-
-
-class LaunchpadOcean(ElasticOcean):
-    """Launchpad Ocean feeder"""
-
-    mapping = Mapping
-
-    @classmethod
-    def get_perceval_params_from_url(cls, url):
-        params = []
-        splits = url.split('/')
-        if '+source' in url:
-            params.append(splits[-3])
-            params.append('--package')
-            params.append(splits[-1])
-        else:
-            params.append(splits[-1])
-
-        return params
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/phabricator.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/confluence.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -17,74 +17,72 @@
 #
 # Authors:
 #   Alvaro del Castillo San Felix <acs@bitergia.com>
 #
 
 from .elastic import ElasticOcean
 from ..elastic_mapping import Mapping as BaseMapping
+from ..elastic_items import ElasticItems
+from ..enriched.utils import anonymize_url
 
 
 class Mapping(BaseMapping):
 
     @staticmethod
     def get_elastic_mappings(es_major):
         """Get Elasticsearch mapping.
 
         Non dynamic discovery of type for:
-            * data.transaction: has string arrays and dicts arrays
-        Specific type for:
-            * data.fields.priority.subpriority (float)
+            * data.extensions
 
         :param es_major: major version of Elasticsearch, as string
         :returns:        dictionary with a key, 'items', with the mapping
         """
 
         mapping = '''
-        {
+         {
             "dynamic":true,
-            "properties": {
-                "data": {
-                    "properties": {
-                        "transactions": {
-                            "dynamic":false,
-                            "properties": {}
-                        },
-                        "fields": {
-                            "properties": {
-                                "priority" : {
-                                    "properties": {
-                                        "subpriority" : {"type": "float"}
+                "properties": {
+                    "data": {
+                        "properties": {
+                            "extensions": {
+                                "dynamic":false,
+                                "properties": {}
+                            },
+                            "ancestors": {
+                                "properties": {
+                                    "extensions": {
+                                        "dynamic":false,
+                                        "properties": {}
                                     }
-                                },
-                                "description": {
-                                    "dynamic":false,
-                                    "properties": {}
-                                },
-                                "custom_error_stack": {
-                                    "type": "text",
-                                    "index": true
                                 }
+                            },
+                            "body": {
+                                "dynamic":false,
+                                "properties": {}
                             }
                         }
                     }
                 }
-            }
         }
         '''
 
         return {"items": mapping}
 
 
-class PhabricatorOcean(ElasticOcean):
-    """Phabricator Ocean feeder"""
+class ConfluenceOcean(ElasticOcean):
+    """Confluence Ocean feeder"""
 
     mapping = Mapping
 
     def _fix_item(self, item):
-        # fields cannot contain dots in ES 2.2. For consistency reason, this fix is applied also
-        # to more recent versions of ES
-
-        for field in list(item["data"]["fields"]):
-            if '.' in field:
-                undotted_field = field.replace('.', '_')
-                item["data"]["fields"][undotted_field] = item["data"]["fields"][field]
-                item["data"]['fields'].pop(field)
+        item['origin'] = anonymize_url(item['origin'])
+        item['tag'] = anonymize_url(item['tag'])
+        item['data']['content_url'] = anonymize_url(item['data']['content_url'])
+
+    @classmethod
+    def get_perceval_params_from_url(cls, url):
+        url, spaces = ElasticItems.extract_repo_tags(url, "spaces")
+        params = [url]
+        if spaces:
+            params += ["--spaces"] + spaces
+        return params
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/raw/jenkins.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/raw/jenkins.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/elk.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/elk.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -13,39 +13,64 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Authors:
 #   Alvaro del Castillo San Felix <acs@bitergia.com>
+#   Quan Zhou <quan@bitergia.com>
 #
 
 import inspect
 import logging
+from functools import lru_cache
 
-from elasticsearch import Elasticsearch
+from elasticsearch import Elasticsearch, RequestsHttpConnection
 
 from perceval.backend import find_signature_parameters, Archive
 from perceval.errors import RateLimitError
 from grimoirelab_toolkit.datetime import (datetime_utcnow, str_to_datetime)
 
 from .elastic_mapping import Mapping as BaseMapping
 from .elastic_items import ElasticItems
 from .enriched.sortinghat_gelk import SortingHat
 from .enriched.utils import get_last_enrich, grimoire_con, get_diff_current_date, anonymize_url
 from .utils import get_connectors, get_connector_from_name, get_elastic
 
 IDENTITIES_INDEX = "grimoirelab_identities_cache"
+SECRET_PARAMETERS = ["--api-token", "--backend-password"]
 SIZE_SCROLL_IDENTITIES_INDEX = 1000
 
 logger = logging.getLogger(__name__)
 
 requests_ses = grimoire_con()
 
 
+def anonymize_params(parameters):
+    """ The following parameters after SECRET_PARAMETERS will be
+    replaced by 'xxxxx' until the parameter starts with '-'.
+
+    :param parameters: list of parameters
+    :return: list of anonymized parameter
+    """
+
+    secret_param = False
+    param_list = list(parameters)
+    for i, param in enumerate(param_list):
+        if secret_param and param.startswith('-'):
+            secret_param = False
+
+        if not secret_param and param in SECRET_PARAMETERS:
+            secret_param = True
+        elif secret_param:
+            param_list[i] = "xxxxx"
+
+    return tuple(param_list)
+
+
 def feed_backend(url, clean, fetch_archive, backend_name, backend_params,
                  es_index=None, es_index_enrich=None, project=None,
                  es_aliases=None, projects_json_repo=None, repo_labels=None,
                  anonymize=False):
     """ Feed Ocean with backend data """
 
     error_msg = None
@@ -67,14 +92,15 @@
             logger.error("Raw index not defined for {}".format(backend_name))
 
         repo['repo_update_start'] = datetime_utcnow().isoformat()
 
         # perceval backends fetch params
         offset = None
         from_date = None
+        to_date = None
         category = None
         branches = None
         latest_items = None
         filter_classified = None
         no_update = None
 
         backend_cmd = klass(*backend_params)
@@ -106,14 +132,20 @@
         if 'from_date' in signature.parameters:
             try:
                 # Support perceval pre and post BackendCommand refactoring
                 from_date = backend_cmd.from_date
             except AttributeError:
                 from_date = backend_cmd.parsed_args.from_date
 
+        if 'to_date' in signature.parameters:
+            try:
+                to_date = backend_cmd.to_date
+            except AttributeError:
+                to_date = backend_cmd.parsed_args.to_date
+
         if 'offset' in signature.parameters:
             try:
                 offset = backend_cmd.offset
             except AttributeError:
                 offset = backend_cmd.parsed_args.offset
 
         if 'category' in signature.parameters:
@@ -159,14 +191,16 @@
             params['category'] = category
         if branches:
             params['branches'] = branches
         if filter_classified:
             params['filter_classified'] = filter_classified
         if from_date and (from_date.replace(tzinfo=None) != str_to_datetime("1970-01-01").replace(tzinfo=None)):
             params['from_date'] = from_date
+        if to_date and (to_date.replace(tzinfo=None) != str_to_datetime("2100-01-01").replace(tzinfo=None)):
+            params['to_date'] = to_date
         if offset:
             params['from_offset'] = offset
         if no_update:
             params['no_update'] = no_update
 
         ocean_backend.feed(**params)
 
@@ -176,16 +210,26 @@
     except Exception as ex:
         if backend:
             error_msg = "Error feeding raw from {} ({}): {}".format(backend_name, backend.origin, ex)
             logger.error(error_msg, exc_info=True)
         else:
             error_msg = "Error feeding raw from {}".format(ex)
             logger.error(error_msg, exc_info=True)
+    except SystemExit:
+        anonymized_params = anonymize_params(backend_params)
+        msg = "Wrong {} arguments: {}".format(backend_name, anonymized_params)
+        error_msg = "Error feeding raw. {}".format(msg)
+        logger.error(error_msg, exc_info=True)
+
+    try:
+        msg = "[{}] Done collection for {}".format(backend_name, anonymize_url(backend.origin))
+    except AttributeError:
+        msg = "[{}] Done collection for {}".format(backend_name, anonymize_url(projects_json_repo))
+    logger.info(msg)
 
-    logger.info("[{}] Done collection for {}".format(backend_name, anonymize_url(backend.origin)))
     return error_msg
 
 
 def refresh_projects(enrich_backend):
     logger.debug("Refreshing project field in {}".format(
                  anonymize_url(enrich_backend.elastic.index_url)))
     total = 0
@@ -196,63 +240,70 @@
         eitem.update(new_project)
         yield eitem
         total += 1
 
     logger.debug("Total eitems refreshed for project field {}".format(total))
 
 
-def refresh_identities(enrich_backend, author_fields=None, author_values=None):
+def refresh_identities(enrich_backend, author_fields=None, individuals=None):
     """Refresh identities in enriched index.
 
     Retrieve items from the enriched index corresponding to enrich_backend,
     and update their identities information, with fresh data from the
     SortingHat database.
 
     Instead of the whole index, only items matching the filter_author
     filter are fitered, if that parameters is not None.
 
     :param enrich_backend: enriched backend to update
     :param  author_fields: fields to match items authored by a user
-    :param  author_values: values of the authored field to match items
+    :param  individuals: values of the authored field to match items
     """
 
     def create_filter_authors(authors, to_refresh):
         filter_authors = []
         for author in authors:
             author_name = author if author == 'author_uuid' else author + '_uuids'
             field_author = {
                 "name": author_name,
                 "value": to_refresh
             }
             filter_authors.append(field_author)
 
         return filter_authors
 
-    def update_items(new_filter_authors, non_authored_prefix=None):
+    def update_items(new_filter_authors, non_authored_prefix=None, individuals=None):
         for new_filter_author in new_filter_authors:
             for eitem in enrich_backend.fetch(new_filter_author):
                 roles = None
                 try:
                     roles = enrich_backend.roles
                 except AttributeError:
                     pass
 
-                new_identities = enrich_backend.get_item_sh_from_id(eitem, roles)
+                new_identities = enrich_backend.get_item_sh_from_id(eitem, roles, individuals)
                 eitem.update(new_identities)
                 try:
                     meta_fields = enrich_backend.meta_fields
                     meta_fields_suffixes = enrich_backend.meta_fields_suffixes
                     new_identities = enrich_backend.get_item_sh_meta_fields(eitem, meta_fields, meta_fields_suffixes,
-                                                                            non_authored_prefix)
+                                                                            non_authored_prefix, individuals=individuals)
                     eitem.update(new_identities)
                 except AttributeError:
                     pass
 
                 yield eitem
 
+    def get_author_uuids(individuals):
+        author_uuids = []
+        for individual in individuals:
+            for identity in individual['identities']:
+                author_uuids.append(identity['uuid'])
+        return author_uuids
+
     logger.debug("Refreshing identities fields from {}".format(
                  anonymize_url(enrich_backend.elastic.index_url)))
 
     total = 0
 
     max_ids = enrich_backend.elastic.max_items_clause
     logger.debug('Refreshing identities')
@@ -266,40 +317,46 @@
     if author_fields is None:
         # No filter, update all items
         for item in update_items(None):
             yield item
             total += 1
     else:
         to_refresh = []
+        author_values = get_author_uuids(individuals)
         for author_value in author_values:
             to_refresh.append(author_value)
 
             if len(to_refresh) > max_ids:
                 filter_authors = create_filter_authors(author_fields, to_refresh)
-                for item in update_items(filter_authors, non_authored_prefix):
+                for item in update_items(filter_authors, non_authored_prefix, individuals):
                     yield item
                     total += 1
 
                 to_refresh = []
 
         if len(to_refresh) > 0:
             filter_authors = create_filter_authors(author_fields, to_refresh)
-            for item in update_items(filter_authors, non_authored_prefix):
+            for item in update_items(filter_authors, non_authored_prefix, individuals):
                 yield item
                 total += 1
 
     logger.debug("Total eitems refreshed for identities fields {}".format(total))
 
 
 def load_identities(ocean_backend, enrich_backend):
     # First we add all new identities to SH
     items_count = 0
     identities_count = 0
     new_identities = []
 
+    @lru_cache(4096)
+    def insert_identity_cache(identity_tuple):
+        uid = dict((x, y) for x, y in identity_tuple)
+        new_identities.append(uid)
+
     # Support that ocean_backend is a list of items (old API)
     if isinstance(ocean_backend, list):
         items = ocean_backend
     else:
         items = ocean_backend.fetch()
 
     for item in items:
@@ -307,42 +364,30 @@
         # Get identities from new items to be added to SortingHat
         identities = enrich_backend.get_identities(item)
 
         if not identities:
             continue
 
         for identity in identities:
-            if identity not in new_identities:
-                new_identities.append(identity)
-
-            if len(new_identities) > 100:
-                inserted_identities = load_bulk_identities(items_count,
-                                                           new_identities,
-                                                           enrich_backend.sh_db,
-                                                           enrich_backend.get_connector_name())
-                identities_count += inserted_identities
+            # Insert the identity in new_identities with cache
+            identity_tuple = tuple(identity.items())
+            insert_identity_cache(identity_tuple)
+
+            if len(new_identities) >= 100:
+                SortingHat.add_identities(enrich_backend.sh_db,
+                                          new_identities,
+                                          enrich_backend.get_sh_backend_name())
+                identities_count += len(new_identities)
                 new_identities = []
 
     if new_identities:
-        inserted_identities = load_bulk_identities(items_count,
-                                                   new_identities,
-                                                   enrich_backend.sh_db,
-                                                   enrich_backend.get_connector_name())
-        identities_count += inserted_identities
-
-    return identities_count
-
-
-def load_bulk_identities(items_count, new_identities, sh_db, connector_name):
-    identities_count = len(new_identities)
-
-    SortingHat.add_identities(sh_db, new_identities, connector_name)
-
-    logger.debug("Processed {} items identities ({} identities) from {}".format(
-                 items_count, len(new_identities), connector_name))
+        SortingHat.add_identities(enrich_backend.sh_db,
+                                  new_identities,
+                                  enrich_backend.get_sh_backend_name())
+        identities_count += len(new_identities)
 
     return identities_count
 
 
 def enrich_items(ocean_backend, enrich_backend, events=False):
     total = 0
 
@@ -350,15 +395,15 @@
         total = enrich_backend.enrich_items(ocean_backend)
         enrich_backend.update_items(ocean_backend, enrich_backend)
     else:
         total = enrich_backend.enrich_events(ocean_backend)
     return total
 
 
-def get_ocean_backend(backend_cmd, enrich_backend, no_incremental, filter_raw=None):
+def get_ocean_backend(backend_cmd, enrich_backend, no_incremental, filter_raw=None, repo_spaces=None):
     """ Get the ocean backend configured to start from the last enriched date """
 
     if no_incremental:
         last_enrich = None
     else:
         last_enrich = get_last_enrich(backend_cmd, enrich_backend, filter_raw=filter_raw)
 
@@ -394,14 +439,16 @@
         if last_enrich:
             ocean_backend = connector[1](backend, from_date=last_enrich)
         else:
             ocean_backend = connector[1](backend)
 
     if filter_raw:
         ocean_backend.set_filter_raw(filter_raw)
+    if repo_spaces:
+        ocean_backend.set_repo_spaces(repo_spaces)
 
     return ocean_backend
 
 
 def do_studies(ocean_backend, enrich_backend, studies_args, retention_time=None):
     """Execute studies related to a given enrich backend. If `retention_time` is not None, the
     study data is deleted based on the number of minutes declared in `retention_time`.
@@ -435,27 +482,29 @@
                 elastic = get_elastic(enrich_backend.elastic_url, index_name)
 
                 elastic.delete_items(retention_time)
 
 
 def enrich_backend(url, clean, backend_name, backend_params, cfg_section_name,
                    ocean_index=None,
-                   ocean_index_enrich=None,
-                   db_projects_map=None, json_projects_map=None,
+                   ocean_index_enrich=None, json_projects_map=None,
                    db_sortinghat=None,
                    no_incremental=False, only_identities=False,
                    github_token=None, studies=False, only_studies=False,
                    url_enrich=None, events_enrich=False,
                    db_user=None, db_password=None, db_host=None,
+                   db_port=None, db_path=None, db_ssl=False,
+                   db_verify_ssl=True, db_tenant=None,
                    do_refresh_projects=False, do_refresh_identities=False,
                    author_id=None, author_uuid=None, filter_raw=None,
                    jenkins_rename_file=None,
                    unaffiliated_group=None, pair_programming=False,
                    node_regex=False, studies_args=None, es_enrich_aliases=None,
-                   last_enrich_date=None, projects_json_repo=None, repo_labels=None):
+                   last_enrich_date=None, projects_json_repo=None, repo_labels=None,
+                   repo_spaces=None):
     """ Enrich Ocean index """
 
     backend = None
     enrich_index = None
 
     if ocean_index or ocean_index_enrich:
         clean = False  # don't remove index, it could be shared
@@ -481,16 +530,24 @@
         else:
             if not ocean_index:
                 ocean_index = backend_name + "_" + backend.origin
             enrich_index = ocean_index + "_enrich"
         if events_enrich:
             enrich_index += "_events"
 
-        enrich_backend = connector[2](db_sortinghat, db_projects_map, json_projects_map,
-                                      db_user, db_password, db_host)
+        enrich_backend = connector[2](db_sortinghat=db_sortinghat,
+                                      json_projects_map=json_projects_map,
+                                      db_user=db_user,
+                                      db_password=db_password,
+                                      db_host=db_host,
+                                      db_port=db_port,
+                                      db_path=db_path,
+                                      db_ssl=db_ssl,
+                                      db_verify_ssl=db_verify_ssl,
+                                      db_tenant=db_tenant)
         enrich_backend.set_params(backend_params)
         # store the cfg section name in the enrich backend to recover the corresponding project name in projects.json
         enrich_backend.set_cfg_section_name(cfg_section_name)
         enrich_backend.set_from_date(last_enrich_date)
         if url_enrich:
             elastic_enrich = get_elastic(url_enrich, enrich_index, clean, enrich_backend, es_enrich_aliases)
         else:
@@ -508,15 +565,17 @@
         # The filter raw is needed to be able to assign the project value to an enriched item
         # see line 544, grimoire_elk/enriched/enrich.py (fltr = eitem['origin'] + ' --filter-raw=' + self.filter_raw)
         if filter_raw:
             enrich_backend.set_filter_raw(filter_raw)
 
         enrich_backend.set_projects_json_repo(projects_json_repo)
         enrich_backend.set_repo_labels(repo_labels)
-        ocean_backend = get_ocean_backend(backend_cmd, enrich_backend, no_incremental, filter_raw)
+        enrich_backend.set_repo_spaces(repo_spaces)
+
+        ocean_backend = get_ocean_backend(backend_cmd, enrich_backend, no_incremental, filter_raw, repo_spaces)
 
         if only_studies:
             logger.info("Running only studies (no SH and no enrichment)")
             do_studies(ocean_backend, enrich_backend, studies_args)
         elif do_refresh_projects:
             logger.info("Refreshing project field in {}".format(
                         anonymize_url(enrich_backend.elastic.index_url)))
@@ -546,15 +605,17 @@
             ocean_backend.set_elastic(elastic_ocean)
 
             logger.debug("Adding enrichment data to {}".format(
                          anonymize_url(enrich_backend.elastic.index_url)))
 
             if db_sortinghat and enrich_backend.has_identities():
                 # FIXME: This step won't be done from enrich in the future
+                logger.info(f"[{backend_name}] Load identities process starts")
                 total_ids = load_identities(ocean_backend, enrich_backend)
+                logger.info(f"[{backend_name}] Load identities process ends")
                 logger.debug("Total identities loaded {} ".format(total_ids))
 
             if only_identities:
                 logger.debug("Only SH identities added. Enrich not done!")
 
             else:
                 # Enrichment for the new items once SH update is finished
@@ -571,16 +632,26 @@
 
     except Exception as ex:
         if backend:
             logger.error("Error enriching raw from {} ({}): {}".format(
                          backend_name, anonymize_url(backend.origin), ex), exc_info=True)
         else:
             logger.error("Error enriching raw {}".format(ex), exc_info=True)
+    except SystemExit:
+        anonymized_params = anonymize_params(backend_params)
+        msg = "Wrong {} arguments: {}".format(backend_name, anonymized_params)
+        error_msg = "Error enriching raw. {}".format(msg)
+        logger.error(error_msg, exc_info=True)
+
+    try:
+        msg = "[{}] Done enrichment for {}".format(backend_name, anonymize_url(backend.origin))
+    except AttributeError:
+        msg = "[{}] Done enrichment for {}".format(backend_name, anonymize_url(projects_json_repo))
 
-    logger.info("[{}] Done enrichment for {}".format(backend_name, anonymize_url(backend.origin)))
+    logger.info(msg)
 
 
 def delete_orphan_unique_identities(es, sortinghat_db, current_data_source, active_data_sources):
     """Delete all unique identities which appear in SortingHat, but not in the IDENTITIES_INDEX.
 
     :param es: ElasticSearchDSL object
     :param sortinghat_db: instance of the SortingHat database
@@ -621,42 +692,42 @@
         """Delete a list of uuids from SortingHat.
 
         :param target_uuids: uuids to be deleted
         """
         count = 0
 
         for uuid in target_uuids:
-            success = SortingHat.remove_unique_identity(sortinghat_db, uuid)
+            success = SortingHat.remove_identity(sortinghat_db, uuid)
             count = count + 1 if success else count
 
         return count
 
     def delete_identities(unique_ident, data_sources):
         """Remove the identities in non active data sources.
 
         :param unique_ident: unique identity object
         :param data_sources: target data sources
         """
         count = 0
-        for ident in unique_ident.identities:
-            if ident.source not in data_sources:
-                success = SortingHat.remove_identity(sortinghat_db, ident.id)
+        for ident in unique_ident['identities']:
+            if ident['source'] not in data_sources:
+                success = SortingHat.remove_identity(sortinghat_db, ident['uuid'])
                 count = count + 1 if success else count
 
         return count
 
     def has_identities_in_data_sources(unique_ident, data_sources):
         """Check if a unique identity has identities in a set of data sources.
 
         :param unique_ident: unique identity object
         :param data_sources: target data sources
         """
         in_active = False
-        for ident in unique_ident.identities:
-            if ident.source in data_sources:
+        for ident in unique_ident['identities']:
+            if ident['source'] in data_sources:
                 in_active = True
                 break
 
         return in_active
 
     deleted_unique_identities = 0
     deleted_identities = 0
@@ -676,15 +747,15 @@
         # Process only the unique identities that include the current data source, since
         # it may be that unique identities in other data source have not been
         # added yet to IDENTITIES_INDEX
         if not has_identities_in_data_sources(unique_identity, [current_data_source]):
             continue
 
         # Add the uuid to the list to check its existence in the IDENTITIES_INDEX
-        uuids_to_process.append(unique_identity.uuid)
+        uuids_to_process.append(unique_identity['mk'])
 
         # Process the uuids in block of SIZE_SCROLL_IDENTITIES_INDEX
         if len(uuids_to_process) != SIZE_SCROLL_IDENTITIES_INDEX:
             continue
 
         # Find which uuids to be processed exist in IDENTITIES_INDEX
         results = get_uuids_in_index(uuids_to_process)
@@ -747,15 +818,15 @@
         return
 
     count = 0
 
     while scroll_size > 0:
         for item in page['hits']['hits']:
             to_delete = item['_source']['sh_uuid']
-            success = SortingHat.remove_unique_identity(sortinghat_db, to_delete)
+            success = SortingHat.remove_identity(sortinghat_db, to_delete)
             # increment the number of deleted identities only if the corresponding command was successful
             count = count + 1 if success else count
 
         page = es.scroll(scroll_id=sid, scroll='60m')
         sid = page['_scroll_id']
         scroll_size = len(page['hits']['hits'])
 
@@ -772,15 +843,16 @@
     :param sortinghat_db: instance of the SortingHat database
     :param data_source: target data source (e.g., git, github, slack)
     :param active_data_sources: list of active data sources
     """
     before_date = get_diff_current_date(minutes=retention_time)
     before_date_str = before_date.isoformat()
 
-    es = Elasticsearch([es_enrichment_url], timeout=120, max_retries=20, retry_on_timeout=True, verify_certs=False)
+    es = Elasticsearch([es_enrichment_url], timeout=120, max_retries=20, retry_on_timeout=True,
+                       connection_class=RequestsHttpConnection, verify_certs=False)
 
     # delete the unique identities which have not been seen after `before_date`
     delete_inactive_unique_identities(es, sortinghat_db, before_date_str)
     # delete the unique identities for a given data source which are not in the IDENTITIES_INDEX
     delete_orphan_unique_identities(es, sortinghat_db, data_source, active_data_sources)
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/identities/meetup.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/identities/meetup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2020 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/identities/identities.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/identities/identities.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2020 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/identities/gitlab.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/identities/gitlab.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2020 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/identities/github.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/identities/github.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2020 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/identities/git.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/identities/git.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2020 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/identities/stackexchange.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/identities/stackexchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2020 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/elastic_analyzer.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/elastic_analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2021 Bitergia
+# Copyright (C) 2021-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/utils.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2020 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -22,14 +22,16 @@
 
 import argparse
 import logging
 import sys
 
 import requests
 
+import pkg_resources
+
 from grimoire_elk.errors import ElasticError
 from grimoire_elk.elastic import ElasticSearch
 # Connectors for Graal
 from graal.backends.core.coqua import CoQua, CoQuaCommand
 from graal.backends.core.cocom import CoCom, CoComCommand
 from graal.backends.core.codep import CoDep, CoDepCommand
 from graal.backends.core.colic import CoLic, CoLicCommand
@@ -37,15 +39,14 @@
 from grimoire_elk.raw.hyperkitty import HyperKittyOcean
 from perceval.backends.core.askbot import Askbot, AskbotCommand
 from perceval.backends.core.bugzilla import Bugzilla, BugzillaCommand
 from perceval.backends.core.bugzillarest import BugzillaREST, BugzillaRESTCommand
 from perceval.backends.core.confluence import Confluence, ConfluenceCommand
 from perceval.backends.core.discourse import Discourse, DiscourseCommand
 from perceval.backends.core.dockerhub import DockerHub, DockerHubCommand
-from perceval.backends.finos.finosmeetings import FinosMeetings, FinosMeetingsCommand
 from perceval.backends.core.gerrit import Gerrit, GerritCommand
 from perceval.backends.core.git import Git, GitCommand
 from perceval.backends.core.github import GitHub, GitHubCommand
 from perceval.backends.core.githubql import GitHubQL, GitHubQLCommand
 from perceval.backends.core.gitlab import GitLab, GitLabCommand
 from perceval.backends.core.gitter import Gitter, GitterCommand
 from perceval.backends.core.googlehits import GoogleHits, GoogleHitsCommand
@@ -86,15 +87,14 @@
 from .enriched.colic import ColicEnrich
 from .enriched.dockerdeps import Dockerdeps
 from .enriched.dockersmells import Dockersmells
 from .enriched.confluence import ConfluenceEnrich
 from .enriched.crates import CratesEnrich
 from .enriched.discourse import DiscourseEnrich
 from .enriched.dockerhub import DockerHubEnrich
-from .enriched.finosmeetings import FinosMeetingsEnrich
 from .enriched.functest import FunctestEnrich
 from .enriched.gerrit import GerritEnrich
 from .enriched.git import GitEnrich
 from .enriched.github import GitHubEnrich
 from .enriched.githubql import GitHubQLEnrich
 from .enriched.github2 import GitHubEnrich2
 from .enriched.gitlab import GitLabEnrich
@@ -131,15 +131,14 @@
 from .raw.bugzilla import BugzillaOcean
 from .raw.bugzillarest import BugzillaRESTOcean
 from .raw.confluence import ConfluenceOcean
 from .raw.crates import CratesOcean
 from .raw.discourse import DiscourseOcean
 from .raw.dockerhub import DockerHubOcean
 from .raw.elastic import ElasticOcean
-from .raw.finosmeetings import FinosMeetingsOcean
 from .raw.functest import FunctestOcean
 from .raw.gerrit import GerritOcean
 from .raw.git import GitOcean
 from .raw.github import GitHubOcean
 from .raw.githubql import GitHubQLOcean
 from .raw.gitlab import GitLabOcean
 from .raw.gitter import GitterOcean
@@ -171,14 +170,16 @@
 from .raw.twitter import TwitterOcean
 from .raw.weblate import WeblateOcean
 
 logger = logging.getLogger(__name__)
 
 kibiter_version = None
 
+ENTRY_POINT_NAME = "grimoire_elk"
+
 
 def get_connector_from_name(name):
 
     # Remove extra data from data source section: remo:activities
     name = name.split(":")[0]
     found = None
     connectors = get_connectors()
@@ -222,63 +223,66 @@
                 else:
                     found = cname
     return found
 
 
 def get_connectors():
 
-    return {"askbot": [Askbot, AskbotOcean, AskbotEnrich, AskbotCommand],
-            "bugzilla": [Bugzilla, BugzillaOcean, BugzillaEnrich, BugzillaCommand],
-            "bugzillarest": [BugzillaREST, BugzillaRESTOcean, BugzillaRESTEnrich, BugzillaRESTCommand],
-            "cocom": [CoCom, GraalOcean, CocomEnrich, CoComCommand],
-            "colic": [CoLic, GraalOcean, ColicEnrich, CoLicCommand],
-            "dockerdeps": [CoDep, GraalOcean, Dockerdeps, CoDepCommand],
-            "dockersmells": [CoQua, GraalOcean, Dockersmells, CoQuaCommand],
-            "confluence": [Confluence, ConfluenceOcean, ConfluenceEnrich, ConfluenceCommand],
-            "crates": [Crates, CratesOcean, CratesEnrich, CratesCommand],
-            "discourse": [Discourse, DiscourseOcean, DiscourseEnrich, DiscourseCommand],
-            "dockerhub": [DockerHub, DockerHubOcean, DockerHubEnrich, DockerHubCommand],
-            "finosmeetings": [FinosMeetings, FinosMeetingsOcean, FinosMeetingsEnrich, FinosMeetingsCommand],
-            "functest": [Functest, FunctestOcean, FunctestEnrich, FunctestCommand],
-            "gerrit": [Gerrit, GerritOcean, GerritEnrich, GerritCommand],
-            "git": [Git, GitOcean, GitEnrich, GitCommand],
-            "github": [GitHub, GitHubOcean, GitHubEnrich, GitHubCommand],
-            "githubql": [GitHubQL, GitHubQLOcean, GitHubQLEnrich, GitHubQLCommand],
-            "github2": [GitHub, GitHubOcean, GitHubEnrich2, GitHubCommand],
-            "gitlab": [GitLab, GitLabOcean, GitLabEnrich, GitLabCommand],
-            "gitter": [Gitter, GitterOcean, GitterEnrich, GitterCommand],
-            "google_hits": [GoogleHits, GoogleHitsOcean, GoogleHitsEnrich, GoogleHitsCommand],
-            "groupsio": [Groupsio, GroupsioOcean, GroupsioEnrich, GroupsioCommand],
-            "hyperkitty": [HyperKitty, HyperKittyOcean, HyperKittyEnrich, HyperKittyCommand],
-            "jenkins": [Jenkins, JenkinsOcean, JenkinsEnrich, JenkinsCommand],
-            "jira": [Jira, JiraOcean, JiraEnrich, JiraCommand],
-            "kitsune": [Kitsune, KitsuneOcean, KitsuneEnrich, KitsuneCommand],
-            "launchpad": [Launchpad, LaunchpadOcean, LaunchpadEnrich, LaunchpadCommand],
-            "mattermost": [Mattermost, MattermostOcean, MattermostEnrich, MattermostCommand],
-            "mbox": [MBox, MBoxOcean, MBoxEnrich, MBoxCommand],
-            "mediawiki": [MediaWiki, MediaWikiOcean, MediaWikiEnrich, MediaWikiCommand],
-            "meetup": [Meetup, MeetupOcean, MeetupEnrich, MeetupCommand],
-            "mozillaclub": [MozillaClub, MozillaClubOcean, MozillaClubEnrich, MozillaClubCommand],
-            "nntp": [NNTP, NNTPOcean, NNTPEnrich, NNTPCommand],
-            "pagure": [Pagure, PagureOcean, PagureEnrich, PagureCommand],
-            "phabricator": [Phabricator, PhabricatorOcean, PhabricatorEnrich, PhabricatorCommand],
-            "pipermail": [Pipermail, PipermailOcean, PipermailEnrich, PipermailCommand],
-            "puppetforge": [PuppetForge, PuppetForgeOcean, PuppetForgeEnrich, PuppetForgeCommand],
-            "redmine": [Redmine, RedmineOcean, RedmineEnrich, RedmineCommand],
-            "remo": [ReMo, ReMoOcean, ReMoEnrich, ReMoCommand],
-            "rocketchat": [RocketChat, RocketChatOcean, RocketChatEnrich, RocketChatCommand],
-            "rss": [RSS, RSSOcean, RSSEnrich, RSSCommand],
-            "slack": [Slack, SlackOcean, SlackEnrich, SlackCommand],
-            "stackexchange": [StackExchange, StackExchangeOcean,
-                              StackExchangeEnrich, StackExchangeCommand],
-            "supybot": [Supybot, SupybotOcean, SupybotEnrich, SupybotCommand],
-            "telegram": [Telegram, TelegramOcean, TelegramEnrich, TelegramCommand],
-            "twitter": [Twitter, TwitterOcean, TwitterEnrich, TwitterCommand],
-            "weblate": [Weblate, WeblateOcean, WeblateEnrich, WeblateCommand]
-            }  # Will come from Registry
+    connectors = {"askbot": [Askbot, AskbotOcean, AskbotEnrich, AskbotCommand],
+                  "bugzilla": [Bugzilla, BugzillaOcean, BugzillaEnrich, BugzillaCommand],
+                  "bugzillarest": [BugzillaREST, BugzillaRESTOcean, BugzillaRESTEnrich, BugzillaRESTCommand],
+                  "cocom": [CoCom, GraalOcean, CocomEnrich, CoComCommand],
+                  "colic": [CoLic, GraalOcean, ColicEnrich, CoLicCommand],
+                  "dockerdeps": [CoDep, GraalOcean, Dockerdeps, CoDepCommand],
+                  "dockersmells": [CoQua, GraalOcean, Dockersmells, CoQuaCommand],
+                  "confluence": [Confluence, ConfluenceOcean, ConfluenceEnrich, ConfluenceCommand],
+                  "crates": [Crates, CratesOcean, CratesEnrich, CratesCommand],
+                  "discourse": [Discourse, DiscourseOcean, DiscourseEnrich, DiscourseCommand],
+                  "dockerhub": [DockerHub, DockerHubOcean, DockerHubEnrich, DockerHubCommand],
+                  "functest": [Functest, FunctestOcean, FunctestEnrich, FunctestCommand],
+                  "gerrit": [Gerrit, GerritOcean, GerritEnrich, GerritCommand],
+                  "git": [Git, GitOcean, GitEnrich, GitCommand],
+                  "github": [GitHub, GitHubOcean, GitHubEnrich, GitHubCommand],
+                  "githubql": [GitHubQL, GitHubQLOcean, GitHubQLEnrich, GitHubQLCommand],
+                  "github2": [GitHub, GitHubOcean, GitHubEnrich2, GitHubCommand],
+                  "gitlab": [GitLab, GitLabOcean, GitLabEnrich, GitLabCommand],
+                  "gitter": [Gitter, GitterOcean, GitterEnrich, GitterCommand],
+                  "google_hits": [GoogleHits, GoogleHitsOcean, GoogleHitsEnrich, GoogleHitsCommand],
+                  "groupsio": [Groupsio, GroupsioOcean, GroupsioEnrich, GroupsioCommand],
+                  "hyperkitty": [HyperKitty, HyperKittyOcean, HyperKittyEnrich, HyperKittyCommand],
+                  "jenkins": [Jenkins, JenkinsOcean, JenkinsEnrich, JenkinsCommand],
+                  "jira": [Jira, JiraOcean, JiraEnrich, JiraCommand],
+                  "kitsune": [Kitsune, KitsuneOcean, KitsuneEnrich, KitsuneCommand],
+                  "launchpad": [Launchpad, LaunchpadOcean, LaunchpadEnrich, LaunchpadCommand],
+                  "mattermost": [Mattermost, MattermostOcean, MattermostEnrich, MattermostCommand],
+                  "mbox": [MBox, MBoxOcean, MBoxEnrich, MBoxCommand],
+                  "mediawiki": [MediaWiki, MediaWikiOcean, MediaWikiEnrich, MediaWikiCommand],
+                  "meetup": [Meetup, MeetupOcean, MeetupEnrich, MeetupCommand],
+                  "mozillaclub": [MozillaClub, MozillaClubOcean, MozillaClubEnrich, MozillaClubCommand],
+                  "nntp": [NNTP, NNTPOcean, NNTPEnrich, NNTPCommand],
+                  "pagure": [Pagure, PagureOcean, PagureEnrich, PagureCommand],
+                  "phabricator": [Phabricator, PhabricatorOcean, PhabricatorEnrich, PhabricatorCommand],
+                  "pipermail": [Pipermail, PipermailOcean, PipermailEnrich, PipermailCommand],
+                  "puppetforge": [PuppetForge, PuppetForgeOcean, PuppetForgeEnrich, PuppetForgeCommand],
+                  "redmine": [Redmine, RedmineOcean, RedmineEnrich, RedmineCommand],
+                  "remo": [ReMo, ReMoOcean, ReMoEnrich, ReMoCommand],
+                  "rocketchat": [RocketChat, RocketChatOcean, RocketChatEnrich, RocketChatCommand],
+                  "rss": [RSS, RSSOcean, RSSEnrich, RSSCommand],
+                  "slack": [Slack, SlackOcean, SlackEnrich, SlackCommand],
+                  "stackexchange": [StackExchange, StackExchangeOcean,
+                                    StackExchangeEnrich, StackExchangeCommand],
+                  "supybot": [Supybot, SupybotOcean, SupybotEnrich, SupybotCommand],
+                  "telegram": [Telegram, TelegramOcean, TelegramEnrich, TelegramCommand],
+                  "twitter": [Twitter, TwitterOcean, TwitterEnrich, TwitterCommand],
+                  "weblate": [Weblate, WeblateOcean, WeblateEnrich, WeblateCommand]
+                  }  # Will come from Registry
+
+    for entry_point in pkg_resources.iter_entry_points(ENTRY_POINT_NAME):
+        connectors.update(entry_point.load()())
+    return connectors
 
 
 def get_elastic(url, es_index, clean=None, backend=None, es_aliases=None, mapping=None):
 
     analyzers = None
 
     if backend:
```

### Comparing `grimoire-elk-0.99.0/grimoire_elk/elastic.py` & `grimoire_elk-1.0.0rc1/grimoire_elk/elastic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2015-2019 Bitergia
+# Copyright (C) 2015-2023 Bitergia
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -55,17 +55,19 @@
         :param mappings: an instance of the Mapping class
         :param clean: if True, deletes an existing index and create it again
         :param insecure: support https with invalid certificates
         :param analyzers: analyzers for ElasticSearch
         :param aliases: list of aliases, defined as strings, to be added to the index
         """
         # Get major version of Elasticsearch instance
-        self.major = self.check_instance(url, insecure)
-        logger.debug("Found version of ES instance at {}: {}.".format(
-                     anonymize_url(url), self.major))
+        major, distribution = self.check_instance(url, insecure)
+        self.major = major
+        self.distribution = distribution
+        logger.debug("Found version of {} instance at {}: {}.".format(
+                     self.distribution, anonymize_url(url), self.major))
 
         self.url = url
 
         # Valid index for elastic
         self.index = self.safe_index(index)
         self.aliases = aliases
 
@@ -107,35 +109,36 @@
         index = unique_id
         if unique_id:
             index = unique_id.replace("/", "_").lower()
         return index
 
     @staticmethod
     def check_instance(url, insecure):
-        """Checks if there is an instance of Elasticsearch in url.
+        """Checks if there is an instance of ElasticSearch/OpenSearch in url.
 
         Actually, it checks if GET on the url returns a JSON document
         with a field tagline "You know, for search",
         and a field version.number.
 
         :value      url: url of the instance to check
         :value insecure: don't verify ssl connection (boolean)
 
-        :returns:        major version of Elasticsearch, as string.
+        :returns:        major version, as str and the distribution name.
         """
         res = grimoire_con(insecure).get(url)
         if res.status_code != 200:
             msg = "Got {} from url {}".format(res.status_code, url)
             logger.error(msg)
             raise ElasticError(cause=msg)
         else:
             try:
                 version_str = res.json()['version']['number']
                 version_major = version_str.split('.')[0]
-                return version_major
+                distribution = res.json()['version'].get('distribution', 'elasticsearch')
+                return version_major, distribution
             except Exception:
                 msg = "Could not read proper welcome message from url {}, {}".format(
                     anonymize_url(url),
                     res.text
                 )
                 logger.error(msg)
                 raise ElasticError(cause=msg)
@@ -291,27 +294,27 @@
             return
 
         logger.info("Alias {} created on {}.".format(alias, anonymize_url(self.index_url)))
 
     def get_bulk_url(self):
         """Get the bulk URL endpoint"""
 
-        if self.major == '7':
+        if not self.is_legacy():
             bulk_url = self.index_url + '/_bulk'
         else:
             bulk_url = self.index_url + '/items/_bulk'
 
         return bulk_url
 
     def get_mapping_url(self, _type=None):
         """Get the mapping URL endpoint
 
-        :param _type: type of the mapping. In case of ES7, it is None
+        :param _type: type of the mapping. In case of ES >= 7, it is None
         """
-        if self.major == '7':
+        if not self.is_legacy():
             mapping_url = self.index_url + "/_mapping"
         else:
             mapping_url = self.index_url + "/" + _type + "/_mapping"
 
         return mapping_url
 
     def bulk_upload(self, items, field_id):
@@ -600,7 +603,21 @@
                 properties = items_mapping.get('properties', {}) if items_mapping else {}
 
         except requests.exceptions.HTTPError as ex:
             logger.error("Error all attributes for {}. {}".format(anonymize_url(self.index_url), ex))
             return
 
         return properties
+
+    def is_legacy(self):
+        """ Simply calls the static version with it's own values """
+        return ElasticSearch.is_legacy_static(self.major, self.distribution)
+
+    @staticmethod
+    def is_legacy_static(major, distribution):
+        """ Returns true if ES < 7 or OS < 1, false otherwise.
+        Static version exists because not every place that uses this check has an ES object."""
+        if major is None:
+            return False
+        int_maj = int(major)
+        return ((int_maj < 7 and distribution == 'elasticsearch')
+                or (int_maj < 1 and distribution == 'opensearch'))
```

