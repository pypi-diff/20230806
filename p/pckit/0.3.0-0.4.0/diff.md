# Comparing `tmp/pckit-0.3.0.tar.gz` & `tmp/pckit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pckit-0.3.0.tar", max compression
+gzip compressed data, was "pckit-0.4.0.tar", max compression
```

## Comparing `pckit-0.3.0.tar` & `pckit-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0     1066 2023-08-04 11:23:30.757670 pckit-0.3.0/LICENSE
--rw-r--r--   0        0        0     2287 2023-08-04 11:23:30.757670 pckit-0.3.0/README.md
--rw-r--r--   0        0        0      441 2023-08-04 11:23:30.757670 pckit-0.3.0/pckit/__init__.py
--rw-r--r--   0        0        0      109 2023-08-04 11:23:30.757670 pckit-0.3.0/pckit/_typevars.py
--rw-r--r--   0        0        0     1866 2023-08-04 11:23:30.757670 pckit-0.3.0/pckit/_utils.py
--rw-r--r--   0        0        0     1492 2023-08-04 11:23:30.757670 pckit-0.3.0/pckit/cache.py
--rw-r--r--   0        0        0     5676 2023-08-04 11:23:30.757670 pckit-0.3.0/pckit/models.py
--rw-r--r--   0        0        0     9465 2023-08-04 11:23:30.757670 pckit-0.3.0/pckit/solvers.py
--rw-r--r--   0        0        0      156 2023-08-04 11:23:30.761670 pckit-0.3.0/pckit/task.py
--rw-r--r--   0        0        0     5089 2023-08-04 11:23:30.761670 pckit-0.3.0/pckit/workers.py
--rw-r--r--   0        0        0      617 2023-08-04 11:23:30.761670 pckit-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2969 1970-01-01 00:00:00.000000 pckit-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-08-05 23:43:15.088502 pckit-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2226 2023-08-05 23:43:15.088502 pckit-0.4.0/README.md
+-rw-r--r--   0        0        0      331 2023-08-05 23:43:15.116503 pckit-0.4.0/pckit/__init__.py
+-rw-r--r--   0        0        0      109 2023-08-05 23:43:15.116503 pckit-0.4.0/pckit/_typevars.py
+-rw-r--r--   0        0        0     1143 2023-08-05 23:43:15.116503 pckit-0.4.0/pckit/_utils.py
+-rw-r--r--   0        0        0     1525 2023-08-05 23:43:15.116503 pckit-0.4.0/pckit/cache.py
+-rw-r--r--   0        0        0      110 2023-08-05 23:43:15.116503 pckit-0.4.0/pckit/comsol/__init__.py
+-rw-r--r--   0        0        0     5900 2023-08-05 23:43:15.116503 pckit-0.4.0/pckit/comsol/model.py
+-rw-r--r--   0        0        0     2005 2023-08-05 23:43:15.116503 pckit-0.4.0/pckit/comsol/worker.py
+-rw-r--r--   0        0        0      392 2023-08-05 23:43:15.116503 pckit-0.4.0/pckit/models.py
+-rw-r--r--   0        0        0     9265 2023-08-05 23:43:15.116503 pckit-0.4.0/pckit/solvers.py
+-rw-r--r--   0        0        0      593 2023-08-05 23:43:15.116503 pckit-0.4.0/pckit/task.py
+-rw-r--r--   0        0        0     3425 2023-08-05 23:43:15.116503 pckit-0.4.0/pckit/workers.py
+-rw-r--r--   0        0        0      617 2023-08-05 23:43:15.116503 pckit-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2833 1970-01-01 00:00:00.000000 pckit-0.4.0/PKG-INFO
```

### Comparing `pckit-0.3.0/LICENSE` & `pckit-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pckit-0.3.0/README.md` & `pckit-0.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -18,16 +18,15 @@
         return x ** 2
 
 
 if __name__ == '__main__':
     model = MyModel()
     worker = pckit.MultiprocessingWorker(model)
     with pckit.get_solver(worker, workers_num=2) as solver:
