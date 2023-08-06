# Comparing `tmp/PyDSAlgo-1.0.1.tar.gz` & `tmp/PyDSAlgo-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDSAlgo-1.0.1.tar", last modified: Tue Jul 25 04:39:02 2023, max compression
+gzip compressed data, was "PyDSAlgo-1.1.0.tar", last modified: Sun Aug  6 10:56:53 2023, max compression
```

## Comparing `PyDSAlgo-1.0.1.tar` & `PyDSAlgo-1.1.0.tar`

### file list

```diff
@@ -1,48 +1,79 @@
-drwxrwxr-x   0 mindfreek  (1000) mindfreek  (1000)        0 2023-07-25 04:39:02.341938 PyDSAlgo-1.0.1/
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     1069 2023-06-05 09:59:08.000000 PyDSAlgo-1.0.1/LICENSE
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     3599 2023-07-25 04:39:02.341938 PyDSAlgo-1.0.1/PKG-INFO
-drwxrwxr-x   0 mindfreek  (1000) mindfreek  (1000)        0 2023-07-25 04:39:02.337938 PyDSAlgo-1.0.1/PyDSAlgo.egg-info/
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     3599 2023-07-25 04:39:02.000000 PyDSAlgo-1.0.1/PyDSAlgo.egg-info/PKG-INFO
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     1051 2023-07-25 04:39:02.000000 PyDSAlgo-1.0.1/PyDSAlgo.egg-info/SOURCES.txt
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)        1 2023-07-25 04:39:02.000000 PyDSAlgo-1.0.1/PyDSAlgo.egg-info/dependency_links.txt
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)        6 2023-07-25 04:39:02.000000 PyDSAlgo-1.0.1/PyDSAlgo.egg-info/top_level.txt
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     2865 2023-07-25 04:19:01.000000 PyDSAlgo-1.0.1/README.md
-drwxrwxr-x   0 mindfreek  (1000) mindfreek  (1000)        0 2023-07-25 04:39:02.337938 PyDSAlgo-1.0.1/pyDSA/
-drwxrwxr-x   0 mindfreek  (1000) mindfreek  (1000)        0 2023-07-25 04:39:02.337938 PyDSAlgo-1.0.1/pyDSA/DS/
-drwxrwxr-x   0 mindfreek  (1000) mindfreek  (1000)        0 2023-07-25 04:39:02.337938 PyDSAlgo-1.0.1/pyDSA/DS/Graph/
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     1676 2023-07-24 15:34:28.000000 PyDSAlgo-1.0.1/pyDSA/DS/Graph/PyGraph.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     2063 2023-07-20 17:23:10.000000 PyDSAlgo-1.0.1/pyDSA/DS/Graph/PyLinkedGraph.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)        0 2023-07-20 17:16:21.000000 PyDSAlgo-1.0.1/pyDSA/DS/Graph/__init__.py
-drwxrwxr-x   0 mindfreek  (1000) mindfreek  (1000)        0 2023-07-25 04:39:02.337938 PyDSAlgo-1.0.1/pyDSA/DS/Heap/
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     1610 2023-07-24 17:20:37.000000 PyDSAlgo-1.0.1/pyDSA/DS/Heap/PyMaxHeap.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     1618 2023-07-24 17:20:37.000000 PyDSAlgo-1.0.1/pyDSA/DS/Heap/PyMinHeap.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)        0 2023-07-24 16:53:56.000000 PyDSAlgo-1.0.1/pyDSA/DS/Heap/__init__.py
-drwxrwxr-x   0 mindfreek  (1000) mindfreek  (1000)        0 2023-07-25 04:39:02.337938 PyDSAlgo-1.0.1/pyDSA/DS/LinkedList/
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     1798 2023-07-24 17:53:59.000000 PyDSAlgo-1.0.1/pyDSA/DS/LinkedList/PyCircularLinkedList.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     2004 2023-07-24 17:53:57.000000 PyDSAlgo-1.0.1/pyDSA/DS/LinkedList/PyDoublyCircularLinkedLIst.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     1396 2023-07-24 17:27:59.000000 PyDSAlgo-1.0.1/pyDSA/DS/LinkedList/PyDoublyLinkedList.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     1223 2023-07-24 17:53:59.000000 PyDSAlgo-1.0.1/pyDSA/DS/LinkedList/PyHeaderLinkedList.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     1090 2023-06-10 04:12:36.000000 PyDSAlgo-1.0.1/pyDSA/DS/LinkedList/PyLinkedList.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     1624 2023-07-24 17:53:57.000000 PyDSAlgo-1.0.1/pyDSA/DS/LinkedList/PySkipLinkedList.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)        0 2023-06-10 04:19:54.000000 PyDSAlgo-1.0.1/pyDSA/DS/LinkedList/__init__.py
-drwxrwxr-x   0 mindfreek  (1000) mindfreek  (1000)        0 2023-07-25 04:39:02.337938 PyDSAlgo-1.0.1/pyDSA/DS/Queue/
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     1282 2023-06-10 04:12:36.000000 PyDSAlgo-1.0.1/pyDSA/DS/Queue/PyCircularQueue.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     1001 2023-06-10 04:19:11.000000 PyDSAlgo-1.0.1/pyDSA/DS/Queue/PyDeque.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     1033 2023-06-10 04:12:36.000000 PyDSAlgo-1.0.1/pyDSA/DS/Queue/PyPriorityQueue.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)      641 2023-06-10 04:12:36.000000 PyDSAlgo-1.0.1/pyDSA/DS/Queue/PyQueue.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)        0 2023-06-10 04:19:14.000000 PyDSAlgo-1.0.1/pyDSA/DS/Queue/__init__.py
-drwxrwxr-x   0 mindfreek  (1000) mindfreek  (1000)        0 2023-07-25 04:39:02.341938 PyDSAlgo-1.0.1/pyDSA/DS/Stack/
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)      591 2023-06-10 04:12:36.000000 PyDSAlgo-1.0.1/pyDSA/DS/Stack/PyStack.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)        0 2023-06-10 04:19:49.000000 PyDSAlgo-1.0.1/pyDSA/DS/Stack/__init__.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)      854 2023-06-10 04:24:12.000000 PyDSAlgo-1.0.1/pyDSA/DS/Stack/pyLinkedStack.py
-drwxrwxr-x   0 mindfreek  (1000) mindfreek  (1000)        0 2023-07-25 04:39:02.341938 PyDSAlgo-1.0.1/pyDSA/DS/Tree/
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     2710 2023-07-24 17:53:57.000000 PyDSAlgo-1.0.1/pyDSA/DS/Tree/PyAVLTree.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     7907 2023-07-24 17:53:59.000000 PyDSAlgo-1.0.1/pyDSA/DS/Tree/PyBTree.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     2096 2023-07-24 15:34:28.000000 PyDSAlgo-1.0.1/pyDSA/DS/Tree/PyBinarySearchTree.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     1587 2023-07-24 16:33:58.000000 PyDSAlgo-1.0.1/pyDSA/DS/Tree/PyBinaryTree.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     1902 2023-07-24 17:20:37.000000 PyDSAlgo-1.0.1/pyDSA/DS/Tree/PyGenericTree.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)        0 2023-06-10 04:27:29.000000 PyDSAlgo-1.0.1/pyDSA/DS/Tree/__init__.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)      472 2023-06-10 04:12:36.000000 PyDSAlgo-1.0.1/pyDSA/DS/__init__.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)        0 2023-06-05 10:01:37.000000 PyDSAlgo-1.0.1/pyDSA/__init__.py
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)       38 2023-07-25 04:39:02.341938 PyDSAlgo-1.0.1/setup.cfg
--rw-rw-r--   0 mindfreek  (1000) mindfreek  (1000)     1129 2023-07-25 04:38:22.000000 PyDSAlgo-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:56:53.716565 PyDSAlgo-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-08-06 10:56:53.716565 PyDSAlgo-1.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:56:53.712565 PyDSAlgo-1.1.0/PyDSAlgo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-08-06 10:56:53.000000 PyDSAlgo-1.1.0/PyDSAlgo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-06 10:56:53.000000 PyDSAlgo-1.1.0/PyDSAlgo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 10:56:53.000000 PyDSAlgo-1.1.0/PyDSAlgo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 10:56:53.000000 PyDSAlgo-1.1.0/PyDSAlgo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:56:53.712565 PyDSAlgo-1.1.0/pyDSAlgo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:56:53.712565 PyDSAlgo-1.1.0/pyDSAlgo/Algo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:56:53.716565 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/Py3WayMergeSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/PyBIngoSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/PyBitonicSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/PyBogoSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/PyBubbleSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/PyBucketSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/PyCocktailSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/PyCombSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/PyCountingSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/PyCycleSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/PyGnomeSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/PyHeapSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/PyInsertionSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/PyMergeSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/PyOddEvenSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/PyPancakeSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/PyPigeonholeSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/PyQuickSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/PyRadixSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/PySelectionSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/PyShellSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/PySleepSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/PyStoogeSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/PyStrandSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/PyTagSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/PyTimSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/PyTreeSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/Sorting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/Algo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:56:53.716565 PyDSAlgo-1.1.0/pyDSAlgo/DS/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:56:53.716565 PyDSAlgo-1.1.0/pyDSAlgo/DS/Graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/Graph/PyGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/Graph/PyLinkedGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/Graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:56:53.716565 PyDSAlgo-1.1.0/pyDSAlgo/DS/Heap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/Heap/PyMaxHeap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/Heap/PyMinHeap.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/Heap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:56:53.716565 PyDSAlgo-1.1.0/pyDSAlgo/DS/LinkedList/
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/LinkedList/PyCircularLinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/LinkedList/PyDoublyCircularLinkedLIst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/LinkedList/PyDoublyLinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/LinkedList/PyHeaderLinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/LinkedList/PyLinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/LinkedList/PySkipLinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/LinkedList/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:56:53.716565 PyDSAlgo-1.1.0/pyDSAlgo/DS/Queue/
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/Queue/PyCircularQueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/Queue/PyDeque.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/Queue/PyPriorityQueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/Queue/PyQueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/Queue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:56:53.716565 PyDSAlgo-1.1.0/pyDSAlgo/DS/Stack/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/Stack/PyStack.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/Stack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/Stack/pyLinkedStack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:56:53.716565 PyDSAlgo-1.1.0/pyDSAlgo/DS/Tree/
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/Tree/PyAVLTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/Tree/PyBTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/Tree/PyBinarySearchTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/Tree/PyBinaryTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/Tree/PyGenericTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/Tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/DS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/pyDSAlgo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 10:56:53.716565 PyDSAlgo-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-08-06 10:56:40.000000 PyDSAlgo-1.1.0/setup.py
```

### Comparing `PyDSAlgo-1.0.1/LICENSE` & `PyDSAlgo-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyDSAlgo-1.0.1/pyDSA/DS/Graph/PyGraph.py` & `PyDSAlgo-1.1.0/pyDSAlgo/DS/Graph/PyGraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyDSA.DS import PyDS
+from pyDSAlgo.DS import PyDS
 
 
 class PyGraph(PyDS):
     def __init__(self):
         super().__init__()
         self.adjacency_list = {}
