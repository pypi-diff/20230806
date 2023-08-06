# Comparing `tmp/bdd_tags_processor-0.1.0.tar.gz` & `tmp/bdd_tags_processor-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdd_tags_processor-0.1.0.tar", last modified: Sat Aug  5 08:17:25 2023, max compression
+gzip compressed data, was "bdd_tags_processor-0.2.0.tar", last modified: Sun Aug  6 14:04:59 2023, max compression
```

## Comparing `bdd_tags_processor-0.1.0.tar` & `bdd_tags_processor-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 tanwadhw   (501) staff       (20)        0 2023-08-05 08:17:25.547118 bdd_tags_processor-0.1.0/
--rw-r--r--   0 tanwadhw   (501) staff       (20)    35149 2023-08-05 06:40:05.000000 bdd_tags_processor-0.1.0/LICENSE
--rw-r--r--   0 tanwadhw   (501) staff       (20)     3928 2023-08-05 08:17:25.546994 bdd_tags_processor-0.1.0/PKG-INFO
--rw-r--r--   0 tanwadhw   (501) staff       (20)     3398 2023-08-05 08:08:16.000000 bdd_tags_processor-0.1.0/README.md
-drwxr-xr-x   0 tanwadhw   (501) staff       (20)        0 2023-08-05 08:17:25.545366 bdd_tags_processor-0.1.0/bdd_tags_processor/
--rw-r--r--   0 tanwadhw   (501) staff       (20)        0 2023-08-05 08:08:12.000000 bdd_tags_processor-0.1.0/bdd_tags_processor/__init__.py
--rw-r--r--   0 tanwadhw   (501) staff       (20)     7923 2023-08-05 08:08:12.000000 bdd_tags_processor-0.1.0/bdd_tags_processor/bdd_tags_expression_processor.py
-drwxr-xr-x   0 tanwadhw   (501) staff       (20)        0 2023-08-05 08:17:25.546642 bdd_tags_processor-0.1.0/bdd_tags_processor.egg-info/
--rw-r--r--   0 tanwadhw   (501) staff       (20)     3928 2023-08-05 08:17:25.000000 bdd_tags_processor-0.1.0/bdd_tags_processor.egg-info/PKG-INFO
--rw-r--r--   0 tanwadhw   (501) staff       (20)      322 2023-08-05 08:17:25.000000 bdd_tags_processor-0.1.0/bdd_tags_processor.egg-info/SOURCES.txt
--rw-r--r--   0 tanwadhw   (501) staff       (20)        1 2023-08-05 08:17:25.000000 bdd_tags_processor-0.1.0/bdd_tags_processor.egg-info/dependency_links.txt
--rw-r--r--   0 tanwadhw   (501) staff       (20)       93 2023-08-05 08:17:25.000000 bdd_tags_processor-0.1.0/bdd_tags_processor.egg-info/entry_points.txt
--rw-r--r--   0 tanwadhw   (501) staff       (20)       19 2023-08-05 08:17:25.000000 bdd_tags_processor-0.1.0/bdd_tags_processor.egg-info/top_level.txt
--rw-r--r--   0 tanwadhw   (501) staff       (20)       38 2023-08-05 08:17:25.547163 bdd_tags_processor-0.1.0/setup.cfg
--rw-r--r--   0 tanwadhw   (501) staff       (20)      927 2023-08-05 08:17:16.000000 bdd_tags_processor-0.1.0/setup.py
+drwxr-xr-x   0 tanwadhw   (501) staff       (20)        0 2023-08-06 14:04:59.438392 bdd_tags_processor-0.2.0/
+-rw-r--r--   0 tanwadhw   (501) staff       (20)    35149 2023-08-05 06:40:05.000000 bdd_tags_processor-0.2.0/LICENSE
+-rw-r--r--   0 tanwadhw   (501) staff       (20)     3941 2023-08-06 14:04:59.438269 bdd_tags_processor-0.2.0/PKG-INFO
+-rw-r--r--   0 tanwadhw   (501) staff       (20)     3398 2023-08-05 08:08:16.000000 bdd_tags_processor-0.2.0/README.md
+drwxr-xr-x   0 tanwadhw   (501) staff       (20)        0 2023-08-06 14:04:59.433483 bdd_tags_processor-0.2.0/bdd_tags_processor/
+-rw-r--r--   0 tanwadhw   (501) staff       (20)        0 2023-08-05 08:08:12.000000 bdd_tags_processor-0.2.0/bdd_tags_processor/__init__.py
+-rw-r--r--   0 tanwadhw   (501) staff       (20)     8938 2023-08-06 13:58:12.000000 bdd_tags_processor-0.2.0/bdd_tags_processor/bdd_tags_expression_processor.py
+drwxr-xr-x   0 tanwadhw   (501) staff       (20)        0 2023-08-06 14:04:59.437981 bdd_tags_processor-0.2.0/bdd_tags_processor.egg-info/
+-rw-r--r--   0 tanwadhw   (501) staff       (20)     3941 2023-08-06 14:04:59.000000 bdd_tags_processor-0.2.0/bdd_tags_processor.egg-info/PKG-INFO
+-rw-r--r--   0 tanwadhw   (501) staff       (20)      322 2023-08-06 14:04:59.000000 bdd_tags_processor-0.2.0/bdd_tags_processor.egg-info/SOURCES.txt
+-rw-r--r--   0 tanwadhw   (501) staff       (20)        1 2023-08-06 14:04:59.000000 bdd_tags_processor-0.2.0/bdd_tags_processor.egg-info/dependency_links.txt
+-rw-r--r--   0 tanwadhw   (501) staff       (20)       93 2023-08-06 14:04:59.000000 bdd_tags_processor-0.2.0/bdd_tags_processor.egg-info/entry_points.txt
+-rw-r--r--   0 tanwadhw   (501) staff       (20)       19 2023-08-06 14:04:59.000000 bdd_tags_processor-0.2.0/bdd_tags_processor.egg-info/top_level.txt
+-rw-r--r--   0 tanwadhw   (501) staff       (20)       38 2023-08-06 14:04:59.438440 bdd_tags_processor-0.2.0/setup.cfg
+-rw-r--r--   0 tanwadhw   (501) staff       (20)      940 2023-08-06 13:59:28.000000 bdd_tags_processor-0.2.0/setup.py
```

### Comparing `bdd_tags_processor-0.1.0/LICENSE` & `bdd_tags_processor-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bdd_tags_processor-0.1.0/PKG-INFO` & `bdd_tags_processor-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bdd_tags_processor
-Version: 0.1.0
-Summary: Filter Feature-Files based on Scenario Tag expressions
+Version: 0.2.0
+Summary: Filter Cucumber BDD Feature files based on Scenario Tag expressions
 Home-page: https://github.com/qarampage/bdd-tags-processor
 Author: QA Rampage
 Author-email: 16265665+qarampage@users.noreply.github.co
 Keywords: bdd cucumber tag expression processor filter feature files
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
```

### Comparing `bdd_tags_processor-0.1.0/README.md` & `bdd_tags_processor-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bdd_tags_processor-0.1.0/bdd_tags_processor/bdd_tags_expression_processor.py` & `bdd_tags_processor-0.2.0/bdd_tags_processor/bdd_tags_expression_processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-import logging
+import argparse
 import os
 import re
 import sys
 from glob import glob
 from pathlib import Path
 
