# Comparing `tmp/unitgrade-devel-0.1.7a0.tar.gz` & `tmp/unitgrade-devel-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\tuhe\Documents\unitgrade_private\dist\tmpm9w_19co\unitgrade-devel-0.1.7a0.tar", last modified: Thu Sep 16 10:50:11 2021, max compression
+gzip compressed data, was "C:\Users\tuhe\Documents\unitgrade_private\dist\tmpevuge7wf\unitgrade-devel-0.1.9.tar", last modified: Fri Sep 17 11:54:20 2021, max compression
```

## Comparing `unitgrade-devel-0.1.7a0.tar` & `unitgrade-devel-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2021-09-16 10:50:11.839141 unitgrade-devel-0.1.7a0/
--rw-rw-rw-   0        0        0     1091 2021-09-02 10:11:20.000000 unitgrade-devel-0.1.7a0/LICENSE
--rw-rw-rw-   0        0        0    25699 2021-09-16 10:50:11.839141 unitgrade-devel-0.1.7a0/PKG-INFO
--rw-rw-rw-   0        0        0    25078 2021-09-15 15:37:06.000000 unitgrade-devel-0.1.7a0/README.md
--rw-rw-rw-   0        0        0      108 2021-09-02 10:05:30.000000 unitgrade-devel-0.1.7a0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2021-09-16 10:50:11.839141 unitgrade-devel-0.1.7a0/setup.cfg
--rw-rw-rw-   0        0        0     1307 2021-09-16 09:17:10.000000 unitgrade-devel-0.1.7a0/setup.py
-drwxrwxrwx   0        0        0        0 2021-09-16 10:50:11.580552 unitgrade-devel-0.1.7a0/src/
-drwxrwxrwx   0        0        0        0 2021-09-16 10:50:11.779500 unitgrade-devel-0.1.7a0/src/unitgrade_devel.egg-info/
--rw-rw-rw-   0        0        0    25699 2021-09-16 10:50:11.000000 unitgrade-devel-0.1.7a0/src/unitgrade_devel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      740 2021-09-16 10:50:11.000000 unitgrade-devel-0.1.7a0/src/unitgrade_devel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-09-16 10:50:11.000000 unitgrade-devel-0.1.7a0/src/unitgrade_devel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2021-09-16 10:50:11.000000 unitgrade-devel-0.1.7a0/src/unitgrade_devel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2021-09-16 10:50:11.000000 unitgrade-devel-0.1.7a0/src/unitgrade_devel.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-09-16 10:50:11.807878 unitgrade-devel-0.1.7a0/src/unitgrade_private/
--rw-rw-rw-   0        0        0      991 2021-09-16 10:32:15.000000 unitgrade-devel-0.1.7a0/src/unitgrade_private/__init__.py
-drwxrwxrwx   0        0        0        0 2021-09-16 10:50:11.823505 unitgrade-devel-0.1.7a0/src/unitgrade_private/autolab/
--rw-rw-rw-   0        0        0        0 2021-08-31 11:53:29.000000 unitgrade-devel-0.1.7a0/src/unitgrade_private/autolab/__init__.py
--rw-rw-rw-   0        0        0     9020 2021-09-15 15:40:01.000000 unitgrade-devel-0.1.7a0/src/unitgrade_private/autolab/autolab.py
--rw-rw-rw-   0        0        0     1361 2021-09-15 15:40:00.000000 unitgrade-devel-0.1.7a0/src/unitgrade_private/deployment.py
--rw-rw-rw-   0        0        0     4736 2021-08-31 12:11:40.000000 unitgrade-devel-0.1.7a0/src/unitgrade_private/docker_helpers.py
--rw-rw-rw-   0        0        0     6164 2021-09-15 22:39:16.000000 unitgrade-devel-0.1.7a0/src/unitgrade_private/hidden_create_files.py
--rw-rw-rw-   0        0        0     8021 2021-09-16 10:30:33.000000 unitgrade-devel-0.1.7a0/src/unitgrade_private/hidden_gather_upload.py
-drwxrwxrwx   0        0        0        0 2021-09-16 10:50:11.839141 unitgrade-devel-0.1.7a0/src/unitgrade_private/plagiarism/
--rw-rw-rw-   0        0        0        2 2021-09-16 10:42:24.000000 unitgrade-devel-0.1.7a0/src/unitgrade_private/plagiarism/__init__.py
--rw-rw-rw-   0        0        0     2699 2021-09-16 10:30:33.000000 unitgrade-devel-0.1.7a0/src/unitgrade_private/plagiarism/mossit.py
--rw-rw-rw-   0        0        0     2546 2021-09-08 14:31:46.000000 unitgrade-devel-0.1.7a0/src/unitgrade_private/plagiarism/utils.py
--rw-rw-rw-   0        0        0     1004 2021-09-16 10:49:51.000000 unitgrade-devel-0.1.7a0/src/unitgrade_private/token_loader.py
--rw-rw-rw-   0        0        0       18 2021-09-16 10:49:51.000000 unitgrade-devel-0.1.7a0/src/unitgrade_private/version.py
+drwxrwxrwx   0        0        0        0 2021-09-17 11:54:20.183545 unitgrade-devel-0.1.9/
+-rw-rw-rw-   0        0        0     1091 2021-09-02 10:11:20.000000 unitgrade-devel-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0    26097 2021-09-17 11:54:20.183545 unitgrade-devel-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    25478 2021-09-17 11:43:46.000000 unitgrade-devel-0.1.9/README.md
+-rw-rw-rw-   0        0        0      108 2021-09-02 10:05:30.000000 unitgrade-devel-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2021-09-17 11:54:20.183545 unitgrade-devel-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1354 2021-09-16 22:45:46.000000 unitgrade-devel-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-09-17 11:54:19.920775 unitgrade-devel-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2021-09-17 11:54:20.030170 unitgrade-devel-0.1.9/src/unitgrade_devel.egg-info/
+-rw-rw-rw-   0        0        0    26097 2021-09-17 11:54:19.000000 unitgrade-devel-0.1.9/src/unitgrade_devel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      740 2021-09-17 11:54:19.000000 unitgrade-devel-0.1.9/src/unitgrade_devel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-09-17 11:54:19.000000 unitgrade-devel-0.1.9/src/unitgrade_devel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2021-09-17 11:54:19.000000 unitgrade-devel-0.1.9/src/unitgrade_devel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2021-09-17 11:54:19.000000 unitgrade-devel-0.1.9/src/unitgrade_devel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-09-17 11:54:20.152294 unitgrade-devel-0.1.9/src/unitgrade_private/
+-rw-rw-rw-   0        0        0      851 2021-09-16 22:44:04.000000 unitgrade-devel-0.1.9/src/unitgrade_private/__init__.py
+drwxrwxrwx   0        0        0        0 2021-09-17 11:54:20.167936 unitgrade-devel-0.1.9/src/unitgrade_private/autolab/
+-rw-rw-rw-   0        0        0        0 2021-08-31 11:53:29.000000 unitgrade-devel-0.1.9/src/unitgrade_private/autolab/__init__.py
+-rw-rw-rw-   0        0        0     9020 2021-09-16 15:58:19.000000 unitgrade-devel-0.1.9/src/unitgrade_private/autolab/autolab.py
+-rw-rw-rw-   0        0        0     1373 2021-09-17 11:43:46.000000 unitgrade-devel-0.1.9/src/unitgrade_private/deployment.py
+-rw-rw-rw-   0        0        0     4837 2021-09-16 21:51:32.000000 unitgrade-devel-0.1.9/src/unitgrade_private/docker_helpers.py
+-rw-rw-rw-   0        0        0     4798 2021-09-16 22:59:13.000000 unitgrade-devel-0.1.9/src/unitgrade_private/hidden_create_files.py
+-rw-rw-rw-   0        0        0     7525 2021-09-16 22:51:24.000000 unitgrade-devel-0.1.9/src/unitgrade_private/hidden_gather_upload.py
+drwxrwxrwx   0        0        0        0 2021-09-17 11:54:20.183545 unitgrade-devel-0.1.9/src/unitgrade_private/plagiarism/
+-rw-rw-rw-   0        0        0        2 2021-09-16 10:42:24.000000 unitgrade-devel-0.1.9/src/unitgrade_private/plagiarism/__init__.py
+-rw-rw-rw-   0        0        0     2709 2021-09-16 22:51:24.000000 unitgrade-devel-0.1.9/src/unitgrade_private/plagiarism/mossit.py
+-rw-rw-rw-   0        0        0        4 2021-09-16 11:25:42.000000 unitgrade-devel-0.1.9/src/unitgrade_private/plagiarism/utils.py
+-rw-rw-rw-   0        0        0      574 2021-09-16 22:51:24.000000 unitgrade-devel-0.1.9/src/unitgrade_private/token_loader.py
+-rw-rw-rw-   0        0        0       19 2021-09-17 11:52:55.000000 unitgrade-devel-0.1.9/src/unitgrade_private/version.py
```

### Comparing `unitgrade-devel-0.1.7a0/LICENSE` & `unitgrade-devel-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `unitgrade-devel-0.1.7a0/PKG-INFO` & `unitgrade-devel-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: unitgrade-devel
-Version: 0.1.7a0
-Summary: A set of tools to develop unitgrade tests and reports and later evaluate them
-Home-page: https://lab.compute.dtu.dk/tuhe/unitgrade_private
-Author: Tue Herlau
-Author-email: tuhe@dtu.dk
-License: MIT
-Project-URL: Bug Tracker, https://lab.compute.dtu.dk/tuhe/unitgrade_private/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Unitgrade-devel
 **Note: This is the development version of unitgrade. If you are a student, please see http://gitlab.compute.dtu.dk/tuhe/unitgrade.**
 
 Unitgrade is an automatic report and exam evaluation framework that enables instructors to offer automatically evaluated programming assignments. 
  Unitgrade is build on pythons `unittest` framework so that the tests can be specified in a familiar syntax and will integrate with any modern IDE. What it offers beyond `unittest` is the ability to collect tests in reports (for automatic evaluation) and an easy and 100% safe mechanism for verifying the students results and creating additional, hidden tests. A powerful cache system allows instructors to automatically create test-answers based on a working solution. 
 
  - 100% Python `unittest` compatible
@@ -29,16 +12,26 @@
  - Granular security model: 
     - Students get public `unittests` for easy development of solutions
     - Students use a tamper-resistant file to create submissions which are uploaded
     - Instructors can automatically verify the students solution using a Docker VM and run hidden tests
  - Automatic Moss anti-plagiarism detection
  - CMU Autolab integration (Experimental)
 
-# Using unitgrade
-The examples can be found in the `/examples/` directory: https://gitlab.compute.dtu.dk/tuhe/unitgrade_private/examples
+### Install
+Simply use `pip`
+```terminal
+pip install unitgrade-devel
+```
+This will install `unitgrade-devel` (this package) and all dependencies to get you started.
+
+### Videos
+For videos see the `/videos` directory : https://gitlab.compute.dtu.dk/tuhe/unitgrade_private/-/tree/master/videos
+
+# Instructions and examples of use
+The examples can be found in the `/examples` directory: https://gitlab.compute.dtu.dk/tuhe/unitgrade_private/-/tree/master/examples
 
 ## A simple example
 Unitgrade makes the following assumptions:
  - Your code is in python
  - Whatever you want to do can be specified as a `unittest`
 
 Although not required, it is recommended you maintain two version of the code: 
@@ -86,15 +79,14 @@
         self.assertEqual(add(2,2), 4)
         self.assertEqual(add(-100, 5), -95)
 
     def test_reverse(self):
         self.assertEqual(reverse_list([1,2,3]), [3,2,1]) 
 ```
 A number of tests can be collected into a `Report`, which will allow us to assign points to the tests and use the more advanced features of the framework later. A complete, minimal example:
-
 ```python
 # example_simplest/instructor/cs101/report1.py
 import unittest 
 from unitgrade import Report, evaluate_report_student
 import cs101
 from cs101.homework1 import reverse_list, add 
 
@@ -114,27 +106,20 @@
 if __name__ == "__main__":
     evaluate_report_student(Report1()) 
 ```
 
 ### Deployment
 The above is all you need if you simply want to use the framework as a self-check: Students can run the code and see how well they did. 
 In order to begin using the framework for evaluation we need to create a bit more structure. We do that by deploying the report class as follows:
-
 ```python
 # example_simplest/instructor/cs101/deploy.py
 from cs101.report1 import Report1 
 from unitgrade_private.hidden_create_files import setup_grade_file_report
 from snipper import snip_dir
 
-a = 34 #!i
-print(a)
-a
-z = 23 #!i
-
-
 if __name__ == "__main__":
     setup_grade_file_report(Report1)  # Make the report1_grade.py report file
 
     # Deploy the files using snipper: https://gitlab.compute.dtu.dk/tuhe/snipper
     snip_dir("./", "../../students/cs101", exclude=['__pycache__', '*.token', 'deploy.py']) 
 ```
  - The first line creates the `report1_grade.py` script and any additional data files needed by the tests (none in this case)
@@ -191,15 +176,15 @@
 If this is not enough, you can consider using `pyarmor` on the `_grade.py` script to create a **very** difficult challenge for a prospective hacker.
 
 ## Example 2: The framework
 One of the main advantages of `unitgrade` over web-based autograders it that tests are really easy to develop and maintain. To take advantage of this, we simply change the class the questions inherit from to `UTestCase` (this is still a `unittest.TestCase`) and we can make use of the chache system. As an example:
 
 ```python 
 # example_framework/instructor/cs102/report2.py
-from unitgrade2 import UTestCase 
+from unitgrade import UTestCase 
 
 class Week1(UTestCase):
     def test_add(self):
         self.assertEqualC(add(2,2))
         self.assertEqualC(add(-100, 5))
 
     def test_reverse(self):
@@ -230,29 +215,29 @@
 When this is run, the titles are shown as follows:
 ```terminal
  _   _       _ _   _____               _      
 | | | |     (_) | |  __ \             | |     
 | | | |_ __  _| |_| |  \/_ __ __ _  __| | ___ 
 | | | | '_ \| | __| | __| '__/ _` |/ _` |/ _ \
 | |_| | | | | | |_| |_\ \ | | (_| | (_| |  __/
- \___/|_| |_|_|\__|\____/_|  \__,_|\__,_|\___| v0.1.0, started: 09/09/2021 19:52:23
+ \___/|_| |_|_|\__|\____/_|  \__,_|\__,_|\___| v0.1.5, started: 16/09/2021 17:42:18
 
 CS 101 Report 2 (use --help for options)
 Question 1: Week1                                                                                                       
  * q1.1) test_add...................................................................................................PASS
  * q1.2) test_reverse...............................................................................................PASS
  * q1.3) test_output_capture........................................................................................PASS
  * q1)   Total.................................................................................................... 10/10
  
 Question 2: The same problem as before with nicer titles                                                                
  * q2.1) Test the addition method add(a,b)..........................................................................PASS
  * q2.2) Checking if reverse_list([1, 2, 3]) = [3, 2, 1]............................................................PASS
  * q2)   Total...................................................................................................... 8/8
  
