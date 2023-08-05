# Comparing `tmp/sagemath-bliss-10.1b9.tar.gz` & `tmp/sagemath-bliss-9.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemath-bliss-10.1b9.tar", last modified: Sat Aug  5 23:33:08 2023, max compression
+gzip compressed data, was "sagemath-bliss-9.8b1.tar", last modified: Mon Nov 21 07:31:28 2022, max compression
```

## Comparing `sagemath-bliss-10.1b9.tar` & `sagemath-bliss-9.8b1.tar`

### file list

```diff
@@ -1,21 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:33:08.329748 sagemath-bliss-10.1b9/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-08-05 23:29:06.000000 sagemath-bliss-10.1b9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-08-05 23:33:08.329748 sagemath-bliss-10.1b9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-08-05 23:29:06.000000 sagemath-bliss-10.1b9/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-05 23:29:06.000000 sagemath-bliss-10.1b9/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-05 23:29:22.000000 sagemath-bliss-10.1b9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:33:08.329748 sagemath-bliss-10.1b9/sage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 23:29:06.000000 sagemath-bliss-10.1b9/sage/all__sagemath_bliss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:33:08.329748 sagemath-bliss-10.1b9/sage/graphs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 23:29:06.000000 sagemath-bliss-10.1b9/sage/graphs/all__sagemath_bliss.py
--rw-r--r--   0 runner    (1001) docker     (123)    32376 2023-08-05 23:29:06.000000 sagemath-bliss-10.1b9/sage/graphs/bliss.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:33:08.329748 sagemath-bliss-10.1b9/sage/graphs/bliss_cpp/
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-08-05 23:29:06.000000 sagemath-bliss-10.1b9/sage/graphs/bliss_cpp/bliss_find_automorphisms.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:33:08.329748 sagemath-bliss-10.1b9/sagemath_bliss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-08-05 23:33:08.000000 sagemath-bliss-10.1b9/sagemath_bliss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-05 23:33:08.000000 sagemath-bliss-10.1b9/sagemath_bliss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 23:33:08.000000 sagemath-bliss-10.1b9/sagemath_bliss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-05 23:33:08.000000 sagemath-bliss-10.1b9/sagemath_bliss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-05 23:33:08.000000 sagemath-bliss-10.1b9/sagemath_bliss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-05 23:33:08.329748 sagemath-bliss-10.1b9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-08-05 23:29:06.000000 sagemath-bliss-10.1b9/setup.py
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:28.289780 sagemath-bliss-9.8b1/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      185 2022-11-20 23:45:29.000000 sagemath-bliss-9.8b1/MANIFEST.in
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2370 2022-11-21 07:31:28.289916 sagemath-bliss-9.8b1/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1296 2022-11-20 23:45:29.000000 sagemath-bliss-9.8b1/README.rst
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      292 2022-11-21 07:28:42.000000 sagemath-bliss-9.8b1/pyproject.toml
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:28.285772 sagemath-bliss-9.8b1/sage/
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:28.287619 sagemath-bliss-9.8b1/sage/graphs/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)    34899 2022-11-16 06:02:58.000000 sagemath-bliss-9.8b1/sage/graphs/bliss.pyx
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:28.289510 sagemath-bliss-9.8b1/sagemath_bliss.egg-info/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2370 2022-11-21 07:31:28.000000 sagemath-bliss-9.8b1/sagemath_bliss.egg-info/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      267 2022-11-21 07:31:28.000000 sagemath-bliss-9.8b1/sagemath_bliss.egg-info/SOURCES.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        1 2022-11-21 07:31:28.000000 sagemath-bliss-9.8b1/sagemath_bliss.egg-info/dependency_links.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)       25 2022-11-21 07:31:28.000000 sagemath-bliss-9.8b1/sagemath_bliss.egg-info/requires.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        5 2022-11-21 07:31:28.000000 sagemath-bliss-9.8b1/sagemath_bliss.egg-info/top_level.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1093 2022-11-21 07:31:28.290521 sagemath-bliss-9.8b1/setup.cfg
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2057 2022-11-20 23:45:29.000000 sagemath-bliss-9.8b1/setup.py
```

### Comparing `sagemath-bliss-10.1b9/PKG-INFO` & `sagemath-bliss-9.8b1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemath-bliss
-Version: 10.1b9
+Version: 9.8b1
 Summary: Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with bliss
 Home-page: https://www.sagemath.org
 Author: The Sage Developers
 Author-email: sage-support@googlegroups.com
 License: GNU General Public License (GPL) v2 or later
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Education
@@ -17,27 +17,26 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: test
 
 ==============================================================================
  Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with bliss
 ==============================================================================
 
 About SageMath
 --------------
 
    "Creating a Viable Open Source Alternative to
     Magma, Maple, Mathematica, and MATLAB"
 
