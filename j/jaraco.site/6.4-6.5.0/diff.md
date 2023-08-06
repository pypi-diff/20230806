# Comparing `tmp/jaraco.site-6.4.tar.gz` & `tmp/jaraco.site-6.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmp0w76z5nf/tmpnz5xpk1r/jaraco.site-6.4.tar", last modified: Mon Sep 23 22:36:01 2019, max compression
+gzip compressed data, was "jaraco.site-6.5.0.tar", last modified: Sun Aug  6 17:04:21 2023, max compression
```

## Comparing `jaraco.site-6.4.tar` & `jaraco.site-6.5.0.tar`

### file list

```diff
@@ -1,327 +1,333 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/
--rw-rw-r--   0 travis    (2000) travis    (2000)       50 2019-09-23 22:35:45.000000 jaraco.site-6.4/.coveragerc
--rw-rw-r--   0 travis    (2000) travis    (2000)      246 2019-09-23 22:35:45.000000 jaraco.site-6.4/.flake8
--rw-rw-r--   0 travis    (2000) travis    (2000)       82 2019-09-23 22:35:45.000000 jaraco.site-6.4/.pre-commit-config.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       74 2019-09-23 22:35:45.000000 jaraco.site-6.4/.readthedocs.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      466 2019-09-23 22:35:45.000000 jaraco.site-6.4/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-09-23 22:35:45.000000 jaraco.site-6.4/CHANGES.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      152 2019-09-23 22:35:45.000000 jaraco.site-6.4/Dockerfile
--rw-rw-r--   0 travis    (2000) travis    (2000)     1050 2019-09-23 22:35:45.000000 jaraco.site-6.4/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     1395 2019-09-23 22:36:01.000000 jaraco.site-6.4/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)       32 2019-09-23 22:35:45.000000 jaraco.site-6.4/Procfile
--rw-rw-r--   0 travis    (2000) travis    (2000)      752 2019-09-23 22:35:45.000000 jaraco.site-6.4/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      468 2019-09-23 22:35:45.000000 jaraco.site-6.4/appveyor.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)       32 2019-09-23 22:35:45.000000 jaraco.site-6.4/conftest.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      755 2019-09-23 22:35:45.000000 jaraco.site-6.4/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       81 2019-09-23 22:35:45.000000 jaraco.site-6.4/docs/history.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      299 2019-09-23 22:35:45.000000 jaraco.site-6.4/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2586 2019-09-23 22:35:45.000000 jaraco.site-6.4/fabfile.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/
--rw-rw-r--   0 travis    (2000) travis    (2000)       65 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2433 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1491 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/charts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4203 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/controllers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5560 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/openid.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/projecthoneypot/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1043 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/projecthoneypot/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35505 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/projecthoneypot/croakysteel.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1200 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/resume.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1105 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/run.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/static/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/static/css/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2796 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/css/style.css
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/static/images/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2889 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/images/info.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    25753 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/images/ok.png
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)      429 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/README
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/css/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1231 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/css/NOTICE
--rw-rw-r--   0 travis    (2000) travis    (2000)     1609 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/css/blueorange.css
--rw-rw-r--   0 travis    (2000) travis    (2000)     1792 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/css/compact.css
--rw-rw-r--   0 travis    (2000) travis    (2000)      310 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/css/cssClasses.sh
--rw-rw-r--   0 travis    (2000) travis    (2000)      445 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/css/cssClasses.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1259 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/css/gray.css
--rw-rw-r--   0 travis    (2000) travis    (2000)     1720 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/css/original.css
--rw-rw-r--   0 travis    (2000) travis    (2000)    16321 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/css/professional.css
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/authors/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2645 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/authors/index.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/changelog/
--rw-rw-r--   0 travis    (2000) travis    (2000)   101285 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/changelog/index.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/copying/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1802 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/copying/index.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    11531 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/index.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/install/
--rw-rw-r--   0 travis    (2000) travis    (2000)      801 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/install/index.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3113 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/appendixes.html
--rw-rw-r--   0 travis    (2000) travis    (2000)       54 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/box-0.gif
--rw-rw-r--   0 travis    (2000) travis    (2000)       53 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/box-1.gif
--rw-rw-r--   0 travis    (2000) travis    (2000)       56 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/caret-l.gif
--rw-rw-r--   0 travis    (2000) travis    (2000)       56 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/caret-r.gif
--rw-rw-r--   0 travis    (2000) travis    (2000)       58 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/caret-t.gif
--rw-rw-r--   0 travis    (2000) travis    (2000)       54 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/caret-u.gif
--rw-rw-r--   0 travis    (2000) travis    (2000)     9345 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/cssref.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4702 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.academics.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4839 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.achievement.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3889 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.achievements.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     8616 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.address.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4225 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.annotation.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4346 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.artTitle.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5568 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.author.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4372 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.award.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4335 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.awards.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4489 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.birth.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4671 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.bookTitle.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4071 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.break.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4724 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.citation.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4790 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.city.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4309 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.clearance.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4017 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.clearances.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3825 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.company.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4784 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.contact.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4362 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.copyright.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4551 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.country.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5335 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.county.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5998 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.date.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3605 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.dayOfMonth.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     6169 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.degree.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3966 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.degrees.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4994 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.description.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3876 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.docpath.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4088 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.email.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5486 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.emphasis.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5627 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.employer.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5081 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.fax.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4001 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.firstname.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4426 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.from.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4896 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.gpa.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3773 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.head.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5057 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.header.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5748 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.history.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5283 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.instantMessage.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4771 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.institution.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5206 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.interest.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5260 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.interests.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5834 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.job.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3556 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.jobtitle.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4111 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.keyword.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3745 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.keywords.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3826 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.label.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3842 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.lastModified.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3705 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.legalnotice.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4695 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.level.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     6181 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.link.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4639 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.location.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3869 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.major.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4546 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.membership.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4557 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.memberships.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4184 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.middlenames.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3852 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.minor.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4149 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.misc.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3964 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.month.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5098 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.name.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3767 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.node.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4273 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.note.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4363 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.objective.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4955 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.organization.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4026 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pageNums.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4226 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pager.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5061 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.para.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4985 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.period.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5671 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.phone.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3871 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.possible.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4361 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.postalCode.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4822 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.prefecture.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4316 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.present.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4556 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.project.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4191 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.projects.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4594 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.province.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5817 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pub.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4950 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pubDate.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4785 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.publisher.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3971 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pubs.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5026 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.referee.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4099 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.referees.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4198 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.result.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    12917 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.resume.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5376 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.resumes.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3742 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.score.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5893 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skill.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     6705 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skillarea.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5665 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skillareas.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5333 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skills.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4668 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skillset.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5093 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.state.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4407 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.street.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5236 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.street2.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4398 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.subject.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4115 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.subjects.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4776 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.suburb.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4037 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.suffix.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3526 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.surname.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3699 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.tail.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    10213 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.title.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4139 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.to.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3756 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.uri.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     7088 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.url.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4789 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.ward.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3858 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.year.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4582 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.zip.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    26387 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/elementref.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     2938 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.about.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3291 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.create.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    10886 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.features.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4786 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4109 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.next-steps.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3480 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5414 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.setup.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     7362 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.setup.install.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5308 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.setup.software.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5814 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-1.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3286 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-10.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3367 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-11.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3051 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-2.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4359 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-3.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     7621 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-4.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3590 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-5.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     2990 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-6.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3230 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-7.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     2952 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-8.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     2739 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-9.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4836 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4057 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/gloss.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    15177 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/index.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3659 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/intro.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1724 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/manual.css
--rw-rw-r--   0 travis    (2000) travis    (2000)     5012 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/param.address.format.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     2903 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/param.css.href.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4547 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/param.header.format.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5501 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/param.interest.description.format.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3315 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/param.referees.display.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4167 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/param.skills.format.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3664 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/param.skills.level.display.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4198 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/param.subjects.format.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3833 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/paramref.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    12805 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/ref.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1724 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/manual.css
--rw-rw-r--   0 travis    (2000) travis    (2000)   410745 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/manual.html
--rw-rw-r--   0 travis    (2000) travis    (2000)   172000 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/manual.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/news/
--rw-rw-r--   0 travis    (2000) travis    (2000)    18005 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/news/index.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/todo/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1666 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/todo/index.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/dtd/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1763 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/dtd/catalog
--rw-rw-r--   0 travis    (2000) travis    (2000)     6145 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/dtd/iso-lat1.ent
--rw-rw-r--   0 travis    (2000) travis    (2000)     6801 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/dtd/resume.dcl
--rw-rw-r--   0 travis    (2000) travis    (2000)    15192 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/dtd/resume.dtd
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6024 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/Makefile
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/addressing/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3733 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/addressing/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)      405 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/addressing/README
--rw-rw-r--   0 travis    (2000) travis    (2000)     1100 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/addressing/brazil.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      789 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/addressing/canada.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      704 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/addressing/ireland.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      745 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/addressing/italy.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      697 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/addressing/norway.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      779 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/addressing/nz.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      874 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/addressing/uk.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      616 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/addressing/untagged.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      702 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/addressing/usa.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     6179 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/build.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     3751 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/example1.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)    11538 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/example2.xml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/java/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9913 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/java/xmlresume-filter.jar
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/country/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5612 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/country/br.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     4909 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/country/de.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     4399 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/country/es.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     4647 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/country/fr.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     4258 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/country/it.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     4403 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/country/nl.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     1634 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/country/propogate-params.sh
--rw-rw-r--   0 travis    (2000) travis    (2000)     4343 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/country/uk.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     5086 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/country/us.xsl
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/format/
--rw-rw-r--   0 travis    (2000) travis    (2000)    36336 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/format/fo.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)    31697 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/format/html.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)    37763 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/format/text.xsl
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/lib/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4874 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/lib/address.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)    10757 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/lib/common.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     5441 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/lib/deprecated.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     5159 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/lib/pub.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     5621 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/lib/string.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)    14127 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/lib/textlayout.xsl
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/misc/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2019 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/misc/124-130.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     3230 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/misc/13x-140.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)    11678 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/misc/default.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)    20357 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/misc/html_contemporary.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)    20694 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/misc/html_professional.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     4880 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/misc/normalize-whitespace.xsl
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1695 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/br-a4.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     1646 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/br-html.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     1652 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/br-text.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     1691 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/de-a4.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     1642 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/de-html.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     1648 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/de-text.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     1691 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/fr-a4.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     1642 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/fr-html.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     1648 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/fr-text.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     1692 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/it-a4.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     1643 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/it-html.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     1649 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/it-text.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     1743 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/nl-a4.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     1694 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/nl-html.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     1700 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/nl-text.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     1687 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/uk-a4.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     1638 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/uk-html.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     1644 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/uk-text.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     1762 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/us-html.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     1828 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/us-letter.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     1768 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/us-text.xsl
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/paper/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2903 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/paper/a4.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)     3011 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/paper/letter.xsl
--rw-rw-r--   0 travis    (2000) travis    (2000)    10166 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/params.xsl
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1432 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/templates/Account Management.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      502 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/templates/Change Password.html
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/templates/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      565 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/templates/chart example.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      564 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/templates/downloader.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3084 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/templates/login.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      955 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/templates/master.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco/site/templates/openid/
--rw-rw-r--   0 travis    (2000) travis    (2000)      883 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/templates/openid/about.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      674 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/templates/openid/id.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      526 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/templates/openid/yadis.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      643 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/templates/password gen.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1115 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/templates/project list.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     6441 2019-09-23 22:35:45.000000 jaraco.site-6.4/jaraco/site/templates/welcome.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco.site.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1395 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco.site.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    16278 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco.site.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco.site.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      228 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco.site.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2019-09-23 22:36:01.000000 jaraco.site-6.4/jaraco.site.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      167 2019-09-23 22:35:45.000000 jaraco.site-6.4/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)      719 2019-09-23 22:35:45.000000 jaraco.site-6.4/pytest.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2019-09-23 22:35:45.000000 jaraco.site-6.4/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      909 2019-09-23 22:36:01.000000 jaraco.site-6.4/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      112 2019-09-23 22:35:45.000000 jaraco.site-6.4/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8150 2019-09-23 22:35:45.000000 jaraco.site-6.4/skeleton.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      644 2019-09-23 22:35:45.000000 jaraco.site-6.4/tox.ini
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-23 22:36:01.000000 jaraco.site-6.4/ubuntu/
--rw-rw-r--   0 travis    (2000) travis    (2000)      333 2019-09-23 22:35:45.000000 jaraco.site-6.4/ubuntu/jaraco.site.service
--rw-rw-r--   0 travis    (2000) travis    (2000)     1477 2019-09-23 22:35:45.000000 jaraco.site-6.4/ubuntu/nginx config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.549375 jaraco.site-6.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.485374 jaraco.site-6.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.485374 jaraco.site-6.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-08-06 17:04:21.549375 jaraco.site-6.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/Procfile
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.485374 jaraco.site-6.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/fabfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.477374 jaraco.site-6.5.0/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.485374 jaraco.site-6.5.0/jaraco/site/
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/landing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/openid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.489374 jaraco.site-6.5.0/jaraco/site/projecthoneypot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/projecthoneypot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29425 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/projecthoneypot/croakysteel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/resume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.481374 jaraco.site-6.5.0/jaraco/site/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.489374 jaraco.site-6.5.0/jaraco/site/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.489374 jaraco.site-6.5.0/jaraco/site/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/images/blog.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/images/fosstodon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/images/github.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/images/info.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/images/keybase.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/images/linkedin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25753 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/images/ok.png
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/images/stackoverflow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/images/twitter.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.489374 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.489374 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/css/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/css/blueorange.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/css/compact.css
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/css/cssClasses.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/css/cssClasses.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/css/gray.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/css/original.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16321 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/css/professional.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.489374 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.489374 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/authors/
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/authors/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.489374 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/changelog/
+-rw-r--r--   0 runner    (1001) docker     (123)   101285 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/changelog/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.489374 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/copying/
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/copying/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.489374 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/install/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/install/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.493374 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.529374 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/appendixes.html
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/box-0.gif
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/box-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/caret-l.gif
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/caret-r.gif
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/caret-t.gif
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/caret-u.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/cssref.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.academics.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.achievement.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.achievements.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.address.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.annotation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.artTitle.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.author.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.award.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.awards.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.birth.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.bookTitle.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.break.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.citation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.city.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.clearance.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.clearances.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.company.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.contact.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.copyright.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.country.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.county.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.date.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.dayOfMonth.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.degree.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.degrees.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.description.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.docpath.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.email.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.emphasis.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.employer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.fax.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.firstname.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.from.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.gpa.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.head.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.header.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.history.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.instantMessage.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.institution.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.interest.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.interests.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.job.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.jobtitle.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.keyword.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.keywords.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.label.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.lastModified.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.legalnotice.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.level.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.link.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.location.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.major.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.membership.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.memberships.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.middlenames.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.minor.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.misc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.month.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.name.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.node.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.note.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.objective.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.organization.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pageNums.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pager.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.para.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.period.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.phone.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.possible.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.postalCode.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.prefecture.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.present.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.project.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.projects.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.province.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pub.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pubDate.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.publisher.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pubs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.referee.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.referees.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.result.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.resume.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.resumes.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.score.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skill.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skillarea.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skillareas.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skills.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skillset.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.state.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.street.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.street2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.subject.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.subjects.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.suburb.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.suffix.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.surname.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.tail.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10213 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.title.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.to.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.uri.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.url.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.ward.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.year.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.zip.html
+-rw-r--r--   0 runner    (1001) docker     (123)    26387 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/elementref.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.about.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.create.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10886 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.features.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.next-steps.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.setup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.setup.install.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.setup.software.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-1.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-10.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-11.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-3.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-4.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-5.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-6.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-7.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-8.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-9.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gloss.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/intro.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/manual.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.address.format.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.css.href.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.header.format.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.interest.description.format.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.referees.display.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.skills.format.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.skills.level.display.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.subjects.format.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/paramref.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12805 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/ref.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/manual.css
+-rw-r--r--   0 runner    (1001) docker     (123)   410745 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/manual.html
+-rw-r--r--   0 runner    (1001) docker     (123)   172000 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/manual.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.529374 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/news/
+-rw-r--r--   0 runner    (1001) docker     (123)    18005 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/news/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.529374 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/todo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/todo/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.529374 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/dtd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/dtd/catalog
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/dtd/iso-lat1.ent
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/dtd/resume.dcl
+-rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/dtd/resume.dtd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.529374 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.533375 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/addressing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/addressing/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/addressing/README
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/addressing/brazil.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/addressing/canada.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/addressing/ireland.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/addressing/italy.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/addressing/norway.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/addressing/nz.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/addressing/uk.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/addressing/untagged.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/addressing/usa.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/build.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/example1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    11538 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/example2.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.533375 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/java/
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/java/xmlresume-filter.jar
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.533375 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.537375 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/country/
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/country/br.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/country/de.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/country/es.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/country/fr.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/country/it.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/country/nl.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/country/propogate-params.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/country/uk.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/country/us.xsl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.537375 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/format/
+-rw-r--r--   0 runner    (1001) docker     (123)    36336 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/format/fo.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)    31697 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/format/html.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)    37763 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/format/text.xsl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.537375 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/lib/address.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/lib/common.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/lib/deprecated.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/lib/pub.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/lib/string.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/lib/textlayout.xsl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.537375 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/misc/124-130.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/misc/13x-140.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/misc/default.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)    20357 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/misc/html_contemporary.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)    20694 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/misc/html_professional.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/misc/normalize-whitespace.xsl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.549375 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/br-a4.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/br-html.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/br-text.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/de-a4.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/de-html.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/de-text.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/fr-a4.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/fr-html.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/fr-text.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/it-a4.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/it-html.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/it-text.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/nl-a4.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/nl-html.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/nl-text.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/uk-a4.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/uk-html.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/uk-text.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/us-html.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/us-letter.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/us-text.xsl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.549375 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/paper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/paper/a4.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/paper/letter.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/params.xsl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.549375 jaraco.site-6.5.0/jaraco/site/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/templates/chart example.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/templates/master.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.549375 jaraco.site-6.5.0/jaraco/site/templates/openid/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/templates/openid/about.html
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/templates/openid/id.html
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/templates/openid/yadis.html
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/jaraco/site/templates/welcome.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.485374 jaraco.site-6.5.0/jaraco.site.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-08-06 17:04:21.000000 jaraco.site-6.5.0/jaraco.site.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16392 2023-08-06 17:04:21.000000 jaraco.site-6.5.0/jaraco.site.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 17:04:21.000000 jaraco.site-6.5.0/jaraco.site.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-06 17:04:21.000000 jaraco.site-6.5.0/jaraco.site.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-06 17:04:21.000000 jaraco.site-6.5.0/jaraco.site.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.549375 jaraco.site-6.5.0/newsfragments/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/newsfragments/+drop-py37.feature.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-06 17:04:21.549375 jaraco.site-6.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:21.549375 jaraco.site-6.5.0/ubuntu/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/ubuntu/jaraco.site.service
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-08-06 17:03:55.000000 jaraco.site-6.5.0/ubuntu/nginx config
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jaraco.site-6.4/jaraco/site/__init__.py` & `jaraco.site-6.5.0/jaraco/site/__init__.py`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/charts.py` & `jaraco.site-6.5.0/jaraco/site/charts.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 def get_data_set():
     "get 10-15 datapoints"
     return itertools.islice(get_random_data_pairs(), random.randint(1, 10) + 5)
 
 
-class Charts(object):
+class Charts:
     @cherrypy.expose
     @output('chart example', method='xhtml', content_type='text/xml')
     def plot(self):
         g = Plot(
             dict(
                 width=640,
                 height=480,
```