```

### Comparing `PyDSAlgo-1.0.1/pyDSA/DS/Graph/PyLinkedGraph.py` & `PyDSAlgo-1.1.0/pyDSAlgo/DS/Graph/PyLinkedGraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyDSA.DS import PyDS
+from pyDSAlgo.DS import PyDS
 
 
 class Node:
     def __init__(self, vertex):
         self.vertex = vertex
         self.next = None
```

### Comparing `PyDSAlgo-1.0.1/pyDSA/DS/Heap/PyMaxHeap.py` & `PyDSAlgo-1.1.0/pyDSAlgo/DS/Heap/PyMaxHeap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyDSA.DS import PyDS
+from pyDSAlgo.DS import PyDS
 
 
 class PyMaxHeap(PyDS):
     def __init__(self):
         super().__init__()
         self.heap = []
```

### Comparing `PyDSAlgo-1.0.1/pyDSA/DS/Heap/PyMinHeap.py` & `PyDSAlgo-1.1.0/pyDSAlgo/DS/Heap/PyMinHeap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyDSA.DS import PyDS
+from pyDSAlgo.DS import PyDS
 
 
 class PyMinHeap(PyDS):
     def __init__(self):
         super().__init__()
         self.heap = []
```

### Comparing `PyDSAlgo-1.0.1/pyDSA/DS/LinkedList/PyCircularLinkedList.py` & `PyDSAlgo-1.1.0/pyDSAlgo/DS/LinkedList/PyCircularLinkedList.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyDSA.DS import PyDS
+from pyDSAlgo.DS import PyDS
 
 
 class Node:
     def __init__(self, data):
         self.data = data
         self.next = None