-   Copyright (C) 2005-2023 The Sage Development Team
+   Copyright (C) 2005-2022 The Sage Development Team
 
    https://www.sagemath.org
 
 SageMath fully supports all major Linux distributions, recent versions of
 macOS, and Windows (using Cygwin or Windows Subsystem for Linux).
 
 The traditional and recommended way to install SageMath is from source via
```

### Comparing `sagemath-bliss-10.1b9/README.rst` & `sagemath-bliss-9.8b1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 About SageMath
 --------------
 
    "Creating a Viable Open Source Alternative to
     Magma, Maple, Mathematica, and MATLAB"
 
-   Copyright (C) 2005-2023 The Sage Development Team
+   Copyright (C) 2005-2022 The Sage Development Team
 
    https://www.sagemath.org
 
 SageMath fully supports all major Linux distributions, recent versions of
 macOS, and Windows (using Cygwin or Windows Subsystem for Linux).
 
 The traditional and recommended way to install SageMath is from source via
```

### Comparing `sagemath-bliss-10.1b9/sage/graphs/bliss.pyx` & `sagemath-bliss-9.8b1/sage/graphs/bliss.pyx`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # distutils: language = c++
-# distutils: extra_compile_args = -std=c++11
 # distutils: libraries = bliss
 # sage_setup: distribution = sagemath-bliss
 
 r"""
 Interface with bliss: graph (iso/auto)morphism
 
 Implemented functions:
@@ -44,30 +43,30 @@
 
     cdef cppclass AbstractGraph:
         pass
 
     cdef cppclass Graph(AbstractGraph):
         Graph(const unsigned int)
         void add_edge(const unsigned int, const unsigned int)
+        void find_automorphisms(Stats&, void (*)(void*, unsigned int,
+                                                 const unsigned int*), void*)
         void change_color(const unsigned int, const unsigned int)
-        const unsigned int* canonical_form(Stats&)
-
-cdef extern from "bliss/digraph.hh" namespace "bliss":
+        const unsigned int* canonical_form(Stats&, void (*)(void*, unsigned int,
+                                                            const unsigned int*), void*)
 
     cdef cppclass Digraph(AbstractGraph):
         Digraph(const unsigned int)
         void add_edge(const unsigned int, const unsigned int)
+        void find_automorphisms(Stats&, void (*)(void*, unsigned int,
+                                                 const unsigned int*), void*)
         void change_color(const unsigned int, const unsigned int)
-        const unsigned int* canonical_form(Stats&)
+        const unsigned int* canonical_form(Stats&, void (*)(void*, unsigned int,
+                                                            const unsigned int*), void*)
         unsigned int get_hash()
 
-cdef extern from "bliss_cpp/bliss_find_automorphisms.h":
-
-    void bliss_find_automorphisms(Graph*, void (*)(void*, unsigned int, const unsigned int*), void*, Stats&)
-    void bliss_find_automorphisms(Digraph*, void (*)(void*, unsigned int, const unsigned int*), void*, Stats&)
 
 cdef int encoding_numbits(int n):
     r"""
     Return the number of bits needed to encode the ``n`` numbers from ``1`` to ``n``. In
     other words, the last bit set in ``n``.
     """
     if n <= 0:
@@ -121,14 +120,18 @@
 
         cur += 1
 
     gens.append(perm)
 
     sig_free(done)
 
+
+cdef void empty_hook(void *user_param, unsigned int n, const unsigned int *aut):
+    return
+
 #####################################################
 # constructing bliss graphs from edge lists
 #####################################################
 
 cdef Graph *bliss_graph_from_labelled_edges(int Vnr, int Lnr, Vout, Vin, labels, partition):
     r"""
     Return a bliss graph from the input data
@@ -339,18 +342,18 @@
     cdef dict relabel
 
     cdef list new_edges = []
     cdef long e, f
 
     if directed:
         d = bliss_digraph_from_labelled_edges(Vnr, Lnr, Vout, Vin, labels, partition)
-        aut = d.canonical_form(s)
+        aut = d.canonical_form(s, empty_hook, NULL)
     else:
         g = bliss_graph_from_labelled_edges(Vnr, Lnr, Vout, Vin, labels, partition)
-        aut = g.canonical_form(s)
+        aut = g.canonical_form(s, empty_hook, NULL)
 
     for i in range(len(Vout)):
         x = Vout[i]
         y = Vin[i]
         e = aut[x]
         f = aut[y]
         if Lnr == 1:
@@ -433,21 +436,20 @@
 
         sage: canonical_form(Graph(15), return_graph=True)                  # optional - bliss
         Graph on 15 vertices
         sage: g = digraphs.RandomTournament(40)                             # optional - bliss
         sage: g.is_isomorphic(canonical_form(g, return_graph=True))         # optional - bliss
         True
 
-        sage: # optional - bliss
-        sage: g1 = graphs.RandomGNP(100, .4)
-        sage: r = Permutations(range(100)).random_element()
-        sage: g2 = Graph([(r[u],r[v]) for u,v in g1.edges(sort=True, labels=False)])
-        sage: g1 = canonical_form(g1, return_graph=True)
-        sage: g2 = canonical_form(g2, return_graph=True)
-        sage: g2 == g2
+        sage: g1 = graphs.RandomGNP(100, .4)                                # optional - bliss
+        sage: r = Permutations(range(100)).random_element()                 # optional - bliss
+        sage: g2 = Graph([(r[u],r[v]) for u,v in g1.edges(sort=True, labels=False)])   # optional - bliss
+        sage: g1 = canonical_form(g1, return_graph=True)                    # optional - bliss
+        sage: g2 = canonical_form(g2, return_graph=True)                    # optional - bliss
+        sage: g2 == g2                                                      # optional - bliss
         True
 
         sage: g = Graph({1: [2]})
         sage: g_ = canonical_form(g, return_graph=True, certificate=True)   # optional - bliss
         sage: 0 in g_[0]                                                    # optional - bliss
         True
 
@@ -473,20 +475,19 @@
         ....:             h = Graph([(p[u], p[v], lab) for u,v,lab in g.edges(sort=True)])
         ....:             hcan = canonical_form(h, use_edge_labels=True)
         ....:             if gcan != hcan: print(edges, labels, p)
 
     Check that it works with non hashable non sortable edge labels (relying
     on string representations of the labels)::
 
-        sage: # needs sage.modules
         sage: g1 = Graph([(0, 1, matrix(ZZ, 2)), (0, 2, RDF.pi()), (1, 2, 'a')])
         sage: g2 = Graph([(1, 2, matrix(ZZ, 2)), (2, 0, RDF.pi()), (0, 1, 'a')])
-        sage: g1can = canonical_form(g1, use_edge_labels=True)  # optional - bliss
-        sage: g2can = canonical_form(g2, use_edge_labels=True)  # optional - bliss
-        sage: g1can == g2can                    # optional - bliss
+        sage: g1can = canonical_form(g1, use_edge_labels=True)               # optional - bliss
+        sage: g2can = canonical_form(g2, use_edge_labels=True)               # optional - bliss
+        sage: g1can == g2can                                                 # optional - bliss
         True
 
     Check that :trac:`32395` is fixed::
 
         sage: g = Graph([[0, 2]])  # 1 is not a vertex!
         sage: g.canonical_label(partition=[[0], [1], [2]], algorithm="bliss")  # optional - bliss
         Traceback (most recent call last):
@@ -638,19 +639,19 @@
         int2vert = list(range(Vnr))
 
     cdef list gens = []
     cdef tuple data = (gens, int2vert, Vnr)
 
     if directed:
         d = bliss_digraph_from_labelled_edges(Vnr, Lnr, Vout, Vin, labels, partition)
-        bliss_find_automorphisms(d, add_gen, <void*>data, s)
+        d.find_automorphisms(s, add_gen, <void*>data)
         del d
     else:
         g = bliss_graph_from_labelled_edges(Vnr, Lnr, Vout, Vin, labels, partition)
-        bliss_find_automorphisms(g, add_gen, <void*>data, s)
+        g.find_automorphisms(s, add_gen, <void*>data)
         del g
 
     return [[cyc for cyc in gen if cyc[0] is not None] for gen in gens]
 
 cpdef automorphism_group(G, partition=None, use_edge_labels=True):
     """
     Return the automorphism group of the given (di)graph.
@@ -675,128 +676,121 @@
 
     EXAMPLES::
 
         sage: from sage.graphs.bliss import automorphism_group                  # optional - bliss
 
     Computing the automorphism group of a graph or digraph::
 
-        sage: # optional - bliss
-        sage: G = graphs.CompleteMultipartiteGraph([1, 1, 1, 2])
-        sage: automorphism_group(G).cardinality()
+        sage: G = graphs.CompleteMultipartiteGraph([1, 1, 1, 2])                # optional - bliss
+        sage: automorphism_group(G).cardinality()                               # optional - bliss
         12
-        sage: D = DiGraph(G.edges(sort=True))
-        sage: automorphism_group(D).cardinality()
+        sage: D = DiGraph(G.edges(sort=True))                                   # optional - bliss
+        sage: automorphism_group(D).cardinality()                               # optional - bliss
         2
 
     Observe that the order 12 is given by permuting the first three vertices, or the last two
     in the case of a graph, while only the latter two are possible in the case of a directed
     graph.
 
     Partitioning the vertices into classes::
 
-        sage: # optional - bliss
-        sage: G = graphs.CompleteMultipartiteGraph([3, 2])
-        sage: automorphism_group(G).cardinality()
+        sage: G = graphs.CompleteMultipartiteGraph([3, 2])                      # optional - bliss
+        sage: automorphism_group(G).cardinality()                               # optional - bliss
         12
-        sage: automorphism_group(G,partition=[[0],[1],[2],[3,4]]).cardinality()
+        sage: automorphism_group(G,partition=[[0],[1],[2],[3,4]]).cardinality() # optional - bliss
         2
-        sage: automorphism_group(G,partition=[[0],[1,2],[3,4]]).cardinality()
+        sage: automorphism_group(G,partition=[[0],[1,2],[3,4]]).cardinality()   # optional - bliss
         4
 
         sage: automorphism_group(G,partition=[[1,2],[0,3],[4]]).cardinality()   # optional - bliss
         2
 
     Partitioning the edges into classes::
 
         sage: G = Graph(graphs.CompleteMultipartiteGraph([8, 2]), sparse=True)  # optional - bliss
         sage: for i,j in G.edges(labels=False, sort=False):                     # optional - bliss
-        ....:     if 0 <= i < 3:
-        ....:         G.set_edge_label(i, j, "A")
-        ....:     if 3 <= i < 6:
-        ....:         G.set_edge_label(i, j, "B")
-        ....:     if 6 <= i < 8:
-        ....:         G.set_edge_label(i, j, "C")
+        ....:     if 0 <= i < 3:                                                # optional - bliss
+        ....:         G.set_edge_label(i, j, "A")                               # optional - bliss
+        ....:     if 3 <= i < 6:                                                # optional - bliss
+        ....:         G.set_edge_label(i, j, "B")                               # optional - bliss
+        ....:     if 6 <= i < 8:                                                # optional - bliss
+        ....:         G.set_edge_label(i, j, "C")                               # optional - bliss
 
         sage: factor(automorphism_group(G).cardinality())                       # optional - bliss
         2^4 * 3^2
         sage: automorphism_group(G,[[0],[1],[2,3],[4,5],[6,7],[8],[9]]).cardinality()   # optional - bliss
         4
 
     TESTS::
 
         sage: from sage.graphs.bliss import automorphism_group                  # optional - bliss
         sage: G = graphs.PetersenGraph()                                        # optional - bliss
         sage: automorphism_group(G).is_isomorphic(G.automorphism_group())       # optional - bliss
         True
 
-        sage: # optional - bliss
-        sage: G = graphs.HeawoodGraph()
-        sage: p = G.bipartite_sets()
-        sage: A = G.automorphism_group(partition=[list(p[0]), list(p[1])])
-        sage: automorphism_group(G, partition=p).is_isomorphic(A)
+        sage: G = graphs.HeawoodGraph()                                         # optional - bliss
+        sage: p = G.bipartite_sets()                                            # optional - bliss
+        sage: A = G.automorphism_group(partition=[list(p[0]), list(p[1])])      # optional - bliss
+        sage: automorphism_group(G, partition=p).is_isomorphic(A)               # optional - bliss
         True
 
         sage: G = graphs.CompleteMultipartiteGraph([5,7,11])
         sage: B = automorphism_group(G)                                         # optional - bliss
         sage: B.cardinality() == prod(factorial(n) for n in [5,7,11])           # optional - bliss
         True
 
-        sage: # optional - bliss
-        sage: G = Graph(graphs.CompleteMultipartiteGraph([8,8,8,5]),sparse=True)
-        sage: for i,j in G.edges(labels=False, sort=False):
-        ....:     if 0 <= i < 3:
-        ....:         G.set_edge_label(i, j, "A")
-        ....:     if 3 <= i < 6:
-        ....:         G.set_edge_label(i, j, "B")
-        ....:     if 6 <= i < 8:
-        ....:         G.set_edge_label(i, j, "C")
-        sage: automorphism_group(G).cardinality() == prod( factorial(n) for n in [3,3,2,8,8,5,2] )
-        True
-        sage: automorphism_group(G, use_edge_labels=False).cardinality() == prod( factorial(n) for n in [8,8,8,5,3] )
-        True
-        sage: automorphism_group(G,[[0 .. 7],[8 .. 11],[12 .. 28]]).cardinality() == prod( factorial(n) for n in [3,3,2,4,4,8,5] )
-        True
-
-        sage: # optional - bliss
-        sage: G = Graph()
-        sage: G.add_edges((i,j,"A") for i in range(0, 2) for j in range(14,20))
-        sage: G.add_edges((i,j,"B") for i in range(2, 5) for j in range(14,20))
-        sage: G.add_edges((i,j,"C") for i in range(5, 9) for j in range(14,20))
-        sage: G.add_edges((i,j,"D") for i in range(9,14) for j in range(14,20))
-        sage: A = automorphism_group(G)
-        sage: print(A.gens())               # random
+        sage: G = Graph(graphs.CompleteMultipartiteGraph([8,8,8,5]),sparse=True)# optional - bliss
+        sage: for i,j in G.edges(labels=False, sort=False):                     # optional - bliss
+        ....:     if 0 <= i < 3:                                                # optional - bliss
+        ....:         G.set_edge_label(i, j, "A")                               # optional - bliss
+        ....:     if 3 <= i < 6:                                                # optional - bliss
+        ....:         G.set_edge_label(i, j, "B")                               # optional - bliss
+        ....:     if 6 <= i < 8:                                                # optional - bliss
+        ....:         G.set_edge_label(i, j, "C")                               # optional - bliss
+        sage: automorphism_group(G).cardinality() == prod( factorial(n) for n in [3,3,2,8,8,5,2] )  # optional - bliss
+        True
+        sage: automorphism_group(G, use_edge_labels=False).cardinality() == prod( factorial(n) for n in [8,8,8,5,3] )  # optional - bliss
+        True
+        sage: automorphism_group(G,[[0 .. 7],[8 .. 11],[12 .. 28]]).cardinality() == prod( factorial(n) for n in [3,3,2,4,4,8,5] )  # optional - bliss
+        True
+
+        sage: G = Graph()                                                       # optional - bliss
+        sage: G.add_edges((i,j,"A") for i in range(0, 2) for j in range(14,20)) # optional - bliss
+        sage: G.add_edges((i,j,"B") for i in range(2, 5) for j in range(14,20)) # optional - bliss
+        sage: G.add_edges((i,j,"C") for i in range(5, 9) for j in range(14,20)) # optional - bliss
+        sage: G.add_edges((i,j,"D") for i in range(9,14) for j in range(14,20)) # optional - bliss
+        sage: A = automorphism_group(G)                                         # optional - bliss
+        sage: print(A.gens())                                                   # random, optional - bliss
         [(9,13), (18,19), (17,18), (16,17), (15,16), (14,15), (12,9), (11,12),
          (10,11), (7,8), (6,7), (5,6), (3,4), (2,3), (0,1)]
-        sage: A.cardinality() == prod(factorial(n) for n in [2,3,4,5,6])
+        sage: A.cardinality() == prod(factorial(n) for n in [2,3,4,5,6])        # optional - bliss
         True
 
         sage: alpha = "abcdefghijklmnopqrstuvwxyz"
 
-        sage: # optional - bliss
-        sage: G = Graph()
-        sage: G.add_edges((alpha[i],alpha[j],"A") for i in range(0, 2) for j in range(14,20))
-        sage: G.add_edges((alpha[i],alpha[j],"B") for i in range(2, 5) for j in range(14,20))
-        sage: G.add_edges((alpha[i],alpha[j],"C") for i in range(5, 9) for j in range(14,20))
-        sage: G.add_edges((alpha[i],alpha[j],"D") for i in range(9,14) for j in range(14,20))
-        sage: A = automorphism_group(G)
-        sage: print(A.gens())
+        sage: G = Graph()                                                       # optional - bliss
+        sage: G.add_edges((alpha[i],alpha[j],"A") for i in range(0, 2) for j in range(14,20))   # optional - bliss
+        sage: G.add_edges((alpha[i],alpha[j],"B") for i in range(2, 5) for j in range(14,20))   # optional - bliss
+        sage: G.add_edges((alpha[i],alpha[j],"C") for i in range(5, 9) for j in range(14,20))   # optional - bliss
+        sage: G.add_edges((alpha[i],alpha[j],"D") for i in range(9,14) for j in range(14,20))   # optional - bliss
+        sage: A = automorphism_group(G)                                         # optional - bliss
+        sage: print(A.gens())                                                   # random, optional - bliss
         [('r','t'), ('s','r'), ('p','s'), ('q','p'), ('o','q'), ('l','n'),
          ('m','l'), ('j','m'), ('k','j'), ('i','h'), ('f','i'), ('g','f'),
          ('e','d'), ('c','e'), ('a','b')]
-        sage: A.cardinality() == prod(factorial(n) for n in [2,3,4,5,6])
+        sage: A.cardinality() == prod(factorial(n) for n in [2,3,4,5,6])        # optional - bliss
         True
 
-        sage: # optional - bliss
-        sage: gg = graphs.CompleteGraph(5)
-        sage: gg.allow_loops(True)
-        sage: gg.add_edge(0,0)
-        sage: gg.add_edge(1,1)
-        sage: automorphism_group(gg).cardinality()
+        sage: gg = graphs.CompleteGraph(5)                                      # optional - bliss
+        sage: gg.allow_loops(True)                                              # optional - bliss
+        sage: gg.add_edge(0,0)                                                  # optional - bliss
+        sage: gg.add_edge(1,1)                                                  # optional - bliss
+        sage: automorphism_group(gg).cardinality()                              # optional - bliss
         12
-        sage: automorphism_group(gg,[[0],[1,2,3,4]]).cardinality()
+        sage: automorphism_group(gg,[[0],[1,2,3,4]]).cardinality()              # optional - bliss
         6
     """
     # We need this to convert the numbers from <unsigned int> to
     # <long>. This assertion should be true simply for memory reasons.
     cdef unsigned long Vnr = G.order()
     assert Vnr <= <unsigned long>LONG_MAX
```

