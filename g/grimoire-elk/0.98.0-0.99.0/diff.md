# Comparing `tmp/grimoire-elk-0.98.0.tar.gz` & `tmp/grimoire-elk-0.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/dist/grimoire-elk-0.98.0.tar", last modified: Thu Jan 13 12:48:01 2022, max compression
+gzip compressed data, was "/tmp/dist/grimoire-elk-0.99.0.tar", last modified: Thu Jan 27 11:03:58 2022, max compression
```

## Comparing `grimoire-elk-0.98.0.tar` & `grimoire-elk-0.99.0.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxrwxr-x   0 quan      (1001) quan      (1001)        0 2022-01-13 12:48:01.000000 grimoire-elk-0.98.0/
--rw-rw-r--   0 quan      (1001) quan      (1001)      204 2022-01-13 12:48:01.000000 grimoire-elk-0.98.0/setup.cfg
--rw-rw-r--   0 quan      (1001) quan      (1001)     2421 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/pyproject.toml
-drwxrwxr-x   0 quan      (1001) quan      (1001)        0 2022-01-13 12:48:01.000000 grimoire-elk-0.98.0/grimoire_elk.egg-info/
--rw-rw-r--   0 quan      (1001) quan      (1001)        1 2022-01-13 12:48:01.000000 grimoire-elk-0.98.0/grimoire_elk.egg-info/dependency_links.txt
--rw-rw-r--   0 quan      (1001) quan      (1001)     4275 2022-01-13 12:48:01.000000 grimoire-elk-0.98.0/grimoire_elk.egg-info/SOURCES.txt
--rw-rw-r--   0 quan      (1001) quan      (1001)        1 2022-01-13 12:48:01.000000 grimoire-elk-0.98.0/grimoire_elk.egg-info/not-zip-safe
--rw-rw-r--   0 quan      (1001) quan      (1001)      411 2022-01-13 12:48:01.000000 grimoire-elk-0.98.0/grimoire_elk.egg-info/requires.txt
--rw-rw-r--   0 quan      (1001) quan      (1001)    13847 2022-01-13 12:48:01.000000 grimoire-elk-0.98.0/grimoire_elk.egg-info/PKG-INFO
--rw-rw-r--   0 quan      (1001) quan      (1001)       13 2022-01-13 12:48:01.000000 grimoire-elk-0.98.0/grimoire_elk.egg-info/top_level.txt
--rw-rw-r--   0 quan      (1001) quan      (1001)    13847 2022-01-13 12:48:01.000000 grimoire-elk-0.98.0/PKG-INFO
-drwxrwxr-x   0 quan      (1001) quan      (1001)        0 2022-01-13 12:48:01.000000 grimoire-elk-0.98.0/utils/
--rwxrwxr-x   0 quan      (1001) quan      (1001)     5183 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/utils/gelk_mapping.py
--rwxrwxr-x   0 quan      (1001) quan      (1001)     3963 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/utils/p2o.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    35147 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/LICENSE
--rw-rw-r--   0 quan      (1001) quan      (1001)    13009 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/README.md
--rw-rw-r--   0 quan      (1001) quan      (1001)       18 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/MANIFEST.in
-drwxrwxr-x   0 quan      (1001) quan      (1001)        0 2022-01-13 12:48:01.000000 grimoire-elk-0.98.0/grimoire_elk/
--rw-rw-r--   0 quan      (1001) quan      (1001)       23 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/_version.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1309 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/errors.py
-drwxrwxr-x   0 quan      (1001) quan      (1001)        0 2022-01-13 12:48:01.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/
--rw-rw-r--   0 quan      (1001) quan      (1001)     5209 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/sortinghat_gelk.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    13610 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/meetup.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     6687 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/puppetforge.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    16209 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/gitlab.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    36434 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/github.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    12332 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/discourse.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     6172 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/mozillaclub.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     6144 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/dockerhub.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     8696 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/study_ceres_aoc.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    45718 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/git.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     8036 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/remo.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     6787 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/rocketchat.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     9130 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/mediawiki.py
--rw-rw-r--   0 quan      (1001) quan      (1001)      897 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/groupsio.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     8747 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/kitsune.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    12673 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/ceres_base.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    16606 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/mbox_study_kip.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     5566 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/redmine.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     3481 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/rss.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     5408 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/gitter.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    10011 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/stackexchange.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    18578 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/jira.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    32205 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/gerrit.py
--rw-rw-r--   0 quan      (1001) quan      (1001)      907 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/pipermail.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    12855 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/pagure.py
--rw-rw-r--   0 quan      (1001) quan      (1001)        0 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/__init__.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    33027 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/githubql.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1670 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/google_hits.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     5431 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/twitter.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     4691 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/dockerdeps.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    14023 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/askbot.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     7284 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/bugzilla.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    15829 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/study_ceres_onion.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1052 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/nntp.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    23552 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/slack.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    91958 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/enrich.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     6067 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/bugzillarest.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     5408 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/github_study_evolution.py
--rw-rw-r--   0 quan      (1001) quan      (1001)      908 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/hyperkitty.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     5141 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/confluence.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     8339 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/mattermost.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     5328 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/telegram.py
--rwxrwxr-x   0 quan      (1001) quan      (1001)     7997 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/utils.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     3747 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/finosmeetings.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     3362 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/supybot.py
-drwxrwxr-x   0 quan      (1001) quan      (1001)        0 2022-01-13 12:48:01.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/mappings/
--rw-rw-r--   0 quan      (1001) quan      (1001)      981 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/mappings/onion.json
--rw-rw-r--   0 quan      (1001) quan      (1001)      961 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/mappings/onion_es7.json
--rw-rw-r--   0 quan      (1001) quan      (1001)     2552 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/mappings/git_aoc.json
--rw-rw-r--   0 quan      (1001) quan      (1001)     2295 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/mappings/git_aoc_es7.json
--rw-rw-r--   0 quan      (1001) quan      (1001)     8144 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/mbox.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    27230 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/github2.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    15340 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/cocom.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     5296 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/crates.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     6286 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/weblate.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     5648 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/graal_study_evolution.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     6242 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/functest.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    16216 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/colic.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     4922 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/dockersmells.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     7797 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/launchpad.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2233 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/database.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    15732 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/phabricator.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     8332 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/enriched/jenkins.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    14188 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/elastic_items.py
-drwxrwxr-x   0 quan      (1001) quan      (1001)        0 2022-01-13 12:48:01.000000 grimoire-elk-0.98.0/grimoire_elk/raw/
--rw-rw-r--   0 quan      (1001) quan      (1001)     2666 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/meetup.py
--rw-rw-r--   0 quan      (1001) quan      (1001)      874 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/puppetforge.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2074 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/graal.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     3448 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/gitlab.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     4828 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/github.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     3488 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/discourse.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1882 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/mozillaclub.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2036 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/dockerhub.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2178 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/git.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1788 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/remo.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1863 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/rocketchat.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2128 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/mediawiki.py
--rw-rw-r--   0 quan      (1001) quan      (1001)      882 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/groupsio.py
--rw-rw-r--   0 quan      (1001) quan      (1001)      875 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/kitsune.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2088 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/redmine.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2023 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/rss.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1831 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/gitter.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2613 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/stackexchange.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     3442 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/jira.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     3017 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/gerrit.py
--rw-rw-r--   0 quan      (1001) quan      (1001)      892 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/pipermail.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1921 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/pagure.py
--rw-rw-r--   0 quan      (1001) quan      (1001)        0 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/__init__.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1853 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/githubql.py
--rw-rw-r--   0 quan      (1001) quan      (1001)      903 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/google_hits.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     3815 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/twitter.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2181 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/askbot.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2450 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/bugzilla.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2113 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/nntp.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2900 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/slack.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     4458 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/bugzillarest.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1831 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/hyperkitty.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2288 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/confluence.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     5204 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/mattermost.py
--rw-rw-r--   0 quan      (1001) quan      (1001)      877 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/telegram.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1594 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/finosmeetings.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1044 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/supybot.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    11043 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/elastic.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2249 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/mbox.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1836 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/crates.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1899 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/weblate.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2341 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/functest.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1870 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/launchpad.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     3052 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/phabricator.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     5603 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/raw/jenkins.py
--rwxrwxr-x   0 quan      (1001) quan      (1001)    33930 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/elk.py
-drwxrwxr-x   0 quan      (1001) quan      (1001)        0 2022-01-13 12:48:01.000000 grimoire-elk-0.98.0/grimoire_elk/identities/
--rw-rw-r--   0 quan      (1001) quan      (1001)     1835 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/identities/meetup.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1237 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/identities/identities.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1722 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/identities/gitlab.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     2712 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/identities/github.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1732 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/identities/git.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1916 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/identities/stackexchange.py
--rw-rw-r--   0 quan      (1001) quan      (1001)        0 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/identities/__init__.py
--rw-rw-r--   0 quan      (1001) quan      (1001)      894 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/__init__.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1637 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/elastic_analyzer.py
--rw-rw-r--   0 quan      (1001) quan      (1001)     1653 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/elastic_mapping.py
--rwxrwxr-x   0 quan      (1001) quan      (1001)    19994 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/utils.py
--rw-rw-r--   0 quan      (1001) quan      (1001)    22450 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/grimoire_elk/elastic.py
--rwxrwxr-x   0 quan      (1001) quan      (1001)     3397 2022-01-13 12:48:00.000000 grimoire-elk-0.98.0/setup.py
+drwxrwxr-x   0 quan      (1001) quan      (1001)        0 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/
+-rw-rw-r--   0 quan      (1001) quan      (1001)      204 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/setup.cfg
+-rw-rw-r--   0 quan      (1001) quan      (1001)     2421 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/pyproject.toml
+drwxrwxr-x   0 quan      (1001) quan      (1001)        0 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/grimoire_elk.egg-info/
+-rw-rw-r--   0 quan      (1001) quan      (1001)        1 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/grimoire_elk.egg-info/dependency_links.txt
+-rw-rw-r--   0 quan      (1001) quan      (1001)     4275 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/grimoire_elk.egg-info/SOURCES.txt
+-rw-rw-r--   0 quan      (1001) quan      (1001)        1 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/grimoire_elk.egg-info/not-zip-safe
+-rw-rw-r--   0 quan      (1001) quan      (1001)      411 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/grimoire_elk.egg-info/requires.txt
+-rw-rw-r--   0 quan      (1001) quan      (1001)    13847 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/grimoire_elk.egg-info/PKG-INFO
+-rw-rw-r--   0 quan      (1001) quan      (1001)       13 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/grimoire_elk.egg-info/top_level.txt
+-rw-rw-r--   0 quan      (1001) quan      (1001)    13847 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/PKG-INFO
+drwxrwxr-x   0 quan      (1001) quan      (1001)        0 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/utils/
+-rwxrwxr-x   0 quan      (1001) quan      (1001)     5183 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/utils/gelk_mapping.py
+-rwxrwxr-x   0 quan      (1001) quan      (1001)     3963 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/utils/p2o.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)    35147 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/LICENSE
+-rw-rw-r--   0 quan      (1001) quan      (1001)    13009 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/README.md
+-rw-rw-r--   0 quan      (1001) quan      (1001)       18 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/MANIFEST.in
+drwxrwxr-x   0 quan      (1001) quan      (1001)        0 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/grimoire_elk/
+-rw-rw-r--   0 quan      (1001) quan      (1001)       23 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/_version.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     1309 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/errors.py
+drwxrwxr-x   0 quan      (1001) quan      (1001)        0 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/
+-rw-rw-r--   0 quan      (1001) quan      (1001)     5209 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/sortinghat_gelk.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)    13610 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/meetup.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     6687 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/puppetforge.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)    16209 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/gitlab.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)    36434 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/github.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)    12332 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/discourse.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     6172 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/mozillaclub.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     6144 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/dockerhub.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     8696 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/study_ceres_aoc.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)    45718 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/git.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     8036 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/remo.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     6787 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/rocketchat.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     9130 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/mediawiki.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)      897 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/groupsio.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     8747 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/kitsune.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)    12673 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/ceres_base.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)    16606 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/mbox_study_kip.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     5566 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/redmine.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     3481 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/rss.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     5408 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/gitter.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)    10011 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/stackexchange.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)    18578 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/jira.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)    32205 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/gerrit.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)      907 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/pipermail.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)    12855 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/pagure.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)        0 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/__init__.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)    33027 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/githubql.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     1670 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/google_hits.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     5431 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/twitter.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     4691 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/dockerdeps.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)    14023 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/askbot.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     7284 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/bugzilla.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)    15829 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/study_ceres_onion.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     1052 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/nntp.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)    23552 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/slack.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)    92030 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/enrich.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     6067 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/bugzillarest.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     5408 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/github_study_evolution.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)      908 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/hyperkitty.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     5141 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/confluence.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     8339 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/mattermost.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     5328 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/telegram.py
+-rwxrwxr-x   0 quan      (1001) quan      (1001)     7997 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/utils.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     3747 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/finosmeetings.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     3362 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/supybot.py
+drwxrwxr-x   0 quan      (1001) quan      (1001)        0 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/mappings/
+-rw-rw-r--   0 quan      (1001) quan      (1001)      981 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/mappings/onion.json
+-rw-rw-r--   0 quan      (1001) quan      (1001)      961 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/mappings/onion_es7.json
+-rw-rw-r--   0 quan      (1001) quan      (1001)     2552 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/mappings/git_aoc.json
+-rw-rw-r--   0 quan      (1001) quan      (1001)     2295 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/mappings/git_aoc_es7.json
+-rw-rw-r--   0 quan      (1001) quan      (1001)     8144 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/mbox.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)    27867 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/github2.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)    15340 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/cocom.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     5296 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/crates.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     6286 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/weblate.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     5648 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/graal_study_evolution.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     6242 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/functest.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)    16216 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/colic.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     4922 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/dockersmells.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     7797 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/launchpad.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     2233 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/database.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)    15732 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/phabricator.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     8332 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/enriched/jenkins.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)    14188 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/elastic_items.py
+drwxrwxr-x   0 quan      (1001) quan      (1001)        0 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/grimoire_elk/raw/
+-rw-rw-r--   0 quan      (1001) quan      (1001)     2666 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/meetup.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)      874 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/puppetforge.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     2074 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/graal.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     3448 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/gitlab.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     4828 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/github.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     3488 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/discourse.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     1882 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/mozillaclub.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     2036 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/dockerhub.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     2178 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/git.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     1788 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/remo.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     1863 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/rocketchat.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     2128 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/mediawiki.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)      882 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/groupsio.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)      875 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/kitsune.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     2088 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/redmine.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     2023 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/rss.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     1831 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/gitter.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     2613 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/stackexchange.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     3442 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/jira.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     3017 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/gerrit.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)      892 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/pipermail.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     1921 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/pagure.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)        0 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/__init__.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     1853 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/githubql.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)      903 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/google_hits.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     3815 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/twitter.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     2181 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/askbot.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     2450 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/bugzilla.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     2113 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/nntp.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     2900 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/slack.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     4458 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/bugzillarest.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     1831 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/hyperkitty.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     2288 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/confluence.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     5204 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/mattermost.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)      877 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/telegram.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     1594 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/finosmeetings.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     1044 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/supybot.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)    11043 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/elastic.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     2249 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/mbox.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     1836 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/crates.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     1899 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/weblate.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     2341 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/functest.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     1870 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/launchpad.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     3052 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/phabricator.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     5603 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/raw/jenkins.py
+-rwxrwxr-x   0 quan      (1001) quan      (1001)    33930 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/elk.py
+drwxrwxr-x   0 quan      (1001) quan      (1001)        0 2022-01-27 11:03:58.000000 grimoire-elk-0.99.0/grimoire_elk/identities/
+-rw-rw-r--   0 quan      (1001) quan      (1001)     1835 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/identities/meetup.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     1237 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/identities/identities.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     1722 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/identities/gitlab.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     2712 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/identities/github.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     1732 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/identities/git.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     1916 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/identities/stackexchange.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)        0 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/identities/__init__.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)      894 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/__init__.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     1637 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/elastic_analyzer.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)     1653 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/elastic_mapping.py
+-rwxrwxr-x   0 quan      (1001) quan      (1001)    19994 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/utils.py
+-rw-rw-r--   0 quan      (1001) quan      (1001)    22450 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/grimoire_elk/elastic.py
+-rwxrwxr-x   0 quan      (1001) quan      (1001)     3397 2022-01-27 11:03:57.000000 grimoire-elk-0.99.0/setup.py
```

### Comparing `grimoire-elk-0.98.0/pyproject.toml` & `grimoire-elk-0.99.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk.egg-info/SOURCES.txt` & `grimoire-elk-0.99.0/grimoire_elk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk.egg-info/PKG-INFO` & `grimoire-elk-0.99.0/grimoire_elk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grimoire-elk
-Version: 0.98.0
+Version: 0.99.0
 Summary: GrimoireLab library to produce indexes for ElasticSearch
 Home-page: https://github.com/grimoirelab/GrimoireELK
 Author: Bitergia
 Author-email: metrics-grimoire@lists.libresoft.info
 License: GPLv3
 Keywords: development repositories analytics
 Platform: UNKNOWN