-logging.basicConfig(level=logging.INFO)
-
 user_ands = []
 user_ors = []
 no_run_list = []
 
 
 def process_tags_expression(user_tag_expression):
     global user_ands
@@ -31,60 +29,35 @@
     for tag in no_run_list:
         copyUserArgs = copyUserArgs.replace(tag, '')
 
     copyUserArgs = ' '.join(copyUserArgs.split())
     # remove the unwanted and in the no_run_list
     no_run_list = [item.lstrip('and ~') for item in no_run_list]
 
+    # Process user expression
     if 'and (' in copyUserArgs:
         andBracket = copyUserArgs.split('and (')
         andAry = andBracket[0].split('and')
-        if len(andAry) == 1 and andAry[0] == '':
-            pass
-        else:
-            for strItm in andAry:
-                if len(strItm.strip()) > 0:
-                    if not strItm.strip().startswith('@'):
-                        print('Incorrect Expression in ANDs')
-                        sys.exit(1)
-                    user_ands.append(strItm.strip())
+        andAry = [strItm.strip() for strItm in andAry if strItm.strip().startswith('@')]
+        user_ands.extend(andAry)
 
         orAry = andBracket[1].split(' or ')
-        if len(orAry) == 1 and orAry[0] == '':
-            pass
-        else:
-            for strItm in orAry:
-                if not strItm.strip().startswith('@'):
-                    print('Incorrect Expression in ORs')
-                    sys.exit(1)
-                user_ors.append(strItm.strip())
+        orAry = [strItm.strip() for strItm in orAry if strItm.strip().startswith('@')]
+        user_ors.extend(orAry)
 
     elif 'or' in copyUserArgs:
         orAry = copyUserArgs.split('or ')