-Total points at 19:52:23 (0 minutes, 0 seconds)....................................................................18/18
+Total points at 17:42:18 (0 minutes, 0 seconds)....................................................................18/18
 
 ```
 What happens behind the scenes when we set `self.title` is that the result is pre-computed on the instructors machine and cached. This means the last test will display the correct result regardless of how `reverse_list` has been implemented by the student. The titles are also shown correctly when the method is run as a unittest. 
 
 ### Caching computations
 The `@cache`-decorator offers a direct ways to compute the correct result on an instructors computer and submit it to the student. For instance:
 ```python
@@ -285,26 +270,29 @@
 ## Example 3: Hidden and secure tests
 To use `unitgrade` as part of automatic grading, it is recommended you check the students output locally and use hidden tests. Fortunately, this is very easy.
 
 Let's start with the hidden tests. As usual we write a complete report script (`report3_complete.py`), but this time we use the `@hide`-decorator to mark tests as hidden:
 
 ```python
 # example_docker/instructor/cs103/report3_complete.py
-from unitgrade import UTestCase, Report, hide 
+from unitgrade import UTestCase, Report
+from unitgrade.utils import hide
 from unitgrade import evaluate_report_student
 import cs103
 
+
 class AutomaticPass(UTestCase):
     def test_automatic_pass(self):
         self.assertEqual(2, 2)  # For simplicity, this test will always pass
 
     @hide  # The @hide-decorator tells unitgrade_v1 to hide the test for students.
     def test_hidden_fail(self):
         self.assertEqual(2, 3)  # For simplicity, this test will always fail.
 
+
 class Report3(Report):
     title = "CS 101 Report 3"
     questions = [(AutomaticPass, 10)]  # Include a single question for 10 credits.
     pack_imports = [cs103] 
 ```
 For simplicity, non-hidden test will always pass, and the hidden test will always fail: This makes it easy to interpret the results in the following.
 
@@ -321,18 +309,20 @@
     student_directory = "../../students/cs103"
     snip_dir("./", student_directory, exclude=['__pycache__', '*.token', 'deploy.py', 'report3_complete*.py', '.*']) 
 ```
 Just to check, let's have a quick look at the students report script `report3.py`:
 
 ```python
 # example_docker/instructor/cs103/report3.py
-from unitgrade import UTestCase, Report, hide 
+from unitgrade import UTestCase, Report
+from unitgrade.utils import hide
 from unitgrade import evaluate_report_student
 import cs103
 
+
 class AutomaticPass(UTestCase):
     def test_automatic_pass(self):
         self.assertEqual(2, 2)  # For simplicity, this test will always pass
 
 
 class Report3(Report):
     title = "CS 101 Report 3"
@@ -406,15 +396,15 @@
 /submissions/<student-id-2>/Report1_130_of_144.token
 ...
 ```
 The files in the whitelist/student directory can be either `.token` files (which are unpacked) or python files, and they may contain subdirectories: Everything will be unpacked and flattened. The simplest way to set it up is simply to download all files from DTU learn as a zip-file and unzip it somewhere.
 When done just call moss as follows:
 ```python 
 # example_moss/moss_example.py