```

### Comparing `grimoire-elk-0.98.0/PKG-INFO` & `grimoire-elk-0.99.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grimoire-elk
-Version: 0.98.0
+Version: 0.99.0
 Summary: GrimoireLab library to produce indexes for ElasticSearch
 Home-page: https://github.com/grimoirelab/GrimoireELK
 Author: Bitergia
 Author-email: metrics-grimoire@lists.libresoft.info
 License: GPLv3
 Keywords: development repositories analytics
 Platform: UNKNOWN
```

### Comparing `grimoire-elk-0.98.0/utils/gelk_mapping.py` & `grimoire-elk-0.99.0/utils/gelk_mapping.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/utils/p2o.py` & `grimoire-elk-0.99.0/utils/p2o.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/LICENSE` & `grimoire-elk-0.99.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/README.md` & `grimoire-elk-0.99.0/README.md`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/errors.py` & `grimoire-elk-0.99.0/grimoire_elk/errors.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/sortinghat_gelk.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/sortinghat_gelk.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/meetup.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/meetup.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/puppetforge.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/puppetforge.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/gitlab.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/gitlab.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/github.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/github.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/discourse.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/discourse.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/mozillaclub.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/mozillaclub.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/dockerhub.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/dockerhub.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/study_ceres_aoc.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/study_ceres_aoc.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/git.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/git.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/remo.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/remo.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/rocketchat.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/rocketchat.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/mediawiki.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/mediawiki.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/groupsio.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/groupsio.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/kitsune.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/kitsune.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/ceres_base.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/ceres_base.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/mbox_study_kip.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/mbox_study_kip.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/redmine.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/redmine.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/rss.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/rss.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/gitter.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/gitter.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/stackexchange.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/stackexchange.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/jira.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/jira.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/gerrit.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/gerrit.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/pipermail.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/pipermail.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/pagure.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/pagure.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/githubql.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/githubql.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/google_hits.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/google_hits.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/twitter.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/twitter.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/dockerdeps.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/dockerdeps.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/askbot.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/askbot.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/bugzilla.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/bugzilla.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/study_ceres_onion.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/study_ceres_onion.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/nntp.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/nntp.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/slack.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/slack.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/enrich.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/enrich.py`

 * *Files 1% similar despite different names*