### Comparing `sagemath-bliss-10.1b9/sagemath_bliss.egg-info/PKG-INFO` & `sagemath-bliss-9.8b1/sagemath_bliss.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemath-bliss
-Version: 10.1b9
+Version: 9.8b1
 Summary: Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with bliss
 Home-page: https://www.sagemath.org
 Author: The Sage Developers
 Author-email: sage-support@googlegroups.com
 License: GNU General Public License (GPL) v2 or later
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Education
@@ -17,27 +17,26 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: test
 
 ==============================================================================
  Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with bliss
 ==============================================================================
 
 About SageMath
 --------------
 
    "Creating a Viable Open Source Alternative to
     Magma, Maple, Mathematica, and MATLAB"
 
-   Copyright (C) 2005-2023 The Sage Development Team
+   Copyright (C) 2005-2022 The Sage Development Team
 
    https://www.sagemath.org
 
 SageMath fully supports all major Linux distributions, recent versions of
 macOS, and Windows (using Cygwin or Windows Subsystem for Linux).
 
 The traditional and recommended way to install SageMath is from source via
```

### Comparing `sagemath-bliss-10.1b9/setup.cfg` & `sagemath-bliss-9.8b1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -22,17 +22,13 @@
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Scientific/Engineering :: Mathematics
 
 [options]
 python_requires = >=3.8, <3.12
 install_requires = 