-        if len(orAry) == 1 and orAry[0] == '':
-            pass
-        else:
-            for strItm in orAry:
-                if len(strItm.strip()) > 0 and not strItm.strip().startswith('@'):
-                    print('Incorrect Expression in ORs')
-                    sys.exit(1)
-                user_ors.append(strItm.strip())
+        orAry = [strItm.strip() for strItm in orAry if strItm.strip().startswith('@')]
+        user_ors.extend(orAry)
 
     else:
         if copyUserArgs.strip() != '':
             andAry = copyUserArgs.split('and ')
-            if len(andAry) == 1 and andAry[0] == '':
-                pass
-            else:
-                for strItm in andAry:
-                    if len(strItm.strip()) > 0:
-                        if not strItm.strip().startswith('@'):
-                            print('Incorrect Expression in ANDs')
-                            sys.exit(1)
-                        user_ands.append(strItm.strip())
+            andAry = [strItm.strip() for strItm in andAry if strItm.strip().startswith('@')]
+            user_ands.extend(andAry)
 
 
 def filter_feature_and_scenarios(features_dir, result_dir, tags):
     Path(result_dir).mkdir(parents=True, exist_ok=True)
     for f in os.listdir(result_dir):
         os.remove(os.path.join(result_dir, f))
 
@@ -150,50 +123,81 @@
         # Only when at least 1 Scenario has been identified, flush the buffer into new file
         if found_cases > 0:
             total_features += 1
             total_scenarios += found_cases
             with open(f'{filename_head}.feature', 'w', encoding='utf-8') as result:
                 result.writelines(sequence_cases)
 
-    logging.info(f'{total_scenarios} Scenarios found in {total_features} Features files')
+    print(f'{total_scenarios} Scenarios found in {total_features} Features files')
 
     return total_scenarios
 
 
-
 def main():
-
+    args = None
     test_expressions = ['{@web}', '  {  @web    and @regression    and ~@norun}', '{~@norun and @web and (@test1 or @test2)}',
                         '{~@norun and (@test1 or @test2)}', '{@web and ~@browser and @sanity and ~@norun}', '{~@norun}', '{@sanity or @regression}',
                         '{@web and @browser and ~@norun and (@regression or @Sanity)}', '{@web and ~@norun and (@regression or @Sanity)}',
                         '{  ~@web   and   @browser   and   @checkout   and    ~@norun and (  @regression   or   @Sanity    )}',
                         '{  ~@web   and   @browser   and   @checkout   and    @norun and (  @test1   or   @test2    )}',
                         '{  @web   and   @regression   and    @norun and (  @test1   or   @test2    )}', '{@web and (@regression or @Sanity)}',
                         '{  @web   and   ~@browser   and   ~@checkout   and    @norun and (  @regression   or   @Sanity    )}',
-                        '{@web and ~@norun and (@p1)}', '@web', '', '{~@test-2}', '{~@norun and @web}']
+                        '{@web and ~@norun and (@p1)}', '@web', '', '{~@test-2}', '{~@norun and @web}',
+                        '{@web and @browser and ~@norun and (@regression or @Sanity or @titan-ic-ship)}',
+                        '{@web-browser and @browser-desktop and ~@no-run and (@regression or @Sanity or @titan-ic-ship)}']
+
+    try:
+        parser = argparse.ArgumentParser(description='Allows the user to run either (1)Veriy-Tags or (2)Verify-Tags-Extract-Files')
+        parser.add_argument('argopt', type=int, help='Specify which option you want to run')
+        parser.add_argument("argparam", type=str, nargs="?", default=None, help="Tag Expression")
+
+        args = parser.parse_args()
+    except SystemExit:
+        print('To test only Tag Expression Processor, please choose: ')
+        print('\t $ python bdd_tags_expression_processor.py 1')
+        print('\t $ python bdd_tags_expression_processor.py 1 "{@web}"')
+        print('To test filtering Feature files based on Tag Expression, please choose: ')
+        print('\t $ python bdd_tags_expression_processor.py 2')
+        print('\t $ python bdd_tags_expression_processor.py 2 "{@web}"')
+        sys.exit(1)
 
