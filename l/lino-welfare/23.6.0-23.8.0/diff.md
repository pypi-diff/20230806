# Comparing `tmp/lino-welfare-23.6.0.tar.gz` & `tmp/lino-welfare-23.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lino-welfare-23.6.0.tar", last modified: Tue Jun 20 12:11:07 2023, max compression
+gzip compressed data, was "lino-welfare-23.8.0.tar", last modified: Sun Aug  6 15:48:40 2023, max compression
```

## Comparing `lino-welfare-23.6.0.tar` & `lino-welfare-23.8.0.tar`

### file list

```diff
@@ -1,521 +1,529 @@
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.138802 lino-welfare-23.6.0/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    34523 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/COPYING
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      244 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/MANIFEST.in
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2037 2023-06-20 12:11:07.138802 lino-welfare-23.6.0/PKG-INFO
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1130 2023-03-18 07:37:29.000000 lino-welfare-23.6.0/README.rst
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.054801 lino-welfare-23.6.0/lino_welfare/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      653 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    21221 2023-04-02 10:55:01.000000 lino-welfare-23.6.0/lino_welfare/migrate.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)   193321 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/migrate_old.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.054801 lino-welfare-23.6.0/lino_welfare/modlib/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      659 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.054801 lino-welfare-23.6.0/lino_welfare/modlib/active_job_search/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      562 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/active_job_search/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.054801 lino-welfare-23.6.0/lino_welfare/modlib/active_job_search/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/active_job_search/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      984 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/active_job_search/fixtures/demo.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2329 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/active_job_search/models.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/active_job_search__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.054801 lino-welfare-23.6.0/lino_welfare/modlib/aids/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1538 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2458 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/choicelists.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.058802 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1142 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/certificate.body.html
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      890 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/clothing_bank.body.html
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       65 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/default.body.html
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      713 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/fixed_income.body.html
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      872 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/food_bank.body.html
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      774 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/foreigner_income.body.html
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      575 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/furniture.body.html
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      564 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/heating_refund.body.html
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      763 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/integ_income.body.html
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     4798 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/medical_refund.body.html
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      745 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/urgent_medical_care.body.html
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.058802 lino-welfare-23.6.0/lino_welfare/modlib/aids/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     6723 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/fixtures/demo.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     6340 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/fixtures/std.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    11507 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/mixins.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    27336 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/models.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      366 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/roles.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.058802 lino-welfare-23.6.0/lino_welfare/modlib/art60/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1138 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/art60/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/art60/config/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/art60/config/art60/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.058802 lino-welfare-23.6.0/lino_welfare/modlib/art60/config/art60/Contract/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    46358 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/art60/config/art60/Contract/Default.odt
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.058802 lino-welfare-23.6.0/lino_welfare/modlib/art60/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/art60/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      806 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/art60/fixtures/std.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    10776 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/art60/models.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.058802 lino-welfare-23.6.0/lino_welfare/modlib/art61/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      983 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/art61/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1739 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/art61/choicelists.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/art61/config/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/art61/config/art61/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.058802 lino-welfare-23.6.0/lino_welfare/modlib/art61/config/art61/Contract/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     8721 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/art61/config/art61/Contract/contract.body.html
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.058802 lino-welfare-23.6.0/lino_welfare/modlib/art61/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/art61/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      347 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/art61/fixtures/std.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     7238 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/art61/models.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.058802 lino-welfare-23.6.0/lino_welfare/modlib/badges/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1244 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/badges/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1693 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/badges/models.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.062801 lino-welfare-23.6.0/lino_welfare/modlib/cal/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      472 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cal/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/cal/config/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/cal/config/cal/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.062801 lino-welfare-23.6.0/lino_welfare/modlib/cal/config/cal/Guest/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1249 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cal/config/cal/Guest/Colleague.eml.html
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      248 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cal/config/cal/Guest/Visitor.eml.html
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1700 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cal/config/cal/Guest/presence_certificate.body.html
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.062801 lino-welfare-23.6.0/lino_welfare/modlib/cal/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cal/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       44 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cal/fixtures/demo.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      825 2023-04-27 06:29:51.000000 lino-welfare-23.6.0/lino_welfare/modlib/cal/fixtures/demo2.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       43 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cal/fixtures/std.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    14042 2023-04-27 06:29:51.000000 lino-welfare-23.6.0/lino_welfare/modlib/cal/models.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.062801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.066801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/WSDL/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     4120 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v1.wsdl
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3740 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v2.wsdl
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2846 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/WSDL/TestConnectionService.wsdl
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2075 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/WSDL/WebServiceConnector.wsdl
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.066801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.066801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/20190612/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    11616 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/20190612/RetrieveTIGroupsV5.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)   139908 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/20190612/rn25_Release201411.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      154 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/README.txt
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.066801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     8507 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/CommonDataTypes.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      777 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/ExtensionPlaceHolder.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      933 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/NamespaceRoot.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     4198 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/ResultSummary.xsd
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.066801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     9867 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/IdentifyPersonReply.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     7931 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/IdentifyPersonRequest.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1042 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/NamespaceRoot.xsd
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.070802 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     5622 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_AB_decision_Reply.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    13874 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_AB_decision_Request.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2435 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_C_decision_Reply.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     5569 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_C_decision_Request.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     5699 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_Common.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     9421 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_DF_decision_Reply.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    19800 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_DF_decision_Request.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1361 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/NamespaceRoot.xsd
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.070802 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1600 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/CommonDataTypes.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     4063 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/ManageAccessReply.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     5074 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/ManageAccessRequest.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1146 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/NamespaceRoot.xsd
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.074802 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3334 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/AddressHistory.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2591 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/FamilyComposition.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1460 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/NamespaceRoot.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3450 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/PerformInvestigationRequest.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3938 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/PerformInvetigationReply.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    11981 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/WaitRegister.xsd
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.074802 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     5436 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/AddressInformation.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     6504 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/Citizen.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3332 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/CommonDataTypes.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1119 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/NamespaceRoot.xsd
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.078801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1969 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/CommonDataTypes.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1044 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/NamespaceRoot.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     4562 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/SSDNReply.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3627 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/SSDNRequest.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     6440 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/TestConnectionServiceV1.xsd
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/intf/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.078801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/intf/RetrieveTIGroupsService/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3491 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/intf/RetrieveTIGroupsService/RetrieveTIGroupsV2.wsdl
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.078801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/RetrieveTIGroups/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2902 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/RetrieveTIGroups/RetrieveTIGroupsV2.xsd
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.078801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/common/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    26504 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/common/CommonV3.xsd
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/xsd/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.078801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/xsd/xm25/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)   121083 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/xsd/xm25/xm25.xsd
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2715 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3241 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/choicelists.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/config/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/config/cbss/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.078801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/config/cbss/IdentifyPersonRequest/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    21764 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/config/cbss/IdentifyPersonRequest/Default.odt
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.078801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/config/cbss/RetrieveTIGroupsRequest/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    15865 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/config/cbss/RetrieveTIGroupsRequest/Default.odt
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.082801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      538 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/cbss.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3295 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/cbss_demo.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1961 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_1.xml
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2109 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_2.xml
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2579 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_3.xml
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     4542 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_4.xml
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1826 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_5.xml
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    11618 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_1.xml
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    24155 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_2.xml
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    26292 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_3.xml
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      619 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/democfg.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     6081 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/garble_tx25.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    20869 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/lijst_van_sectoren_liste_des_secteurs.csv
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     9170 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/purposes.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2401 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/sectors.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    16822 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/tx25_1107.xml
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    23231 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/tx25_1358.xml
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    25160 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/tx25_1373.xml
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.082801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/management/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/management/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.082801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/management/commands/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/management/commands/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1895 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/management/commands/cbss_validate_request.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    23598 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/mixins.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    26644 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/models.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      401 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/roles.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    37959 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/tx25.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     9036 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/ui.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2468 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/utils.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.086802 lino-welfare-23.6.0/lino_welfare/modlib/client_vouchers/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      656 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/client_vouchers/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3449 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/client_vouchers/models.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1764 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/client_vouchers/ui.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.086802 lino-welfare-23.6.0/lino_welfare/modlib/contacts/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      872 2023-03-30 05:52:14.000000 lino-welfare-23.6.0/lino_welfare/modlib/contacts/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.086802 lino-welfare-23.6.0/lino_welfare/modlib/contacts/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/contacts/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       49 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/contacts/fixtures/demo.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       48 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/contacts/fixtures/std.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.086802 lino-welfare-23.6.0/lino_welfare/modlib/contacts/management/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/contacts/management/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.086802 lino-welfare-23.6.0/lino_welfare/modlib/contacts/management/commands/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/contacts/management/commands/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       70 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/contacts/management/commands/garble_persons.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     9487 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/contacts/models.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.086802 lino-welfare-23.6.0/lino_welfare/modlib/cv/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      479 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cv/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.086802 lino-welfare-23.6.0/lino_welfare/modlib/cv/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cv/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      945 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cv/fixtures/demo.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     7545 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cv/fixtures/props.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       48 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cv/fixtures/std.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     5673 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cv/models.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.090802 lino-welfare-23.6.0/lino_welfare/modlib/debts/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1551 2023-04-02 08:02:31.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     4424 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/choicelists.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/debts/config/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/debts/config/debts/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.090802 lino-welfare-23.6.0/lino_welfare/modlib/debts/config/debts/Budget/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    17514 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/config/debts/Budget/Default.odt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    24679 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/config/debts/Budget/Default_2.odt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    19964 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/config/debts/Budget/Default_new.odt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      661 2023-04-02 08:02:31.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/fields.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.090802 lino-welfare-23.6.0/lino_welfare/modlib/debts/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     4587 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/fixtures/demo.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    20553 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/fixtures/minimal.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      577 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/fixtures/std.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1866 2023-04-02 08:02:31.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/mixins.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    22106 2023-04-02 08:02:31.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/models.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      352 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/roles.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    21350 2023-04-02 08:02:31.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/ui.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.090802 lino-welfare-23.6.0/lino_welfare/modlib/dupable_clients/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      824 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/dupable_clients/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.090802 lino-welfare-23.6.0/lino_welfare/modlib/dupable_clients/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/dupable_clients/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      420 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/dupable_clients/fixtures/demo2.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1924 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/dupable_clients/mixins.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1679 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/dupable_clients/models.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.094802 lino-welfare-23.6.0/lino_welfare/modlib/esf/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      852 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/esf/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     6282 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/esf/choicelists.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/esf/config/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/esf/config/esf/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.094802 lino-welfare-23.6.0/lino_welfare/modlib/esf/config/esf/Client/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      742 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/esf/config/esf/Client/esf_file.weasy.html
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.094802 lino-welfare-23.6.0/lino_welfare/modlib/esf/config/esf/ClientSummary/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      905 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/esf/config/esf/ClientSummary/base.weasy.html
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      620 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/esf/config/esf/ClientSummary/default.weasy.html
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.094802 lino-welfare-23.6.0/lino_welfare/modlib/esf/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/esf/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      360 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/esf/fixtures/demo.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      482 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/esf/fixtures/std.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     5631 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/esf/models.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.094802 lino-welfare-23.6.0/lino_welfare/modlib/finan/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      381 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/finan/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.094802 lino-welfare-23.6.0/lino_welfare/modlib/finan/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/finan/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      467 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/finan/fixtures/payments.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1969 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/finan/models.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.094802 lino-welfare-23.6.0/lino_welfare/modlib/households/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      306 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/households/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.094802 lino-welfare-23.6.0/lino_welfare/modlib/households/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/households/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       51 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/households/fixtures/demo.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       50 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/households/fixtures/std.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3807 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/households/models.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.094802 lino-welfare-23.6.0/lino_welfare/modlib/immersion/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1107 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/immersion/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/immersion/config/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/immersion/config/immersion/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.098802 lino-welfare-23.6.0/lino_welfare/modlib/immersion/config/immersion/Contract/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)   667935 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/immersion/config/immersion/Contract/StageForem.odt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     5587 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/immersion/config/immersion/Contract/immersion.body.html
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.098802 lino-welfare-23.6.0/lino_welfare/modlib/immersion/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/immersion/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1446 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/immersion/fixtures/std.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3463 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/immersion/models.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3921 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/immersion/ui.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.098802 lino-welfare-23.6.0/lino_welfare/modlib/integ/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2406 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/integ/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.098802 lino-welfare-23.6.0/lino_welfare/modlib/integ/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/integ/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     8565 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/integ/fixtures/demo.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2470 2023-04-02 10:54:19.000000 lino-welfare-23.6.0/lino_welfare/modlib/integ/fixtures/std.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    23997 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/integ/models.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      377 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/integ/roles.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.102802 lino-welfare-23.6.0/lino_welfare/modlib/isip/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      351 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/isip/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      722 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/isip/choicelists.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/isip/config/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/isip/config/isip/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.102802 lino-welfare-23.6.0/lino_welfare/modlib/isip/config/isip/Contract/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    55172 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/isip/config/isip/Contract/Default.odt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    17714 2023-04-02 09:54:45.000000 lino-welfare-23.6.0/lino_welfare/modlib/isip/mixins.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    11361 2023-04-02 09:44:08.000000 lino-welfare-23.6.0/lino_welfare/modlib/isip/models.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.102802 lino-welfare-23.6.0/lino_welfare/modlib/jobs/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      903 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/jobs/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/jobs/config/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/jobs/config/jobs/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.102802 lino-welfare-23.6.0/lino_welfare/modlib/jobs/config/jobs/Contract/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    94813 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/jobs/config/jobs/Contract/Default.odt
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.102802 lino-welfare-23.6.0/lino_welfare/modlib/jobs/config/jobs/ContractsSituation/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     9896 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/jobs/config/jobs/ContractsSituation/Default.odt
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.102802 lino-welfare-23.6.0/lino_welfare/modlib/jobs/config/jobs/OldJobsOverview/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     9876 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/jobs/config/jobs/OldJobsOverview/Default.odt
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.102802 lino-welfare-23.6.0/lino_welfare/modlib/jobs/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/jobs/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      935 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/jobs/fixtures/std.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2930 2023-04-02 09:55:26.000000 lino-welfare-23.6.0/lino_welfare/modlib/jobs/mixins.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    13181 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/jobs/models.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      327 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/jobs/template_messages.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    17073 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/jobs/ui.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.102802 lino-welfare-23.6.0/lino_welfare/modlib/ledger/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      419 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/ledger/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.106802 lino-welfare-23.6.0/lino_welfare/modlib/ledger/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/ledger/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      531 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/ledger/fixtures/demo.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2758 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/ledger/fixtures/std.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3082 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/ledger/fixtures/std_journals.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2438 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/ledger/models.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.106802 lino-welfare-23.6.0/lino_welfare/modlib/newcomers/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      996 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/newcomers/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.106802 lino-welfare-23.6.0/lino_welfare/modlib/newcomers/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/newcomers/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3181 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/newcomers/fixtures/demo.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    16680 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/newcomers/models.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      416 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/newcomers/roles.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.106802 lino-welfare-23.6.0/lino_welfare/modlib/notes/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      282 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/notes/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.106802 lino-welfare-23.6.0/lino_welfare/modlib/notes/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/notes/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      889 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/notes/fixtures/demo.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       45 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/notes/fixtures/std.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2462 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/notes/models.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.110802 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1516 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     4420 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/actions.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2558 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/choicelists.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      366 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/client_address.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.110802 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/config/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/config/pcsw/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.110802 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/config/pcsw/Client/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    32053 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/config/pcsw/Client/cv.odt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)   157223 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/config/pcsw/Client/eid-content.odt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    31905 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/config/pcsw/Client/file_sheet.odt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      373 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/config/pcsw/Client/pac.body.html
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      487 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/config/welcome.html
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.110802 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2287 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/fixtures/demo2.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1595 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/fixtures/std.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    36618 2023-04-02 09:58:50.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/models.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      509 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/roles.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.114802 lino-welfare-23.6.0/lino_welfare/modlib/polls/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      335 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/polls/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.114802 lino-welfare-23.6.0/lino_welfare/modlib/polls/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/polls/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     5736 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/polls/fixtures/demo.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      328 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/polls/fixtures/jobsearch.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       51 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/polls/fixtures/std.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      214 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/polls/models.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.114802 lino-welfare-23.6.0/lino_welfare/modlib/projects/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      619 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/projects/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2069 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/projects/models.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.114802 lino-welfare-23.6.0/lino_welfare/modlib/reception/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      532 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/reception/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    14505 2023-03-22 06:06:32.000000 lino-welfare-23.6.0/lino_welfare/modlib/reception/models.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.114802 lino-welfare-23.6.0/lino_welfare/modlib/sales/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/sales/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      466 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/sales/models.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.114802 lino-welfare-23.6.0/lino_welfare/modlib/sepa/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      308 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/sepa/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.114802 lino-welfare-23.6.0/lino_welfare/modlib/sepa/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/sepa/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     4013 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/sepa/fixtures/demo.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1603 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/sepa/models.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.114802 lino-welfare-23.6.0/lino_welfare/modlib/system/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      216 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/system/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     4076 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/system/models.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.114802 lino-welfare-23.6.0/lino_welfare/modlib/users/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      345 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/users/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.114802 lino-welfare-23.6.0/lino_welfare/modlib/users/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/users/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       46 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/users/fixtures/demo.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       48 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/users/fixtures/demo2.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       52 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/users/fixtures/demo_users.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2777 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/users/models.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1050 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/users/ui.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.118802 lino-welfare-23.6.0/lino_welfare/modlib/welfare/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      407 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.118802 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.118802 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)   672907 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/Default.odt
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.122802 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      511 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/TasksByClient.body.html
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1221 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/anw.body.html
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1146 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/aus.body.html
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      533 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/certificate.body.html
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       40 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/default.body.html
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      624 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/summary.body.html
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      800 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/base.body.html
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/integ/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.122802 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/integ/ActivityReport/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    11787 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/integ/ActivityReport/Default.odt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      585 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/letter_margin_bottom.html
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/notes/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.122802 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/notes/Note/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    50685 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/notes/Note/Letter.odt
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.122802 lino-welfare-23.6.0/lino_welfare/modlib/welfare/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    43393 2023-04-02 10:53:58.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/fixtures/demo.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1040 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/fixtures/demo2.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    29832 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/fixtures/pp2lino.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     4243 2023-03-05 11:09:30.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/fixtures/std.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3232 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/fixtures/std2.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    26073 2023-04-02 08:02:31.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/help_texts.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/de/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.122802 lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    38241 2023-04-02 08:02:31.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 blurry    (1000) blurry    (1000)   131485 2023-04-02 08:02:31.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/django.po
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/fr/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.126802 lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    35602 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 blurry    (1000) blurry    (1000)   130979 2023-04-02 08:02:31.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/django.po
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/nl/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.126802 lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/nl/LC_MESSAGES/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      409 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/nl/LC_MESSAGES/django.mo
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    93297 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/nl/LC_MESSAGES/django.po
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.126802 lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.130802 lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/commands/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/commands/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    18127 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/commands/cpas2lino.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     4743 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/commands/garble.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     4518 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/commands/gd2lino.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    14642 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/commands/initdb_tim.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    35429 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/commands/watch_tim.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     5859 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/models.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     6296 2023-03-31 11:56:45.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/settings.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     7612 2023-04-27 06:29:51.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/user_types.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1635 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/workflows.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.130802 lino-welfare-23.6.0/lino_welfare/modlib/xcourses/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1055 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/xcourses/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.050801 lino-welfare-23.6.0/lino_welfare/modlib/xcourses/config/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.050801 lino-welfare-23.6.0/lino_welfare/modlib/xcourses/config/courses/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.130802 lino-welfare-23.6.0/lino_welfare/modlib/xcourses/config/courses/Course/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    12127 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/xcourses/config/courses/Course/candidates.odt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    12100 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/xcourses/config/courses/Course/participants.odt
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.130802 lino-welfare-23.6.0/lino_welfare/modlib/xcourses/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/xcourses/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3037 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/xcourses/fixtures/demo.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    20702 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/xcourses/models.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      363 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/xcourses/roles.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.130802 lino-welfare-23.6.0/lino_welfare/projects/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      206 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.130802 lino-welfare-23.6.0/lino_welfare/projects/gerd/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      297 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      415 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/django110_isnull.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      278 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/manage.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1388 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/print_tx25.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.130802 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      342 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      763 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/demo.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      388 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/doctests.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.050801 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/media/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.134802 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/media/beid/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3046 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/media/beid/123456789012.jpg
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     7615 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/media/beid/591413288107.jpg
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.050801 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/media/webdav/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.050801 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/media/webdav/userdocs/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.134802 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/media/webdav/userdocs/appyodt/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    13377 2023-04-05 09:05:00.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/media/webdav/userdocs/appyodt/jobs.JobsOverview.odt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       85 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/memory.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1038 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/mysql.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.134802 lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      183 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2459 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/test_aids.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2765 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/test_broken_gfks.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     7909 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/test_cbss.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2948 2023-04-02 10:54:08.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/test_clients.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     4214 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/test_debts.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      253 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/test_restore.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    35630 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/test_watchtim.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.134802 lino-welfare-23.6.0/lino_welfare/projects/mathieu/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      365 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/mathieu/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      280 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/mathieu/manage.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.134802 lino-welfare-23.6.0/lino_welfare/projects/mathieu/settings/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      281 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/mathieu/settings/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      512 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/mathieu/settings/demo.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      347 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/mathieu/settings/doctests.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.050801 lino-welfare-23.6.0/lino_welfare/projects/mathieu/settings/media/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.134802 lino-welfare-23.6.0/lino_welfare/projects/mathieu/settings/media/beid/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3046 2023-02-28 05:23:17.000000 lino-welfare-23.6.0/lino_welfare/projects/mathieu/settings/media/beid/123456789012.jpg
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     7615 2023-02-28 05:23:17.000000 lino-welfare-23.6.0/lino_welfare/projects/mathieu/settings/media/beid/591413288107.jpg
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       85 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/mathieu/settings/memory.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.138802 lino-welfare-23.6.0/lino_welfare/projects/mathieu/tests/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:17.000000 lino-welfare-23.6.0/lino_welfare/projects/mathieu/tests/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     6890 2023-04-29 06:46:42.000000 lino-welfare-23.6.0/lino_welfare/projects/mathieu/tests/test_chatelet.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    18271 2023-02-28 05:23:17.000000 lino-welfare-23.6.0/lino_welfare/projects/mathieu/tests/test_notify.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.138802 lino-welfare-23.6.0/lino_welfare/scripts/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:17.000000 lino-welfare-23.6.0/lino_welfare/scripts/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     7346 2023-02-28 05:23:17.000000 lino-welfare-23.6.0/lino_welfare/scripts/load_plp.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     7750 2023-06-20 12:09:45.000000 lino-welfare-23.6.0/lino_welfare/setup_info.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.054801 lino-welfare-23.6.0/lino_welfare.egg-info/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2037 2023-06-20 12:11:06.000000 lino-welfare-23.6.0/lino_welfare.egg-info/PKG-INFO
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    17726 2023-06-20 12:11:07.000000 lino-welfare-23.6.0/lino_welfare.egg-info/SOURCES.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        1 2023-06-20 12:11:06.000000 lino-welfare-23.6.0/lino_welfare.egg-info/dependency_links.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        1 2023-02-28 05:23:17.000000 lino-welfare-23.6.0/lino_welfare.egg-info/not-zip-safe
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       60 2023-06-20 12:11:06.000000 lino-welfare-23.6.0/lino_welfare.egg-info/requires.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       13 2023-06-20 12:11:06.000000 lino-welfare-23.6.0/lino_welfare.egg-info/top_level.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      141 2023-03-31 12:17:48.000000 lino-welfare-23.6.0/requirements-install.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      362 2023-02-28 05:23:17.000000 lino-welfare-23.6.0/requirements.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       38 2023-06-20 12:11:07.138802 lino-welfare-23.6.0/setup.cfg
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      164 2023-02-28 05:23:17.000000 lino-welfare-23.6.0/setup.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      619 2023-02-28 05:23:17.000000 lino-welfare-23.6.0/tasks.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.138802 lino-welfare-23.6.0/tests/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      559 2023-02-28 05:23:17.000000 lino-welfare-23.6.0/tests/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      457 2023-02-28 05:23:17.000000 lino-welfare-23.6.0/tests/test_demo.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      172 2023-02-28 05:23:17.000000 lino-welfare-23.6.0/tests/test_docs.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.865707 lino-welfare-23.8.0/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:55:53.000000 lino-welfare-23.8.0/COPYING
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      244 2022-12-15 17:33:14.000000 lino-welfare-23.8.0/MANIFEST.in
+-rw-rw-r--   0 luc       (1000) www-data    (33)     2074 2023-08-06 15:48:40.865707 lino-welfare-23.8.0/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1130 2023-03-17 19:57:59.000000 lino-welfare-23.8.0/README.rst
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.837707 lino-welfare-23.8.0/lino_welfare/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      653 2021-04-28 06:36:41.000000 lino-welfare-23.8.0/lino_welfare/__init__.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    21221 2023-04-05 09:42:33.000000 lino-welfare-23.8.0/lino_welfare/migrate.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)   193321 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/migrate_old.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.837707 lino-welfare-23.8.0/lino_welfare/modlib/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      659 2017-06-14 02:24:21.000000 lino-welfare-23.8.0/lino_welfare/modlib/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.837707 lino-welfare-23.8.0/lino_welfare/modlib/active_job_search/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      562 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/active_job_search/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.837707 lino-welfare-23.8.0/lino_welfare/modlib/active_job_search/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:50.000000 lino-welfare-23.8.0/lino_welfare/modlib/active_job_search/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      984 2021-04-15 06:04:24.000000 lino-welfare-23.8.0/lino_welfare/modlib/active_job_search/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2329 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/active_job_search/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:54:02.000000 lino-welfare-23.8.0/lino_welfare/modlib/active_job_search__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.837707 lino-welfare-23.8.0/lino_welfare/modlib/aids/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1538 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/aids/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2458 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/aids/choicelists.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.829707 lino-welfare-23.8.0/lino_welfare/modlib/aids/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.829707 lino-welfare-23.8.0/lino_welfare/modlib/aids/config/aids/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.837707 lino-welfare-23.8.0/lino_welfare/modlib/aids/config/aids/Confirmation/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1142 2020-07-22 09:24:05.000000 lino-welfare-23.8.0/lino_welfare/modlib/aids/config/aids/Confirmation/certificate.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      890 2019-08-01 14:29:04.000000 lino-welfare-23.8.0/lino_welfare/modlib/aids/config/aids/Confirmation/clothing_bank.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       65 2015-09-19 03:53:59.000000 lino-welfare-23.8.0/lino_welfare/modlib/aids/config/aids/Confirmation/default.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      713 2015-09-19 03:53:59.000000 lino-welfare-23.8.0/lino_welfare/modlib/aids/config/aids/Confirmation/fixed_income.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      872 2021-02-18 14:09:18.000000 lino-welfare-23.8.0/lino_welfare/modlib/aids/config/aids/Confirmation/food_bank.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      774 2015-09-19 03:54:00.000000 lino-welfare-23.8.0/lino_welfare/modlib/aids/config/aids/Confirmation/foreigner_income.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      575 2015-09-19 03:54:00.000000 lino-welfare-23.8.0/lino_welfare/modlib/aids/config/aids/Confirmation/furniture.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      564 2018-05-25 10:09:23.000000 lino-welfare-23.8.0/lino_welfare/modlib/aids/config/aids/Confirmation/heating_refund.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      763 2015-09-19 03:53:59.000000 lino-welfare-23.8.0/lino_welfare/modlib/aids/config/aids/Confirmation/integ_income.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4798 2015-12-16 12:20:46.000000 lino-welfare-23.8.0/lino_welfare/modlib/aids/config/aids/Confirmation/medical_refund.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      745 2015-09-19 03:54:00.000000 lino-welfare-23.8.0/lino_welfare/modlib/aids/config/aids/Confirmation/urgent_medical_care.body.html
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.837707 lino-welfare-23.8.0/lino_welfare/modlib/aids/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:54:00.000000 lino-welfare-23.8.0/lino_welfare/modlib/aids/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     6723 2021-04-17 00:36:55.000000 lino-welfare-23.8.0/lino_welfare/modlib/aids/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     6340 2021-04-11 05:44:50.000000 lino-welfare-23.8.0/lino_welfare/modlib/aids/fixtures/std.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    11507 2022-10-30 00:46:13.000000 lino-welfare-23.8.0/lino_welfare/modlib/aids/mixins.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    27336 2022-04-23 09:53:58.000000 lino-welfare-23.8.0/lino_welfare/modlib/aids/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      366 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/aids/roles.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.837707 lino-welfare-23.8.0/lino_welfare/modlib/art60/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1138 2022-10-07 01:12:03.000000 lino-welfare-23.8.0/lino_welfare/modlib/art60/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.829707 lino-welfare-23.8.0/lino_welfare/modlib/art60/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.829707 lino-welfare-23.8.0/lino_welfare/modlib/art60/config/art60/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.837707 lino-welfare-23.8.0/lino_welfare/modlib/art60/config/art60/Contract/
+-rw-rw-r--   0 luc       (1000) www-data    (33)    46358 2022-10-05 09:08:36.000000 lino-welfare-23.8.0/lino_welfare/modlib/art60/config/art60/Contract/Default.odt
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.837707 lino-welfare-23.8.0/lino_welfare/modlib/art60/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:45.000000 lino-welfare-23.8.0/lino_welfare/modlib/art60/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      806 2022-10-05 09:04:45.000000 lino-welfare-23.8.0/lino_welfare/modlib/art60/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    11002 2023-07-19 12:36:47.000000 lino-welfare-23.8.0/lino_welfare/modlib/art60/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.837707 lino-welfare-23.8.0/lino_welfare/modlib/art61/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      983 2022-10-01 01:36:58.000000 lino-welfare-23.8.0/lino_welfare/modlib/art61/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1739 2022-10-17 02:01:30.000000 lino-welfare-23.8.0/lino_welfare/modlib/art61/choicelists.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.829707 lino-welfare-23.8.0/lino_welfare/modlib/art61/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.829707 lino-welfare-23.8.0/lino_welfare/modlib/art61/config/art61/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.837707 lino-welfare-23.8.0/lino_welfare/modlib/art61/config/art61/Contract/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     8721 2015-09-19 03:53:45.000000 lino-welfare-23.8.0/lino_welfare/modlib/art61/config/art61/Contract/contract.body.html
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.837707 lino-welfare-23.8.0/lino_welfare/modlib/art61/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:45.000000 lino-welfare-23.8.0/lino_welfare/modlib/art61/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      347 2021-04-07 10:22:55.000000 lino-welfare-23.8.0/lino_welfare/modlib/art61/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     7239 2023-07-20 07:11:31.000000 lino-welfare-23.8.0/lino_welfare/modlib/art61/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.837707 lino-welfare-23.8.0/lino_welfare/modlib/badges/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1244 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/badges/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1693 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/badges/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.841707 lino-welfare-23.8.0/lino_welfare/modlib/cal/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      472 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/cal/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.829707 lino-welfare-23.8.0/lino_welfare/modlib/cal/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.829707 lino-welfare-23.8.0/lino_welfare/modlib/cal/config/cal/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.841707 lino-welfare-23.8.0/lino_welfare/modlib/cal/config/cal/Guest/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1249 2015-09-19 03:53:48.000000 lino-welfare-23.8.0/lino_welfare/modlib/cal/config/cal/Guest/Colleague.eml.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      248 2015-09-19 03:53:48.000000 lino-welfare-23.8.0/lino_welfare/modlib/cal/config/cal/Guest/Visitor.eml.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1700 2016-03-11 22:32:06.000000 lino-welfare-23.8.0/lino_welfare/modlib/cal/config/cal/Guest/presence_certificate.body.html
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.841707 lino-welfare-23.8.0/lino_welfare/modlib/cal/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:48.000000 lino-welfare-23.8.0/lino_welfare/modlib/cal/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       44 2016-02-22 08:52:32.000000 lino-welfare-23.8.0/lino_welfare/modlib/cal/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      825 2023-04-25 17:45:23.000000 lino-welfare-23.8.0/lino_welfare/modlib/cal/fixtures/demo2.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       43 2016-02-22 08:52:32.000000 lino-welfare-23.8.0/lino_welfare/modlib/cal/fixtures/std.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    14042 2023-04-15 09:50:28.000000 lino-welfare-23.8.0/lino_welfare/modlib/cal/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.841707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.841707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/WSDL/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     8464 2016-11-17 14:00:41.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/WSDL/2013HealthCareInsurance.wsdl
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4120 2017-04-21 06:04:21.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v1.wsdl
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3740 2019-10-02 18:54:22.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v2.wsdl
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2846 2015-09-19 03:53:40.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/WSDL/TestConnectionService.wsdl
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.841707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/WSDL/UnemploymentData/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    23800 2016-07-01 08:28:52.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/WSDL/UnemploymentData/UnemploymentDataTypesV2.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    15771 2016-05-18 07:19:58.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/WSDL/UnemploymentData/UnemploymentDataV2.wsdl
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3353 2016-05-18 07:19:58.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/WSDL/UnemploymentData/UnemploymentDataV2.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2075 2015-09-19 03:53:40.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/WSDL/WebServiceConnector.wsdl
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.841707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.841707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/20190612/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    11616 2016-09-30 09:59:39.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/20190612/RetrieveTIGroupsV5.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)   139908 2016-09-30 09:59:26.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/20190612/rn25_Release201411.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    16746 2013-12-23 11:43:40.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/HealthCareInsuranceTypesV1.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1639 2013-11-06 13:08:24.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/HealthCareInsuranceV1.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      154 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/README.txt
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.829707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.841707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     8507 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/CommonDataTypes.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      777 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/ExtensionPlaceHolder.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      933 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/NamespaceRoot.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4198 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/ResultSummary.xsd
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.829707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.841707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     9867 2015-09-19 03:53:43.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/IdentifyPersonReply.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     7931 2015-09-19 03:53:43.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/IdentifyPersonRequest.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1042 2015-09-19 03:53:43.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/NamespaceRoot.xsd
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.845707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     5622 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_AB_decision_Reply.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    13874 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_AB_decision_Request.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2435 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_C_decision_Reply.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     5569 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_C_decision_Request.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     5699 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_Common.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     9421 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_DF_decision_Reply.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    19800 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_DF_decision_Request.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1361 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/NamespaceRoot.xsd
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.845707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1600 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/CommonDataTypes.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4063 2015-09-19 03:53:43.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/ManageAccessReply.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     5074 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/ManageAccessRequest.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1146 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/NamespaceRoot.xsd
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.845707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3334 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/AddressHistory.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2591 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/FamilyComposition.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1460 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/NamespaceRoot.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3450 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/PerformInvestigationRequest.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3938 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/PerformInvetigationReply.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    11981 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/WaitRegister.xsd
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.845707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     5436 2015-09-19 03:53:43.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/AddressInformation.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     6504 2015-09-19 03:53:43.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/Citizen.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3332 2015-09-19 03:53:43.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/CommonDataTypes.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1119 2015-09-19 03:53:43.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/NamespaceRoot.xsd
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.845707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1969 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/CommonDataTypes.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1044 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/NamespaceRoot.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4562 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/SSDNReply.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3627 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/SSDNRequest.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     6440 2015-09-19 03:53:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/TestConnectionServiceV1.xsd
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/be/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/be/fgov/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/intf/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.845707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/intf/RetrieveTIGroupsService/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3491 2019-03-22 11:35:44.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/intf/RetrieveTIGroupsService/RetrieveTIGroupsV2.wsdl
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.845707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/RetrieveTIGroups/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2902 2019-03-22 11:35:44.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/RetrieveTIGroups/RetrieveTIGroupsV2.xsd
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.845707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/common/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    26504 2019-03-22 11:35:44.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/common/CommonV3.xsd
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/xsd/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.845707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/xsd/xm25/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)   121083 2019-03-22 11:35:44.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/xsd/xm25/xm25.xsd
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2715 2022-12-16 07:03:40.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3241 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/choicelists.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/config/cbss/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.845707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/config/cbss/IdentifyPersonRequest/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    21764 2015-09-19 03:53:40.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/config/cbss/IdentifyPersonRequest/Default.odt
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.845707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/config/cbss/RetrieveTIGroupsRequest/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    15865 2015-09-19 03:53:40.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/config/cbss/RetrieveTIGroupsRequest/Default.odt
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.849707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:41.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      538 2021-04-07 10:22:55.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/cbss.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3295 2021-04-09 12:30:52.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/cbss_demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1961 2015-09-19 03:53:41.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_1.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2109 2015-09-19 03:53:41.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_2.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2579 2015-09-19 03:53:41.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_3.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4542 2015-09-19 03:53:41.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_4.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1826 2015-09-19 03:53:41.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_5.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    11618 2015-09-19 03:53:41.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_1.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    24155 2015-09-19 03:53:41.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_2.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    26292 2015-11-29 20:09:07.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_3.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      619 2021-04-07 10:22:55.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/democfg.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     6081 2021-04-14 07:25:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/garble_tx25.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    20869 2015-09-19 03:53:41.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/lijst_van_sectoren_liste_des_secteurs.csv
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     9170 2021-04-07 10:22:55.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/purposes.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2401 2021-04-07 10:22:55.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/sectors.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    16822 2016-09-29 13:14:34.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/tx25_1107.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    23231 2016-09-30 11:44:50.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/tx25_1358.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    25160 2016-09-30 11:41:01.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/tx25_1373.xml
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.849707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/management/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:41.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/management/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.849707 lino-welfare-23.8.0/lino_welfare/modlib/cbss/management/commands/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:41.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/management/commands/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1895 2021-04-07 10:22:55.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/management/commands/cbss_validate_request.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    23598 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/mixins.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    26644 2022-12-16 07:04:27.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      401 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/roles.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    37959 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/tx25.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     9036 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/ui.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2468 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/cbss/utils.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.849707 lino-welfare-23.8.0/lino_welfare/modlib/client_vouchers/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      656 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/client_vouchers/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3463 2023-05-12 18:46:48.000000 lino-welfare-23.8.0/lino_welfare/modlib/client_vouchers/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1764 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/client_vouchers/ui.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.849707 lino-welfare-23.8.0/lino_welfare/modlib/contacts/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      872 2023-03-25 08:39:43.000000 lino-welfare-23.8.0/lino_welfare/modlib/contacts/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.849707 lino-welfare-23.8.0/lino_welfare/modlib/contacts/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:52.000000 lino-welfare-23.8.0/lino_welfare/modlib/contacts/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       49 2016-07-06 14:59:14.000000 lino-welfare-23.8.0/lino_welfare/modlib/contacts/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2016-07-06 14:59:14.000000 lino-welfare-23.8.0/lino_welfare/modlib/contacts/fixtures/std.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.849707 lino-welfare-23.8.0/lino_welfare/modlib/contacts/management/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2016-06-12 00:26:17.000000 lino-welfare-23.8.0/lino_welfare/modlib/contacts/management/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.849707 lino-welfare-23.8.0/lino_welfare/modlib/contacts/management/commands/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2016-06-12 00:27:23.000000 lino-welfare-23.8.0/lino_welfare/modlib/contacts/management/commands/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       70 2016-07-06 14:59:13.000000 lino-welfare-23.8.0/lino_welfare/modlib/contacts/management/commands/garble_persons.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     9487 2022-10-16 03:27:14.000000 lino-welfare-23.8.0/lino_welfare/modlib/contacts/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.849707 lino-welfare-23.8.0/lino_welfare/modlib/cv/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      479 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/cv/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.849707 lino-welfare-23.8.0/lino_welfare/modlib/cv/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:58.000000 lino-welfare-23.8.0/lino_welfare/modlib/cv/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      945 2021-04-14 07:26:02.000000 lino-welfare-23.8.0/lino_welfare/modlib/cv/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     7545 2023-02-19 18:56:17.000000 lino-welfare-23.8.0/lino_welfare/modlib/cv/fixtures/props.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2016-02-22 08:56:29.000000 lino-welfare-23.8.0/lino_welfare/modlib/cv/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     5673 2023-02-19 16:53:04.000000 lino-welfare-23.8.0/lino_welfare/modlib/cv/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.849707 lino-welfare-23.8.0/lino_welfare/modlib/debts/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1551 2023-04-01 17:02:15.000000 lino-welfare-23.8.0/lino_welfare/modlib/debts/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4424 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/debts/choicelists.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/debts/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/debts/config/debts/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.849707 lino-welfare-23.8.0/lino_welfare/modlib/debts/config/debts/Budget/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    17514 2018-09-28 15:27:47.000000 lino-welfare-23.8.0/lino_welfare/modlib/debts/config/debts/Budget/Default.odt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    24679 2015-09-19 03:53:44.000000 lino-welfare-23.8.0/lino_welfare/modlib/debts/config/debts/Budget/Default_2.odt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    19964 2015-09-19 03:53:43.000000 lino-welfare-23.8.0/lino_welfare/modlib/debts/config/debts/Budget/Default_new.odt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      661 2023-04-01 16:59:59.000000 lino-welfare-23.8.0/lino_welfare/modlib/debts/fields.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.849707 lino-welfare-23.8.0/lino_welfare/modlib/debts/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:44.000000 lino-welfare-23.8.0/lino_welfare/modlib/debts/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4587 2021-04-16 13:14:18.000000 lino-welfare-23.8.0/lino_welfare/modlib/debts/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    20553 2021-04-09 10:55:49.000000 lino-welfare-23.8.0/lino_welfare/modlib/debts/fixtures/minimal.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      577 2021-04-09 10:56:01.000000 lino-welfare-23.8.0/lino_welfare/modlib/debts/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1866 2023-04-01 16:57:27.000000 lino-welfare-23.8.0/lino_welfare/modlib/debts/mixins.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    22106 2023-04-01 16:29:04.000000 lino-welfare-23.8.0/lino_welfare/modlib/debts/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      352 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/debts/roles.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    21350 2023-04-01 15:00:13.000000 lino-welfare-23.8.0/lino_welfare/modlib/debts/ui.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.849707 lino-welfare-23.8.0/lino_welfare/modlib/dupable_clients/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      824 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/dupable_clients/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.849707 lino-welfare-23.8.0/lino_welfare/modlib/dupable_clients/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:54:03.000000 lino-welfare-23.8.0/lino_welfare/modlib/dupable_clients/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      420 2021-04-14 07:26:11.000000 lino-welfare-23.8.0/lino_welfare/modlib/dupable_clients/fixtures/demo2.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1924 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/dupable_clients/mixins.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1679 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/dupable_clients/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.849707 lino-welfare-23.8.0/lino_welfare/modlib/esf/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      852 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/esf/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     6282 2021-04-16 13:12:12.000000 lino-welfare-23.8.0/lino_welfare/modlib/esf/choicelists.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/esf/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/esf/config/esf/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.849707 lino-welfare-23.8.0/lino_welfare/modlib/esf/config/esf/Client/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      742 2020-11-20 03:16:25.000000 lino-welfare-23.8.0/lino_welfare/modlib/esf/config/esf/Client/esf_file.weasy.html
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.849707 lino-welfare-23.8.0/lino_welfare/modlib/esf/config/esf/ClientSummary/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      905 2016-06-07 02:40:58.000000 lino-welfare-23.8.0/lino_welfare/modlib/esf/config/esf/ClientSummary/base.weasy.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      620 2018-03-08 12:32:06.000000 lino-welfare-23.8.0/lino_welfare/modlib/esf/config/esf/ClientSummary/default.weasy.html
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.849707 lino-welfare-23.8.0/lino_welfare/modlib/esf/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2016-01-19 01:49:31.000000 lino-welfare-23.8.0/lino_welfare/modlib/esf/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      360 2018-05-25 08:15:58.000000 lino-welfare-23.8.0/lino_welfare/modlib/esf/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      482 2021-04-07 10:22:55.000000 lino-welfare-23.8.0/lino_welfare/modlib/esf/fixtures/std.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     5631 2022-10-17 13:39:01.000000 lino-welfare-23.8.0/lino_welfare/modlib/esf/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.849707 lino-welfare-23.8.0/lino_welfare/modlib/finan/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      381 2021-04-09 10:56:41.000000 lino-welfare-23.8.0/lino_welfare/modlib/finan/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.849707 lino-welfare-23.8.0/lino_welfare/modlib/finan/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-12-12 21:53:36.000000 lino-welfare-23.8.0/lino_welfare/modlib/finan/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      467 2021-04-07 10:22:55.000000 lino-welfare-23.8.0/lino_welfare/modlib/finan/fixtures/payments.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1969 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/finan/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.849707 lino-welfare-23.8.0/lino_welfare/modlib/households/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      306 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/households/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.849707 lino-welfare-23.8.0/lino_welfare/modlib/households/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:45.000000 lino-welfare-23.8.0/lino_welfare/modlib/households/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       51 2016-02-22 08:57:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/households/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       50 2016-02-22 08:57:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/households/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3807 2021-12-14 02:24:13.000000 lino-welfare-23.8.0/lino_welfare/modlib/households/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.849707 lino-welfare-23.8.0/lino_welfare/modlib/immersion/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1107 2021-04-10 14:05:48.000000 lino-welfare-23.8.0/lino_welfare/modlib/immersion/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/immersion/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/immersion/config/immersion/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.853707 lino-welfare-23.8.0/lino_welfare/modlib/immersion/config/immersion/Contract/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)   667935 2018-05-10 19:37:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/immersion/config/immersion/Contract/StageForem.odt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     5587 2016-02-11 13:18:18.000000 lino-welfare-23.8.0/lino_welfare/modlib/immersion/config/immersion/Contract/immersion.body.html
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.853707 lino-welfare-23.8.0/lino_welfare/modlib/immersion/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:47.000000 lino-welfare-23.8.0/lino_welfare/modlib/immersion/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1446 2021-04-09 13:17:47.000000 lino-welfare-23.8.0/lino_welfare/modlib/immersion/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3463 2022-10-17 19:12:30.000000 lino-welfare-23.8.0/lino_welfare/modlib/immersion/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3921 2022-12-15 10:10:45.000000 lino-welfare-23.8.0/lino_welfare/modlib/immersion/ui.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.853707 lino-welfare-23.8.0/lino_welfare/modlib/integ/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2406 2022-10-16 06:00:46.000000 lino-welfare-23.8.0/lino_welfare/modlib/integ/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.853707 lino-welfare-23.8.0/lino_welfare/modlib/integ/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:46.000000 lino-welfare-23.8.0/lino_welfare/modlib/integ/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     8565 2022-10-17 13:22:39.000000 lino-welfare-23.8.0/lino_welfare/modlib/integ/fixtures/demo.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     2470 2023-04-05 09:42:33.000000 lino-welfare-23.8.0/lino_welfare/modlib/integ/fixtures/std.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    23997 2022-11-08 12:30:48.000000 lino-welfare-23.8.0/lino_welfare/modlib/integ/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      377 2021-04-09 10:57:42.000000 lino-welfare-23.8.0/lino_welfare/modlib/integ/roles.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.853707 lino-welfare-23.8.0/lino_welfare/modlib/isip/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      351 2022-10-07 00:51:22.000000 lino-welfare-23.8.0/lino_welfare/modlib/isip/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      722 2021-04-09 10:57:53.000000 lino-welfare-23.8.0/lino_welfare/modlib/isip/choicelists.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/isip/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/isip/config/isip/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.853707 lino-welfare-23.8.0/lino_welfare/modlib/isip/config/isip/Contract/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    55172 2016-08-02 05:50:22.000000 lino-welfare-23.8.0/lino_welfare/modlib/isip/config/isip/Contract/Default.odt
+-rw-rw-r--   0 luc       (1000) www-data    (33)    17714 2023-04-05 09:42:33.000000 lino-welfare-23.8.0/lino_welfare/modlib/isip/mixins.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    11361 2023-04-05 09:42:33.000000 lino-welfare-23.8.0/lino_welfare/modlib/isip/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.853707 lino-welfare-23.8.0/lino_welfare/modlib/jobs/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      903 2022-10-16 05:44:50.000000 lino-welfare-23.8.0/lino_welfare/modlib/jobs/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/jobs/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/jobs/config/jobs/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.853707 lino-welfare-23.8.0/lino_welfare/modlib/jobs/config/jobs/Contract/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    94813 2015-09-19 03:54:01.000000 lino-welfare-23.8.0/lino_welfare/modlib/jobs/config/jobs/Contract/Default.odt
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.853707 lino-welfare-23.8.0/lino_welfare/modlib/jobs/config/jobs/ContractsSituation/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     9896 2015-09-19 03:54:01.000000 lino-welfare-23.8.0/lino_welfare/modlib/jobs/config/jobs/ContractsSituation/Default.odt
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.853707 lino-welfare-23.8.0/lino_welfare/modlib/jobs/config/jobs/OldJobsOverview/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     9876 2015-09-19 03:54:01.000000 lino-welfare-23.8.0/lino_welfare/modlib/jobs/config/jobs/OldJobsOverview/Default.odt
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.853707 lino-welfare-23.8.0/lino_welfare/modlib/jobs/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:54:02.000000 lino-welfare-23.8.0/lino_welfare/modlib/jobs/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      935 2021-04-07 10:22:55.000000 lino-welfare-23.8.0/lino_welfare/modlib/jobs/fixtures/std.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     2930 2023-04-05 09:42:33.000000 lino-welfare-23.8.0/lino_welfare/modlib/jobs/mixins.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    13134 2023-07-19 17:56:38.000000 lino-welfare-23.8.0/lino_welfare/modlib/jobs/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      327 2015-09-19 03:54:02.000000 lino-welfare-23.8.0/lino_welfare/modlib/jobs/template_messages.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    17073 2022-12-15 10:11:11.000000 lino-welfare-23.8.0/lino_welfare/modlib/jobs/ui.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.853707 lino-welfare-23.8.0/lino_welfare/modlib/ledger/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      419 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/ledger/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.853707 lino-welfare-23.8.0/lino_welfare/modlib/ledger/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:50.000000 lino-welfare-23.8.0/lino_welfare/modlib/ledger/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      531 2021-04-07 10:22:55.000000 lino-welfare-23.8.0/lino_welfare/modlib/ledger/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2758 2021-04-07 10:22:55.000000 lino-welfare-23.8.0/lino_welfare/modlib/ledger/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3082 2021-04-07 10:22:55.000000 lino-welfare-23.8.0/lino_welfare/modlib/ledger/fixtures/std_journals.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2438 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/ledger/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.853707 lino-welfare-23.8.0/lino_welfare/modlib/newcomers/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      996 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/newcomers/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.853707 lino-welfare-23.8.0/lino_welfare/modlib/newcomers/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:56.000000 lino-welfare-23.8.0/lino_welfare/modlib/newcomers/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3181 2021-04-14 07:26:29.000000 lino-welfare-23.8.0/lino_welfare/modlib/newcomers/fixtures/demo.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    16680 2022-11-08 12:30:48.000000 lino-welfare-23.8.0/lino_welfare/modlib/newcomers/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      416 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/newcomers/roles.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.853707 lino-welfare-23.8.0/lino_welfare/modlib/notes/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      282 2018-11-22 22:34:11.000000 lino-welfare-23.8.0/lino_welfare/modlib/notes/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.853707 lino-welfare-23.8.0/lino_welfare/modlib/notes/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:57.000000 lino-welfare-23.8.0/lino_welfare/modlib/notes/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      889 2021-04-14 07:26:37.000000 lino-welfare-23.8.0/lino_welfare/modlib/notes/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       45 2016-02-22 09:05:22.000000 lino-welfare-23.8.0/lino_welfare/modlib/notes/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2462 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/notes/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.853707 lino-welfare-23.8.0/lino_welfare/modlib/pcsw/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1516 2022-10-25 08:21:59.000000 lino-welfare-23.8.0/lino_welfare/modlib/pcsw/__init__.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     4420 2023-01-25 03:54:22.000000 lino-welfare-23.8.0/lino_welfare/modlib/pcsw/actions.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2558 2021-04-09 10:58:06.000000 lino-welfare-23.8.0/lino_welfare/modlib/pcsw/choicelists.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      366 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/pcsw/client_address.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.853707 lino-welfare-23.8.0/lino_welfare/modlib/pcsw/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/pcsw/config/pcsw/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.853707 lino-welfare-23.8.0/lino_welfare/modlib/pcsw/config/pcsw/Client/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    32053 2015-09-19 03:53:51.000000 lino-welfare-23.8.0/lino_welfare/modlib/pcsw/config/pcsw/Client/cv.odt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)   157223 2015-09-19 03:53:51.000000 lino-welfare-23.8.0/lino_welfare/modlib/pcsw/config/pcsw/Client/eid-content.odt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    31905 2015-09-19 03:53:51.000000 lino-welfare-23.8.0/lino_welfare/modlib/pcsw/config/pcsw/Client/file_sheet.odt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      373 2015-09-19 03:53:51.000000 lino-welfare-23.8.0/lino_welfare/modlib/pcsw/config/pcsw/Client/pac.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      487 2015-09-19 03:53:51.000000 lino-welfare-23.8.0/lino_welfare/modlib/pcsw/config/welcome.html
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.853707 lino-welfare-23.8.0/lino_welfare/modlib/pcsw/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:52.000000 lino-welfare-23.8.0/lino_welfare/modlib/pcsw/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2287 2021-04-07 10:22:55.000000 lino-welfare-23.8.0/lino_welfare/modlib/pcsw/fixtures/demo2.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1595 2021-04-09 10:58:22.000000 lino-welfare-23.8.0/lino_welfare/modlib/pcsw/fixtures/std.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    36618 2023-04-05 09:42:33.000000 lino-welfare-23.8.0/lino_welfare/modlib/pcsw/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      509 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/pcsw/roles.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.857707 lino-welfare-23.8.0/lino_welfare/modlib/polls/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      335 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/polls/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.857707 lino-welfare-23.8.0/lino_welfare/modlib/polls/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:39.000000 lino-welfare-23.8.0/lino_welfare/modlib/polls/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     5736 2021-04-14 07:26:52.000000 lino-welfare-23.8.0/lino_welfare/modlib/polls/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      328 2021-04-07 10:22:55.000000 lino-welfare-23.8.0/lino_welfare/modlib/polls/fixtures/jobsearch.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       51 2016-07-06 15:15:32.000000 lino-welfare-23.8.0/lino_welfare/modlib/polls/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      214 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/polls/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.857707 lino-welfare-23.8.0/lino_welfare/modlib/projects/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      619 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/projects/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2069 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/projects/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.857707 lino-welfare-23.8.0/lino_welfare/modlib/reception/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      532 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/reception/__init__.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    14515 2023-07-19 12:25:39.000000 lino-welfare-23.8.0/lino_welfare/modlib/reception/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.857707 lino-welfare-23.8.0/lino_welfare/modlib/sales/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:50.000000 lino-welfare-23.8.0/lino_welfare/modlib/sales/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      466 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/sales/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.857707 lino-welfare-23.8.0/lino_welfare/modlib/sepa/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      308 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/sepa/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.857707 lino-welfare-23.8.0/lino_welfare/modlib/sepa/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:58.000000 lino-welfare-23.8.0/lino_welfare/modlib/sepa/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4013 2021-04-14 07:27:02.000000 lino-welfare-23.8.0/lino_welfare/modlib/sepa/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1603 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/sepa/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.857707 lino-welfare-23.8.0/lino_welfare/modlib/system/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      216 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/system/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4076 2023-02-18 15:38:45.000000 lino-welfare-23.8.0/lino_welfare/modlib/system/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.857707 lino-welfare-23.8.0/lino_welfare/modlib/users/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      345 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/users/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.857707 lino-welfare-23.8.0/lino_welfare/modlib/users/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:53.000000 lino-welfare-23.8.0/lino_welfare/modlib/users/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       46 2017-06-13 23:57:01.000000 lino-welfare-23.8.0/lino_welfare/modlib/users/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2017-06-13 23:57:01.000000 lino-welfare-23.8.0/lino_welfare/modlib/users/fixtures/demo2.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       52 2017-06-13 23:57:01.000000 lino-welfare-23.8.0/lino_welfare/modlib/users/fixtures/demo_users.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2777 2022-11-08 12:29:27.000000 lino-welfare-23.8.0/lino_welfare/modlib/users/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1050 2022-11-08 12:29:57.000000 lino-welfare-23.8.0/lino_welfare/modlib/users/ui.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.857707 lino-welfare-23.8.0/lino_welfare/modlib/welfare/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      407 2021-04-15 05:57:45.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.857707 lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.857707 lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/excerpts/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)   672907 2021-02-18 17:59:31.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/excerpts/Default.odt
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.857707 lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      511 2015-09-19 03:53:55.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/TasksByClient.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1221 2015-09-19 03:53:55.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/anw.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1146 2015-09-19 03:53:55.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/aus.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      533 2015-10-21 13:33:32.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/certificate.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       40 2015-09-19 03:53:55.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/default.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      624 2015-09-19 03:53:55.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/summary.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      800 2021-02-03 10:12:55.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/excerpts/base.body.html
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/integ/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.857707 lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/integ/ActivityReport/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    11787 2015-09-19 03:53:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/integ/ActivityReport/Default.odt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      585 2021-02-18 18:02:26.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/letter_margin_bottom.html
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/notes/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.857707 lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/notes/Note/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    50685 2015-09-19 03:53:55.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/notes/Note/Letter.odt
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.857707 lino-welfare-23.8.0/lino_welfare/modlib/welfare/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:55.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/fixtures/__init__.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    43393 2023-04-05 09:42:34.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1040 2021-04-14 07:27:52.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/fixtures/demo2.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    29832 2021-04-07 10:22:55.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/fixtures/pp2lino.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4243 2023-03-04 02:06:08.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3232 2022-10-03 06:09:37.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/fixtures/std2.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    26073 2023-06-23 05:19:06.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/help_texts.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/welfare/locale/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/welfare/locale/de/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.857707 lino-welfare-23.8.0/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    38241 2023-04-01 16:28:46.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 luc       (1000) www-data    (33)   131485 2023-04-01 16:28:46.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/django.po
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/welfare/locale/fr/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.861707 lino-welfare-23.8.0/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    35373 2023-08-04 18:10:23.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 luc       (1000) www-data    (33)   130333 2023-08-04 18:10:23.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/django.po
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/welfare/locale/nl/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.861707 lino-welfare-23.8.0/lino_welfare/modlib/welfare/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      409 2015-09-19 03:53:53.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    93297 2021-02-11 17:36:49.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/locale/nl/LC_MESSAGES/django.po
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.861707 lino-welfare-23.8.0/lino_welfare/modlib/welfare/management/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:56.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/management/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.861707 lino-welfare-23.8.0/lino_welfare/modlib/welfare/management/commands/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:56.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/management/commands/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    18127 2020-01-29 15:42:45.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/management/commands/cpas2lino.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4743 2018-11-22 22:34:07.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/management/commands/garble.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4518 2018-11-22 22:34:12.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/management/commands/gd2lino.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    14642 2018-11-22 22:34:09.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/management/commands/initdb_tim.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    35429 2021-04-07 10:22:55.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/management/commands/watch_tim.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     5859 2021-04-15 05:57:38.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/models.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     6296 2023-04-05 00:25:15.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/settings.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     7612 2023-04-25 18:12:17.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/user_types.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1635 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/welfare/workflows.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.861707 lino-welfare-23.8.0/lino_welfare/modlib/xcourses/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1055 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/xcourses/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/xcourses/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/modlib/xcourses/config/courses/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.861707 lino-welfare-23.8.0/lino_welfare/modlib/xcourses/config/courses/Course/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    12127 2015-09-19 03:53:49.000000 lino-welfare-23.8.0/lino_welfare/modlib/xcourses/config/courses/Course/candidates.odt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    12100 2015-09-19 03:53:49.000000 lino-welfare-23.8.0/lino_welfare/modlib/xcourses/config/courses/Course/participants.odt
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.861707 lino-welfare-23.8.0/lino_welfare/modlib/xcourses/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:49.000000 lino-welfare-23.8.0/lino_welfare/modlib/xcourses/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3037 2021-04-14 07:28:00.000000 lino-welfare-23.8.0/lino_welfare/modlib/xcourses/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    20702 2021-05-12 14:10:36.000000 lino-welfare-23.8.0/lino_welfare/modlib/xcourses/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      363 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/modlib/xcourses/roles.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.861707 lino-welfare-23.8.0/lino_welfare/projects/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      206 2019-03-26 11:55:25.000000 lino-welfare-23.8.0/lino_welfare/projects/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.861707 lino-welfare-23.8.0/lino_welfare/projects/gerd/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      297 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/projects/gerd/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      415 2019-02-06 12:35:36.000000 lino-welfare-23.8.0/lino_welfare/projects/gerd/django110_isnull.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)      278 2023-01-10 07:35:10.000000 lino-welfare-23.8.0/lino_welfare/projects/gerd/manage.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1388 2022-11-06 03:59:24.000000 lino-welfare-23.8.0/lino_welfare/projects/gerd/print_tx25.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.861707 lino-welfare-23.8.0/lino_welfare/projects/gerd/settings/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      342 2021-04-16 02:21:20.000000 lino-welfare-23.8.0/lino_welfare/projects/gerd/settings/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      763 2023-03-21 15:30:40.000000 lino-welfare-23.8.0/lino_welfare/projects/gerd/settings/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      388 2019-02-06 12:35:36.000000 lino-welfare-23.8.0/lino_welfare/projects/gerd/settings/doctests.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/projects/gerd/settings/media/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.861707 lino-welfare-23.8.0/lino_welfare/projects/gerd/settings/media/beid/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3046 2019-02-06 20:01:51.000000 lino-welfare-23.8.0/lino_welfare/projects/gerd/settings/media/beid/123456789012.jpg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     7615 2019-02-06 20:01:50.000000 lino-welfare-23.8.0/lino_welfare/projects/gerd/settings/media/beid/591413288107.jpg
+-rw-rw-r--   0 luc       (1000) www-data    (33)     3068 2022-12-05 15:59:46.000000 lino-welfare-23.8.0/lino_welfare/projects/gerd/settings/media/beid/592382784616.jpg
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/projects/gerd/settings/media/webdav/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/projects/gerd/settings/media/webdav/userdocs/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.861707 lino-welfare-23.8.0/lino_welfare/projects/gerd/settings/media/webdav/userdocs/appyodt/
+-rw-rw-r--   0 luc       (1000) www-data    (33)    13380 2023-08-05 09:36:19.000000 lino-welfare-23.8.0/lino_welfare/projects/gerd/settings/media/webdav/userdocs/appyodt/jobs.JobsOverview.odt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       85 2019-02-06 12:35:36.000000 lino-welfare-23.8.0/lino_welfare/projects/gerd/settings/memory.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1038 2019-03-26 11:59:36.000000 lino-welfare-23.8.0/lino_welfare/projects/gerd/settings/mysql.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.865707 lino-welfare-23.8.0/lino_welfare/projects/gerd/tests/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      183 2021-04-07 10:22:55.000000 lino-welfare-23.8.0/lino_welfare/projects/gerd/tests/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2459 2021-04-07 10:22:55.000000 lino-welfare-23.8.0/lino_welfare/projects/gerd/tests/test_aids.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2765 2021-04-07 10:22:55.000000 lino-welfare-23.8.0/lino_welfare/projects/gerd/tests/test_broken_gfks.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     7909 2021-04-07 10:22:55.000000 lino-welfare-23.8.0/lino_welfare/projects/gerd/tests/test_cbss.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     2948 2023-04-05 09:42:34.000000 lino-welfare-23.8.0/lino_welfare/projects/gerd/tests/test_clients.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4214 2021-02-15 07:59:43.000000 lino-welfare-23.8.0/lino_welfare/projects/gerd/tests/test_debts.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      253 2021-02-15 14:17:17.000000 lino-welfare-23.8.0/lino_welfare/projects/gerd/tests/test_restore.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    35518 2023-07-20 07:07:45.000000 lino-welfare-23.8.0/lino_welfare/projects/gerd/tests/test_watchtim.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.865707 lino-welfare-23.8.0/lino_welfare/projects/mathieu/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      365 2021-04-07 10:22:54.000000 lino-welfare-23.8.0/lino_welfare/projects/mathieu/__init__.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)      280 2023-01-10 07:35:10.000000 lino-welfare-23.8.0/lino_welfare/projects/mathieu/manage.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.865707 lino-welfare-23.8.0/lino_welfare/projects/mathieu/settings/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      281 2022-10-05 18:42:47.000000 lino-welfare-23.8.0/lino_welfare/projects/mathieu/settings/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      512 2023-07-19 12:26:24.000000 lino-welfare-23.8.0/lino_welfare/projects/mathieu/settings/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      347 2019-02-06 12:35:36.000000 lino-welfare-23.8.0/lino_welfare/projects/mathieu/settings/doctests.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.833707 lino-welfare-23.8.0/lino_welfare/projects/mathieu/settings/media/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.865707 lino-welfare-23.8.0/lino_welfare/projects/mathieu/settings/media/beid/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3046 2022-10-23 06:31:52.000000 lino-welfare-23.8.0/lino_welfare/projects/mathieu/settings/media/beid/123456789012.jpg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     7615 2022-10-23 06:31:52.000000 lino-welfare-23.8.0/lino_welfare/projects/mathieu/settings/media/beid/591413288107.jpg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       85 2019-02-06 12:35:36.000000 lino-welfare-23.8.0/lino_welfare/projects/mathieu/settings/memory.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.865707 lino-welfare-23.8.0/lino_welfare/projects/mathieu/tests/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2019-02-06 12:35:36.000000 lino-welfare-23.8.0/lino_welfare/projects/mathieu/tests/__init__.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     6890 2023-04-28 16:14:22.000000 lino-welfare-23.8.0/lino_welfare/projects/mathieu/tests/test_chatelet.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    18271 2022-08-15 07:53:16.000000 lino-welfare-23.8.0/lino_welfare/projects/mathieu/tests/test_notify.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.865707 lino-welfare-23.8.0/lino_welfare/scripts/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:30.000000 lino-welfare-23.8.0/lino_welfare/scripts/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     7346 2018-11-22 22:34:35.000000 lino-welfare-23.8.0/lino_welfare/scripts/load_plp.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     7750 2023-08-06 15:48:19.000000 lino-welfare-23.8.0/lino_welfare/setup_info.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.837707 lino-welfare-23.8.0/lino_welfare.egg-info/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2074 2023-08-06 15:48:40.000000 lino-welfare-23.8.0/lino_welfare.egg-info/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    18180 2023-08-06 15:48:40.000000 lino-welfare-23.8.0/lino_welfare.egg-info/SOURCES.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2023-08-06 15:48:40.000000 lino-welfare-23.8.0/lino_welfare.egg-info/dependency_links.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2016-09-02 10:20:26.000000 lino-welfare-23.8.0/lino_welfare.egg-info/not-zip-safe
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       60 2023-08-06 15:48:40.000000 lino-welfare-23.8.0/lino_welfare.egg-info/requires.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       13 2023-08-06 15:48:40.000000 lino-welfare-23.8.0/lino_welfare.egg-info/top_level.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)      141 2023-04-01 07:25:17.000000 lino-welfare-23.8.0/requirements-install.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)      362 2023-02-04 01:22:52.000000 lino-welfare-23.8.0/requirements.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)       38 2023-08-06 15:48:40.865707 lino-welfare-23.8.0/setup.cfg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      164 2017-01-04 05:50:59.000000 lino-welfare-23.8.0/setup.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      619 2022-10-22 23:43:43.000000 lino-welfare-23.8.0/tasks.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:48:40.865707 lino-welfare-23.8.0/tests/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      559 2021-04-07 10:22:53.000000 lino-welfare-23.8.0/tests/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      457 2021-03-07 17:52:34.000000 lino-welfare-23.8.0/tests/test_demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      172 2018-05-03 15:32:38.000000 lino-welfare-23.8.0/tests/test_docs.py
```

### Comparing `lino-welfare-23.6.0/COPYING` & `lino-welfare-23.8.0/COPYING`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/PKG-INFO` & `lino-welfare-23.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: lino-welfare
-Version: 23.6.0
+Version: 23.8.0
 Summary: A Lino plugin library for Belgian PCSWs
 Home-page: https://gitlab.com/lino-framework/welfare
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -55,7 +57,9 @@
 - For introductions, commercial information and hosting solutions
   see https://www.saffre-rumma.net
 
 - This is a sustainably free open-source project. Your contributions are
   welcome.  See https://community.lino-framework.org for details.
 
 
+
+
```