### Comparing `jaraco.site-6.4/jaraco/site/controllers.py` & `jaraco.site-6.5.0/jaraco/site/controllers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,79 @@
-import grampg
+import itertools
+import logging
+
 import cherrypy
-import requests
 
 from jaraco.site.charts import Charts
 from jaraco.site.openid import OpenID
 from jaraco.site import render, output
 from jaraco.site.projecthoneypot import from_cherrypy
 from . import resume
+from . import landing
 
-import logging
 
 log = logging.getLogger(__name__)
 
 
-class Downloader:
-    @cherrypy.expose
-    @output('downloader')
-    def index(self):
-        return render()
-
+class Locator:
     @cherrypy.expose
-    def download(self, name, url, submit):
-        filename = name + '.mp4'
-        referer = 'http://permaculture.kajabi.com/posts/earthworks-introduction'
-        headers = dict(Referer=referer)
-        resp = requests.get(url, stream=True, headers=headers)
-        resp.raise_for_status()
-        cd = 'attachment; filename="{filename}"'.format_map(locals())
-        cherrypy.response.headers['Content-Disposition'] = cd
-        return resp.iter_content()
+    def default(self, key):
+        if key == 'cu':
+            cherrypy.log(f"CU request for {cherrypy.request.remote.ip}")
+            raise cherrypy.HTTPRedirect('https://co-opcreditunions.org/locator/')
+        raise cherrypy.NotFound()
 
 
-class Root(object):
+class Root:
     """
     Create a server:
 
     >>> root = Root()
     """
 
     charts = Charts()
     openid = OpenID()