+    argopt = args.argopt
+    argparam = args.argparam
 
     def verify_sample_tag_expressions(one_sample_tag=None):
         if one_sample_tag is None:
+            print('Considering all the expression from the sample test_expressions provided in the code')
             for expression in test_expressions:
                 process_tags_expression(expression)
-                print(f'Given expression: {expression}\n\t Result: --> NORUNs: {no_run_list},  ANDs: {user_ands}, ORs: {user_ors}')
+                print(f'\nGiven expression: {expression}\n\t Result: --> NORUNs: {no_run_list},  ANDs: {user_ands}, ORs: {user_ors}')
         else:
+            print('Considering the given expression as everything available')
             process_tags_expression(one_sample_tag)
-            print(f'NORUNs: {no_run_list},  ANDs: {user_ands}, ORs: {user_ors}')
-
+            print(f'Given expression: {one_sample_tag}\n\t Result: --> NORUNs: {no_run_list},  ANDs: {user_ands}, ORs: {user_ors}')
 
-    def verify_extracted_files(input_path: str, output_path: str, one_sample_tag: str = None):
+    def verify_extracted_files(input_path: str, output_path: str, one_sample_tag=None):
         if one_sample_tag is None:
             for expression in test_expressions:
-                filter_feature_and_scenarios('feature', 'features/final', expression)
-                print(f' {expression} ... completed.. please check files')
+                filter_feature_and_scenarios(input_path, output_path, expression)
+                print(f'{expression} ... completed.. please check files\n')
         else:
             filter_feature_and_scenarios(input_path, output_path, one_sample_tag)
             print(f' {one_sample_tag} ... completed.. please check files')
 
+    if argopt == 1:
+        if argparam:
+            verify_sample_tag_expressions(argparam)
+        else:
+            verify_sample_tag_expressions(test_expressions)
+    elif argopt == 2:
+        print("Ensure that you have input_path='features/web', output_path='features/final'. Default assumption is not created")
+        input("Do you want to continue? (yes/no): ").strip().lower()
+        if argparam:
+            verify_extracted_files(input_path='features/web', output_path='features/final', one_sample_tag=argparam)
+        else:
+            verify_extracted_files(input_path='features/web', output_path='features/final')
+    else:
+        print('Choose only from 1 or 2 as choices in the argument')
 
-    verify_sample_tag_expressions()
-    verify_extracted_files(input_path='features/scenarios/web', output_path='features/final')
 
 if __name__ == '__main__':
     main()
```

### Comparing `bdd_tags_processor-0.1.0/bdd_tags_processor.egg-info/PKG-INFO` & `bdd_tags_processor-0.2.0/bdd_tags_processor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bdd-tags-processor
-Version: 0.1.0
-Summary: Filter Feature-Files based on Scenario Tag expressions
+Version: 0.2.0
+Summary: Filter Cucumber BDD Feature files based on Scenario Tag expressions
 Home-page: https://github.com/qarampage/bdd-tags-processor
 Author: QA Rampage
 Author-email: 16265665+qarampage@users.noreply.github.co
 Keywords: bdd cucumber tag expression processor filter feature files
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
```

### Comparing `bdd_tags_processor-0.1.0/setup.py` & `bdd_tags_processor-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="bdd_tags_processor",
-    version="0.1.0",
-    description="Filter Feature-Files based on Scenario Tag expressions",
+    version="0.2.0",
+    description="Filter Cucumber BDD Feature files based on Scenario Tag expressions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="QA Rampage",
     author_email="16265665+qarampage@users.noreply.github.co",
     url="https://github.com/qarampage/bdd-tags-processor",
     packages=find_packages(),
     install_requires=[],
```