### Comparing `lino-welfare-23.6.0/README.rst` & `lino-welfare-23.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/__init__.py` & `lino-welfare-23.8.0/lino_welfare/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/migrate.py` & `lino-welfare-23.8.0/lino_welfare/migrate.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/migrate_old.py` & `lino-welfare-23.8.0/lino_welfare/migrate_old.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/__init__.py` & `lino-welfare-23.8.0/lino_welfare/modlib/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/active_job_search/__init__.py` & `lino-welfare-23.8.0/lino_welfare/modlib/active_job_search/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/active_job_search/fixtures/demo.py` & `lino-welfare-23.8.0/lino_welfare/modlib/active_job_search/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/active_job_search/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/active_job_search/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/aids/__init__.py` & `lino-welfare-23.8.0/lino_welfare/modlib/aids/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/aids/choicelists.py` & `lino-welfare-23.8.0/lino_welfare/modlib/aids/choicelists.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/certificate.body.html` & `lino-welfare-23.8.0/lino_welfare/modlib/aids/config/aids/Confirmation/certificate.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/clothing_bank.body.html` & `lino-welfare-23.8.0/lino_welfare/modlib/aids/config/aids/Confirmation/clothing_bank.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/fixed_income.body.html` & `lino-welfare-23.8.0/lino_welfare/modlib/aids/config/aids/Confirmation/fixed_income.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/food_bank.body.html` & `lino-welfare-23.8.0/lino_welfare/modlib/aids/config/aids/Confirmation/food_bank.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/foreigner_income.body.html` & `lino-welfare-23.8.0/lino_welfare/modlib/aids/config/aids/Confirmation/foreigner_income.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/furniture.body.html` & `lino-welfare-23.8.0/lino_welfare/modlib/aids/config/aids/Confirmation/furniture.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/heating_refund.body.html` & `lino-welfare-23.8.0/lino_welfare/modlib/aids/config/aids/Confirmation/heating_refund.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/integ_income.body.html` & `lino-welfare-23.8.0/lino_welfare/modlib/aids/config/aids/Confirmation/integ_income.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/medical_refund.body.html` & `lino-welfare-23.8.0/lino_welfare/modlib/aids/config/aids/Confirmation/medical_refund.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/urgent_medical_care.body.html` & `lino-welfare-23.8.0/lino_welfare/modlib/aids/config/aids/Confirmation/urgent_medical_care.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/aids/fixtures/demo.py` & `lino-welfare-23.8.0/lino_welfare/modlib/aids/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/aids/fixtures/std.py` & `lino-welfare-23.8.0/lino_welfare/modlib/aids/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/aids/mixins.py` & `lino-welfare-23.8.0/lino_welfare/modlib/aids/mixins.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/aids/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/aids/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/art60/__init__.py` & `lino-welfare-23.8.0/lino_welfare/modlib/art60/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/art60/config/art60/Contract/Default.odt` & `lino-welfare-23.8.0/lino_welfare/modlib/art60/config/art60/Contract/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/art60/fixtures/std.py` & `lino-welfare-23.8.0/lino_welfare/modlib/art60/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/art60/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/art60/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,17 +77,22 @@
         return (
             'client type '
             'applies_from applies_until duration '
             'language user user_asd exam_policy '
             'date_decided date_issued ')
 
     @property