-    downloader = Downloader()
+    locate = Locator()
 
     @cherrypy.expose
     @output('welcome')
     def index(self):
-        return render()
+        return render(
+            icons=self.icons(),
+            meta=dict(
+                description="Personal website of Jason R. Coombs",
+            ),
+            title="jaraco.com",
+            name="Jason R. Coombs",
+        )
+
+    def icons(self):
+        urls = """
+            https://github.com/jaraco
+            http://stackoverflow.com/users/70170/jason-r-coombs
+            https://twitter.com/jaraco
+            https://keybase.io/jaraco
+            https://linkedin.com/in/jaraco
+            https://blog.jaraco.com/
+            https://fosstodon.org/@jaraco
+            """.split()
+        addl = [
+            landing.RefIcon(
+                'https://pypi.org/user/jaraco',
+                """
+                <img style="width: 38px; height: 38px; position: relative; top: 15px;"
+                src="https://upload.wikimedia.org/wikipedia/commons/0/0a/Python.svg" />
+                """,
+            )
+        ]
+        return itertools.chain(map(landing.Icon, urls), addl)
 
     @cherrypy.expose
-    @output('project list')
-    def projects(self, name=None):
-        return render()
+    def e5a6ifyiqj_txt(self):
+        return "IPv6 confirmed"
 
     @cherrypy.expose
     def allurbase(self):
         return str(cherrypy.request.base)
 
     @cherrypy.expose
     def resume(self, url=None):