-	cysignals >=1.10.2
-
-[options.extras_require]
-test = 
-	sagemath-repl ~= 10.1b9
+	sagemath-standard ~= 9.8b3
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sagemath-bliss-10.1b9/setup.py` & `sagemath-bliss-9.8b1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,21 +43,26 @@
     from sage_setup.command.sage_build_cython import sage_build_cython
     from sage_setup.command.sage_build_ext import sage_build_ext
     sage_build_cython.built_distributions = ['sagemath-bliss']
 
     cmdclass = dict(build_cython=sage_build_cython,
                     build_ext=sage_build_ext)
 
-from sage_setup.find import find_python_sources
-python_packages, python_modules, cython_modules = find_python_sources(
-    '.', ['sage'], distributions=['sagemath-bliss'])
+if sdist:
+    python_packages = []
+    python_modules = []
+    cython_modules = []
+else:
+    from sage_setup.find import find_python_sources
+    python_packages, python_modules, cython_modules = find_python_sources(
+        '.', ['sage'], distributions=['sagemath-bliss'])
 
-log.warn('python_packages = {0}'.format(python_packages))
-log.warn('python_modules = {0}'.format(python_modules))
-log.warn('cython_modules = {0}'.format(cython_modules))
+    log.warn('python_packages = {0}'.format(python_packages))
+    log.warn('python_modules = {0}'.format(python_modules))
+    log.warn('cython_modules = {0}'.format(cython_modules))
 
 setup(
     cmdclass = cmdclass,
     packages = python_packages,
     py_modules  = python_modules,
     ext_modules = cython_modules,
 )
```