-    def active_convention(self):
+    def active_convention_property(self):
         return Convention.objects.filter(contract=self).first()
 
+    @dd.virtualfield(dd.ForeignKey('art60.Convention', verbose_name=_("Active convention")))
+    def active_convention(self, ar):
+        return Convention.objects.filter(contract=self).first()
+
+
     @property
     def excerpt_type(self):  # temporary workaround.
         return rt.models.excerpts.ExcerptType()
 
 
 
 # dd.update_field(Contract, 'user', verbose_name=_("responsible (IS)"))
@@ -253,15 +258,15 @@
 
 
 class ContractsByClient(Contracts):
     required_roles = dd.login_required((SocialUser, SocialCoordinator))
     master_key = 'client'
     auto_fit_column_widths = True
     no_phantom_row = False  # override ContractBaseTable
-    column_names = "applies_from applies_until date_ended duration type user remark:30 *"
+    column_names = "applies_from applies_until date_ended duration type user active_convention:20 remark:30 *"
     # hidden_columns = """
     # language contact_person contact_role
     # printed regime schedule hourly_rate
     # date_decided date_issued user_asd exam_policy ending date_ended
     # duration reference_person responsibilities remark
     # """
```

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/art61/__init__.py` & `lino-welfare-23.8.0/lino_welfare/modlib/art61/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/art61/choicelists.py` & `lino-welfare-23.8.0/lino_welfare/modlib/art61/choicelists.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/art61/config/art61/Contract/contract.body.html` & `lino-welfare-23.8.0/lino_welfare/modlib/art61/config/art61/Contract/contract.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/art61/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/art61/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,29 +6,25 @@
 import logging; logger = logging.getLogger(__name__)
 
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 
 from lino.api import dd
 from lino import mixins
-
 from lino_xl.lib.cv.mixins import SectorFunction
 from lino_welfare.modlib.integ.roles import IntegUser, IntegrationStaff
-
 from lino_welfare.modlib.isip.mixins import ContractPartnerBase, ContractBase
 from lino_welfare.modlib.isip.mixins import (ContractBaseTable,
                                              ContractTypeBase)
 from lino_welfare.modlib.jobs.mixins import JobSupplyment
-
-from .choicelists import Subsidizations
-
 from lino_xl.lib.coachings.utils import has_contracts_filter
 from lino_xl.lib.clients.choicelists import ClientEvents, ObservedEvent
 from lino_welfare.modlib.pcsw.roles import SocialCoordinator
 
+from .choicelists import Subsidizations
 
 class ClientHasContract(ObservedEvent):
     text = _("Art61 job supplyment")
 
     def add_filter(self, qs, pv):
         period = (pv.start_date, pv.end_date)
         flt = has_contracts_filter('art61_contract_set_by_client', period)
@@ -152,15 +148,15 @@
     column_names = 'id client client__national_id ' \
                    'applies_from date_ended user type *'
     order_by = ['id']
     detail_layout = ContractDetail()
     insert_layout = """
     client
     company
-    function
+    type function
     """
 
     parameters = dict(
         type=dd.ForeignKey(
             'art61.ContractType', blank=True,
             verbose_name=_("Only job supplies of type")),
         **ContractBaseTable.parameters)
```

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/badges/__init__.py` & `lino-welfare-23.8.0/lino_welfare/modlib/badges/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/badges/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/badges/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cal/config/cal/Guest/Colleague.eml.html` & `lino-welfare-23.8.0/lino_welfare/modlib/cal/config/cal/Guest/Colleague.eml.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cal/config/cal/Guest/presence_certificate.body.html` & `lino-welfare-23.8.0/lino_welfare/modlib/cal/config/cal/Guest/presence_certificate.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cal/fixtures/demo2.py` & `lino-welfare-23.8.0/lino_welfare/modlib/cal/fixtures/demo2.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cal/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/cal/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v1.wsdl` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v1.wsdl`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v2.wsdl` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v2.wsdl`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/WSDL/TestConnectionService.wsdl` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/WSDL/TestConnectionService.wsdl`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/WSDL/WebServiceConnector.wsdl` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/WSDL/WebServiceConnector.wsdl`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/20190612/RetrieveTIGroupsV5.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/20190612/RetrieveTIGroupsV5.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/20190612/rn25_Release201411.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/20190612/rn25_Release201411.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/CommonDataTypes.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/CommonDataTypes.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/ExtensionPlaceHolder.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/ExtensionPlaceHolder.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/NamespaceRoot.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/NamespaceRoot.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/ResultSummary.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/ResultSummary.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/IdentifyPersonReply.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/IdentifyPersonReply.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/IdentifyPersonRequest.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/IdentifyPersonRequest.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/NamespaceRoot.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/NamespaceRoot.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_AB_decision_Reply.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_AB_decision_Reply.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_AB_decision_Request.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_AB_decision_Request.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_C_decision_Reply.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_C_decision_Reply.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_C_decision_Request.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_C_decision_Request.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_Common.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_Common.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_DF_decision_Reply.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_DF_decision_Reply.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_DF_decision_Request.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_DF_decision_Request.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/NamespaceRoot.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/NamespaceRoot.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/CommonDataTypes.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/CommonDataTypes.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/ManageAccessReply.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/ManageAccessReply.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/ManageAccessRequest.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/ManageAccessRequest.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/NamespaceRoot.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/NamespaceRoot.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/AddressHistory.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/AddressHistory.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/FamilyComposition.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/FamilyComposition.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/NamespaceRoot.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/NamespaceRoot.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/PerformInvestigationRequest.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/PerformInvestigationRequest.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/PerformInvetigationReply.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/PerformInvetigationReply.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/WaitRegister.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/WaitRegister.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/AddressInformation.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/AddressInformation.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/Citizen.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/Citizen.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/CommonDataTypes.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/CommonDataTypes.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/NamespaceRoot.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/NamespaceRoot.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/CommonDataTypes.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/CommonDataTypes.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/NamespaceRoot.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/NamespaceRoot.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/SSDNReply.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/SSDNReply.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/SSDNRequest.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/SSDNRequest.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/TestConnectionServiceV1.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/TestConnectionServiceV1.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/intf/RetrieveTIGroupsService/RetrieveTIGroupsV2.wsdl` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/intf/RetrieveTIGroupsService/RetrieveTIGroupsV2.wsdl`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/RetrieveTIGroups/RetrieveTIGroupsV2.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/RetrieveTIGroups/RetrieveTIGroupsV2.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/common/CommonV3.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/common/CommonV3.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/xsd/xm25/xm25.xsd` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/xsd/xm25/xm25.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/__init__.py` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/choicelists.py` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/choicelists.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/config/cbss/IdentifyPersonRequest/Default.odt` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/config/cbss/IdentifyPersonRequest/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/config/cbss/RetrieveTIGroupsRequest/Default.odt` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/config/cbss/RetrieveTIGroupsRequest/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/cbss.py` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/cbss.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/cbss_demo.py` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/cbss_demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_1.xml` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_1.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_2.xml` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_2.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_3.xml` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_3.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_4.xml` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_4.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_5.xml` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_5.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_1.xml` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_1.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_2.xml` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_2.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_3.xml` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_3.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/democfg.py` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/democfg.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/garble_tx25.py` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/garble_tx25.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/lijst_van_sectoren_liste_des_secteurs.csv` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/lijst_van_sectoren_liste_des_secteurs.csv`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/purposes.py` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/purposes.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/sectors.py` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/sectors.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/tx25_1107.xml` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/tx25_1107.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/tx25_1358.xml` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/tx25_1358.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/tx25_1373.xml` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/fixtures/tx25_1373.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/management/commands/cbss_validate_request.py` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/management/commands/cbss_validate_request.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/mixins.py` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/mixins.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/tx25.py` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/tx25.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/ui.py` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/ui.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cbss/utils.py` & `lino-welfare-23.8.0/lino_welfare/modlib/cbss/utils.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/client_vouchers/__init__.py` & `lino-welfare-23.8.0/lino_welfare/modlib/client_vouchers/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/client_vouchers/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/client_vouchers/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,21 +66,21 @@
 
     def get_wanted_movements(self):
         sums_dict = self.get_vat_sums()
         #~ logger.info("20120901 get_wanted_movements %s",sums_dict)
         sum = Decimal()
         for acc, m in sums_dict.items():
             if m:
-                yield self.create_movement(
+                yield self.create_ledger_movement(
                     None, acc, not self.journal.dc, m)
                 sum += m
 
         acc = self.get_trade_type().get_main_account()
         if acc is not None:
-            yield self.create_movement(
+            yield self.create_ledger_movement(
                 None, acc, self.journal.dc, sum,
                 partner=self.partner,
                 project=self.project,
                 match=self.match)
 
     def full_clean(self, *args, **kw):
         self.compute_totals()
```

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/client_vouchers/ui.py` & `lino-welfare-23.8.0/lino_welfare/modlib/client_vouchers/ui.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/contacts/__init__.py` & `lino-welfare-23.8.0/lino_welfare/modlib/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/contacts/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/contacts/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cv/fixtures/demo.py` & `lino-welfare-23.8.0/lino_welfare/modlib/cv/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cv/fixtures/props.py` & `lino-welfare-23.8.0/lino_welfare/modlib/cv/fixtures/props.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/cv/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/cv/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/debts/__init__.py` & `lino-welfare-23.8.0/lino_welfare/modlib/debts/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/debts/choicelists.py` & `lino-welfare-23.8.0/lino_welfare/modlib/debts/choicelists.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/debts/config/debts/Budget/Default.odt` & `lino-welfare-23.8.0/lino_welfare/modlib/debts/config/debts/Budget/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/debts/config/debts/Budget/Default_2.odt` & `lino-welfare-23.8.0/lino_welfare/modlib/debts/config/debts/Budget/Default_2.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/debts/config/debts/Budget/Default_new.odt` & `lino-welfare-23.8.0/lino_welfare/modlib/debts/config/debts/Budget/Default_new.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/debts/fields.py` & `lino-welfare-23.8.0/lino_welfare/modlib/debts/fields.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/debts/fixtures/demo.py` & `lino-welfare-23.8.0/lino_welfare/modlib/debts/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/debts/fixtures/minimal.py` & `lino-welfare-23.8.0/lino_welfare/modlib/debts/fixtures/minimal.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/debts/fixtures/std.py` & `lino-welfare-23.8.0/lino_welfare/modlib/debts/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/debts/mixins.py` & `lino-welfare-23.8.0/lino_welfare/modlib/debts/mixins.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/debts/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/debts/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/debts/ui.py` & `lino-welfare-23.8.0/lino_welfare/modlib/debts/ui.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/dupable_clients/__init__.py` & `lino-welfare-23.8.0/lino_welfare/modlib/dupable_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/dupable_clients/mixins.py` & `lino-welfare-23.8.0/lino_welfare/modlib/dupable_clients/mixins.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/dupable_clients/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/dupable_clients/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/esf/__init__.py` & `lino-welfare-23.8.0/lino_welfare/modlib/esf/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/esf/choicelists.py` & `lino-welfare-23.8.0/lino_welfare/modlib/esf/choicelists.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/esf/config/esf/Client/esf_file.weasy.html` & `lino-welfare-23.8.0/lino_welfare/modlib/esf/config/esf/Client/esf_file.weasy.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/esf/config/esf/ClientSummary/base.weasy.html` & `lino-welfare-23.8.0/lino_welfare/modlib/esf/config/esf/ClientSummary/base.weasy.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/esf/config/esf/ClientSummary/default.weasy.html` & `lino-welfare-23.8.0/lino_welfare/modlib/esf/config/esf/ClientSummary/default.weasy.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/esf/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/esf/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/finan/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/finan/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/households/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/households/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/immersion/__init__.py` & `lino-welfare-23.8.0/lino_welfare/modlib/immersion/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/immersion/config/immersion/Contract/StageForem.odt` & `lino-welfare-23.8.0/lino_welfare/modlib/immersion/config/immersion/Contract/StageForem.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/immersion/config/immersion/Contract/immersion.body.html` & `lino-welfare-23.8.0/lino_welfare/modlib/immersion/config/immersion/Contract/immersion.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/immersion/fixtures/std.py` & `lino-welfare-23.8.0/lino_welfare/modlib/immersion/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/immersion/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/immersion/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/immersion/ui.py` & `lino-welfare-23.8.0/lino_welfare/modlib/immersion/ui.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/integ/__init__.py` & `lino-welfare-23.8.0/lino_welfare/modlib/integ/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/integ/fixtures/demo.py` & `lino-welfare-23.8.0/lino_welfare/modlib/integ/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/integ/fixtures/std.py` & `lino-welfare-23.8.0/lino_welfare/modlib/integ/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/integ/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/integ/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/isip/choicelists.py` & `lino-welfare-23.8.0/lino_welfare/modlib/isip/choicelists.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/isip/config/isip/Contract/Default.odt` & `lino-welfare-23.8.0/lino_welfare/modlib/isip/config/isip/Contract/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/isip/mixins.py` & `lino-welfare-23.8.0/lino_welfare/modlib/isip/mixins.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/isip/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/isip/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/jobs/__init__.py` & `lino-welfare-23.8.0/lino_welfare/modlib/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/jobs/config/jobs/Contract/Default.odt` & `lino-welfare-23.8.0/lino_welfare/modlib/jobs/config/jobs/Contract/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/jobs/config/jobs/ContractsSituation/Default.odt` & `lino-welfare-23.8.0/lino_welfare/modlib/jobs/config/jobs/ContractsSituation/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/jobs/config/jobs/OldJobsOverview/Default.odt` & `lino-welfare-23.8.0/lino_welfare/modlib/jobs/config/jobs/OldJobsOverview/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/jobs/fixtures/std.py` & `lino-welfare-23.8.0/lino_welfare/modlib/jobs/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/jobs/mixins.py` & `lino-welfare-23.8.0/lino_welfare/modlib/jobs/mixins.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/jobs/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/jobs/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,16 +57,14 @@
         # skip the is_imported_partner test
         return super(contacts.Partner, self).disable_delete(ar)
 
 if dd.get_plugin_setting('jobs', 'with_employer_model'):
 
     class Employer(contacts.Company):
 
-        # TODO: Rename this to `JobSupplier`?
-
         class Meta:
             app_label = 'jobs'
             verbose_name = _("Employer")
             verbose_name_plural = _('Employers')
 
         is_social = models.BooleanField(_("Social economy"), default=False)
```

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/jobs/ui.py` & `lino-welfare-23.8.0/lino_welfare/modlib/jobs/ui.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/ledger/fixtures/demo.py` & `lino-welfare-23.8.0/lino_welfare/modlib/ledger/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/ledger/fixtures/std.py` & `lino-welfare-23.8.0/lino_welfare/modlib/ledger/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/ledger/fixtures/std_journals.py` & `lino-welfare-23.8.0/lino_welfare/modlib/ledger/fixtures/std_journals.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/ledger/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/ledger/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/newcomers/__init__.py` & `lino-welfare-23.8.0/lino_welfare/modlib/newcomers/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/newcomers/fixtures/demo.py` & `lino-welfare-23.8.0/lino_welfare/modlib/newcomers/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/newcomers/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/newcomers/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/notes/fixtures/demo.py` & `lino-welfare-23.8.0/lino_welfare/modlib/notes/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/notes/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/notes/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/pcsw/__init__.py` & `lino-welfare-23.8.0/lino_welfare/modlib/pcsw/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/pcsw/actions.py` & `lino-welfare-23.8.0/lino_welfare/modlib/pcsw/actions.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/pcsw/choicelists.py` & `lino-welfare-23.8.0/lino_welfare/modlib/pcsw/choicelists.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/pcsw/config/pcsw/Client/cv.odt` & `lino-welfare-23.8.0/lino_welfare/modlib/pcsw/config/pcsw/Client/cv.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/pcsw/config/pcsw/Client/eid-content.odt` & `lino-welfare-23.8.0/lino_welfare/modlib/pcsw/config/pcsw/Client/eid-content.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/pcsw/config/pcsw/Client/file_sheet.odt` & `lino-welfare-23.8.0/lino_welfare/modlib/pcsw/config/pcsw/Client/file_sheet.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/pcsw/fixtures/demo2.py` & `lino-welfare-23.8.0/lino_welfare/modlib/pcsw/fixtures/demo2.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/pcsw/fixtures/std.py` & `lino-welfare-23.8.0/lino_welfare/modlib/pcsw/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/pcsw/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/pcsw/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/polls/fixtures/demo.py` & `lino-welfare-23.8.0/lino_welfare/modlib/polls/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/projects/__init__.py` & `lino-welfare-23.8.0/lino_welfare/modlib/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/projects/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/projects/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/reception/__init__.py` & `lino-welfare-23.8.0/lino_welfare/modlib/reception/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/reception/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/reception/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     qs = settings.SITE.user_model.objects.exclude(user_type='')
     kw.update(calendar__isnull=False)
     qs = qs.filter(*args, **kw)
     return qs
 
 
 class FindDateByClientTable(ButtonsTable):
-    """A :class:`ButtonsTable <lino.core.tables.ButtonsTable>` which shows
+    """A :class:`ButtonsTable <lino.core.tables.ButtonsTable>` that shows
     all users who are candidates responsible of new client
     appointment. Clicking on one of them will open the
     `extensible.CalendarPanel` with appropriate parameters
     (`subst_user` and `current_project`).
 
     """
     master = 'pcsw.Client'
@@ -348,15 +348,15 @@
                     request_kwargs=dict(action_param_values=apv),
                     icon_name=CreateClientVisit.icon_name)
             elems += [btn, ' ']
 
         if client.client_state == ClientStates.coached \
                 or user.newcomer_appointments:
                 # or user.newcomer_quota > 0:
-            if extensible is not None:
+            if dd.plugins.extensible.is_active():
                 sar = extensible.CalendarPanel.request(
                     subst_user=user,
                     current_project=client.pk)
                 elems += [ar.href_to_request(
                     sar, _("Find date"),
                     title=_("Find date"),
                     icon_name=FindDateByClientTable.icon_name), ' ']
```

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/sepa/fixtures/demo.py` & `lino-welfare-23.8.0/lino_welfare/modlib/sepa/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/sepa/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/sepa/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/system/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/system/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/users/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/users/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/users/ui.py` & `lino-welfare-23.8.0/lino_welfare/modlib/users/ui.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/Default.odt` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/excerpts/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/anw.body.html` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/anw.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/aus.body.html` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/aus.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/certificate.body.html` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/certificate.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/summary.body.html` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/summary.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/base.body.html` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/excerpts/base.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/integ/ActivityReport/Default.odt` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/integ/ActivityReport/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/letter_margin_bottom.html` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/letter_margin_bottom.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/notes/Note/Letter.odt` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/config/notes/Note/Letter.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/fixtures/demo.py` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/fixtures/demo2.py` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/fixtures/demo2.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/fixtures/pp2lino.py` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/fixtures/pp2lino.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/fixtures/std.py` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/fixtures/std2.py` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/fixtures/std2.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/help_texts.py` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/help_texts.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/django.mo` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/django.po` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/django.mo` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,20 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: lino_welfare\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2022-11-22 10:25+0100\n"
+"PO-Revision-Date: 2023-08-04 21:10+0300\n"
 "Last-Translator: Luc Saffre <luc.saffre@gmail.com>\n"
 "Language-Team: fr <info@lino-framework.org>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n>1;\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 "X-Generator: Poedit 3.0.1\n"
 
 msgid " and "
 msgstr " et "
 
 msgid " born "
 msgstr " né(e) "
@@ -908,18 +908,18 @@
 msgid "Integration"
 msgstr "Intégration"
 
 msgid "Integration Clients"
 msgstr "Bénéficiares (SI)"
 
 msgid "Integration Phase"
-msgstr "Phase d'intégration"
+msgstr "Phase d'insertion"
 
 msgid "Integration Phases"
-msgstr "Phases d'intégration"
+msgstr "Phases d'insertion"
 
 msgid "Integration agent"
 msgstr "Agent d'insertion"
 
 msgid "Integration agent (Flexible)"
 msgstr "Agent d'insertion (Flexible)"
 
@@ -1150,17 +1150,14 @@
 
 msgid "Newcomers consultant"
 msgstr "Consultant nouveaux bénéficiaires"
 
 msgid "Observed events"
 msgstr "Critère"
 
-msgid "Obstacles Property Group"
-msgstr "Groupe de propriétés 'Freins'"
-
 msgid "Occupations"
 msgstr "Occupations"
 
 msgid "Once after 10 days"
 msgstr "Une fois après 10 jours"
 
 msgid "Only active clients"
@@ -1489,17 +1486,14 @@
 
 msgid "Simple confirmations"
 msgstr "Confirmations simple"
 
 msgid "Since"
 msgstr "Depuis"
 
-msgid "Skills Property Group"
-msgstr "Groupe de propriétés 'Skills'"
-
 msgid "Social Welfare Centre"
 msgstr "CPAS"
 
 msgid "Social agent"
 msgstr "Agent social"
 
 msgid "Social agent (Flexible)"
@@ -1507,17 +1501,14 @@
 
 msgid "Social agent (Manager)"
 msgstr "Agent social (Chef de service)"
 
 msgid "Social economy"
 msgstr "Économie sociale"
 
-msgid "Soft Skills Property Group"
-msgstr "Groupe de propriétés 'Soft Skills'"
-
 msgid "Sozialhilfe"
 msgstr "Aide sociale"
 
 msgid "Special Infos"
 msgstr "Information complémentaire"
 
 msgid "Special Retirement Certificates"
```

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/django.po` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 # Copyright (C) 2016 ORGANIZATION
 # This file is distributed under the same license as the lino-welfare
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2016.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version:  lino_welfare\n"
+"Project-Id-Version: lino_welfare\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-04-01 18:26+0200\n"
-"PO-Revision-Date: 2022-11-22 10:25+0100\n"
+"PO-Revision-Date: 2023-08-04 21:10+0300\n"
 "Last-Translator: Luc Saffre <luc.saffre@gmail.com>\n"
-"Language: fr\n"
 "Language-Team: fr <info@lino-framework.org>\n"
-"Plural-Forms: nplurals=2; plural=n>1;\n"
+"Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=n>1;\n"
 "Generated-By: Babel 2.12.1\n"
+"X-Generator: Poedit 3.0.1\n"
 
 #: lino_welfare/modlib/active_job_search/__init__.py:19
 msgid "Active Job Search"
 msgstr "Recherche active d'emploi"
 
 #: lino_welfare/modlib/active_job_search/__init__.py:20
 msgid "AJS"
@@ -32,21 +33,21 @@
 msgstr "Preuve de recherche"
 
 #: lino_welfare/modlib/active_job_search/models.py:24
 msgid "Proofs of search"
 msgstr "Preuves de recherche"
 
 #: lino_welfare/modlib/active_job_search/models.py:28
-#: lino_welfare/modlib/badges/models.py:45
-#: lino_welfare/modlib/cal/models.py:357 lino_welfare/modlib/cbss/tx25.py:316
-#: lino_welfare/modlib/cbss/tx25.py:363 lino_welfare/modlib/cbss/tx25.py:372
-#: lino_welfare/modlib/cbss/tx25.py:384 lino_welfare/modlib/cbss/tx25.py:475
-#: lino_welfare/modlib/cbss/tx25.py:487 lino_welfare/modlib/debts/models.py:108
-#: lino_welfare/modlib/isip/models.py:365 lino_welfare/modlib/jobs/ui.py:427
-#: lino_welfare/modlib/jobs/ui.py:548 lino_welfare/modlib/pcsw/models.py:1004
+#: lino_welfare/modlib/badges/models.py:45 lino_welfare/modlib/cal/models.py:357
+#: lino_welfare/modlib/cbss/tx25.py:316 lino_welfare/modlib/cbss/tx25.py:363
+#: lino_welfare/modlib/cbss/tx25.py:372 lino_welfare/modlib/cbss/tx25.py:384
+#: lino_welfare/modlib/cbss/tx25.py:475 lino_welfare/modlib/cbss/tx25.py:487
+#: lino_welfare/modlib/debts/models.py:108 lino_welfare/modlib/isip/models.py:365
+#: lino_welfare/modlib/jobs/ui.py:427 lino_welfare/modlib/jobs/ui.py:548
+#: lino_welfare/modlib/pcsw/models.py:1004
 msgid "Date"
 msgstr ""
 
 #: lino_welfare/modlib/active_job_search/models.py:30
 msgid "Spontaneous"
 msgstr "Spontanée"
 
@@ -72,16 +73,15 @@
 msgstr "Garde d'enfant"
 
 #: lino_welfare/modlib/active_job_search/models.py:75
 msgid "Notes concerning child custody."
 msgstr ""
 
 #: lino_welfare/modlib/aids/__init__.py:14
-#: lino_welfare/modlib/ledger/models.py:54
-#: lino_welfare/modlib/pcsw/models.py:508
+#: lino_welfare/modlib/ledger/models.py:54 lino_welfare/modlib/pcsw/models.py:508
 msgid "Aids"
 msgstr "Aides"
 
 #: lino_welfare/modlib/aids/choicelists.py:50
 msgid "Aid confirmation type"
 msgstr "Type de confirmation d'aide"
 
@@ -144,57 +144,49 @@
 msgstr "Révoquer"
 
 #: lino_welfare/modlib/aids/mixins.py:97
 #, python-format
 msgid "You revoke your confirmation that %(client)s %(text)s"
 msgstr "Vous annullez votre confirmation que %(client)s %(text)s"
 
-#: lino_welfare/modlib/aids/mixins.py:111
-#: lino_welfare/modlib/aids/mixins.py:137
+#: lino_welfare/modlib/aids/mixins.py:111 lino_welfare/modlib/aids/mixins.py:137
 msgctxt "aids"
 msgid "Signer"
 msgstr "Signataire"
 
 #: lino_welfare/modlib/aids/mixins.py:181
 #, python-format
 msgid "receives %(what)s %(when)s."
 msgstr "béneficie d'une aide %(what)s %(when)s."
 
-#: lino_welfare/modlib/aids/mixins.py:213
-#: lino_welfare/modlib/badges/models.py:50 lino_welfare/modlib/cv/models.py:46
-#: lino_welfare/modlib/debts/models.py:397
+#: lino_welfare/modlib/aids/mixins.py:213 lino_welfare/modlib/badges/models.py:50
+#: lino_welfare/modlib/cv/models.py:46 lino_welfare/modlib/debts/models.py:397
 #: lino_welfare/modlib/debts/models.py:437 lino_welfare/modlib/esf/models.py:37
 #: lino_welfare/modlib/immersion/models.py:100
 #: lino_welfare/modlib/jobs/mixins.py:44 lino_welfare/modlib/jobs/models.py:236
-#: lino_welfare/modlib/jobs/models.py:266
-#: lino_welfare/modlib/jobs/models.py:336
-#: lino_welfare/modlib/jobs/models.py:406
-#: lino_welfare/modlib/pcsw/actions.py:40
-#: lino_welfare/modlib/pcsw/models.py:908
-#: lino_welfare/modlib/pcsw/models.py:969
+#: lino_welfare/modlib/jobs/models.py:266 lino_welfare/modlib/jobs/models.py:336
+#: lino_welfare/modlib/jobs/models.py:406 lino_welfare/modlib/pcsw/actions.py:40
+#: lino_welfare/modlib/pcsw/models.py:908 lino_welfare/modlib/pcsw/models.py:969
 #: lino_welfare/modlib/projects/models.py:44
 #: lino_welfare/modlib/xcourses/models.py:186
 #: lino_welfare/modlib/xcourses/models.py:363
 msgid "Remark"
 msgstr "Remarque"
 
 #: lino_welfare/modlib/aids/mixins.py:245
 #, python-format
 msgid "Date range %(p1)s lies outside of granted period %(p2)s."
 msgstr "Période %(p1)s hors de la période d'ocroi %(p2)s."
 
-#: lino_welfare/modlib/aids/mixins.py:317
-#: lino_welfare/modlib/cbss/models.py:279
+#: lino_welfare/modlib/aids/mixins.py:317 lino_welfare/modlib/cbss/models.py:279
 msgid "Period from"
 msgstr "Période du"
 
-#: lino_welfare/modlib/aids/mixins.py:319
-#: lino_welfare/modlib/aids/models.py:210
-#: lino_welfare/modlib/pcsw/models.py:914
-#: lino_welfare/modlib/pcsw/models.py:968
+#: lino_welfare/modlib/aids/mixins.py:319 lino_welfare/modlib/aids/models.py:210
+#: lino_welfare/modlib/pcsw/models.py:914 lino_welfare/modlib/pcsw/models.py:968
 msgid "until"
 msgstr "jusque"
 
 #: lino_welfare/modlib/aids/mixins.py:322
 msgid "Recipient (Organization)"
 msgstr "Destinataire (Organisation)"
 
@@ -234,16 +226,16 @@
 #: lino_welfare/modlib/aids/models.py:72
 #, fuzzy
 msgid "Integration duty"
 msgstr "Intégration"
 
 #: lino_welfare/modlib/aids/models.py:73
 msgid ""
-"Whether aid grantings of this type are considered as duty for integration"
-" contract."
+"Whether aid grantings of this type are considered as duty for integration "
+"contract."
 msgstr ""
 
 #: lino_welfare/modlib/aids/models.py:77
 #, fuzzy
 msgid "Urgent"
 msgstr "Budget"
 
@@ -253,22 +245,22 @@
 
 #: lino_welfare/modlib/aids/models.py:82
 msgid "Confirmed by primary coach"
 msgstr "Confirmé par le titulaire"
 
 #: lino_welfare/modlib/aids/models.py:83
 msgid ""
-"Whether grantings for this aid type are to be signed by the client's "
-"primary coach."
+"Whether grantings for this aid type are to be signed by the client's primary "
+"coach."
 msgstr ""
 
 #: lino_welfare/modlib/aids/models.py:90
 msgid ""
-"Which client address to print on confirmations. If this is empty, Lino "
-"will use the primary address."
+"Which client address to print on confirmations. If this is empty, Lino will "
+"use the primary address."
 msgstr ""
 
 #: lino_welfare/modlib/aids/models.py:95
 msgid "Body template"
 msgstr ""
 
 #: lino_welfare/modlib/aids/models.py:149
@@ -294,21 +286,19 @@
 msgid "Create confirmation"
 msgstr "Créer attestation"
 
 #: lino_welfare/modlib/aids/models.py:207
 msgid "Applies from"
 msgstr "Date de début"
 
-#: lino_welfare/modlib/aids/models.py:238
-#: lino_welfare/modlib/aids/models.py:360
+#: lino_welfare/modlib/aids/models.py:238 lino_welfare/modlib/aids/models.py:360
 msgid "Only rows decided by this board."
 msgstr ""
 
-#: lino_welfare/modlib/aids/models.py:242
-#: lino_welfare/modlib/aids/models.py:369
+#: lino_welfare/modlib/aids/models.py:242 lino_welfare/modlib/aids/models.py:369
 msgid "Only confirmations about this aid type."
 msgstr ""
 
 #: lino_welfare/modlib/aids/models.py:299
 msgid "Grantings to confirm"
 msgstr "Octrois à confirmer"
 
@@ -371,16 +361,15 @@
 #: lino_welfare/modlib/aids/models.py:666
 #, fuzzy
 msgid "Can refund"
 msgstr "Fin de l'accompagnement"
 
 #: lino_welfare/modlib/aids/models.py:667
 msgid ""
-"Whether persons of this type can be used as doctor of a refund "
-"confirmation."
+"Whether persons of this type can be used as doctor of a refund confirmation."
 msgstr ""
 
 #: lino_welfare/modlib/aids/models.py:703
 #, fuzzy
 msgid "Refund confirmation"
 msgstr "Certificat de revenu"
 
@@ -459,26 +448,24 @@
 msgid "Art60 job supplying"
 msgstr "Mise à l'emploi art60"
 
 #: lino_welfare/modlib/art60/models.py:36
 msgid "Art60 job supplyment"
 msgstr "Mise à l'emploi art60§7"
 
-#: lino_welfare/modlib/art60/models.py:50
-#: lino_welfare/modlib/jobs/models.py:118 lino_welfare/modlib/jobs/ui.py:38
+#: lino_welfare/modlib/art60/models.py:50 lino_welfare/modlib/jobs/models.py:118
+#: lino_welfare/modlib/jobs/ui.py:38
 msgid "Art60§7 job supplyment"
 msgstr "Mise à l'emploi art60§7"
 
-#: lino_welfare/modlib/art60/models.py:51
-#: lino_welfare/modlib/jobs/models.py:119
+#: lino_welfare/modlib/art60/models.py:51 lino_welfare/modlib/jobs/models.py:119
 msgid "Art60§7 job supplyments"
 msgstr "Mises à l'emploi art60§7"
 
-#: lino_welfare/modlib/art60/models.py:58
-#: lino_welfare/modlib/art61/models.py:77
+#: lino_welfare/modlib/art60/models.py:58 lino_welfare/modlib/art61/models.py:77
 #: lino_welfare/modlib/jobs/models.py:132
 #, fuzzy
 msgid "Type"
 msgstr "Type d'aide sociale"
 
 #: lino_welfare/modlib/art60/models.py:98
 msgid "Art60§7 convention"
@@ -493,35 +480,30 @@
 msgstr "Date de début"
 
 #: lino_welfare/modlib/art60/models.py:114
 #: lino_welfare/modlib/art60/models.py:222
 msgid "Monthly refund"
 msgstr "Rétrocession mensuelle"
 
-#: lino_welfare/modlib/art60/models.py:115
-#: lino_welfare/modlib/jobs/models.py:141
+#: lino_welfare/modlib/art60/models.py:115 lino_welfare/modlib/jobs/models.py:141
 #: lino_welfare/modlib/jobs/models.py:264
 msgid "hourly rate"
 msgstr "coût horaire"
 
-#: lino_welfare/modlib/art60/models.py:116
-#: lino_welfare/modlib/jobs/models.py:142
+#: lino_welfare/modlib/art60/models.py:116 lino_welfare/modlib/jobs/models.py:142
 msgid "refund rate"
 msgstr "tarif de remboursement"
 
-#: lino_welfare/modlib/art60/models.py:167
-#: lino_welfare/modlib/jobs/models.py:184
+#: lino_welfare/modlib/art60/models.py:167 lino_welfare/modlib/jobs/models.py:184
 #, python-format
 msgid "(%d candidatures have been marked inactive)"
 msgstr ""
 
-#: lino_welfare/modlib/art60/models.py:168
-#: lino_welfare/modlib/isip/models.py:116
-#: lino_welfare/modlib/jobs/models.py:185
-#: lino_welfare/modlib/pcsw/actions.py:84
+#: lino_welfare/modlib/art60/models.py:168 lino_welfare/modlib/isip/models.py:116
+#: lino_welfare/modlib/jobs/models.py:185 lino_welfare/modlib/pcsw/actions.py:84
 #: lino_welfare/modlib/pcsw/actions.py:115
 msgid "Success"
 msgstr "Réussi"
 
 #: lino_welfare/modlib/art60/models.py:225 lino_welfare/modlib/jobs/ui.py:171
 msgid "Only contracts of type"
 msgstr "Uniquement contrats de type"
@@ -567,16 +549,15 @@
 msgid "Tutorate"
 msgstr "Tutorat"
 
 #: lino_welfare/modlib/art61/choicelists.py:48
 msgid "Walloon Region"
 msgstr "Région Wallonne"
 
-#: lino_welfare/modlib/art61/models.py:30
-#: lino_welfare/modlib/art61/models.py:66
+#: lino_welfare/modlib/art61/models.py:30 lino_welfare/modlib/art61/models.py:66
 msgid "Art61 job supplyment"
 msgstr "Mise à l'emploi art.61"
 
 #: lino_welfare/modlib/art61/models.py:48
 msgid "Art61 job supplyment type"
 msgstr "Type de mise à l'emploi art.61"
 
@@ -617,16 +598,15 @@
 msgid "Badge Awards"
 msgstr "Tests de niveau"
 
 #: lino_welfare/modlib/badges/models.py:42
 msgid "Holder"
 msgstr ""
 
-#: lino_welfare/modlib/badges/models.py:47
-#: lino_welfare/modlib/cbss/mixins.py:286
+#: lino_welfare/modlib/badges/models.py:47 lino_welfare/modlib/cbss/mixins.py:286
 #: lino_welfare/modlib/projects/models.py:45
 msgid "Result"
 msgstr "Résultat"
 
 #: lino_welfare/modlib/badges/models.py:60
 #: lino_welfare/modlib/badges/models.py:68
 msgid "Awards"
@@ -695,17 +675,16 @@
 msgid "Notes"
 msgstr ""
 
 #: lino_welfare/modlib/cal/models.py:334
 #: lino_welfare/modlib/client_vouchers/ui.py:38
 #: lino_welfare/modlib/contacts/models.py:118
 #: lino_welfare/modlib/contacts/models.py:204
-#: lino_welfare/modlib/contacts/models.py:294
-#: lino_welfare/modlib/debts/ui.py:125 lino_welfare/modlib/finan/models.py:19
-#: lino_welfare/modlib/isip/models.py:253
+#: lino_welfare/modlib/contacts/models.py:294 lino_welfare/modlib/debts/ui.py:125
+#: lino_welfare/modlib/finan/models.py:19 lino_welfare/modlib/isip/models.py:253
 #: lino_welfare/modlib/system/models.py:106 lino_welfare/modlib/users/ui.py:23
 #: lino_welfare/modlib/welfare/workflows.py:48
 msgid "General"
 msgstr "Général"
 
 #: lino_welfare/modlib/cal/models.py:338 lino_welfare/modlib/finan/models.py:24
 msgid "More"
@@ -734,16 +713,15 @@
 msgid "Tasks"
 msgstr ""
 
 #: lino_welfare/modlib/cal/models.py:416
 msgid "Delegated to client"
 msgstr "à faire par bénéficiaire"
 
-#: lino_welfare/modlib/cbss/__init__.py:34
-#: lino_welfare/modlib/pcsw/models.py:401
+#: lino_welfare/modlib/cbss/__init__.py:34 lino_welfare/modlib/pcsw/models.py:401
 msgid "CBSS"
 msgstr "BCSS"
 
 #: lino_welfare/modlib/cbss/choicelists.py:20
 #: lino_welfare/modlib/cbss/mixins.py:85
 msgid "Sent"
 msgstr "Exécuté"
@@ -933,16 +911,15 @@
 msgid "Tx25 Request"
 msgstr "Requête Tx25"
 
 #: lino_welfare/modlib/cbss/models.py:407
 msgid "Tx25 Requests"
 msgstr "Requêtes Tx25"
 
-#: lino_welfare/modlib/cbss/models.py:415
-#: lino_welfare/modlib/pcsw/models.py:515
+#: lino_welfare/modlib/cbss/models.py:415 lino_welfare/modlib/pcsw/models.py:515
 msgid "History"
 msgstr "Historique"
 
 #: lino_welfare/modlib/cbss/models.py:558
 msgid "Requesting organisation"
 msgstr ""
 
@@ -1105,16 +1082,15 @@
 
 #: lino_welfare/modlib/cbss/tx25.py:709 lino_welfare/modlib/cbss/tx25.py:751
 msgid "SSIN "
 msgstr "NISS "
 
 #: lino_welfare/modlib/cbss/tx25.py:729
 #: lino_welfare/modlib/immersion/models.py:87
-#: lino_welfare/modlib/isip/models.py:149
-#: lino_welfare/modlib/jobs/models.py:127
+#: lino_welfare/modlib/isip/models.py:149 lino_welfare/modlib/jobs/models.py:127
 msgid "Organization"
 msgstr "Organisation"
 
 #: lino_welfare/modlib/cbss/tx25.py:810 lino_welfare/modlib/isip/models.py:56
 msgid "Reference"
 msgstr "Référence"
 
@@ -1357,16 +1333,15 @@
 msgstr "Permis de conduire"
 
 #: lino_welfare/modlib/cbss/tx25.py:1217
 msgid "Identity Cards"
 msgstr "Cartes d'identité"
 
 #: lino_welfare/modlib/cbss/tx25.py:1233 lino_welfare/modlib/pcsw/models.py:117
-#: lino_welfare/modlib/pcsw/models.py:907
-#: lino_welfare/modlib/pcsw/models.py:963
+#: lino_welfare/modlib/pcsw/models.py:907 lino_welfare/modlib/pcsw/models.py:963
 #: lino_welfare/modlib/reception/models.py:108
 #: lino_welfare/modlib/reception/models.py:136
 msgid "Reason"
 msgstr "Raison"
 
 #: lino_welfare/modlib/cbss/tx25.py:1246
 msgid "Legal cohabitations"
@@ -1441,16 +1416,15 @@
 msgid "Birth location"
 msgstr "Lieu de naissance"
 
 #: lino_welfare/modlib/cbss/ui.py:205
 msgid "Civil state"
 msgstr "Etat civil"
 
-#: lino_welfare/modlib/cbss/ui.py:209
-#: lino_welfare/modlib/xcourses/models.py:612
+#: lino_welfare/modlib/cbss/ui.py:209 lino_welfare/modlib/xcourses/models.py:612
 msgid "Address"
 msgstr "Adresse"
 
 #: lino_welfare/modlib/cbss/ui.py:219 lino_welfare/modlib/cbss/ui.py:239
 msgid "Requested action"
 msgstr "Action demandée"
 
@@ -1697,16 +1671,15 @@
 msgid "Required for Households"
 msgstr "obligatoire pour ménages"
 
 #: lino_welfare/modlib/debts/models.py:78
 msgid "Required for Persons"
 msgstr "obligatoire pour personnes"
 
-#: lino_welfare/modlib/debts/models.py:79
-#: lino_welfare/modlib/debts/models.py:449
+#: lino_welfare/modlib/debts/models.py:79 lino_welfare/modlib/debts/models.py:449
 msgid "Periods"
 msgstr "Périodes"
 
 #: lino_welfare/modlib/debts/models.py:80
 msgid "Default amount"
 msgstr "Montant par défaut"
 
@@ -1854,16 +1827,16 @@
 #: lino_welfare/modlib/debts/models.py:462
 #: lino_welfare/modlib/debts/models.py:576 lino_welfare/modlib/debts/ui.py:473
 msgid "Debt collection agency"
 msgstr ""
 
 #: lino_welfare/modlib/debts/models.py:463
 msgid ""
-"Leave empty for simple debts, otherwise select         here the "
-"responsible bailiff or collection agency"
+"Leave empty for simple debts, otherwise select         here the responsible "
+"bailiff or collection agency"
 msgstr ""
 
 #: lino_welfare/modlib/debts/models.py:529
 msgid "Periods must be > 0"
 msgstr ""
 
 #: lino_welfare/modlib/debts/models.py:533
@@ -1983,16 +1956,15 @@
 msgstr "Répartition au marc-le-franc"
 
 #: lino_welfare/modlib/debts/ui.py:641
 msgid ""
 "Répartition au marc-le-franc.\n"
 "A table with one row per entry in Liabilities which has \"distribute\" "
 "checked,\n"
-"proportionally distributing the `Distributable amount` among the debtors."
-"\n"
+"proportionally distributing the `Distributable amount` among the debtors.\n"
 msgstr ""
 
 #: lino_welfare/modlib/debts/ui.py:679
 msgid "%"
 msgstr ""
 
 #: lino_welfare/modlib/debts/ui.py:683
@@ -2169,16 +2141,15 @@
 msgstr "Répartition au marc-le-franc"
 
 #: lino_welfare/modlib/finan/models.py:59
 #, fuzzy
 msgid "Internal reference"
 msgstr "référence circulaire ?"
 
-#: lino_welfare/modlib/finan/models.py:61
-#: lino_welfare/modlib/finan/models.py:66
+#: lino_welfare/modlib/finan/models.py:61 lino_welfare/modlib/finan/models.py:66
 #, fuzzy
 msgid "External reference"
 msgstr "référence circulaire ?"
 
 #: lino_welfare/modlib/households/models.py:133
 #, python-format
 msgid "%(count)d adult"
@@ -2232,16 +2203,15 @@
 
 #: lino_welfare/modlib/immersion/models.py:99
 #: lino_welfare/modlib/isip/mixins.py:328
 msgid "responsibilities"
 msgstr "responsabilités"
 
 #: lino_welfare/modlib/immersion/models.py:117
-#: lino_welfare/modlib/isip/mixins.py:318
-#: lino_welfare/modlib/isip/mixins.py:416
+#: lino_welfare/modlib/isip/mixins.py:318 lino_welfare/modlib/isip/mixins.py:416
 #: lino_welfare/modlib/isip/models.py:214
 msgid "Responsible (IS)"
 msgstr "Titulaire (SI)"
 
 #: lino_welfare/modlib/immersion/ui.py:99
 msgid "Only immersion trainings of type"
 msgstr "Seulement stages d'immersion de ce type"
@@ -2383,16 +2353,15 @@
 msgstr ""
 
 #: lino_welfare/modlib/integ/models.py:599
 msgid "Activity Report"
 msgstr "Rapport d'activité"
 
 #: lino_welfare/modlib/integ/models.py:606
-#: lino_welfare/modlib/isip/__init__.py:14
-#: lino_welfare/modlib/isip/models.py:183
+#: lino_welfare/modlib/isip/__init__.py:14 lino_welfare/modlib/isip/models.py:183
 #: lino_welfare/modlib/isip/models.py:258
 msgid "ISIP"
 msgstr "PIIS"
 
 #: lino_welfare/modlib/integ/models.py:630
 msgid "Indicateurs généraux"
 msgstr ""
@@ -2578,18 +2547,16 @@
 msgid "Reason of termination"
 msgstr "Motif d'arrêt"
 
 #: lino_welfare/modlib/isip/models.py:111
 msgid "Contract termination reasons"
 msgstr "Motifs d’arrêt de contrat"
 
-#: lino_welfare/modlib/isip/models.py:113
-#: lino_welfare/modlib/jobs/models.py:404
-#: lino_welfare/modlib/pcsw/models.py:827
-#: lino_welfare/modlib/pcsw/models.py:1007
+#: lino_welfare/modlib/isip/models.py:113 lino_welfare/modlib/jobs/models.py:404
+#: lino_welfare/modlib/pcsw/models.py:827 lino_welfare/modlib/pcsw/models.py:1007
 msgid "Designation"
 msgstr "Désignation"
 
 #: lino_welfare/modlib/isip/models.py:118
 #, fuzzy
 msgid "Require date ended"
 msgstr "Date de fin"
@@ -2606,16 +2573,15 @@
 msgid "duties company"
 msgstr "Obligations de l'entreprise"
 
 #: lino_welfare/modlib/isip/models.py:184
 msgid "ISIPs"
 msgstr "PIISs"
 
-#: lino_welfare/modlib/isip/models.py:189
-#: lino_welfare/modlib/jobs/models.py:263
+#: lino_welfare/modlib/isip/models.py:189 lino_welfare/modlib/jobs/models.py:263
 msgid "Contract Type"
 msgstr "Type de contrat"
 
 #: lino_welfare/modlib/isip/models.py:194
 msgid "stages"
 msgstr "stages"
 
@@ -2637,16 +2603,16 @@
 
 #: lino_welfare/modlib/isip/models.py:209
 msgid "duties person"
 msgstr "Obligations du bénéficiaire"
 
 #: lino_welfare/modlib/isip/models.py:238
 msgid ""
-"Cannot print {} because there is no active aid confirmation and Duties "
-"(PCSW) is empty."
+"Cannot print {} because there is no active aid confirmation and Duties (PCSW) "
+"is empty."
 msgstr ""
 
 #: lino_welfare/modlib/isip/models.py:354
 msgid "Proceedings"
 msgstr "Démarches"
 
 #: lino_welfare/modlib/jobs/__init__.py:18
@@ -2733,16 +2699,15 @@
 msgid "Job Offer"
 msgstr "Offre d'emploi"
 
 #: lino_welfare/modlib/jobs/models.py:217
 msgid "Job Offers"
 msgstr "Offres d'emploi"
 
-#: lino_welfare/modlib/jobs/models.py:222
-#: lino_welfare/modlib/jobs/models.py:258
+#: lino_welfare/modlib/jobs/models.py:222 lino_welfare/modlib/jobs/models.py:258
 #: lino_welfare/modlib/xcourses/models.py:78
 #: lino_welfare/modlib/xcourses/models.py:108
 #: lino_welfare/modlib/xcourses/models.py:179
 msgid "Name"
 msgstr ""
 
 #: lino_welfare/modlib/jobs/models.py:227
@@ -2763,16 +2728,15 @@
 msgstr "Poste de travail"
 
 #: lino_welfare/modlib/jobs/models.py:255 lino_welfare/modlib/jobs/ui.py:83
 #: lino_welfare/modlib/jobs/ui.py:101
 msgid "Jobs"
 msgstr "Postes de travail"
 
-#: lino_welfare/modlib/jobs/models.py:259
-#: lino_welfare/modlib/jobs/models.py:399
+#: lino_welfare/modlib/jobs/models.py:259 lino_welfare/modlib/jobs/models.py:399
 msgid "Job Type"
 msgstr "Type de poste"
 
 #: lino_welfare/modlib/jobs/models.py:265
 msgid "capacity"
 msgstr "Capacité"
 
@@ -3361,19 +3325,19 @@
 
 #: lino_welfare/modlib/pcsw/models.py:829
 msgid "Considered active"
 msgstr "Considéré actif"
 
 #: lino_welfare/modlib/pcsw/models.py:834
 msgid "Integration Phase"
-msgstr "Phase d'intégration"
+msgstr "Phase d'insertion"
 
 #: lino_welfare/modlib/pcsw/models.py:835
 msgid "Integration Phases"
-msgstr "Phases d'intégration"
+msgstr "Phases d'insertion"
 
 #: lino_welfare/modlib/pcsw/models.py:842
 msgid "Liste des phases d'intégration possibles."
 msgstr ""
 
 #: lino_welfare/modlib/pcsw/models.py:857
 msgid "activity"
@@ -3683,18 +3647,16 @@
 #: lino_welfare/modlib/welfare/help_texts.py:7
 msgid "The plugin."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:8
 msgid ""
 "Optionally specify the primary key (an integer) of the last granting for\n"
-"which you want to deactivate date range validation in confirmations.  "
-"This\n"
-"is useful for keeping legacy confirmations that have been issued before "
-"the\n"
+"which you want to deactivate date range validation in confirmations.  This\n"
+"is useful for keeping legacy confirmations that have been issued before the\n"
 "rule was activated."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:12
 #: lino_welfare/modlib/welfare/help_texts.py:15
 #: lino_welfare/modlib/welfare/help_texts.py:76
 #: lino_welfare/modlib/welfare/help_texts.py:84
@@ -3831,16 +3793,15 @@
 "requests."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:60
 msgid ""
 "Validates the generated XML against the XSD files.\n"
 "Used by test suite.\n"
-"It is not necessary to validate each real request before actually sending"
-" it."
+"It is not necessary to validate each real request before actually sending it."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:63
 msgid "SSDN specific part of a request."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:64
@@ -4259,16 +4220,15 @@
 
 #: lino_welfare/modlib/welfare/help_texts.py:204
 msgid "Count a fixed time for each presence."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:205
 msgid ""
-"Shows the members of the primary household of this person together with "
-"an\n"
+"Shows the members of the primary household of this person together with an\n"
 "amount which depends on whether that member is adult or not."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:207
 msgid ""
 "The amount to refund for children (household members less than\n"
 "lino_xl.lib.households.Plugin.adult_age years old)."
@@ -4662,16 +4622,15 @@
 
 #: lino_welfare/modlib/welfare/models.py:71
 msgid "usable in contracts"
 msgstr "utilisable dans contrats"
 
 #: lino_welfare/modlib/welfare/models.py:73
 msgid ""
-"Whether Links of this type can be used as contact person of a job "
-"contract."
+"Whether Links of this type can be used as contact person of a job contract."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/user_types.py:173
 msgid "Anonymous"
 msgstr "Anonyme"
 
 #: lino_welfare/modlib/welfare/user_types.py:175
@@ -5105,34 +5064,12 @@
 
 #~ msgid "(SiteConfig %s is empty)"
 #~ msgstr "(les paramètres de site %s sont vides)"
 
 #~ msgid "Skills Property Group"
 #~ msgstr "Groupe de propriétés 'Skills'"
 
-#~ msgid "The property group to be used as master for the SkillsByPerson table."
-#~ msgstr ""
-
 #~ msgid "Soft Skills Property Group"
 #~ msgstr "Groupe de propriétés 'Soft Skills'"
 
-#~ msgid ""
-#~ "The property group to be used as"
-#~ " master for the SoftSkillsByPerson table."
-#~ msgstr ""
-
 #~ msgid "Obstacles Property Group"
 #~ msgstr "Groupe de propriétés 'Freins'"
-
-#~ msgid ""
-#~ "The property group to be used as"
-#~ " master for the ObstaclesByPerson table."
-#~ msgstr ""
-
-#~ msgid "Django model used to represent a debts mediation budget."
-#~ msgstr ""
-
-#~ msgid ""
-#~ "An actor of a budget is a partner who is part of the household\n"
-#~ "for which the budget has been established."
-#~ msgstr ""
-
```

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/nl/LC_MESSAGES/django.po` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/commands/cpas2lino.py` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/management/commands/cpas2lino.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/commands/garble.py` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/management/commands/garble.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/commands/gd2lino.py` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/management/commands/gd2lino.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/commands/initdb_tim.py` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/management/commands/initdb_tim.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/commands/watch_tim.py` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/management/commands/watch_tim.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/settings.py` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/settings.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/user_types.py` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/user_types.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/welfare/workflows.py` & `lino-welfare-23.8.0/lino_welfare/modlib/welfare/workflows.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/xcourses/__init__.py` & `lino-welfare-23.8.0/lino_welfare/modlib/xcourses/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/xcourses/config/courses/Course/candidates.odt` & `lino-welfare-23.8.0/lino_welfare/modlib/xcourses/config/courses/Course/candidates.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/xcourses/config/courses/Course/participants.odt` & `lino-welfare-23.8.0/lino_welfare/modlib/xcourses/config/courses/Course/participants.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/xcourses/fixtures/demo.py` & `lino-welfare-23.8.0/lino_welfare/modlib/xcourses/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/modlib/xcourses/models.py` & `lino-welfare-23.8.0/lino_welfare/modlib/xcourses/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/projects/gerd/print_tx25.py` & `lino-welfare-23.8.0/lino_welfare/projects/gerd/print_tx25.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/demo.py` & `lino-welfare-23.8.0/lino_welfare/projects/gerd/settings/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/media/beid/123456789012.jpg` & `lino-welfare-23.8.0/lino_welfare/projects/gerd/settings/media/beid/123456789012.jpg`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/media/beid/591413288107.jpg` & `lino-welfare-23.8.0/lino_welfare/projects/gerd/settings/media/beid/591413288107.jpg`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/mysql.py` & `lino-welfare-23.8.0/lino_welfare/projects/gerd/settings/mysql.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/test_aids.py` & `lino-welfare-23.8.0/lino_welfare/projects/gerd/tests/test_aids.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/test_broken_gfks.py` & `lino-welfare-23.8.0/lino_welfare/projects/gerd/tests/test_broken_gfks.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/test_cbss.py` & `lino-welfare-23.8.0/lino_welfare/projects/gerd/tests/test_cbss.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/test_clients.py` & `lino-welfare-23.8.0/lino_welfare/projects/gerd/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/test_debts.py` & `lino-welfare-23.8.0/lino_welfare/projects/gerd/tests/test_debts.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/test_watchtim.py` & `lino-welfare-23.8.0/lino_welfare/projects/gerd/tests/test_watchtim.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 # -*- coding: UTF-8 -*-
-# Copyright 2013-2017 Rumma & Ko Ltd
+# Copyright 2013-2023 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
 """This module contains tests for the :mod:`watch_tim
 <lino_welfare.management.commands.watch_tim>` command.
 
 You can run only these tests by issuing::
 
-  $ cd lino_welfare/projects/eupen
+  $ go gerd
   $ python manage.py test tests.test_watchtim
-  
+
 The module contains a single huge test case because we don't want
 Django to recreate a virgin test database for each of them.
 
 """
 
-from __future__ import unicode_literals
-
-from builtins import str
-import logging
-logger = logging.getLogger(__name__)
+import logging ; logger = logging.getLogger(__name__)
 
 from django.conf import settings
 from django.core.exceptions import ValidationError
 from django.utils import translation
 
 from lino.api import dd, rt
 from lino.utils import i2d
@@ -143,29 +139,29 @@
         georges = Client.objects.get(id=23633)
         self.assertEqual(georges.first_name, "Georges")
 
         ar = rt.models.changes.ChangesByMaster.request(georges)
         self.assertEqual(ar.get_total_count(), 0)
 
         # Company becomes Client
-        
+
         # ValidationError([u'A Partner cannot be parent for a Client']) (201302-22 12:42:07)
 
         # A Partner in TIM has both `PAR->NoTva` nonempty and
         # `PARATTR_N` set.  It currently exists in Lino as a Company but
         # not as a Client.  `watch_tim` then must create a Client after
         # creating also the intermediate Person.  The Company child must
         # be removed.
 
         obj = Company(name="Müller Max Moritz", id=5088)
         obj.save()
 
         ar = rt.models.changes.ChangesByMaster.request(obj)
         self.assertEqual(ar.get_total_count(), 0)
-        
+
         global PUT_MAX_MORITZ
         process_line(PUT_MAX_MORITZ)
         self.assertDoesNotExist(Company, id=5088)
         # ~ company = Company.objects.get(id=5088) # has not been deleted
         person = Person.objects.get(id=5088)  # has been created
         client = Client.objects.get(id=5088)  # has been created
         # one coaching has been created
@@ -184,15 +180,15 @@
         process_line(PUT_MAX_MORITZ)
         #~ company = Company.objects.get(id=5088)
         self.assertDoesNotExist(Client, id=5088)  # has been deleted
         self.assertDoesNotExist(Coaching, client_id=5088)
 
         #~ def test03(self):
         """
-        Test whether watch_tim raises Exception 
+        Test whether watch_tim raises Exception
         'Cannot create Client ... from PXS' when necessary.
         """
         self.assertDoesNotExist(Client, id=23635)
         try:
             process_line(POST_PXS)
             self.fail("Expected an exception")
         except Exception as e:
@@ -215,26 +211,26 @@
         self.assertEqual(coaching.user.username, 'alicia')
         self.assertEqual(coaching.start_date, i2d(19850723))
         with translation.override('en'):
             s = changes_to_rst(client.partner_ptr)
         # print s
         self.assertEqual(s, """\
 =========== ============= ==================================== ============================================================================= ============= ===========
- User        Change Type   Object                               Changes                                                                       Object type   object id
+ Author      Change Type   Object                               Changes                                                                       Object type   object id
 ----------- ------------- ------------------------------------ ----------------------------------------------------------------------------- ------------- -----------
  watch_tim   Create        *alicia / Voldemort-Potter H*        Coaching(id=2,start_date=1985-07-23,user=2,client=4260,type=2,primary=True)   Coaching      2
  watch_tim   Add child     *Eheleute Harald VOLDEMORT-POTTER*   pcsw.Client                                                                   Person        4260
  watch_tim   Add child     *Voldemort-Potter Harald*            contacts.Person                                                               Partner       4260
 =========== ============= ==================================== ============================================================================= ============= ===========
 
 """)
 
         #~ def test05(self):
         """
-        Person becomes Household 
+        Person becomes Household
         """
         Person(id=6283, first_name="Paul",
                last_name="Willekens-Delanuit").save()
         process_line(PUT_PAR_6283)
         household = Household.objects.get(id=6283)  # has been created
         self.assertDoesNotExist(Person, id=6283)
 
@@ -325,15 +321,15 @@
         obj = Company.objects.get(id=5)
         self.assertEqual(obj.name, "Air Liquide Belgium")
         with translation.override('en'):
             s = changes_to_rst(obj.partner_ptr)
         # print s
         self.assertEqual(s, """\
 +-----------+-------------+----------------------------+--------------------------------------------------------+--------------+-----------+
-| User      | Change Type | Object                     | Changes                                                | Object type  | object id |
+| Author    | Change Type | Object                     | Changes                                                | Object type  | object id |
 +===========+=============+============================+========================================================+==============+===========+
 | watch_tim | Update      | *S.A. Air Liquide Belgium* | - activity_id : None --> 19                            | Organization | 5         |
 |           |             |                            | - bank_account1 : None --> 'GKCCBEBB:BE57551373330235' |              |           |
 |           |             |                            | - bank_account2 : None --> 'BBRUBEBB:BE12310110444892' |              |           |
 |           |             |                            | - city_id : None --> 3                                 |              |           |
 |           |             |                            | - country_id : None --> 'B'                            |              |           |
 |           |             |                            | - fax : '' --> '04/341.20.70'                          |              |           |
@@ -360,24 +356,24 @@
         self.assertEqual(obj.name, "Andenne, CPAS")
 
         with translation.override('en'):
             s = changes_to_rst(obj.partner_ptr)
         #~ print s
         self.assertEqual(s, """\
 =========== ============== ================= ================== ============= ===========
- User        Change Type    Object            Changes            Object type   object id
+ Author      Change Type    Object            Changes            Object type   object id
 ----------- -------------- ----------------- ------------------ ------------- -----------
  watch_tim   Add child      *Andenne, CPAS*   contacts.Company   Partner       9932
  watch_tim   Remove child                     contacts.Person    Person        9932
 =========== ============== ================= ================== ============= ===========
 
 """)
 
         """
-        A PAR without NoTVA becomes a Person, but if no first_name can 
+        A PAR without NoTVA becomes a Person, but if no first_name can
         be detected, then it is just a simple partner
         """
         ln = """{"method":"PUT","alias":"PAR","id":"0000001267","time":"20130517 12:34:15",
         "user":"","data":{"IDPAR":"0000001267","FIRME":"Velopa","NAME2":"",
         "RUE":"Leuvenselaan","CP":"3300","IDPRT":"I","PAYS":"B","TEL":"",
         "FAX":"","COMPTE1":"","NOTVA":"","COMPTE3":"","IDPGP":"",
         "DC.debit":"","DC.credit":"","ATTRIB":"","IDMFC":"30","LANGUE":"F","IDBUD":"",
@@ -431,15 +427,15 @@
         "IDUSR":"ALICIA","DOMI1":""}}"""
         process_line(ln)
         self.assertDoesNotExist(Client, id=7826)
 
         """
         20130602 : datum_bis einer primären Begleitung eines Ehemaligen darf
         nicht leer sein. Wenn es das ist, soll watch_tim es auf PAR->DatCrea
-        setzen. 
+        setzen.
         """
         with translation.override('de'):
             self.assertDoesNotExist(Coaching, client_id=7826)
             ln = ln.replace('"NB2":""', '"NB2":"940702 234-24"')
             process_line(ln)
             obj = Client.objects.get(id=7826)
             self.assertEqual(obj.name, "Mustermann Peter")
@@ -467,17 +463,17 @@
 ---------------- ---------- ----------- -------- -------- ------------------
  05.01.06         05.01.06   alicia      Ja       DSBE
 ================ ========== =========== ======== ======== ==================
 
 """)
 
             """
-            20131029 
+            20131029
             Begleitung wird in Lino manuell als nicht primär markiert.
-            Dann wird Kunde in TIM (1) zurück nach S versetzt und (2) 
+            Dann wird Kunde in TIM (1) zurück nach S versetzt und (2)
             von ALICIA zu ROGER.
             """
             coaching = rt.models.coachings.Coaching.objects.get(client=obj, primary=True)
             coaching.primary = False
             coaching.save()
             s = coachings_to_rst(obj)
             #~ print s
@@ -516,15 +512,15 @@
  17.05.13                    roger       Ja       ASD
 ================ ========== =========== ======== ======== ==================
 
 """)
 
         """
         A non-client partner with empty PAR->NoTva will become a Person, not a Company.
-        If the partner is in fact a company whose NoTva has just been forgotten, 
+        If the partner is in fact a company whose NoTva has just been forgotten,
         then watch_tim will raise a ValidationError:
         """
         ln = """{"method":"POST","alias":"PAR","id":"0000087683","time":"20130610 11:26:30",
         "user":"ROGER","data":{"IDPAR":"0000087683","FIRME":"Bellavilla","NAME2":"","RUE":"",
         "CP":"","IDPRT":"V","PAYS":"","TEL":"","FAX":"","COMPTE1":"","NOTVA":"","COMPTE3":"",
         "IDPGP":"","DC.debit":"","DC.credit":"","ATTRIB":"","IDMFC":"30","LANGUE":"D","IDBUD":"",
         "PROF":"00","CODE1":"","CODE2":"","CODE3":"",
```

### Comparing `lino-welfare-23.6.0/lino_welfare/projects/mathieu/settings/demo.py` & `lino-welfare-23.8.0/lino_welfare/projects/mathieu/settings/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/projects/mathieu/settings/media/beid/123456789012.jpg` & `lino-welfare-23.8.0/lino_welfare/projects/mathieu/settings/media/beid/123456789012.jpg`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/projects/mathieu/settings/media/beid/591413288107.jpg` & `lino-welfare-23.8.0/lino_welfare/projects/mathieu/settings/media/beid/591413288107.jpg`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/projects/mathieu/tests/test_chatelet.py` & `lino-welfare-23.8.0/lino_welfare/projects/mathieu/tests/test_chatelet.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/projects/mathieu/tests/test_notify.py` & `lino-welfare-23.8.0/lino_welfare/projects/mathieu/tests/test_notify.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/scripts/load_plp.py` & `lino-welfare-23.8.0/lino_welfare/scripts/load_plp.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/lino_welfare/setup_info.py` & `lino-welfare-23.8.0/lino_welfare/setup_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
             'pytidylib',
             'django-iban', 'metafone',
             'cairocffi']
 requires.append('suds-py3')
 
 SETUP_INFO = dict(
     name='lino-welfare',
-    version='23.6.0',
+    version='23.8.0',
     install_requires=requires,
     test_suite='tests',
     tests_require=['pytest'],
     include_package_data=True,
     zip_safe=False,
     description="A Lino plugin library for Belgian PCSWs",
     long_description="""\
```

### Comparing `lino-welfare-23.6.0/lino_welfare.egg-info/PKG-INFO` & `lino-welfare-23.8.0/lino_welfare.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: lino-welfare
-Version: 23.6.0
+Version: 23.8.0
 Summary: A Lino plugin library for Belgian PCSWs
 Home-page: https://gitlab.com/lino-framework/welfare
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -55,7 +57,9 @@
 - For introductions, commercial information and hosting solutions
   see https://www.saffre-rumma.net
 
 - This is a sustainably free open-source project. Your contributions are
   welcome.  See https://community.lino-framework.org for details.
 
 
+
+
```

### Comparing `lino-welfare-23.6.0/lino_welfare.egg-info/SOURCES.txt` & `lino-welfare-23.8.0/lino_welfare.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -66,18 +66,24 @@
 lino_welfare/modlib/cbss/choicelists.py
 lino_welfare/modlib/cbss/mixins.py
 lino_welfare/modlib/cbss/models.py
 lino_welfare/modlib/cbss/roles.py
 lino_welfare/modlib/cbss/tx25.py
 lino_welfare/modlib/cbss/ui.py
 lino_welfare/modlib/cbss/utils.py
+lino_welfare/modlib/cbss/WSDL/2013HealthCareInsurance.wsdl
 lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v1.wsdl
 lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v2.wsdl
 lino_welfare/modlib/cbss/WSDL/TestConnectionService.wsdl
 lino_welfare/modlib/cbss/WSDL/WebServiceConnector.wsdl
+lino_welfare/modlib/cbss/WSDL/UnemploymentData/UnemploymentDataTypesV2.xsd
+lino_welfare/modlib/cbss/WSDL/UnemploymentData/UnemploymentDataV2.wsdl
+lino_welfare/modlib/cbss/WSDL/UnemploymentData/UnemploymentDataV2.xsd
+lino_welfare/modlib/cbss/XSD/HealthCareInsuranceTypesV1.xsd
+lino_welfare/modlib/cbss/XSD/HealthCareInsuranceV1.xsd
 lino_welfare/modlib/cbss/XSD/README.txt
 lino_welfare/modlib/cbss/XSD/TestConnectionServiceV1.xsd
 lino_welfare/modlib/cbss/XSD/20190612/RetrieveTIGroupsV5.xsd
 lino_welfare/modlib/cbss/XSD/20190612/rn25_Release201411.xsd
 lino_welfare/modlib/cbss/XSD/SSDN/Common/CommonDataTypes.xsd
 lino_welfare/modlib/cbss/XSD/SSDN/Common/ExtensionPlaceHolder.xsd
 lino_welfare/modlib/cbss/XSD/SSDN/Common/NamespaceRoot.xsd
@@ -327,14 +333,15 @@
 lino_welfare/projects/gerd/settings/__init__.py
 lino_welfare/projects/gerd/settings/demo.py
 lino_welfare/projects/gerd/settings/doctests.py
 lino_welfare/projects/gerd/settings/memory.py
 lino_welfare/projects/gerd/settings/mysql.py
 lino_welfare/projects/gerd/settings/media/beid/123456789012.jpg
 lino_welfare/projects/gerd/settings/media/beid/591413288107.jpg
+lino_welfare/projects/gerd/settings/media/beid/592382784616.jpg
 lino_welfare/projects/gerd/settings/media/webdav/userdocs/appyodt/jobs.JobsOverview.odt
 lino_welfare/projects/gerd/tests/__init__.py
 lino_welfare/projects/gerd/tests/test_aids.py
 lino_welfare/projects/gerd/tests/test_broken_gfks.py
 lino_welfare/projects/gerd/tests/test_cbss.py
 lino_welfare/projects/gerd/tests/test_clients.py
 lino_welfare/projects/gerd/tests/test_debts.py
```

### Comparing `lino-welfare-23.6.0/tasks.py` & `lino-welfare-23.8.0/tasks.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.6.0/tests/__init__.py` & `lino-welfare-23.8.0/tests/__init__.py`

 * *Files identical despite different names*