@@ -72,71 +91,15 @@
         return "You authenticated as %s" % cherrypy.request.login
 
     @cherrypy.expose
     def croakysteel_py(self):
         return from_cherrypy()
 
 
-class AcctMgmt(object):
-    @cherrypy.expose
-    @output('Account Management')
-    def index(self):
-        return render()
-
-    @cherrypy.expose
-    @output('Change Password')
-    def change_password(
-        self,
-        submit,
-        username,
-        old_password,
-        new_password,
-        new_password_confirm,
-        system=None,
-    ):
-        from jaraco.site.sysadmin import NTUser
-
-        try:
-            if not new_password:
-                raise ValueError("Blank passwords not allowed")
-            if not new_password == new_password_confirm:
-                raise ValueError("Passwords don't match")
-            nt = NTUser(username, system or '.')
-            nt.reset(old_password, new_password)
-        except ValueError as e:
-            response_messages = ['Password change has failed.', str(e)]
-        else:
-            response_messages = [
-                'Password change for {nt.user.FullName} was successful!'.format(
-                    **vars()
-                )
-            ]
-        return render(response_messages=response_messages)
-
-    @cherrypy.expose
-    @output('password gen')
-    def password_gen(self, length=None):
-        if length is None:
-            return render(password=None, length=8)
-        length = int(length)
-        return render(password=self._gen_password(length), length=length)
-
-    @staticmethod
-    def _gen_password(length):
-        """
-        >>> pw = AcctMgmt._gen_password(10)
-        >>> len(pw)
-        10
-        """
-        gengen = grampg.PasswordGenerator()
-        gen = gengen.of().some('alphanumeric').length(length).done()
-        return gen.generate()
-
-
-class IPTool(object):
+class IPTool:
     def __init__(self):
         self.registry = dict()
 
     @cherrypy.expose
     def register(self, hostname, ip):
         self.registry[hostname] = ip
 