```

### Comparing `PyDSAlgo-1.0.1/pyDSA/DS/LinkedList/PyDoublyCircularLinkedLIst.py` & `PyDSAlgo-1.1.0/pyDSAlgo/DS/LinkedList/PyDoublyCircularLinkedLIst.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyDSA.DS import PyDS
+from pyDSAlgo.DS import PyDS
 
 
 class Node:
     def __init__(self, data):
         self.data = data
         self.prev = None
         self.next = None
```

### Comparing `PyDSAlgo-1.0.1/pyDSA/DS/LinkedList/PyDoublyLinkedList.py` & `PyDSAlgo-1.1.0/pyDSAlgo/DS/LinkedList/PyDoublyLinkedList.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from pyDSA.DS import PyDS
+from pyDSAlgo.DS import PyDS
 
 
 class Node:
     def __init__(self, data):
         self.data = data
         self.prev = None
         self.next = None
```

### Comparing `PyDSAlgo-1.0.1/pyDSA/DS/LinkedList/PyHeaderLinkedList.py` & `PyDSAlgo-1.1.0/pyDSAlgo/DS/LinkedList/PyHeaderLinkedList.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from pyDSA.DS import PyDS
+from pyDSAlgo.DS import PyDS
 
 
 class Node:
     def __init__(self, data=None):
         self.data = data
         self.next = None