-        # Create tasks to solve. You can put args or
-        # kwargs for model.results() method in the Task
+        # Create tasks to solve
         tasks = [2, 3]
         results = solver.solve(tasks)
         print(results)
         # >>> [4, 9]
 ```
 
 ### MPI
@@ -54,23 +53,24 @@
 Dict based cache is available by `caching` argument in `get_solver()`.
 Tasks are required to be hashable.
 
 ```python
 with pckit.get_solver(worker, caching=True) as solver:
     tasks = [2, 2]
 ```
+
 The second task's solution will be reused from the cache.
 
 ### Custom iterators
-You can send the email or print anything with custom iterator.
+You can send emails or print anything during evaluation with custom iterator.
 [tqdm](https://pypi.org/project/tqdm/) is also supported.
 ```python
 import tqdm
 
 results = solver.solve(tasks, iterator=tqdm.tqdm)
 ```
-See [example](https://github.com/djiboshin/pckit/blob/main/examples/custom_iterator.py) to create your own iterator.
+See [example](https://github.com/djiboshin/pckit/blob/main/examples/iterator_custom.py) to create your own iterator.
 
 ### Comsol Models, Solvers, Workers
 Based on [MPh](https://pypi.org/project/MPh/) package.
 
 **TBD**ocumented
```

### Comparing `pckit-0.3.0/pckit/cache.py` & `pckit-0.4.0/pckit/cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+This module contains cache classes
+"""
 from abc import ABCMeta, abstractmethod
 from typing import Generic, Dict
 from ._typevars import Task, Result
 
 
 class BaseCache(Generic[Task, Result], metaclass=ABCMeta):
     @abstractmethod
@@ -42,21 +45,21 @@
         :return:
         """
         if item in self:
             return self[item]
         return None
 
 
-class Cache(BaseCache):
+class DictCache(BaseCache):
     """Simple cache based on dict."""
     def __init__(self):
-        self._cache: Dict[Task, Result] = {}
+        self._cache: Dict[Task, Result] = dict()
 
     def __getitem__(self, item: Task) -> Result:
-        return self._cache.get(hash(item))
+        return self._cache.get(item)
 
     def __setitem__(self, item: Task, value: Result):
-        self._cache[hash(item)] = value
+        self._cache[item] = value
 
     def __contains__(self, item: Task) -> bool:
-        return hash(item) in self._cache
+        return item in self._cache
```

### Comparing `pckit-0.3.0/pckit/models.py` & `pckit-0.4.0/pckit/comsol/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-"""
-This module contains different Models
-"""
-from abc import ABC, abstractmethod, ABCMeta
-from typing import Any, AnyStr, Dict, Generic, TypeVar, Type, Protocol, Callable
-
 import mph
+from abc import ABCMeta
+from typing import Any, AnyStr, Dict, Sequence
+
 import pandas as pd
 import numpy as np
 
-from ._utils import make_unique
-from ._typevars import Task, Result
+from ..models import Model
+from .._typevars import Task
 
 
-class Model(Generic[Task, Result]):
-    """
-    The Model abstract base class.
+def make_unique(labels: Sequence) -> list:
+    """Gets labels list and makes all labels unique by adding '(number of inclusion)' postfix
+
+    :param labels: List of labels
+    :return: List of renamed labels
     """
-    @abstractmethod
-    def results(self, task: Task) -> Result:
-        """
-        Function to be solved
-        """
+    new_labels = []
+    _, real_index, counts = np.unique(labels, return_counts=True, return_inverse=True)
+    for index in range(len(labels)):
+        for count in range(counts[real_index[index]]):
+            new_label = labels[index] + (f'({count})' if count != 0 else '')
+            if new_label not in new_labels:
+                new_labels.append(new_label)
+                break
 
+    return new_labels
 
-# TODO SMUTHI Model
-# TODO logging here?
 
-# noinspection PyMissingOrEmptyDocstring
 class ComsolModel(mph.Model, Model, metaclass=ABCMeta):
     def __init__(self):
         super().__init__(None)
 
     def add_circle(
             self,
             name: str,
```

### Comparing `pckit-0.3.0/pckit/solvers.py` & `pckit-0.4.0/pckit/solvers.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,44 +2,50 @@
 This module contains different Solvers
 """
 import multiprocessing
 import sys
 from abc import ABC, abstractmethod
 
 from multiprocessing import Queue, JoinableQueue
-from typing import Any, Sequence, Union, List, Iterator, Callable, Iterable, Generic
+from typing import Any, Sequence, Union, List, Iterator, Callable, Iterable, Generic, Optional
 from ._typevars import Task, Result
 import time
 import logging
 
 from .workers import Worker, MultiprocessingWorker, MPIWorker
 from ._utils import tasks_sort