@@ -157,10 +120,9 @@
         raise cherrypy.HTTPRedirect('there/')
 
     @cherrypy.expose
     def there(self):
         return "You got there!"
 
 
-Root.acctmgmt = AcctMgmt()
-Root.ip = IPTool()
-Root.auth_demo = AuthRedirectDemo()
+Root.ip = IPTool()  # type: ignore
+Root.auth_demo = AuthRedirectDemo()  # type: ignore
```

### Comparing `jaraco.site-6.4/jaraco/site/openid.py` & `jaraco.site-6.5.0/jaraco/site/openid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import absolute_import
-
 import cherrypy
 import os
 import logging
 from jaraco.site import output as default_output, render
 
 
 try:
@@ -19,15 +17,15 @@
 log = logging.getLogger(__name__)
 
 
 def output(path, *args, **kwargs):
     return default_output('openid/{0}'.format(path), *args, **kwargs)
 
 
-class OpenID(object):
+class OpenID:
     # todo: get this from cherrypy
     _base_url = 'http://drake.jaraco.com:8080/openid/'
 
     def __init__(self):
         store_loc = os.path.join(os.path.dirname(__file__), 'openid store')
         self.store = FileOpenIDStore(store_loc)
         self.openid = server.Server(self.store, self.endpoint_url)