```

### Comparing `PyDSAlgo-1.0.1/pyDSA/DS/LinkedList/PyLinkedList.py` & `PyDSAlgo-1.1.0/pyDSAlgo/DS/LinkedList/PyLinkedList.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyDSA.DS import PyDS
+from pyDSAlgo.DS import PyDS
 
 
 class Node:
     def __init__(self, data):
         self.data = data
         self.next = None
```

### Comparing `PyDSAlgo-1.0.1/pyDSA/DS/LinkedList/PySkipLinkedList.py` & `PyDSAlgo-1.1.0/pyDSAlgo/DS/LinkedList/PySkipLinkedList.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import random
 
-from pyDSA.DS import PyDS
+from pyDSAlgo.DS import PyDS
 
 
 class Node:
     def __init__(self, key, forward=None):
         if forward is None:
             forward = []
         self.key = key
```

### Comparing `PyDSAlgo-1.0.1/pyDSA/DS/Queue/PyCircularQueue.py` & `PyDSAlgo-1.1.0/pyDSAlgo/DS/Queue/PyCircularQueue.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyDSA.DS import PyDS
+from pyDSAlgo.DS import PyDS
 
 
 class CircularQueue(PyDS):
     def __init__(self, k):
         super().__init__()
         self.size = k
         self.queue = [None] * k
```

### Comparing `PyDSAlgo-1.0.1/pyDSA/DS/Queue/PyDeque.py` & `PyDSAlgo-1.1.0/pyDSAlgo/DS/Queue/PyDeque.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyDSA.DS import PyDS
+from pyDSAlgo.DS import PyDS
 
 
 class PyDeque(PyDS):
     def __init__(self):
         super().__init__()
         self.items = []
```

### Comparing `PyDSAlgo-1.0.1/pyDSA/DS/Queue/PyPriorityQueue.py` & `PyDSAlgo-1.1.0/pyDSAlgo/DS/Queue/PyPriorityQueue.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyDSA.DS import PyDS
+from pyDSAlgo.DS import PyDS
 
 
 class PyPriorityQueue(PyDS):
     def __init__(self):
         super().__init__()
         self.queue = []