```diff
@@ -443,15 +443,15 @@
 
         return True
 
     def get_email_domain(self, email):
         domain = None
         try:
             domain = email.split("@")[1]
-        except IndexError:
+        except (IndexError, AttributeError):
             # logger.warning("Bad email format: %s" % (identity['email']))
             pass
         return domain
 
     def get_identity_domain(self, identity):
         domain = None
         if identity['email']:
@@ -797,16 +797,15 @@
         profile = self.get_profile_sh(eitem_sh[rol + "_uuid"])
 
         if profile:
             # If name not in profile, keep its old value (should be empty or identity's name field value)
             eitem_sh[rol + "_name"] = profile.get('name', eitem_sh[rol + "_name"])
 
             email = profile.get('email', None)
-            if email:
-                eitem_sh[rol + "_domain"] = self.get_email_domain(email)
+            eitem_sh[rol + "_domain"] = self.get_email_domain(email)
 
             eitem_sh[rol + "_gender"] = profile.get('gender', self.unknown_gender)
             eitem_sh[rol + "_gender_acc"] = profile.get('gender_acc', 0)
 
         elif not profile and sh_id:
             logger.warning("Can't find SH identity profile: {}".format(sh_id))
 
@@ -2092,15 +2091,16 @@
                   ]
             }
             """ % date_field
 
         logger.info("[enrich-feelings] Start study on {} with data from {}".format(
             anonymize_url(self.elastic.index_url), nlp_rest_url))
 
-        es = ES([self.elastic_url], timeout=3600, max_retries=50, retry_on_timeout=True, verify_certs=False)
+        es = ES([self.elastic_url], timeout=3600, max_retries=50, retry_on_timeout=True,
+                verify_certs=self.elastic.requests.verify, connection_class=RequestsHttpConnection)
         search_fields = [attr for attr in attributes]
         search_fields.extend([uuid_field])
         page = es.search(index=enrich_backend.elastic.index,
                          scroll="1m",
                          _source=search_fields,
                          size=100,
                          body=json.loads(es_query))
```

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/bugzillarest.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/bugzillarest.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/github_study_evolution.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/github_study_evolution.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/hyperkitty.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/hyperkitty.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/confluence.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/confluence.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/mattermost.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/mattermost.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/telegram.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/telegram.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/utils.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/utils.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/finosmeetings.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/finosmeetings.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/supybot.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/supybot.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/mappings/onion.json` & `grimoire-elk-0.99.0/grimoire_elk/enriched/mappings/onion.json`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/mappings/onion_es7.json` & `grimoire-elk-0.99.0/grimoire_elk/enriched/mappings/onion_es7.json`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/mappings/git_aoc.json` & `grimoire-elk-0.99.0/grimoire_elk/enriched/mappings/git_aoc.json`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/mappings/git_aoc_es7.json` & `grimoire-elk-0.99.0/grimoire_elk/enriched/mappings/git_aoc_es7.json`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/mbox.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/mbox.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/github2.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/github2.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,28 +338,40 @@
 
         return ecomments
 
     def enrich_pulls(self, item, eitem):
         eitems = []
 
         comments = item['data'].get('review_comments_data', [])