@@ -152,9 +150,9 @@
     def request_from_session(self, trust_root):
         last_request = cherrypy.session.get('last_request', {})
         return last_request.get(trust_root, None)
 
 
 # disable the OpenID class if openid modules aren't available
 if 'FileOpenIDStore' not in globals():
-    OpenID = lambda: None  # noqa
+    OpenID = lambda: None  # type: ignore  # noqa
     log.error("Unable to import openid modules - OpenID support disabled")
```

### Comparing `jaraco.site-6.4/jaraco/site/projecthoneypot/__init__.py` & `jaraco.site-6.5.0/jaraco/site/projecthoneypot/__init__.py`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/resume.py` & `jaraco.site-6.5.0/jaraco/site/resume.py`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/css/style.css` & `jaraco.site-6.5.0/jaraco/site/static/css/style.css`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/images/info.png` & `jaraco.site-6.5.0/jaraco/site/static/images/info.png`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/images/ok.png` & `jaraco.site-6.5.0/jaraco/site/static/images/ok.png`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/css/NOTICE` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/css/NOTICE`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/css/blueorange.css` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/css/blueorange.css`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/css/compact.css` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/css/compact.css`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/css/gray.css` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/css/gray.css`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/css/original.css` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/css/original.css`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/css/professional.css` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/css/professional.css`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/authors/index.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/authors/index.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/changelog/index.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/changelog/index.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/copying/index.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/copying/index.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/index.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/index.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/install/index.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/install/index.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/appendixes.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/appendixes.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/cssref.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/cssref.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.academics.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.academics.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.achievement.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.achievement.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.achievements.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.achievements.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.address.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.address.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.annotation.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.annotation.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.artTitle.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.artTitle.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.author.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.author.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.award.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.award.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.awards.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.awards.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.birth.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.birth.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.bookTitle.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.bookTitle.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.break.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.break.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.citation.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.citation.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.city.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.city.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.clearance.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.clearance.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.clearances.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.clearances.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.company.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.company.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.contact.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.contact.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.copyright.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.copyright.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.country.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.country.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.county.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.county.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.date.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.date.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.dayOfMonth.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.dayOfMonth.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.degree.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.degree.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.degrees.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.degrees.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.description.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.description.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.docpath.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.docpath.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.email.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.email.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.emphasis.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.emphasis.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.employer.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.employer.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.fax.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.fax.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.firstname.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.firstname.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.from.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.from.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.gpa.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.gpa.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.head.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.head.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.header.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.header.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.history.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.history.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.instantMessage.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.instantMessage.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.institution.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.institution.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.interest.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.interest.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.interests.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.interests.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.job.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.job.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.jobtitle.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.jobtitle.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.keyword.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.keyword.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.keywords.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.keywords.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.label.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.label.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.lastModified.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.lastModified.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.legalnotice.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.legalnotice.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.level.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.level.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.link.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.link.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.location.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.location.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.major.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.major.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.membership.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.membership.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.memberships.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.memberships.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.middlenames.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.middlenames.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.minor.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.minor.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.misc.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.misc.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.month.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.month.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.name.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.name.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.node.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.node.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.note.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.note.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.objective.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.objective.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.organization.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.organization.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pageNums.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pageNums.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pager.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pager.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.para.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.para.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.period.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.period.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.phone.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.phone.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.possible.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.possible.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.postalCode.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.postalCode.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.prefecture.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.prefecture.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.present.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.present.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.project.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.project.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.projects.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.projects.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.province.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.province.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pub.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pub.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pubDate.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pubDate.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.publisher.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.publisher.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pubs.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pubs.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.referee.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.referee.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.referees.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.referees.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.result.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.result.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.resume.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.resume.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.resumes.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.resumes.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.score.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.score.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skill.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skill.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skillarea.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skillarea.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skillareas.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skillareas.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skills.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skills.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skillset.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skillset.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.state.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.state.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.street.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.street.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.street2.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.street2.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.subject.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.subject.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.subjects.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.subjects.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.suburb.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.suburb.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.suffix.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.suffix.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.surname.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.surname.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.tail.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.tail.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.title.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.title.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.to.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.to.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.uri.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.uri.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.url.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.url.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.ward.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.ward.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.year.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.year.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/element.zip.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.zip.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/elementref.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/elementref.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.about.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.about.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.create.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.create.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.features.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.features.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.next-steps.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.next-steps.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.setup.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.setup.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.setup.install.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.setup.install.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.setup.software.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.setup.software.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-1.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-1.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-10.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-10.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-11.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-11.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-2.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-2.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-3.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-3.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-4.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-4.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-5.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-5.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-6.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-6.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-7.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-7.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-8.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-8.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-9.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-9.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/gloss.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gloss.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/index.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/index.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/intro.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/intro.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/manual.css` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/manual.css`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/param.address.format.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.address.format.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/param.css.href.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.css.href.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/param.header.format.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.header.format.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/param.interest.description.format.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.interest.description.format.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/param.referees.display.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.referees.display.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/param.skills.format.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.skills.format.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/param.skills.level.display.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.skills.level.display.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/param.subjects.format.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.subjects.format.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/paramref.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/paramref.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/html/ref.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/html/ref.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/manual.css` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/manual.css`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/manual.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/manual.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/manual/manual.txt` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/manual/manual.txt`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/news/index.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/news/index.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/doc/todo/index.html` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/doc/todo/index.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/dtd/catalog` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/dtd/catalog`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/dtd/iso-lat1.ent` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/dtd/iso-lat1.ent`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/dtd/resume.dcl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/dtd/resume.dcl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/dtd/resume.dtd` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/dtd/resume.dtd`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/Makefile` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/Makefile`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/addressing/Makefile` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/addressing/Makefile`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/addressing/brazil.xml` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/addressing/brazil.xml`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/addressing/canada.xml` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/addressing/canada.xml`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/addressing/ireland.xml` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/addressing/ireland.xml`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/addressing/italy.xml` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/addressing/italy.xml`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/addressing/norway.xml` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/addressing/norway.xml`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/addressing/nz.xml` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/addressing/nz.xml`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/addressing/uk.xml` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/addressing/uk.xml`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/addressing/untagged.xml` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/addressing/untagged.xml`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/addressing/usa.xml` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/addressing/usa.xml`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/build.xml` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/build.xml`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/example1.xml` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/example1.xml`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/examples/example2.xml` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/examples/example2.xml`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/java/xmlresume-filter.jar` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/java/xmlresume-filter.jar`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/country/br.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/country/br.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/country/de.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/country/de.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/country/es.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/country/es.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/country/fr.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/country/fr.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/country/it.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/country/it.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/country/nl.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/country/nl.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/country/propogate-params.sh` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/country/propogate-params.sh`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/country/uk.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/country/uk.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/country/us.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/country/us.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/format/fo.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/format/fo.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/format/html.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/format/html.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/format/text.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/format/text.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/lib/address.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/lib/address.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/lib/common.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/lib/common.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/lib/deprecated.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/lib/deprecated.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/lib/pub.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/lib/pub.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/lib/string.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/lib/string.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/lib/textlayout.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/lib/textlayout.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/misc/124-130.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/misc/124-130.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/misc/13x-140.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/misc/13x-140.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/misc/default.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/misc/default.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/misc/html_contemporary.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/misc/html_contemporary.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/misc/html_professional.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/misc/html_professional.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/misc/normalize-whitespace.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/misc/normalize-whitespace.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/br-a4.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/br-a4.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/br-html.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/br-html.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/br-text.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/br-text.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/de-a4.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/de-a4.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/de-html.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/de-html.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/de-text.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/de-text.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/fr-a4.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/fr-a4.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/fr-html.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/fr-html.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/fr-text.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/fr-text.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/it-a4.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/it-a4.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/it-html.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/it-html.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/it-text.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/it-text.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/nl-a4.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/nl-a4.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/nl-html.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/nl-html.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/nl-text.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/nl-text.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/uk-a4.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/uk-a4.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/uk-html.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/uk-html.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/uk-text.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/uk-text.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/us-html.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/us-html.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/us-letter.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/us-letter.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/output/us-text.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/output/us-text.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/paper/a4.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/paper/a4.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/paper/letter.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/paper/letter.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/static/resume-1.5.1/xsl/params.xsl` & `jaraco.site-6.5.0/jaraco/site/static/resume-1.5.1/xsl/params.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/templates/chart example.html` & `jaraco.site-6.5.0/jaraco/site/templates/chart example.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/templates/master.html` & `jaraco.site-6.5.0/jaraco/site/templates/master.html`

 * *Files 14% similar despite different names*

```diff
@@ -17,13 +17,13 @@
 	<div id="header">
 		<p>jaraco.com</p>
 	</div>
 	<div id="main_content">
 		<div py:replace="select('*|text()')" />
 	</div>
 	<div id="footer">