```

### Comparing `PyDSAlgo-1.0.1/pyDSA/DS/Queue/PyQueue.py` & `PyDSAlgo-1.1.0/pyDSAlgo/DS/Queue/PyQueue.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyDSA.DS import PyDS
+from pyDSAlgo.DS import PyDS
 
 
 class PyQueue(PyDS):
     def __init__(self):
         super().__init__()
         self.queue = []
```

### Comparing `PyDSAlgo-1.0.1/pyDSA/DS/Stack/PyStack.py` & `PyDSAlgo-1.1.0/pyDSAlgo/DS/Stack/PyStack.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyDSA.DS import PyDS
+from pyDSAlgo.DS import PyDS
 
 
 class PyStack(PyDS):
     def __init__(self):
         super().__init__()
         self.stack = []
```

### Comparing `PyDSAlgo-1.0.1/pyDSA/DS/Stack/pyLinkedStack.py` & `PyDSAlgo-1.1.0/pyDSAlgo/DS/Stack/pyLinkedStack.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyDSA.DS import PyDS
+from pyDSAlgo.DS import PyDS
 
 
 class Node:
     def __init__(self, data):
         self.data = data
         self.next = None
```

### Comparing `PyDSAlgo-1.0.1/pyDSA/DS/Tree/PyAVLTree.py` & `PyDSAlgo-1.1.0/pyDSAlgo/DS/Tree/PyAVLTree.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyDSA.DS import PyDS
+from pyDSAlgo.DS import PyDS
 
 
 class Node:
     def __init__(self, key):
         self.key = key
         self.height = 1
         self.left = None
```

### Comparing `PyDSAlgo-1.0.1/pyDSA/DS/Tree/PyBTree.py` & `PyDSAlgo-1.1.0/pyDSAlgo/DS/Tree/PyBTree.py`

 * *Files identical despite different names*

### Comparing `PyDSAlgo-1.0.1/pyDSA/DS/Tree/PyBinarySearchTree.py` & `PyDSAlgo-1.1.0/pyDSAlgo/DS/Tree/PyBinarySearchTree.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyDSA.DS import PyDS
+from pyDSAlgo.DS import PyDS
 
 
 class Node:
     def __init__(self, key):
         self.key = key
         self.left = None
         self.right = None
```

### Comparing `PyDSAlgo-1.0.1/pyDSA/DS/Tree/PyBinaryTree.py` & `PyDSAlgo-1.1.0/pyDSAlgo/DS/Tree/PyBinaryTree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyDSA.DS import PyDS
+from pyDSAlgo.DS import PyDS
 
 
 class Node:
     def __init__(self, key):
         self.key = key
         self.left = None
         self.right = None
```

### Comparing `PyDSAlgo-1.0.1/pyDSA/DS/Tree/PyGenericTree.py` & `PyDSAlgo-1.1.0/pyDSAlgo/DS/Tree/PyGenericTree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyDSA.DS import PyDS
+from pyDSAlgo.DS import PyDS
 
 
 class TreeNode:
     def __init__(self, data):
         self.data = data
         self.children = []
```

### Comparing `PyDSAlgo-1.0.1/setup.py` & `PyDSAlgo-1.1.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,29 +4,38 @@
     requirements = f.read().splitlines()
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="PyDSAlgo",
-    version="1.0.1",
+    version="1.1.0",
     author="Sattyam Jain",
     author_email="sattyamjain96@gmail.com",
     description="Python Package for Data structure and algorithms implementation with its proper explanation",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/sattyamjjain/pyDSA",
+    url="https://github.com/sattyamjjain/pyDSAlgo",
     packages=find_packages(),
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.9",
     ],
-    keywords=["pydsa", "dsa", "data structure", "algo", "algorithm", "ds", "python data structure"],
+    keywords=[
+        "pydsa",
+        "pydsalgo"
+        "dsa",
+        "data structure",
+        "algo",
+        "algorithm",
+        "ds",
+        "python data structure",
+    ],
     python_requires=">=3.9",
     install_requires=requirements,
     project_urls={
-        "Bug Reports": "https://github.com/sattyamjjain/pyDSA",
-        "Source": "https://github.com/sattyamjjain/pyDSA",
+        "Bug Reports": "https://github.com/sattyamjjain/pyDSAlgo",
+        "Source": "https://github.com/sattyamjjain/pyDSAlgo",
     },
 )
```