-from .cache import Cache, BaseCache
+from .cache import DictCache, BaseCache
 
-# TODO(add info to return after .solve())
-# TODO(add additional threads to control workers' errors)
+# TODO add info to return after .solve()
+# TODO add additional threads to control workers' errors(?)
 
 logger = logging.getLogger(__package__ + '.solver')
 
 
 def task_iterator(iterable: Sequence[Task]) -> Iterator[Task]:
     """Returns Iterator from on iterable"""
     return iterable.__iter__()
 
 
 class Solver(ABC, Generic[Task, Result]):
     """Base Solver class"""
     def __init__(
             self,
             worker: Worker[Task, Result],
-            caching: bool = False
+            caching: bool = False,
+            cache: Optional[BaseCache[Task, Result]] = None,
     ):
         self.worker = worker
         self.caching = caching
-        self.cache: BaseCache[Task, Result] = Cache()
+
+        if cache is None and caching:
+            self.cache = DictCache()
+        else:
+            self.cache = cache
+
         self.total_workers = 0
 
     def solve(self,
               tasks: Sequence[Task],
               iterator: Callable[[Sequence[Task]], Union[Iterator[Task], Iterable[Task]]] = task_iterator
               ) -> List[Result]:
         """Solves tasks
@@ -58,27 +64,40 @@
             message += f':\n\t{len(cached)} solutions will be reused\n' \
                        f'\t{len(same)} tasks are the same'
         else:
             message += ' (caching is off)'
         logger.info(message)
         start_time = time.time()
 
-        res = self._solve(tasks, to_solve, cached, same, iterator)
+        results = [None for _ in tasks]
+        task_to_solve = []
+        for i, task in enumerate(tasks):
+            if i in to_solve:
+                task_to_solve.append(task)
+
+        res = self._solve(tasks=task_to_solve, iterator=iterator)
+
+        for i, task, result in zip(to_solve, task_to_solve, res):
+            results[i] = result
+            if self.caching:
+                self.cache[task] = result
+
+        for i in same:
+            results[i] = self.cache[tasks[i]]
+        for i in cached:
+            results[i] = self.cache[tasks[i]]
 
         end_time = time.time()
         logger.info('All the tasks have been solved in %.2fs', end_time - start_time)
-        return res
+        return results
 
     @abstractmethod
     def _solve(
             self,
             tasks: Sequence[Task],
-            to_solve: List[int],
-            cached: List[int],
-            same: List[int],
             iterator: Callable[[Sequence[Task]], Iterator[Task]]
     ) -> List[Result]:
         pass
 
     def __enter__(self):
         return self
 
@@ -87,21 +106,22 @@
 
 
 class MultiprocessingSolver(Solver):
     """Multiprocessing Solver implementation"""
     def __init__(self,
                  worker: MultiprocessingWorker,
                  workers_num: int = 1,
-                 caching: bool = False
+                 caching: bool = False,
+                 cache: Optional[BaseCache[Task, Result]] = None,
                  ):
 
         if not isinstance(worker, MultiprocessingWorker):
             raise TypeError('Worker has to be the object of type MultiprocessingWorker')
 
-        super().__init__(worker=worker, caching=caching)
+        super().__init__(worker=worker, caching=caching, cache=cache)
         self.worker = worker
 
         if workers_num <= 0:
             raise RuntimeError('At least 1 worker is needed')
         self.total_workers = workers_num
 
         self.workers = []
@@ -117,39 +137,27 @@
             )
             process.start()
             self.workers.append(process)
 
     def _solve(
             self,
             tasks: Sequence[Task],
-            to_solve: List[int],
-            cached: List[int],
-            same: List[int],
             iterator: Callable[[Sequence[Task]], Iterator[Task]]
     ) -> List[Result]:
         results = [None for _ in tasks]
+
         for i, task in enumerate(tasks):
-            if i in to_solve:
-                self._jobs.put((i, task))
-            elif i in cached:
-                results[i] = self.cache[task]
-            else:
-                results[i] = None
-        tasks_to_solve = [task for i, task in enumerate(tasks) if i in to_solve]
-        for _ in iterator(tasks_to_solve):
+            self._jobs.put((i, task))
+
+        for _ in iterator(tasks):
             (i, res) = self._results.get()
             if i == -1:
                 raise RuntimeError(res)
-            if self.caching:
-                self.cache[tasks[i]] = res
             results[i] = res
 
-        for i in same:
-            results[i] = self.cache[tasks[i]]
-
         return results
 
     def _stop(self):
         for worker in self.workers:
             if worker.is_alive():
                 worker.terminate()
                 worker.join()
@@ -158,60 +166,55 @@
     def __exit__(self, exc_type, exc_val, exc_tb):
         self._stop()
         return False
 
 
 class SimpleSolver(Solver):
     """Simplest Solver implementation"""
-    def __init__(self, worker: Worker, caching: bool = False):
+    def __init__(
+            self,
+            worker: Worker,
+            caching: bool = False,
+            cache: Optional[BaseCache[Task, Result]] = None
+    ):
         if not isinstance(worker, Worker):
             raise TypeError('Worker has to be the object of type Worker')
-        super().__init__(worker=worker, caching=caching)
+        super().__init__(worker=worker, caching=caching, cache=cache)
         self.worker.start()
         self.total_workers = 1
 
     def _solve(
             self,
             tasks: Sequence[Task],
-            to_solve: List[int],
-            cached: List[int],
-            same: List[int],
             iterator: Callable[[Sequence[Task]], Iterator[Task]]
     ) -> List[Result]:
         results = [None for _ in tasks]
         for i, task in enumerate(iterator(tasks)):
-            if i in to_solve:
-                try:
-                    results[i] = self.worker.do_the_job(task)
-                    print(results[i])
-                except Exception as err:
-                    raise RuntimeError from err
-                if self.caching:
-                    self.cache[task] = results[i]
-            elif i in cached or i in same:
-                results[i] = self.cache[task] if task is not None else None
-            else:
-                results[i] = None
+            try:
+                results[i] = self.worker.do_the_job(task)
+            except Exception as err:
+                raise RuntimeError from err
         return results
 
 
 class MPISolver(Solver):
     """MPI Solver implementation"""
     def __init__(
             self,
             worker: MPIWorker,
             caching: bool = False,
+            cache: Optional[BaseCache[Task, Result]] = None,
             buffer_size: int = 32768
     ):
         from mpi4py import MPI
 
         if not isinstance(worker, MPIWorker):
             raise TypeError('Worker has to be the object of type MPIWorker')
 
-        super().__init__(worker=worker, caching=caching)
+        super().__init__(worker=worker, caching=caching, cache=cache)
         self.worker = worker
 
         self.buffer_size = buffer_size
         self.comm = MPI.COMM_WORLD
         self._MPI = MPI
         self.rank = self.comm.Get_rank()
         self.total_workers = self.comm.Get_size() - 1
@@ -226,40 +229,28 @@
         if self.total_workers < 1:
             raise RuntimeError('Not enough processes! '
                                f'Need at least 2, detected {self.total_workers}.')
 
     def _solve(
             self,
             tasks: Sequence[Task],
-            to_solve: List[int],
-            cached: List[int],
-            same: List[int],
             iterator: Callable[[Sequence[Task]], Iterator[Task]]
     ) -> List[Any]:
         results = [None for _ in tasks]
         requests = []
-        tasks_to_solve = []
         for i, task in enumerate(tasks):
-            if i in to_solve:
-                dest = len(requests) % self.total_workers + 1
-                req = self.comm.isend((i, task), dest=dest, tag=i)
-                req.wait()
-                requests.append(self.comm.irecv(self.buffer_size, source=dest))
-                tasks_to_solve.append(task)
-            elif i in cached:
-                results[i] = self.cache[task]
-        for _ in iterator(tasks_to_solve):
+            dest = len(requests) % self.total_workers + 1
+            req = self.comm.isend((i, task), dest=dest, tag=i)
+            req.wait()
+            requests.append(self.comm.irecv(self.buffer_size, source=dest))
+
+        for _ in iterator(tasks):
             (k, (i, res)) = self._MPI.Request.waitany(requests)
-            if self.caching:
-                self.cache[tasks[i]] = res
             results[i] = res
 
-        for i in same:
-            results[i] = self.cache[tasks[i]]
-
         return results
 
     def _stop(self):
         for i in range(1, self.comm.Get_size()):
             req = self.comm.isend((None, None), dest=i)
             req.wait()
 
@@ -269,25 +260,41 @@
     def __exit__(self, exc_type, exc_val, exc_tb):
         self._stop()
 
 
 def get_solver(
         worker: Union[Worker, MPIWorker, MultiprocessingWorker],
         caching: bool = False,
+        cache: Optional[BaseCache[Task, Result]] = None,
         workers_num: int = 1,
         buffer_size: int = 2**15,
 ) -> Union[SimpleSolver, MPISolver, MultiprocessingSolver]:
     """Automatically choose solver based on worker type.
 
     :param worker: worker instance
     :param caching: is caching enabled