-		<p>Copyright &#169; 2016 Jason R. Coombs</p>
+		<p>Copyright &#169; <span py:replace="__import__('datetime').date.today().year" /> Jason R. Coombs</p>
 	</div>
 
 </body>
 
 </html>
```

#### html2text {}

```diff
@@ -1,4 +1,4 @@
 
 
 jaraco.com
-Copyright © 2016 Jason R. Coombs
+Copyright ©  Jason R. Coombs
```

### Comparing `jaraco.site-6.4/jaraco/site/templates/openid/about.html` & `jaraco.site-6.5.0/jaraco/site/templates/openid/about.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/templates/openid/id.html` & `jaraco.site-6.5.0/jaraco/site/templates/openid/id.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco/site/templates/openid/yadis.html` & `jaraco.site-6.5.0/jaraco/site/templates/openid/yadis.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.4/jaraco.site.egg-info/SOURCES.txt` & `jaraco.site-6.5.0/jaraco.site.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,55 @@
 .coveragerc
-.flake8
+.editorconfig
 .pre-commit-config.yaml
-.readthedocs.yml
-.travis.yml
-CHANGES.rst
+.readthedocs.yaml
 Dockerfile
 LICENSE
+NEWS.rst
 Procfile
 README.rst
-appveyor.yml
 conftest.py
 fabfile.py