+        reviews = item['data'].get('reviews_data', [])
         if comments:
             rich_item_comments = self.get_rich_pull_reviews(comments, eitem)
             eitems.extend(rich_item_comments)
+        if reviews:
+            rich_item_reviews = self.get_rich_pull_reviews(reviews, eitem)
+            eitems.extend(rich_item_reviews)
 
         return eitems
 
     def get_rich_pull_reviews(self, comments, eitem):
         ecomments = []
 
         for comment in comments:
+            # If the comment comes from a review is "Approve" or "Change requests"
+            # there is a "submitted_at" instead of "updated_at"
+            if 'updated_at' not in comment:
+                comment['updated_at'] = comment['submitted_at']
+
             ecomment = {}
 
             self.copy_raw_fields(self.RAW_FIELDS_COPY, eitem, ecomment)
 
+            # Review state
+            ecomment['review_state'] = comment.get('state', '')
+
             # Copy data from the enriched pull
             ecomment['pull_labels'] = eitem['pull_labels']
             ecomment['pull_id'] = eitem['pull_id']
             ecomment['pull_id_in_repo'] = eitem['pull_id_in_repo']
             ecomment['issue_id_in_repo'] = eitem['issue_id_in_repo']
             ecomment['issue_title'] = eitem['issue_title']
             ecomment['issue_url'] = eitem['issue_url']