+    :param cache: BaseCache object
     :param workers_num: number of workers to spawn if worker is instance of MultiprocessingWorker
     :param buffer_size: buffer size for messages with results used by MPI
     :return: solver
     """
     if isinstance(worker, MultiprocessingWorker):
-        return MultiprocessingSolver(worker=worker, workers_num=workers_num, caching=caching)
+        return MultiprocessingSolver(
+            worker=worker,
+            workers_num=workers_num,
+            caching=caching,
+            cache=cache
+        )
     if isinstance(worker, MPIWorker):
-        return MPISolver(worker, caching, buffer_size)
+        return MPISolver(
+            worker=worker,
+            caching=caching,
+            cache=cache,
+            buffer_size=buffer_size
+        )
     if isinstance(worker, Worker):
-        return SimpleSolver(worker, caching)
+        return SimpleSolver(
+            worker=worker,
+            caching=caching,
+            cache=cache
+        )
     raise NotImplementedError(f'can\'t get Solver for {type(worker)} worker type')
```

### Comparing `pckit-0.3.0/pyproject.toml` & `pckit-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "pckit"
-version = "0.3.0"
+version = "0.4.0"
 description = "A simple package for parallel computing with Python"
 authors = ["djiboshin"]
 readme = "README.md"
 homepage = "https://github.com/djiboshin/pckit"
 repository = "https://github.com/djiboshin/pckit"
 license = "MIT"
 
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.25.2"
-pandas = "^2.0.3"
-MPh = "^1.1.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.4.0"
 pylint = "^2.13.8"
 pytest-cov = "^4.1.0"
 tqdm = "^4.64.0"
 mpi4py = "^3.1.3"
+MPh = "^1.1.5"
+pandas = "^2.0.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pckit-0.3.0/PKG-INFO` & `pckit-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: pckit
-Version: 0.3.0
+Version: 0.4.0
 Summary: A simple package for parallel computing with Python
 Home-page: https://github.com/djiboshin/pckit
 License: MIT
 Author: djiboshin
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: MPh (>=1.1.5,<2.0.0)
 Requires-Dist: numpy (>=1.25.2,<2.0.0)
-Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Project-URL: Repository, https://github.com/djiboshin/pckit
 Description-Content-Type: text/markdown
 
 # pckit
 
 This is a simple package for parallel computing with Python.
 
@@ -37,16 +35,15 @@
         return x ** 2
 
 
 if __name__ == '__main__':
     model = MyModel()
     worker = pckit.MultiprocessingWorker(model)
     with pckit.get_solver(worker, workers_num=2) as solver:
-        # Create tasks to solve. You can put args or
-        # kwargs for model.results() method in the Task
+        # Create tasks to solve
         tasks = [2, 3]
         results = solver.solve(tasks)
         print(results)
         # >>> [4, 9]
 ```
 
 ### MPI
@@ -73,24 +70,25 @@
 Dict based cache is available by `caching` argument in `get_solver()`.
 Tasks are required to be hashable.
 
 ```python
 with pckit.get_solver(worker, caching=True) as solver:
     tasks = [2, 2]
 ```
+
 The second task's solution will be reused from the cache.
 
 ### Custom iterators
-You can send the email or print anything with custom iterator.
+You can send emails or print anything during evaluation with custom iterator.
 [tqdm](https://pypi.org/project/tqdm/) is also supported.
 ```python
 import tqdm
 
 results = solver.solve(tasks, iterator=tqdm.tqdm)
 ```
-See [example](https://github.com/djiboshin/pckit/blob/main/examples/custom_iterator.py) to create your own iterator.
+See [example](https://github.com/djiboshin/pckit/blob/main/examples/iterator_custom.py) to create your own iterator.
 
 ### Comsol Models, Solvers, Workers
 Based on [MPh](https://pypi.org/project/MPh/) package.
 
 **TBD**ocumented
```