+mypy.ini
 pyproject.toml
 pytest.ini
 requirements.txt
+ruff.toml
 setup.cfg
-setup.py
-skeleton.md
+towncrier.toml
 tox.ini
+.github/dependabot.yml
+.github/workflows/main.yml
 docs/conf.py
 docs/history.rst
 docs/index.rst
-jaraco/__init__.py
 jaraco.site.egg-info/PKG-INFO
 jaraco.site.egg-info/SOURCES.txt
 jaraco.site.egg-info/dependency_links.txt
 jaraco.site.egg-info/requires.txt
 jaraco.site.egg-info/top_level.txt
 jaraco/site/__init__.py
 jaraco/site/charts.py
 jaraco/site/controllers.py
+jaraco/site/landing.py
 jaraco/site/openid.py
 jaraco/site/resume.py
 jaraco/site/run.py
 jaraco/site/projecthoneypot/__init__.py
 jaraco/site/projecthoneypot/croakysteel.py
 jaraco/site/static/css/style.css
+jaraco/site/static/images/blog.svg
+jaraco/site/static/images/fosstodon.svg
+jaraco/site/static/images/github.svg
 jaraco/site/static/images/info.png
+jaraco/site/static/images/keybase.svg
+jaraco/site/static/images/linkedin.svg
 jaraco/site/static/images/ok.png
+jaraco/site/static/images/stackoverflow.svg
+jaraco/site/static/images/twitter.svg
 jaraco/site/static/resume-1.5.1/README
 jaraco/site/static/resume-1.5.1/css/NOTICE
 jaraco/site/static/resume-1.5.1/css/blueorange.css
 jaraco/site/static/resume-1.5.1/css/compact.css
 jaraco/site/static/resume-1.5.1/css/cssClasses.sh
 jaraco/site/static/resume-1.5.1/css/cssClasses.txt
 jaraco/site/static/resume-1.5.1/css/gray.css
@@ -271,22 +279,17 @@
 jaraco/site/static/resume-1.5.1/xsl/output/uk-html.xsl
 jaraco/site/static/resume-1.5.1/xsl/output/uk-text.xsl
 jaraco/site/static/resume-1.5.1/xsl/output/us-html.xsl
 jaraco/site/static/resume-1.5.1/xsl/output/us-letter.xsl
 jaraco/site/static/resume-1.5.1/xsl/output/us-text.xsl
 jaraco/site/static/resume-1.5.1/xsl/paper/a4.xsl
 jaraco/site/static/resume-1.5.1/xsl/paper/letter.xsl
-jaraco/site/templates/Account Management.html
-jaraco/site/templates/Change Password.html
 jaraco/site/templates/__init__.py
 jaraco/site/templates/chart example.html
-jaraco/site/templates/downloader.html
-jaraco/site/templates/login.html
 jaraco/site/templates/master.html
-jaraco/site/templates/password gen.html
-jaraco/site/templates/project list.html
 jaraco/site/templates/welcome.html
 jaraco/site/templates/openid/about.html
 jaraco/site/templates/openid/id.html
 jaraco/site/templates/openid/yadis.html
+newsfragments/+drop-py37.feature.rst
 ubuntu/jaraco.site.service
 ubuntu/nginx config
```

### Comparing `jaraco.site-6.4/ubuntu/nginx config` & `jaraco.site-6.5.0/ubuntu/nginx config`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
         server [::1]:5000;
 }
 
 server {
         listen 80;
         listen [::]:80;
 
-        server_name jaraco.com www.jaraco.com blog.jaraco.com;
+        server_name jaraco.com www.jaraco.com blog.jaraco.com scicomm.pro www.scicomm.pro;
 
         return 301 https://$host$request_uri;
 }
 
 server {
         listen 443;
         listen [::]:443;
@@ -46,7 +46,35 @@
                 proxy_redirect off;
                 proxy_set_header Host $host;
                 proxy_set_header X-Real-IP $remote_addr;
                 proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
                 proxy_set_header X-Forwarded-Host $server_name;
         }
 }
+
+server {
+        listen 80;
+        listen [::]:80;
+        listen 443 ssl;
+        listen [::]:443 ssl;
+
+        ssl_certificate /etc/letsencrypt/live/pittsburghfreethoughtcommunity.com/fullchain.pem;
+        ssl_certificate_key /etc/letsencrypt/live/pittsburghfreethoughtcommunity.com/privkey.pem;
+
+        server_name pittsburghfreethoughtcommunity.com www.pittsburghfreethoughtcommunity.com;
+
+        return 301 https://pghfreethought.org$request_uri;
+}
+
+server {
+        listen 443 ssl;
+        listen [::]:443 ssl;
+
+        ssl on;
+        ssl_certificate /etc/letsencrypt/live/scicomm.pro/fullchain.pem;
+        ssl_certificate_key /etc/letsencrypt/live/scicomm.pro/privkey.pem;
+
+        server_name scicomm.pro www.scicomm.pro;
+
+        root /opt/scicomm.pro;
+        index index.html;
+}
```