@@ -381,14 +393,15 @@
             ecomment['body_analyzed'] = comment['body']
             ecomment['url'] = comment['html_url']
 
             # extract reactions and add it to enriched item
             ecomment.update(self.__get_reactions(comment))
 
             ecomment['comment_updated_at'] = comment['updated_at']
+            ecomment['comment_created_at'] = comment.get('created_at', comment['updated_at'])
 
             # Add id info to allow to coexistence of items of different types in the same index
             ecomment['id'] = '{}_review_comment_{}'.format(eitem['id'], comment['id'])
             ecomment.update(self.get_grimoire_fields(comment['updated_at'], REVIEW_COMMENT_TYPE))
             # due to backtrack compatibility, `is_github2_*` is replaced with `is_github_*`
             ecomment.pop('is_github2_{}'.format(REVIEW_COMMENT_TYPE))
             ecomment['is_github_{}'.format(REVIEW_COMMENT_TYPE)] = 1
```

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/cocom.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/cocom.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/crates.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/crates.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/weblate.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/weblate.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/graal_study_evolution.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/graal_study_evolution.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/functest.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/functest.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/colic.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/colic.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/dockersmells.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/dockersmells.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/launchpad.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/launchpad.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/database.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/database.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/phabricator.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/phabricator.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/enriched/jenkins.py` & `grimoire-elk-0.99.0/grimoire_elk/enriched/jenkins.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/elastic_items.py` & `grimoire-elk-0.99.0/grimoire_elk/elastic_items.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/meetup.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/meetup.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/puppetforge.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/puppetforge.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/graal.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/graal.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/gitlab.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/gitlab.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/github.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/github.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/discourse.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/discourse.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/mozillaclub.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/mozillaclub.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/dockerhub.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/dockerhub.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/git.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/git.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/remo.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/remo.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/rocketchat.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/rocketchat.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/mediawiki.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/mediawiki.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/groupsio.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/groupsio.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/kitsune.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/kitsune.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/redmine.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/redmine.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/rss.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/rss.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/gitter.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/gitter.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/stackexchange.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/stackexchange.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/jira.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/jira.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/gerrit.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/gerrit.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/pipermail.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/pipermail.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/pagure.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/pagure.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/githubql.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/githubql.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/google_hits.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/google_hits.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/twitter.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/twitter.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/askbot.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/askbot.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/bugzilla.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/bugzilla.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/nntp.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/nntp.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/slack.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/slack.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/bugzillarest.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/bugzillarest.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/hyperkitty.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/hyperkitty.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/confluence.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/confluence.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/mattermost.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/mattermost.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/telegram.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/telegram.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/finosmeetings.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/finosmeetings.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/supybot.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/supybot.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/elastic.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/elastic.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/mbox.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/mbox.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/crates.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/crates.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/weblate.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/weblate.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/functest.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/functest.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/launchpad.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/launchpad.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/phabricator.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/phabricator.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/raw/jenkins.py` & `grimoire-elk-0.99.0/grimoire_elk/raw/jenkins.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/elk.py` & `grimoire-elk-0.99.0/grimoire_elk/elk.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/identities/meetup.py` & `grimoire-elk-0.99.0/grimoire_elk/identities/meetup.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/identities/identities.py` & `grimoire-elk-0.99.0/grimoire_elk/identities/identities.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/identities/gitlab.py` & `grimoire-elk-0.99.0/grimoire_elk/identities/gitlab.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/identities/github.py` & `grimoire-elk-0.99.0/grimoire_elk/identities/github.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/identities/git.py` & `grimoire-elk-0.99.0/grimoire_elk/identities/git.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/identities/stackexchange.py` & `grimoire-elk-0.99.0/grimoire_elk/identities/stackexchange.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/__init__.py` & `grimoire-elk-0.99.0/grimoire_elk/__init__.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/elastic_analyzer.py` & `grimoire-elk-0.99.0/grimoire_elk/elastic_analyzer.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/elastic_mapping.py` & `grimoire-elk-0.99.0/grimoire_elk/elastic_mapping.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/utils.py` & `grimoire-elk-0.99.0/grimoire_elk/utils.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/grimoire_elk/elastic.py` & `grimoire-elk-0.99.0/grimoire_elk/elastic.py`

 * *Files identical despite different names*

### Comparing `grimoire-elk-0.98.0/setup.py` & `grimoire-elk-0.99.0/setup.py`

 * *Files identical despite different names*