-from unitgrade_private2.plagiarism.mossit import moss_it, get_id 
+from unitgrade_private.plagiarism.mossit import moss_it, get_id 
 
 if __name__ == "__main__":
     # Extract the moss id ("12415...") from the perl script and test:
     id = get_id("../../../02465private/admin/moss.pl")
     moss_it(whitelist_dir="whitelist", submissions_dir="student_submissions", moss_id=id) 
 ```
 This will generate a report. You can see the example including the report here: https://lab.compute.dtu.dk/tuhe/unitgrade_private/-/tree/master/examples/example_moss
@@ -452,35 +442,34 @@
 # example_hints/instructor/cs106/report1hints.py
 class Week1(UTestCase): 
     def test_find_all_primes(self):
         """
         Hints:
             * Insert a breakpoint and check what your function find_primes(4) actually outputs
         """
-        self.assertEqual(find_primes(4), [2,3])
+        self.assertEqual(find_primes(4), [2, 3], msg="The list should only contain primes <= 4")
 
 class Report1Hints(Report):
     title = "CS 106 Report 1"
     questions = [(Week1, 10)]
-    pack_imports = [homework1]  
+    pack_imports = [homework_hints]  
 ```
 
 When students run this homework it will fail and display the hints from the two methods:
 ![alt text|small](https://gitlab.compute.dtu.dk/tuhe/unitgrade_private/-/raw/master/docs/hints.png)
 
 What happens behind the scenes is that a code-coverage tool is run on the instructors computer
 to determine which methods are actually used in solving a problem, and then the hint-texts of those methods are 
 collected and displayed. This feature requires no external configuration; simply write `Hints:` in the source code. 
 
 # Citing
 ```bibtex
 @online{unitgrade_devel,
-	title={Unitgrade-devel (0.1.2): \texttt{pip install unitgrade-devel}},
+	title={Unitgrade-devel (0.1.7): \texttt{pip install unitgrade-devel}},
 	url={https://lab.compute.dtu.dk/tuhe/unitgrade_private},
-	urldate = {2021-09-09}, 
+	urldate = {2021-09-16}, 
 	month={9},
 	publisher={Technical University of Denmark (DTU)},
 	author={Tue Herlau},
 	year={2021},
 }
-```
-
+```
```

### Comparing `unitgrade-devel-0.1.7a0/README.md` & `unitgrade-devel-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: unitgrade-devel
+Version: 0.1.9
+Summary: A set of tools to develop unitgrade tests and reports and later evaluate them
+Home-page: https://lab.compute.dtu.dk/tuhe/unitgrade_private
+Author: Tue Herlau
+Author-email: tuhe@dtu.dk
+License: MIT
+Project-URL: Bug Tracker, https://lab.compute.dtu.dk/tuhe/unitgrade_private/issues
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Unitgrade-devel
 **Note: This is the development version of unitgrade. If you are a student, please see http://gitlab.compute.dtu.dk/tuhe/unitgrade.**
 
 Unitgrade is an automatic report and exam evaluation framework that enables instructors to offer automatically evaluated programming assignments. 
  Unitgrade is build on pythons `unittest` framework so that the tests can be specified in a familiar syntax and will integrate with any modern IDE. What it offers beyond `unittest` is the ability to collect tests in reports (for automatic evaluation) and an easy and 100% safe mechanism for verifying the students results and creating additional, hidden tests. A powerful cache system allows instructors to automatically create test-answers based on a working solution. 
 
  - 100% Python `unittest` compatible
@@ -12,16 +29,26 @@
  - Granular security model: 
     - Students get public `unittests` for easy development of solutions
     - Students use a tamper-resistant file to create submissions which are uploaded
     - Instructors can automatically verify the students solution using a Docker VM and run hidden tests
  - Automatic Moss anti-plagiarism detection
  - CMU Autolab integration (Experimental)
 
-# Using unitgrade
-The examples can be found in the `/examples/` directory: https://gitlab.compute.dtu.dk/tuhe/unitgrade_private/examples
+### Install
+Simply use `pip`
+```terminal
+pip install unitgrade-devel
+```
+This will install `unitgrade-devel` (this package) and all dependencies to get you started.
+
+### Videos
+For videos see the `/videos` directory : https://gitlab.compute.dtu.dk/tuhe/unitgrade_private/-/tree/master/videos
+
+# Instructions and examples of use
+The examples can be found in the `/examples` directory: https://gitlab.compute.dtu.dk/tuhe/unitgrade_private/-/tree/master/examples
 
 ## A simple example
 Unitgrade makes the following assumptions:
  - Your code is in python
  - Whatever you want to do can be specified as a `unittest`
 
 Although not required, it is recommended you maintain two version of the code: 
@@ -69,15 +96,14 @@
         self.assertEqual(add(2,2), 4)
         self.assertEqual(add(-100, 5), -95)
 
     def test_reverse(self):
         self.assertEqual(reverse_list([1,2,3]), [3,2,1]) 
 ```
 A number of tests can be collected into a `Report`, which will allow us to assign points to the tests and use the more advanced features of the framework later. A complete, minimal example:
-
 ```python
 # example_simplest/instructor/cs101/report1.py
 import unittest 
 from unitgrade import Report, evaluate_report_student
 import cs101
 from cs101.homework1 import reverse_list, add 
 
@@ -97,27 +123,20 @@
 if __name__ == "__main__":
     evaluate_report_student(Report1()) 
 ```
 
 ### Deployment
 The above is all you need if you simply want to use the framework as a self-check: Students can run the code and see how well they did. 
 In order to begin using the framework for evaluation we need to create a bit more structure. We do that by deploying the report class as follows:
-
 ```python
 # example_simplest/instructor/cs101/deploy.py
 from cs101.report1 import Report1 
 from unitgrade_private.hidden_create_files import setup_grade_file_report
 from snipper import snip_dir
 
-a = 34 #!i
-print(a)
-a
-z = 23 #!i
-
-
 if __name__ == "__main__":
     setup_grade_file_report(Report1)  # Make the report1_grade.py report file
 
     # Deploy the files using snipper: https://gitlab.compute.dtu.dk/tuhe/snipper
     snip_dir("./", "../../students/cs101", exclude=['__pycache__', '*.token', 'deploy.py']) 
 ```
  - The first line creates the `report1_grade.py` script and any additional data files needed by the tests (none in this case)
@@ -174,15 +193,15 @@
 If this is not enough, you can consider using `pyarmor` on the `_grade.py` script to create a **very** difficult challenge for a prospective hacker.
 
 ## Example 2: The framework
 One of the main advantages of `unitgrade` over web-based autograders it that tests are really easy to develop and maintain. To take advantage of this, we simply change the class the questions inherit from to `UTestCase` (this is still a `unittest.TestCase`) and we can make use of the chache system. As an example:
 
 ```python 
 # example_framework/instructor/cs102/report2.py
-from unitgrade2 import UTestCase 
+from unitgrade import UTestCase 
 
 class Week1(UTestCase):
     def test_add(self):
         self.assertEqualC(add(2,2))
         self.assertEqualC(add(-100, 5))
 
     def test_reverse(self):
@@ -213,29 +232,29 @@
 When this is run, the titles are shown as follows:
 ```terminal
  _   _       _ _   _____               _      
 | | | |     (_) | |  __ \             | |     
 | | | |_ __  _| |_| |  \/_ __ __ _  __| | ___ 
 | | | | '_ \| | __| | __| '__/ _` |/ _` |/ _ \
 | |_| | | | | | |_| |_\ \ | | (_| | (_| |  __/
- \___/|_| |_|_|\__|\____/_|  \__,_|\__,_|\___| v0.1.0, started: 09/09/2021 19:52:23
+ \___/|_| |_|_|\__|\____/_|  \__,_|\__,_|\___| v0.1.5, started: 16/09/2021 17:42:18
 
 CS 101 Report 2 (use --help for options)
 Question 1: Week1                                                                                                       
  * q1.1) test_add...................................................................................................PASS
  * q1.2) test_reverse...............................................................................................PASS
  * q1.3) test_output_capture........................................................................................PASS
  * q1)   Total.................................................................................................... 10/10
  
 Question 2: The same problem as before with nicer titles                                                                
  * q2.1) Test the addition method add(a,b)..........................................................................PASS
  * q2.2) Checking if reverse_list([1, 2, 3]) = [3, 2, 1]............................................................PASS
  * q2)   Total...................................................................................................... 8/8
  
-Total points at 19:52:23 (0 minutes, 0 seconds)....................................................................18/18
+Total points at 17:42:18 (0 minutes, 0 seconds)....................................................................18/18
 
 ```
 What happens behind the scenes when we set `self.title` is that the result is pre-computed on the instructors machine and cached. This means the last test will display the correct result regardless of how `reverse_list` has been implemented by the student. The titles are also shown correctly when the method is run as a unittest. 
 
 ### Caching computations
 The `@cache`-decorator offers a direct ways to compute the correct result on an instructors computer and submit it to the student. For instance:
 ```python
@@ -268,26 +287,29 @@
 ## Example 3: Hidden and secure tests
 To use `unitgrade` as part of automatic grading, it is recommended you check the students output locally and use hidden tests. Fortunately, this is very easy.
 
 Let's start with the hidden tests. As usual we write a complete report script (`report3_complete.py`), but this time we use the `@hide`-decorator to mark tests as hidden:
 
 ```python
 # example_docker/instructor/cs103/report3_complete.py
-from unitgrade import UTestCase, Report, hide 
+from unitgrade import UTestCase, Report
+from unitgrade.utils import hide
 from unitgrade import evaluate_report_student
 import cs103
 
+
 class AutomaticPass(UTestCase):
     def test_automatic_pass(self):
         self.assertEqual(2, 2)  # For simplicity, this test will always pass
 
     @hide  # The @hide-decorator tells unitgrade_v1 to hide the test for students.
     def test_hidden_fail(self):
         self.assertEqual(2, 3)  # For simplicity, this test will always fail.
 
+
 class Report3(Report):
     title = "CS 101 Report 3"
     questions = [(AutomaticPass, 10)]  # Include a single question for 10 credits.
     pack_imports = [cs103] 
 ```
 For simplicity, non-hidden test will always pass, and the hidden test will always fail: This makes it easy to interpret the results in the following.
 
@@ -304,18 +326,20 @@
     student_directory = "../../students/cs103"
     snip_dir("./", student_directory, exclude=['__pycache__', '*.token', 'deploy.py', 'report3_complete*.py', '.*']) 
 ```
 Just to check, let's have a quick look at the students report script `report3.py`:
 
 ```python
 # example_docker/instructor/cs103/report3.py
-from unitgrade import UTestCase, Report, hide 
+from unitgrade import UTestCase, Report
+from unitgrade.utils import hide
 from unitgrade import evaluate_report_student
 import cs103
 
+
 class AutomaticPass(UTestCase):
     def test_automatic_pass(self):
         self.assertEqual(2, 2)  # For simplicity, this test will always pass
 
 
 class Report3(Report):
     title = "CS 101 Report 3"
@@ -389,15 +413,15 @@
 /submissions/<student-id-2>/Report1_130_of_144.token
 ...
 ```
 The files in the whitelist/student directory can be either `.token` files (which are unpacked) or python files, and they may contain subdirectories: Everything will be unpacked and flattened. The simplest way to set it up is simply to download all files from DTU learn as a zip-file and unzip it somewhere.
 When done just call moss as follows:
 ```python 
 # example_moss/moss_example.py
-from unitgrade_private2.plagiarism.mossit import moss_it, get_id 
+from unitgrade_private.plagiarism.mossit import moss_it, get_id 
 
 if __name__ == "__main__":
     # Extract the moss id ("12415...") from the perl script and test:
     id = get_id("../../../02465private/admin/moss.pl")
     moss_it(whitelist_dir="whitelist", submissions_dir="student_submissions", moss_id=id) 
 ```
 This will generate a report. You can see the example including the report here: https://lab.compute.dtu.dk/tuhe/unitgrade_private/-/tree/master/examples/example_moss
@@ -435,34 +459,35 @@
 # example_hints/instructor/cs106/report1hints.py
 class Week1(UTestCase): 
     def test_find_all_primes(self):
         """
         Hints:
             * Insert a breakpoint and check what your function find_primes(4) actually outputs
         """
-        self.assertEqual(find_primes(4), [2,3])
+        self.assertEqual(find_primes(4), [2, 3], msg="The list should only contain primes <= 4")
 
 class Report1Hints(Report):
     title = "CS 106 Report 1"
     questions = [(Week1, 10)]
-    pack_imports = [homework1]  
+    pack_imports = [homework_hints]  
 ```
 
 When students run this homework it will fail and display the hints from the two methods:
 ![alt text|small](https://gitlab.compute.dtu.dk/tuhe/unitgrade_private/-/raw/master/docs/hints.png)
 
 What happens behind the scenes is that a code-coverage tool is run on the instructors computer
 to determine which methods are actually used in solving a problem, and then the hint-texts of those methods are 
 collected and displayed. This feature requires no external configuration; simply write `Hints:` in the source code. 
 
 # Citing
 ```bibtex
 @online{unitgrade_devel,
-	title={Unitgrade-devel (0.1.2): \texttt{pip install unitgrade-devel}},
+	title={Unitgrade-devel (0.1.7): \texttt{pip install unitgrade-devel}},
 	url={https://lab.compute.dtu.dk/tuhe/unitgrade_private},
-	urldate = {2021-09-09}, 
+	urldate = {2021-09-16}, 
 	month={9},
 	publisher={Technical University of Denmark (DTU)},
 	author={Tue Herlau},
 	year={2021},
 }
-```
+```
+
```

### Comparing `unitgrade-devel-0.1.7a0/setup.py` & `unitgrade-devel-0.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,9 +25,10 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.8",
-    install_requires=['numpy', "unitgrade", "codesnipper", 'tabulate', 'tqdm', "pyfiglet", "colorama", "coverage", 'mosspy'],
+    install_requires=['numpy', "unitgrade", "codesnipper", 'tabulate', 'tqdm', "pyfiglet",
+                      "colorama", "coverage", 'mosspy', 'pyminifier', 'mosspy'],
 )
```

### Comparing `unitgrade-devel-0.1.7a0/src/unitgrade_devel.egg-info/PKG-INFO` & `unitgrade-devel-0.1.9/src/unitgrade_devel.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitgrade-devel
-Version: 0.1.7a0
+Version: 0.1.9
 Summary: A set of tools to develop unitgrade tests and reports and later evaluate them
 Home-page: https://lab.compute.dtu.dk/tuhe/unitgrade_private
 Author: Tue Herlau
 Author-email: tuhe@dtu.dk
 License: MIT
 Project-URL: Bug Tracker, https://lab.compute.dtu.dk/tuhe/unitgrade_private/issues
 Platform: UNKNOWN
@@ -29,16 +29,26 @@
  - Granular security model: 
     - Students get public `unittests` for easy development of solutions
     - Students use a tamper-resistant file to create submissions which are uploaded
     - Instructors can automatically verify the students solution using a Docker VM and run hidden tests
  - Automatic Moss anti-plagiarism detection
  - CMU Autolab integration (Experimental)
 
-# Using unitgrade
-The examples can be found in the `/examples/` directory: https://gitlab.compute.dtu.dk/tuhe/unitgrade_private/examples
+### Install
+Simply use `pip`
+```terminal
+pip install unitgrade-devel
+```
+This will install `unitgrade-devel` (this package) and all dependencies to get you started.
+
+### Videos
+For videos see the `/videos` directory : https://gitlab.compute.dtu.dk/tuhe/unitgrade_private/-/tree/master/videos
+
+# Instructions and examples of use
+The examples can be found in the `/examples` directory: https://gitlab.compute.dtu.dk/tuhe/unitgrade_private/-/tree/master/examples
 
 ## A simple example
 Unitgrade makes the following assumptions:
  - Your code is in python
  - Whatever you want to do can be specified as a `unittest`
 
 Although not required, it is recommended you maintain two version of the code: 
@@ -86,15 +96,14 @@
         self.assertEqual(add(2,2), 4)
         self.assertEqual(add(-100, 5), -95)
 
     def test_reverse(self):
         self.assertEqual(reverse_list([1,2,3]), [3,2,1]) 
 ```
 A number of tests can be collected into a `Report`, which will allow us to assign points to the tests and use the more advanced features of the framework later. A complete, minimal example:
-
 ```python
 # example_simplest/instructor/cs101/report1.py
 import unittest 
 from unitgrade import Report, evaluate_report_student
 import cs101
 from cs101.homework1 import reverse_list, add 
 
@@ -114,27 +123,20 @@
 if __name__ == "__main__":
     evaluate_report_student(Report1()) 
 ```
 
 ### Deployment
 The above is all you need if you simply want to use the framework as a self-check: Students can run the code and see how well they did. 
 In order to begin using the framework for evaluation we need to create a bit more structure. We do that by deploying the report class as follows:
-
 ```python
 # example_simplest/instructor/cs101/deploy.py
 from cs101.report1 import Report1 
 from unitgrade_private.hidden_create_files import setup_grade_file_report
 from snipper import snip_dir
 
-a = 34 #!i
-print(a)
-a
-z = 23 #!i
-
-
 if __name__ == "__main__":
     setup_grade_file_report(Report1)  # Make the report1_grade.py report file
 
     # Deploy the files using snipper: https://gitlab.compute.dtu.dk/tuhe/snipper
     snip_dir("./", "../../students/cs101", exclude=['__pycache__', '*.token', 'deploy.py']) 
 ```
  - The first line creates the `report1_grade.py` script and any additional data files needed by the tests (none in this case)
@@ -191,15 +193,15 @@
 If this is not enough, you can consider using `pyarmor` on the `_grade.py` script to create a **very** difficult challenge for a prospective hacker.
 
 ## Example 2: The framework
 One of the main advantages of `unitgrade` over web-based autograders it that tests are really easy to develop and maintain. To take advantage of this, we simply change the class the questions inherit from to `UTestCase` (this is still a `unittest.TestCase`) and we can make use of the chache system. As an example:
 
 ```python 
 # example_framework/instructor/cs102/report2.py
-from unitgrade2 import UTestCase 
+from unitgrade import UTestCase 
 
 class Week1(UTestCase):
     def test_add(self):
         self.assertEqualC(add(2,2))
         self.assertEqualC(add(-100, 5))
 
     def test_reverse(self):
@@ -230,29 +232,29 @@
 When this is run, the titles are shown as follows:
 ```terminal
  _   _       _ _   _____               _      
 | | | |     (_) | |  __ \             | |     
 | | | |_ __  _| |_| |  \/_ __ __ _  __| | ___ 
 | | | | '_ \| | __| | __| '__/ _` |/ _` |/ _ \
 | |_| | | | | | |_| |_\ \ | | (_| | (_| |  __/
- \___/|_| |_|_|\__|\____/_|  \__,_|\__,_|\___| v0.1.0, started: 09/09/2021 19:52:23
+ \___/|_| |_|_|\__|\____/_|  \__,_|\__,_|\___| v0.1.5, started: 16/09/2021 17:42:18
 
 CS 101 Report 2 (use --help for options)
 Question 1: Week1                                                                                                       
  * q1.1) test_add...................................................................................................PASS
  * q1.2) test_reverse...............................................................................................PASS
  * q1.3) test_output_capture........................................................................................PASS
  * q1)   Total.................................................................................................... 10/10
  
 Question 2: The same problem as before with nicer titles                                                                
  * q2.1) Test the addition method add(a,b)..........................................................................PASS
  * q2.2) Checking if reverse_list([1, 2, 3]) = [3, 2, 1]............................................................PASS
  * q2)   Total...................................................................................................... 8/8
  
-Total points at 19:52:23 (0 minutes, 0 seconds)....................................................................18/18
+Total points at 17:42:18 (0 minutes, 0 seconds)....................................................................18/18
 
 ```
 What happens behind the scenes when we set `self.title` is that the result is pre-computed on the instructors machine and cached. This means the last test will display the correct result regardless of how `reverse_list` has been implemented by the student. The titles are also shown correctly when the method is run as a unittest. 
 
 ### Caching computations
 The `@cache`-decorator offers a direct ways to compute the correct result on an instructors computer and submit it to the student. For instance:
 ```python
@@ -285,26 +287,29 @@
 ## Example 3: Hidden and secure tests
 To use `unitgrade` as part of automatic grading, it is recommended you check the students output locally and use hidden tests. Fortunately, this is very easy.
 
 Let's start with the hidden tests. As usual we write a complete report script (`report3_complete.py`), but this time we use the `@hide`-decorator to mark tests as hidden:
 
 ```python
 # example_docker/instructor/cs103/report3_complete.py
-from unitgrade import UTestCase, Report, hide 
+from unitgrade import UTestCase, Report
+from unitgrade.utils import hide
 from unitgrade import evaluate_report_student
 import cs103
 
+
 class AutomaticPass(UTestCase):
     def test_automatic_pass(self):
         self.assertEqual(2, 2)  # For simplicity, this test will always pass
 
     @hide  # The @hide-decorator tells unitgrade_v1 to hide the test for students.
     def test_hidden_fail(self):
         self.assertEqual(2, 3)  # For simplicity, this test will always fail.
 
+
 class Report3(Report):
     title = "CS 101 Report 3"
     questions = [(AutomaticPass, 10)]  # Include a single question for 10 credits.
     pack_imports = [cs103] 
 ```
 For simplicity, non-hidden test will always pass, and the hidden test will always fail: This makes it easy to interpret the results in the following.
 
@@ -321,18 +326,20 @@
     student_directory = "../../students/cs103"
     snip_dir("./", student_directory, exclude=['__pycache__', '*.token', 'deploy.py', 'report3_complete*.py', '.*']) 
 ```
 Just to check, let's have a quick look at the students report script `report3.py`:
 
 ```python
 # example_docker/instructor/cs103/report3.py
-from unitgrade import UTestCase, Report, hide 
+from unitgrade import UTestCase, Report
+from unitgrade.utils import hide
 from unitgrade import evaluate_report_student
 import cs103
 
+
 class AutomaticPass(UTestCase):
     def test_automatic_pass(self):
         self.assertEqual(2, 2)  # For simplicity, this test will always pass
 
 
 class Report3(Report):
     title = "CS 101 Report 3"
@@ -406,15 +413,15 @@
 /submissions/<student-id-2>/Report1_130_of_144.token
 ...
 ```
 The files in the whitelist/student directory can be either `.token` files (which are unpacked) or python files, and they may contain subdirectories: Everything will be unpacked and flattened. The simplest way to set it up is simply to download all files from DTU learn as a zip-file and unzip it somewhere.
 When done just call moss as follows:
 ```python 
 # example_moss/moss_example.py
-from unitgrade_private2.plagiarism.mossit import moss_it, get_id 
+from unitgrade_private.plagiarism.mossit import moss_it, get_id 
 
 if __name__ == "__main__":
     # Extract the moss id ("12415...") from the perl script and test:
     id = get_id("../../../02465private/admin/moss.pl")
     moss_it(whitelist_dir="whitelist", submissions_dir="student_submissions", moss_id=id) 
 ```
 This will generate a report. You can see the example including the report here: https://lab.compute.dtu.dk/tuhe/unitgrade_private/-/tree/master/examples/example_moss
@@ -452,35 +459,35 @@
 # example_hints/instructor/cs106/report1hints.py
 class Week1(UTestCase): 
     def test_find_all_primes(self):
         """
         Hints:
             * Insert a breakpoint and check what your function find_primes(4) actually outputs
         """
-        self.assertEqual(find_primes(4), [2,3])
+        self.assertEqual(find_primes(4), [2, 3], msg="The list should only contain primes <= 4")
 
 class Report1Hints(Report):
     title = "CS 106 Report 1"
     questions = [(Week1, 10)]
-    pack_imports = [homework1]  
+    pack_imports = [homework_hints]  
 ```
 
 When students run this homework it will fail and display the hints from the two methods:
 ![alt text|small](https://gitlab.compute.dtu.dk/tuhe/unitgrade_private/-/raw/master/docs/hints.png)
 
 What happens behind the scenes is that a code-coverage tool is run on the instructors computer
 to determine which methods are actually used in solving a problem, and then the hint-texts of those methods are 
 collected and displayed. This feature requires no external configuration; simply write `Hints:` in the source code. 
 
 # Citing
 ```bibtex
 @online{unitgrade_devel,
-	title={Unitgrade-devel (0.1.2): \texttt{pip install unitgrade-devel}},
+	title={Unitgrade-devel (0.1.7): \texttt{pip install unitgrade-devel}},
 	url={https://lab.compute.dtu.dk/tuhe/unitgrade_private},
-	urldate = {2021-09-09}, 
+	urldate = {2021-09-16}, 
 	month={9},
 	publisher={Technical University of Denmark (DTU)},
 	author={Tue Herlau},
 	year={2021},
 }
 ```
```

### Comparing `unitgrade-devel-0.1.7a0/src/unitgrade_devel.egg-info/SOURCES.txt` & `unitgrade-devel-0.1.9/src/unitgrade_devel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `unitgrade-devel-0.1.7a0/src/unitgrade_private/__init__.py` & `unitgrade-devel-0.1.9/src/unitgrade_private/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-
 import os
 import compress_pickle
 from unitgrade_private.hidden_gather_upload import load_token, save_token
 from unitgrade_private.plagiarism.mossit import unpack_sources_from_token
 
-# __version__ = "0.0.1"
 
 def cache_write(object, file_name, verbose=True):
+    assert False
     dn = os.path.dirname(file_name)
     if not os.path.exists(dn):
         os.mkdir(dn)
     if verbose: print("Writing cache...", file_name)
     with open(file_name, 'wb', ) as f:
         compress_pickle.dump(object, f, compression="lzma")
     if verbose: print("Done!")
 
 
 def cache_exists(file_name):
-    # file_name = cn_(file_name) if cache_prefix else file_name
+    assert False
     return os.path.exists(file_name)
 
 
 def cache_read(file_name):
-    # file_name = cn_(file_name) if cache_prefix else file_name
+    assert False
     if os.path.exists(file_name):
         with open(file_name, 'rb') as f:
             return compress_pickle.load(f, compression="lzma")
-            # return pickle.load(f)
     else:
         return None
```

### Comparing `unitgrade-devel-0.1.7a0/src/unitgrade_private/autolab/autolab.py` & `unitgrade-devel-0.1.9/src/unitgrade_private/autolab/autolab.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from zipfile import ZipFile
 from os.path import basename
 import os
 import shutil
 from jinja2 import Environment, FileSystemLoader
 import glob
 import pickle
-from src.unitgrade.unitgrade import Report
+from src.unitgrade.framework import Report
 from unitgrade_private import docker_helpers
 
 COURSES_BASE = "/home/tuhe/Autolab/courses/AutoPopulated"
 
 CURDIR = os.path.dirname(__file__)
 TEMPLATE_BASE = CURDIR + "/lab_template"
```

### Comparing `unitgrade-devel-0.1.7a0/src/unitgrade_private/deployment.py` & `unitgrade-devel-0.1.9/src/unitgrade_private/deployment.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import inspect
-from unitgrade.unitgrade import methodsWithDecorator, hide
+from unitgrade.utils import hide, methodsWithDecorator
 import os
 import importlib
 
+
 def remove_hidden_methods(ReportClass, outfile=None):
     # Given a ReportClass, clean out all @hidden tests from the imports of that class.
     file = ReportClass()._file()
     with open(file, 'r') as f:
         source = f.read().splitlines()
 
     lines_to_rem = []
 
     for Q,_ in ReportClass.questions:
-        print(Q)
         ls = list(methodsWithDecorator(Q, hide))
         print("hide decorateed is", ls)
         for f in ls:
             s, start = inspect.getsourcelines(f)
             end = len(s) + start
             lines_to_rem += list(range(start-1, end-1))
 
@@ -27,17 +27,15 @@
         outfile = file[:-3] + "_nohidden.py"
 
     if os.path.exists(outfile) and os.path.samefile(file, outfile):
         raise Exception("Similar file paths identified!")
     with open(outfile, 'w') as f:
         f.write(source)
 
-    mname = ReportClass.__module__
-    mname.find(".")
-    mname = mname[:mname.rfind(".")] + "." + os.path.basename(outfile)[:-3]
+    module_name = ReportClass.__module__
+    module_name.find(".")
+    module_name = module_name[:module_name.rfind(".")] + "." + os.path.basename(outfile)[:-3]
 
-    module = importlib.import_module(mname)
+    module = importlib.import_module(module_name)
 
     HiddenReportClass = getattr(module, ReportClass.__name__)
     return outfile, HiddenReportClass
-
-
```

### Comparing `unitgrade-devel-0.1.7a0/src/unitgrade_private/docker_helpers.py` & `unitgrade-devel-0.1.9/src/unitgrade_private/docker_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,19 @@
     docker run -v c:/Users/tuhe/Documents/2021/python-docker/tmp:/app python-docker > output.log
 
     """
     # A bunch of tests. This is going to be great!
     assert os.path.exists(Dockerfile_location)
     start = time.time()
 
-    with open(student_token_file, 'rb') as f:
-        results = pickle.load(f)
+    # with open(student_token_file, 'rb') as f:
+    #     results = pickle.load(f)
+    from unitgrade_private import load_token
+    results, _ = load_token(student_token_file)
+
     sources = results['sources'][0]
 
     if os.path.exists(host_tmp_dir):
         shutil.rmtree(host_tmp_dir)
 
     with io.BytesIO(sources['zipfile']) as zb:
         with zipfile.ZipFile(zb) as zip:
```

### Comparing `unitgrade-devel-0.1.7a0/src/unitgrade_private/hidden_create_files.py` & `unitgrade-devel-0.1.9/src/unitgrade_private/hidden_create_files.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from unitgrade import unitgrade_helpers
+from unitgrade import evaluate
 import jinja2
 import pickle
 import inspect
 import time
 import os
 from unitgrade_private import hidden_gather_upload
 import sys
@@ -15,56 +15,34 @@
 name="{{Report1}}"
 
 report = source_instantiate(name, report1_source, report1_payload)
 output_dir = os.path.dirname(__file__)
 gather_upload_to_campusnet(report, output_dir)
 """
 
-def setup_answers(report):
-    """
-    Obtain student answers by executing the test in the report and then same them to the disk.
-    """
-    assert False
-    payloads = {}
-    import tabulate
-
-    from collections import defaultdict
-    rs = defaultdict(lambda: [])
-    for q, _ in report.questions:
-        # for q, _ in report.questions:
-        q()._save_cache()
-
-        q.name = q.__class__
-        payloads[q.name] = {}
-        print("> Setting up question", q)
-        # start = time.time()
-        # q.init_all_item_questions() # Initialize all this questions items questions (i.e. make sure the items can run).
-        # payloads[q.name]['time'] = time.time()-start
-        # for item in q.items:
-        #     print("    Setting up item", item)
-        #     start = time.time()
-        #     item._precomputed_payload = item.precompute_payload()
-        #     answer = item.compute_answer(unmute=True)
-        #
-        #     rs['Name'].append(str(item))
-        #     rs['Answer'].append( sys.getsizeof(pickle.dumps(answer)) )
-        #     rs['Precomputed'].append( sys.getsizeof( pickle.dumps(item._precomputed_payload)))
-        #     payloads[q.name][item.name] = {'payload': answer, 'precomputed': item._precomputed_payload, 'time': time.time() - start, 'title': item.title}
-
-    print(tabulate.tabulate(rs, headers="keys"))
-    # cache_write(payloads, report.computed_answers_file, verbose=False)
-
 
 def strip_main(report1_source):
     dx = report1_source.find("__main__")
     report1_source = report1_source[:dx]
     report1_source = report1_source[:report1_source.rfind("\n")]
     return report1_source
 
 
+def rmimports(s, excl):
+    s = "\n".join([l for l in s.splitlines() if not any([l.strip().startswith(e) for e in excl])])
+    return s
+
+def lload(flist, excl):
+    s = ""
+    for fname in flist:
+        with open(fname, 'r', encoding="utf-8") as f:
+            s += f.read() + "\n" + "\n"
+    s = rmimports(s, excl)  # remove import statements from helper class.
+    return s
+
 def setup_grade_file_report(ReportClass, execute=False, obfuscate=False, minify=False, bzip=True, nonlatin=False, source_process_fun=None, with_coverage=True):
     print("Setting up answers...")
     report = ReportClass()
     payload = report._setup_answers(with_coverage=with_coverage)
     payload['config'] = {}
     from unitgrade_private.hidden_gather_upload import gather_report_source_include
     sources = gather_report_source_include(report)
@@ -90,30 +68,23 @@
     import unitgrade
     excl = ["unitgrade.unitgrade_helpers",
             "from . import",
             "from unitgrade.",
             "from unitgrade ",
             "import unitgrade"]
 
-    def rmimports(s, excl):
-        s = "\n".join([l for l in s.splitlines() if not any([l.strip().startswith(e) for e in excl])])
-        return s
-
-    def lload(flist, excl):
-        s = ""
-        for fname in flist:
-            with open(fname, 'r', encoding="utf-8") as f:
-                s += f.read() + "\n" + "\n"
-        s = rmimports(s, excl)  # remove import statements from helper class.
-        return s
     report1_source = rmimports(report1_source, excl)
 
-    pyhead = lload([unitgrade_helpers.__file__, hidden_gather_upload.__file__], excl)
+    pyhead = lload([evaluate.__file__, hidden_gather_upload.__file__], excl)
     from unitgrade import version
-    report1_source = lload([unitgrade.__file__, unitgrade.unitgrade.__file__, unitgrade_helpers.__file__, hidden_gather_upload.__file__, version.__file__], excl) + "\n" + report1_source
+    from unitgrade import utils
+    print(unitgrade.__file__)
+    report1_source = lload([unitgrade.__file__, unitgrade.framework.__file__, utils.__file__,
+                            unitgrade.evaluate.__file__, hidden_gather_upload.__file__,
+                            version.__file__], excl) + "\n" + report1_source
 
     print(sys.getsizeof(picklestring))
     print(len(picklestring))
     s = jinja2.Environment().from_string(data).render({'Report1': ReportClass.__name__,
                                                        'source': repr(report1_source),
                                                        'payload': picklestring.hex(), #repr(picklestring),
                                                        'token_out': repr(fn[:-3] + "_handin"),
@@ -135,15 +106,15 @@
 
         cmd = f'pyminifier {obs} {" ".join(extra)} -o {output} {output}'
         print(cmd)
         os.system(cmd)
         time.sleep(0.2)
         with open(output, 'r') as f:
             sauce = f.read().splitlines()
-        wa = """WARNING: Modifying, decompiling or otherwise tampering with this script, it's data or the resulting .token file will be investigated as a cheating attempt."""
+        wa = """ WARNING: Modifying, decompiling or otherwise tampering with this script, it's data or the resulting .token file will be investigated as a cheating attempt. """
         sauce = ["'''" + wa + "'''"] + sauce[:-1]
         sauce = "\n".join(sauce)
         with open(output, 'w') as f:
             f.write(sauce)
 
     if execute:
         time.sleep(0.1)
```

### Comparing `unitgrade-devel-0.1.7a0/src/unitgrade_private/hidden_gather_upload.py` & `unitgrade-devel-0.1.9/src/unitgrade_private/hidden_gather_upload.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from unitgrade.unitgrade_helpers import evaluate_report, python_code_str_id, file_id
+from unitgrade.evaluate import evaluate_report, python_code_str_id
 import lzma
 import base64
 import textwrap
 import hashlib
 import bz2
 import pickle
 import os
@@ -10,14 +10,15 @@
 import io
 
 
 def bzwrite(json_str, token): # to get around obfuscation issues
     with getattr(bz2, 'open')(token, "wt") as f:
         f.write(json_str)
 
+
 def gather_imports(imp):
     resources = {}
     m = imp
     f = m.__file__
     if hasattr(m, '__file__') and not hasattr(m, '__path__'):
         top_package = os.path.dirname(m.__file__)
         module_import = True
@@ -81,18 +82,17 @@
             nimp, top_package = gather_imports(m)
             _, report_relative_location, module_import = report._import_base_relative()
 
             nimp['report_relative_location'] = report_relative_location
             nimp['report_module_specification'] = module_import
             nimp['name'] = m.__name__
             sources[k] = nimp
-            # if len([k for k in nimp if k not in sources]) > 0:
             print(f" * {m.__name__}")
     return sources
-                # sources = {**sources, **nimp}
+
 
 def gather_upload_to_campusnet(report, output_dir=None):
     # n = report.nL
     args = parser.parse_args()
     results, table_data = evaluate_report(report, show_help_flag=False, show_expected=False, show_computed=False, silent=True,
                                           show_progress_bar=not args.noprogress,
                                           big_header=not args.autolab)
@@ -166,51 +166,41 @@
 token_sep = "-"*70 + " ..ooO0Ooo.. " + "-"*70
 def save_token(dictionary, plain_text, file_out):
     if plain_text is None:
         plain_text = ""
     if len(plain_text) == 0:
         plain_text = "Start token file"
     plain_text = plain_text.strip()
-
-    # hexed = lzma.compress(pickle.dumps(dictionary))
-    # b_hash = hashlib.blake2b(b).hexdigest()
-
     b, b_hash = dict2picklestring(dictionary)
     b_l1 = len(b)
-    # b_l1 = len(hexed)
-    # b = base64.b64encode(hexed).decode("utf-8")
-    # b_l2 = len(b)
     b = "."+b+"."
-    b = "\n".join( textwrap.wrap(b, 180) )
+    b = "\n".join( textwrap.wrap(b, 180))
 
     out = [plain_text, token_sep, f"{b_hash} {b_l1}", token_sep, b]
     with open(file_out, 'w') as f:
         f.write("\n".join(out))
 
+
 def load_token(file_in):
     with open(file_in, 'r') as f:
         s = f.read()
     splt = s.split(token_sep)
     data = splt[-1]
     info = splt[-2]
     head = token_sep.join(splt[:-2])
     plain_text=head.strip()
     hash, l1 = info.split(" ")
     data = "".join( data.strip()[1:-1].splitlines() )
     l1 = int(l1)
-    # l2 = int(l2)
 
     dictionary, b_hash = picklestring2dict(data)
 
-    # b = base64.b64decode(data)
-    # dictionary = pickle.loads(lzma.decompress(b))
-    # assert len(data) == l2
     assert len(data) == l1
     assert b_hash == hash.strip()
     return dictionary, plain_text
 
+
 def source_instantiate(name, report1_source, payload):
     eval("exec")(report1_source, globals())
     pl = pickle.loads(bytes.fromhex(payload))
     report = eval(name)(payload=pl, strict=True)
-    # report.set_payload(pl)
     return report
```

### Comparing `unitgrade-devel-0.1.7a0/src/unitgrade_private/plagiarism/mossit.py` & `unitgrade-devel-0.1.9/src/unitgrade_private/plagiarism/mossit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from unitgrade.unitgrade_helpers import file_id
+from unitgrade.evaluate import file_id
 import os
 import shutil
 import glob
 from unitgrade_private.token_loader import unpack_sources_from_token
 import mosspy
 
 
@@ -36,27 +36,26 @@
                 continue
             print("> Including", py)
             shutil.copy(py, tmp_student_dir + f"/{k}_" + os.path.basename(py))
 
     return tmp_base, tmp_submission_dir
 
 
-def ensure_tokens_unpacked(dir, flat=True):
-    tokens = glob.glob(dir +"/*/*.token", recursive=True)
+def ensure_tokens_unpacked(directory, flat=True):
+    tokens = glob.glob(directory + "/*/*.token", recursive=True)
     for t in tokens:
         unpack_sources_from_token(t)
 
 
 def get_id(moss_pl):
     with open(moss_pl, "r") as f:
-        pl = [l for l in f.read().splitlines() if "$userid=" in l].pop()
+        pl = [line for line in f.read().splitlines() if "$userid=" in line].pop()
     return pl.split("=")[1][:-1]
 
 
-
 def moss_it(whitelist_dir="", submissions_dir="", moss_id=None):
     whitelist_dir = os.path.abspath(whitelist_dir)
     ensure_tokens_unpacked(whitelist_dir)
     ensure_tokens_unpacked(submissions_dir)
     tmp_base, tmp_submission_dir = moss_prepare(whitelist_dir, submissions_dir)
 
     userid = int(moss_id)
@@ -68,11 +67,11 @@
     url = m.send(lambda file_path, display_name: print('*', end='', flush=True))
     print()
     print("Report Url: " + url)
     report_dir = os.path.dirname(whitelist_dir) + "/report"
     if not os.path.isdir(report_dir):
         os.mkdir(report_dir)
 
-    r = report_dir +"/report.html"
+    r = report_dir + "/report.html"
     m.saveWebPage(url, r)
     print("Saved report to:", r)
-    mosspy.download_report(url, report_dir, connections=8, log_level=10, on_read=lambda url: print('*', end='', flush=True))
+    mosspy.download_report(url, report_dir, connections=8, log_level=10, on_read=lambda u: print('*', end='', flush=True))
```

