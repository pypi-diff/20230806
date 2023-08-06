# Comparing `tmp/assrs-0.1.0.tar.gz` & `tmp/assrs-0.1.1.tar.gz`

## Comparing `assrs-0.1.0.tar` & `assrs-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 assrs-0.1.0/Cargo.toml
--rw-r--r--   0     1001      123     2773 2023-07-30 19:15:57.000000 assrs-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      686 2023-07-30 19:15:57.000000 assrs-0.1.0/.gitignore
--rw-r--r--   0     1001      123      471 2023-07-30 19:15:57.000000 assrs-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0     1001      123     4164 2023-07-30 19:15:57.000000 assrs-0.1.0/README.md
--rw-r--r--   0     1001      123     1072 2023-07-30 19:15:57.000000 assrs-0.1.0/assrs.pyi
--rw-r--r--   0     1001      123      697 2023-07-30 19:15:57.000000 assrs-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123     5503 2023-07-30 19:15:57.000000 assrs-0.1.0/src/bktree.rs
--rw-r--r--   0     1001      123     7432 2023-07-30 19:15:57.000000 assrs-0.1.0/src/levenshtein.rs
--rw-r--r--   0     1001      123      838 2023-07-30 19:15:57.000000 assrs-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123     4799 2023-07-30 19:15:57.000000 assrs-0.1.0/src/trie.rs
--rw-r--r--   0     1001      123     7419 2023-07-30 19:15:57.000000 assrs-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     5028 1970-01-01 00:00:00.000000 assrs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 assrs-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      123     2773 2023-08-06 21:28:00.000000 assrs-0.1.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      686 2023-08-06 21:28:00.000000 assrs-0.1.1/.gitignore
+-rw-r--r--   0     1001      123      471 2023-08-06 21:28:00.000000 assrs-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123     5369 2023-08-06 21:28:00.000000 assrs-0.1.1/README.md
+-rw-r--r--   0     1001      123     1072 2023-08-06 21:28:00.000000 assrs-0.1.1/assrs.pyi
+-rw-r--r--   0     1001      123      804 2023-08-06 21:28:00.000000 assrs-0.1.1/pyproject.toml
+-rw-r--r--   0     1001      123     5631 2023-08-06 21:28:00.000000 assrs-0.1.1/src/bktree.rs
+-rw-r--r--   0     1001      123     8204 2023-08-06 21:28:00.000000 assrs-0.1.1/src/levenshtein.rs
+-rw-r--r--   0     1001      123      955 2023-08-06 21:28:00.000000 assrs-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      123     4672 2023-08-06 21:28:00.000000 assrs-0.1.1/src/trie.rs
+-rw-r--r--   0     1001      123     1789 2023-08-06 21:28:00.000000 assrs-0.1.1/test.py
+-rw-r--r--   0     1001      123     7419 2023-08-06 21:28:10.000000 assrs-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0     6233 1970-01-01 00:00:00.000000 assrs-0.1.1/PKG-INFO
```

### Comparing `assrs-0.1.0/.github/workflows/CI.yml` & `assrs-0.1.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `assrs-0.1.0/.gitignore` & `assrs-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `assrs-0.1.0/README.md` & `assrs-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -62,37 +62,53 @@
 
 The above is combined with a reasonably performant implementation of
 Levenshtein distance, using the bitvector algorithm by [Myers][1] for strings
 up to 64 characters long.
 
 ### Performance
 
-Using [rapidfuzz][4] as a reference.
+Using [rapidfuzz][4] as a reference. Results of running `test.py` with Python
+3.11 on a Mac mini 2020 (M1, 16GB RAM).
 
 Taking a dictionary (235,976 words) as index and every 1000th as a query:
-- `Trie.find_one`: 2.28ms
-- `Trie.find_one(..., max_edits=3)`: 1.31ms
-- `BKTree.find_one`: 11.61ms
-- `BKTree.find_one(..., max_edits=3)`: 3.70ms
-- `levenshtein_extract`: 24.06ms
-- `levenshtein` in a Python loop: 36.94ms
-- `rapidfuzz.process.extractOne(..., scorer=rapidfuzz.distance.Levenshtein.distance)`: 4.08ms
-- `rapidfuzz.distance.Levenshtein.distance` in a Python loop: 43.75ms
+- `assrs.Trie.find_one`: 1.00ms
+- `assrs.Trie.find_one(..., max_edits=3)`: 0.43ms
+- `assrs.BKTree.find_one`: 6.35ms
+- `assrs.BKTree.find_one(..., max_edits=3)`: 3.43ms
+- `assrs.levenshtein_extract`: 11.25ms
+- `assrs.levenshtein` in a Python loop: 31.72ms
+- `rapidfuzz.process.extractOne(..., scorer=rapidfuzz.distance.Levenshtein.distance)`: 4.10ms
+- `rapidfuzz.distance.Levenshtein.distance` in a Python loop: 43.32ms
 
 However, with 100,000 random strings of length 10 as index and querying random strings:
-- `Trie.find_one`: 36.44ms
-- `Trie.find_one(..., max_edits=3)`: 15.84ms
-- `BKTree.find_one`: 15.36ms
-- `BKTree.find_one(..., max_edits=3)`: 13.79ms
-- `levenshtein_extract`: 10.89ms
-- `levenshtein` in a Python loop: 16.45ms
-- `rapidfuzz.process.extractOne(..., scorer=rapidfuzz.distance.Levenshtein.distance)`: 4.29ms
-- `rapidfuzz.distance.Levenshtein.distance` in a Python loop: 17.67ms
-
-
+- `assrs.Trie.find_one`: 17.87ms
+- `assrs.Trie.find_one(..., max_edits=3)`: 5.40ms
+- `assrs.BKTree.find_one`: 11.75ms
+- `assrs.BKTree.find_one(..., max_edits=3)`: 11.67ms
+- `assrs.levenshtein_extract`: 8.61ms
+- `assrs.levenshtein` in a Python loop: 14.06ms
+- `rapidfuzz.process.extractOne(..., scorer=rapidfuzz.distance.Levenshtein.distance)`: 4.21ms
+- `rapidfuzz.distance.Levenshtein.distance` in a Python loop: 17.64ms
+
+The tree based structures have a significant advantage if the index is
+relatively low entropy, like a dictionary of words from a natural language.
+However, a random set of strings causes especially poor performance for tries
+due to the excessive branching (e.g. considering that 62^3 is 238,328, it is
+highly likely that the number of explored nodes is roughly the same order of
+magnitude as the size of the index), and limits the benefits from the structure
+of the index. Instead, the overhead from traversing the tree, and extra
+distance calculations, can mean they are slower than straightforwardly
+iterating through the list of choices. Regardless, using a `Trie` with a
+`max_edits` limit remains competitive even in the worst-case scenario and
+offers a significant speedup in case of a nicer index.
+
+The difference between `assrs.levenshtein_extract` and
+`rapidfuzz.process.extractOne` (that notably disappears when the corresponding
+distance functions are called in a Python loop) seems likely attributable to
+this library not using SIMD operations.
 
 ### Limitations
 
 Currently missing features and known issues:
 - poor worst case performance for lookups,
 - not using bitvectors for strings longer than 64 characters,
 - support for segmenting over grapheme clusters rather than codepoints,
```

### Comparing `assrs-0.1.0/assrs.pyi` & `assrs-0.1.1/assrs.pyi`

 * *Files identical despite different names*

### Comparing `assrs-0.1.0/pyproject.toml` & `assrs-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -17,7 +17,13 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
+
+[tool.pylint.main]
+extension-pkg-whitelist = ["assrs"]
+
+[tool.pylint.reports]
+output-format = "colorized"
```

### Comparing `assrs-0.1.0/src/bktree.rs` & `assrs-0.1.1/src/bktree.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,57 +1,84 @@
 use pyo3::prelude::*;
 use std::collections::hash_map::Entry::{Occupied, Vacant};
-use std::collections::{HashMap, VecDeque};
+use std::collections::HashMap;
 use std::iter::once;
 
 use crate::levenshtein;
 
+#[derive(Debug, Default, Clone)]
 struct Tree {
     value: String,
-    children: HashMap<usize, Tree>,
+    // Expensive to iterate over HashMap as O(capacity) rather than O(len)
+    children_index: HashMap<u32, usize>,
+    children: Vec<(u32, Tree)>,
 }
 
 impl Tree {
     fn new(value: String) -> Self {
         Self {
             value,
-            children: HashMap::new(),
+            ..Default::default()
         }
     }
 
     fn insert(&mut self, value: String) {
         let distance = levenshtein::levenshtein(&value, &self.value);
         if distance == 0 {
             return;
         }
-        match self.children.entry(distance) {
-            Occupied(mut entry) => entry.get_mut().insert(value),
+        match self.children_index.entry(distance) {
+            Occupied(entry) => self.children[*entry.get()].1.insert(value),
             Vacant(entry) => {
-                entry.insert(Self::new(value));
+                entry.insert(self.children.len());
+                self.children.push((distance, Self::new(value)));
             }
         };
     }
+
+    fn find_one(&self, query: &str, max_edits: u32) -> Option<(&str, u32)> {
+        let mut best = None;
+        let mut max_edits = max_edits;
+        let mut stack = vec![self];
+        while let Some(node) = stack.pop() {
+            let distance = levenshtein::levenshtein(query, &node.value);
+            if distance <= max_edits {
+                best = Some((node.value.as_str(), distance));
+                if distance == 0 {
+                    return best;
+                }
+                max_edits = distance - 1;
+            };
+            for (d, subtree) in node.children.iter() {
+                if d.abs_diff(distance) <= max_edits {
+                    stack.push(subtree);
+                }
+            }
+        }
+        best
+    }
 }
 
 /// BK-tree storing the strings to search against
 #[pyclass]
+#[derive(Debug, Default, Clone)]
 pub struct BKTree {
     tree: Option<Tree>,
 }
 
 #[pymethods]
 impl BKTree {
     #[new]
     pub fn py_new(items: Option<Vec<String>>) -> Self {
         items.map_or_else(Self::new, Self::from_iter)
     }
 
     #[staticmethod]
     pub fn new() -> Self {
-        Self { tree: None }
+        Self::default()
     }
 
     pub fn insert(&mut self, value: String) {
         match self.tree.as_mut() {
             Some(t) => t.insert(value),
             None => {
                 self.tree = Some(Tree::new(value));
@@ -62,61 +89,32 @@
     pub fn get(&self, value: &str) -> Option<&str> {
         let mut node = self.tree.as_ref()?;
         loop {
             let distance = levenshtein::levenshtein(value, &node.value);
             if distance == 0 {
                 break;
             }
-            node = node.children.get(&distance)?;
+            let idx = node.children_index.get(&distance)?;
+            node = &node.children[*idx].1;
         }
         Some(&node.value)
     }
 
     pub fn contains(&self, value: &str) -> bool {
         self.get(value).is_some()
     }
 
     pub fn values(&self) -> Vec<&str> {
         self.iter().collect()
     }
 
     /// Find best match in BK-tree for query
-    pub fn find_one(&self, query: &str, max_edits: Option<usize>) -> Option<(&str, usize)> {
+    pub fn find_one(&self, query: &str, max_edits: Option<u32>) -> Option<(&str, u32)> {
         let tree = self.tree.as_ref()?;
-        let mut candidates = VecDeque::new();
-        candidates.push_back(tree);
-
-        let mut best = None;
-        let mut max_edits = max_edits.unwrap_or(usize::MAX);
-
-        while let Some(node) = candidates.pop_front() {
-            let distance = levenshtein::levenshtein(query, &node.value);
-            if distance <= max_edits {
-                max_edits = distance;
-                best = Some((node.value.as_str(), distance));
-            }
-            if !node.children.is_empty() {
-                let lower = distance - max_edits;
-                let upper = distance + max_edits;
-                candidates.extend(node.children.iter().filter_map(|(d, c)| {
-                    if lower < *d && *d < upper {
-                        Some(c)
-                    } else {
-                        None
-                    }
-                }));
-            }
-        }
-        best
-    }
-}
-
-impl Default for BKTree {
-    fn default() -> Self {
-        Self::new()
+        tree.find_one(query, max_edits.unwrap_or(u32::MAX))
     }
 }
 
 impl Extend<String> for BKTree {
     fn extend<I: IntoIterator<Item = String>>(&mut self, iter: I) {
         for item in iter {
             self.insert(item);
@@ -139,15 +137,15 @@
     fn into_iter(self) -> Self::IntoIter {
         self.iter()
     }
 }
 
 impl Tree {
     pub fn iter<'a>(&'a self) -> Box<dyn Iterator<Item = &'a str> + 'a> {
-        Box::new(once(self.value.as_str()).chain(self.children.values().flat_map(|x| x.iter())))
+        Box::new(once(self.value.as_str()).chain(self.children.iter().flat_map(|x| x.1.iter())))
     }
 }
 
 impl<'a> IntoIterator for &'a BKTree {
     type Item = &'a str;
     type IntoIter = Box<dyn Iterator<Item = &'a str> + 'a>;
```

### Comparing `assrs-0.1.0/src/levenshtein.rs` & `assrs-0.1.1/src/levenshtein.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,172 +1,214 @@
 use pyo3::prelude::*;
 
-pub trait AutomatonState {
-    fn step(&self, value: char) -> Self;
-    fn distance(&self) -> usize;
-    fn can_match(&self, max_edits: usize) -> bool;
-}
-
+#[derive(Debug, Clone)]
 pub struct LevenshteinAutomaton<'a> {
     string: &'a str,
     len: usize,
-    mask: u64,
-}
-
-#[derive(Clone)]
-enum LevenshteinState {
-    General(Vec<usize>),
-    Bitvector { vp: u64, vn: u64, offset: usize },
-}
-
-use LevenshteinState::*;
-
-#[derive(Clone)]
-pub struct LevenshteinAutomatonState<'a> {
-    m: &'a LevenshteinAutomaton<'a>,
-    state: LevenshteinState,
+    mask64: u64,
+    chars64: [char; 64],
 }
 
 impl<'a> LevenshteinAutomaton<'a> {
     pub fn new(string: &'a str) -> Self {
         let len = string.chars().count();
+        Self::new_assume_len(string, len)
+    }
+
+    fn new_assume_len(string: &'a str, len: usize) -> Self {
+        let mut chars64 = ['\0'; 64];
+        for (i, c) in string.chars().take(64).enumerate() {
+            chars64[i] = c;
+        }
         Self {
             string,
             len,
-            mask: 1u64.checked_shl(len as u32).unwrap_or(0).wrapping_sub(1),
+            mask64: 1u64.checked_shl(len as u32).unwrap_or(0).wrapping_sub(1),
+            chars64,
         }
     }
 
-    pub fn start(&self) -> LevenshteinAutomatonState {
-        LevenshteinAutomatonState {
-            m: self,
-            state: if self.len <= 64 {
-                LevenshteinState::Bitvector {
-                    vp: self.mask,
-                    vn: 0,
-                    offset: 0,
-                }
-            } else {
-                LevenshteinState::General((0..).take(self.len + 1).collect())
-            },
+    pub fn start(&self) -> LevenshteinState {
+        if self.len <= 64 {
+            LevenshteinState::Bitvector(LevenshteinBitvector {
+                m: self,
+                vp: self.mask64,
+                vn: 0,
+                offset: 0,
+            })
+        } else {
+            LevenshteinState::General(LevenshteinGeneral {
+                m: self,
+                v: (0..).take(self.len + 1).collect(),
+            })
         }
     }
 }
 
-impl LevenshteinAutomatonState<'_> {
+#[derive(Debug, Clone)]
+pub enum LevenshteinState<'a> {
+    General(LevenshteinGeneral<'a>),
+    Bitvector(LevenshteinBitvector<'a>),
+}
+
+pub trait AutomatonState {
+    fn step_mut(&mut self, value: char);
+    fn step(&self, value: char) -> Self;
+    fn distance(&self) -> u32;
+    fn can_match(&self, max_edits: u32) -> bool;
+}
+
+impl AutomatonState for LevenshteinState<'_> {
     fn step_mut(&mut self, value: char) {
-        match self.state {
-            General(ref mut v) => {
-                let mut sub = v[0];
-                let mut add = sub + 1;
-                let mut del;
-                v[0] = add;
-                for (i, c) in self.m.string.chars().enumerate() {
-                    del = v[i + 1];
-                    sub = if c == value { sub } else { sub + 1 };
-                    add = sub.min(add + 1).min(del + 1);
-                    sub = del;
-                    v[i + 1] = add;
-                }
-            }
-            Bitvector {
-                ref mut vp,
-                ref mut vn,
-                ref mut offset,
-            } => {
-                // Myers as described by Hyyro
-                // Step 1: D0
-                let mut pm = 0;
-                let mut x = 1u64;
-                for c in self.m.string.chars() {
-                    if c == value {
-                        pm |= x;
-                    }
-                    x <<= 1;
-                }
-                let d0 = (((pm & *vp).wrapping_add(*vp)) ^ *vp) | pm | *vn;
-                // Step 2-3: HP and HN
-                let mut hp = *vn | !(d0 | *vp);
-                let mut hn = d0 & *vp;
-                // Step 4-5: D[m,j]
-                // if (hp & mask) != 0 {
-                //     score += 1;
-                // }
-                // if (hn & mask) != 0 {
-                //     score -= 1;
-                // }
-                // Step 6-7: VP and VN
-                hp = (hp << 1) | 1;
-                hn <<= 1;
-
-                *vp = hn | !(d0 | hp);
-                *vn = hp & d0;
-                *offset += 1;
-            }
+        match self {
+            Self::General(s) => s.step_mut(value),
+            Self::Bitvector(s) => s.step_mut(value),
+        }
+    }
+
+    fn step(&self, value: char) -> Self {
+        match self {
+            Self::General(s) => Self::General(s.step(value)),
+            Self::Bitvector(s) => Self::Bitvector(s.step(value)),
+        }
+    }
+
+    fn distance(&self) -> u32 {
+        match self {
+            Self::General(s) => s.distance(),
+            Self::Bitvector(s) => s.distance(),
+        }
+    }
+
+    fn can_match(&self, max_edits: u32) -> bool {
+        match self {
+            Self::General(s) => s.can_match(max_edits),
+            Self::Bitvector(s) => s.can_match(max_edits),
         }
     }
 }
 
-impl AutomatonState for LevenshteinAutomatonState<'_> {
+#[derive(Debug, Clone)]
+pub struct LevenshteinGeneral<'a> {
+    m: &'a LevenshteinAutomaton<'a>,
+    v: Vec<u32>,
+}
+
+impl AutomatonState for LevenshteinGeneral<'_> {
+    fn step_mut(&mut self, value: char) {
+        let mut sub = self.v[0];
+        let mut add = sub + 1;
+        let mut del;
+        self.v[0] = add;
+        for (i, c) in self.m.string.chars().enumerate() {
+            del = self.v[i + 1];
+            sub = if c == value { sub } else { sub + 1 };
+            add = sub.min(add + 1).min(del + 1);
+            sub = del;
+            self.v[i + 1] = add;
+        }
+    }
+
     fn step(&self, value: char) -> Self {
         let mut new = self.clone();
         new.step_mut(value);
         new
     }
 
-    fn distance(&self) -> usize {
-        match &self.state {
-            General(v) => *v.last().unwrap(),
-            Bitvector { vp, vn, offset } => {
-                offset + (vp & self.m.mask).count_ones() as usize
-                    - (vn & self.m.mask).count_ones() as usize
+    fn distance(&self) -> u32 {
+        *self.v.last().unwrap()
+    }
+
+    fn can_match(&self, max_edits: u32) -> bool {
+        self.v.iter().min().unwrap() <= &max_edits
+    }
+}
+
+#[derive(Debug, Clone, Copy)]
+pub struct LevenshteinBitvector<'a> {
+    m: &'a LevenshteinAutomaton<'a>,
+    vp: u64,
+    vn: u64,
+    offset: u32,
+}
+
+impl AutomatonState for LevenshteinBitvector<'_> {
+    fn step_mut(&mut self, value: char) {
+        // Myers as described by Hyyro
+        // Step 1: D0
+        let mut pm = 0;
+        let mut x = 1u64;
+        for c in &self.m.chars64[..self.m.len] {
+            if c == &value {
+                pm |= x;
             }
+            x <<= 1;
         }
+        let d0 = (((pm & self.vp).wrapping_add(self.vp)) ^ self.vp) | pm | self.vn;
+        // Step 2-3: HP and HN
+        let mut hp = self.vn | !(d0 | self.vp);
+        let mut hn = d0 & self.vp;
+        // Step 4-5: D[m,j]
+        // if (hp & mask) != 0 {
+        //     score += 1;
+        // }
+        // if (hn & mask) != 0 {
+        //     score -= 1;
+        // }
+        // Step 6-7: VP and VN
+        hp = (hp << 1) | 1;
+        hn <<= 1;
+
+        self.vp = hn | !(d0 | hp);
+        self.vn = hp & d0;
+        self.offset += 1;
     }
 
-    fn can_match(&self, max_edits: usize) -> bool {
-        match &self.state {
-            General(v) => v.iter().min().unwrap() <= &max_edits,
-            Bitvector { vp, vn, offset } => {
-                *offset <= max_edits
-                    || (0..)
-                        .take(self.m.len)
-                        .map(|i| 1 << i)
-                        .scan(*offset, |state, mask| {
-                            if vp & mask != 0 {
-                                *state += 1;
-                            }
-                            if vn & mask != 0 {
-                                *state -= 1;
-                            }
-                            Some(*state)
-                        })
-                        .min()
-                        .unwrap_or(*offset)
-                        <= max_edits
+    fn step(&self, value: char) -> Self {
+        let mut new = *self;
+        new.step_mut(value);
+        new
+    }
+
+    fn distance(&self) -> u32 {
+        self.offset + (self.vp & self.m.mask64).count_ones()
+            - (self.vn & self.m.mask64).count_ones()
+    }
+
+    fn can_match(&self, max_edits: u32) -> bool {
+        self.offset <= max_edits || {
+            let mut vpi = self.vp & self.m.mask64;
+            let mut nvni = !(self.vn & self.m.mask64);
+            while vpi != 0 && !nvni != 0 {
+                // The minimum is preserved in this operation
+                // Earlier positive steps cancel out later negative ones
+                let x = nvni.wrapping_add(vpi);
+                vpi &= x;
+                nvni |= x;
             }
-        }
+            self.offset - nvni.count_zeros()
+        } <= max_edits
     }
 }
 
 /// Find the Levenshtein distance between two strings
 #[pyfunction]
-pub fn levenshtein(a: &str, b: &str) -> usize {
+pub fn levenshtein(a: &str, b: &str) -> u32 {
     if a == b {
         return 0;
     }
     let len_a = a.chars().count();
     let len_b = b.chars().count();
 
-    let (a, b) = if (len_a < len_b || len_a > 64) && len_b <= 64 {
-        (b, a)
+    let (a, len_a, b) = if (len_a < len_b || len_a > 64) && len_b <= 64 {
+        (b, len_b, a)
     } else {
-        (a, b)
+        (a, len_a, b)
     };
-    let automaton = LevenshteinAutomaton::new(a);
+    let automaton = LevenshteinAutomaton::new_assume_len(a, len_a);
     let mut state = automaton.start();
     for value in b.chars() {
         state.step_mut(value);
     }
     state.distance()
 }
 
@@ -193,15 +235,15 @@
 
     #[test]
     fn automaton() {
         let automaton = LevenshteinAutomaton::new("kitten");
         let mut state = automaton.start();
         assert_eq!(state.distance(), 6);
         assert!(state.can_match(0));
-        assert!(state.can_match(usize::MAX));
+        assert!(state.can_match(u32::MAX));
 
         state = state.step('s');
         assert_eq!(state.distance(), 6);
         assert!(!state.can_match(0));
         assert!(state.can_match(1));
 
         state = state.step('i');
@@ -243,10 +285,10 @@
         for _i in 0..128 {
             state = state.step('a');
         }
         assert_eq!(state.distance(), 192);
         assert!(!state.can_match(0));
         assert!(!state.can_match(95));
         assert!(state.can_match(96));
-        assert!(state.can_match(usize::MAX));
+        assert!(state.can_match(u32::MAX));
     }
 }
```

### Comparing `assrs-0.1.0/src/lib.rs` & `assrs-0.1.1/src/lib.rs`

 * *Files 14% similar despite different names*

```diff
@@ -7,21 +7,24 @@
 mod levenshtein;
 mod trie;
 
 /// Find the best match in a list of choices
 ///
 /// Returns (choice, distance, index) or None (for empty choices)
 #[pyfunction]
-fn levenshtein_extract(query: &str, choices: Vec<&str>) -> Option<(String, usize, usize)> {
-    choices
-        .iter()
-        .map(|x| (x, levenshtein::levenshtein(query, x)))
-        .enumerate()
-        .min_by_key(|(_i, (_x, d))| *d)
-        .map(|(i, (x, d))| (x.to_string(), d, i))
+fn levenshtein_extract(query: &str, choices: Vec<&str>) -> Option<(String, u32, usize)> {
+    let mut best = None;
+    for (i, x) in choices.iter().enumerate() {
+        let distance = levenshtein::levenshtein(query, x);
+        best = Some(best.unwrap_or((distance, i, x)).min((distance, i, x)));
+        if distance == 0 {
+            break;
+        }
+    }
+    best.map(|x| (x.2.to_string(), x.0, x.1))
 }
 
 /// Approximate string searching
 #[pymodule]
 fn assrs(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(levenshtein::levenshtein, m)?)?;
     m.add_function(wrap_pyfunction!(levenshtein_extract, m)?)?;
```

### Comparing `assrs-0.1.0/src/trie.rs` & `assrs-0.1.1/src/trie.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,68 @@
 use pyo3::prelude::*;
 use std::collections::HashMap;
 
 use crate::levenshtein::{AutomatonState, LevenshteinAutomaton};
 
-struct FindResult<'a> {
-    value: &'a str,
-    distance: usize,
-}
-
 /// Trie storing the strings to search against
 #[pyclass]
+#[derive(Debug, Default, Clone)]
 pub struct Trie {
     // Indicates terminal and nice when traversing
     value: Option<String>,
-    // Maybe expensive to iterate over O(capacity) rather than O(len)?
-    children: HashMap<char, Trie>,
+    // Expensive to iterate over HashMap as O(capacity) rather than O(len)
+    children_index: HashMap<char, usize>,
+    children: Vec<(char, Trie)>,
 }
 
 #[pymethods]
 impl Trie {
     #[new]
     pub fn py_new(items: Option<Vec<String>>) -> Self {
         items.map_or_else(Self::new, Self::from_iter)
     }
 
     #[staticmethod]
     pub fn new() -> Self {
-        Self {
-            value: None,
-            children: HashMap::new(),
-        }
+        Self::default()
     }
 
     pub fn insert(&mut self, value: String) {
         let mut node = self;
         for c in value.chars() {
-            node = node.children.entry(c).or_insert_with(Self::new);
+            let idx = node.children_index.entry(c).or_insert_with(|| {
+                node.children.push((c, Self::new()));
+                node.children.len() - 1
+            });
+            node = &mut node.children[*idx].1;
         }
         node.value = Some(value);
     }
 
     pub fn get(&self, value: &str) -> Option<&str> {
         let mut node = self;
         for c in value.chars() {
-            node = node.children.get(&c)?;
+            let idx = node.children_index.get(&c)?;
+            node = &node.children[*idx].1;
         }
         node.value.as_deref()
     }
 
     pub fn contains(&self, value: &str) -> bool {
         self.get(value).is_some()
     }
 
     pub fn values(&self) -> Vec<&str> {
         self.iter().collect()
     }
 
     /// Find best match in trie for query
-    pub fn find_one(&self, query: &str, max_edits: Option<usize>) -> Option<(&str, usize)> {
+    pub fn find_one(&self, query: &str, max_edits: Option<u32>) -> Option<(&str, u32)> {
         let automaton = LevenshteinAutomaton::new(query);
-        let result = self.find_automaton(&automaton.start(), max_edits.unwrap_or(usize::MAX))?;
-        Some((result.value, result.distance))
-    }
-}
-
-impl Default for Trie {
-    fn default() -> Self {
-        Self::new()
+        self.find_automaton(&automaton.start(), max_edits.unwrap_or(u32::MAX))
     }
 }
 
 impl Extend<String> for Trie {
     fn extend<I: IntoIterator<Item = String>>(&mut self, iter: I) {
         for item in iter {
             self.insert(item);
@@ -97,40 +89,33 @@
 
 impl Trie {
     pub fn iter<'a>(&'a self) -> Box<dyn Iterator<Item = &'a str> + 'a> {
         Box::new(
             self.value
                 .iter()
                 .map(|v| v.as_str())
-                .chain(self.children.values().flat_map(|x| x.iter())),
+                .chain(self.children.iter().flat_map(|x| x.1.iter())),
         )
     }
 
-    fn find_automaton(&self, state: &impl AutomatonState, max_edits: usize) -> Option<FindResult> {
-        let mut best = None;
+    fn find_automaton(&self, state: &impl AutomatonState, max_edits: u32) -> Option<(&str, u32)> {
         if !state.can_match(max_edits) {
-            return best;
+            return None;
         }
-        let distance = state.distance();
-        if distance <= max_edits {
-            best = self
-                .value
-                .as_ref()
-                .map(|k| FindResult { value: k, distance });
-        }
-        for (next, subtrie) in self.children.iter() {
+        let this = self
+            .value
+            .as_ref()
+            .map(|v| (v.as_str(), state.distance()))
+            .filter(|x| x.1 <= max_edits);
+        self.children.iter().fold(this, |best, (next, subtrie)| {
             // Method returns some iff best is none or distance is lower
-            if let Some(result) = subtrie.find_automaton(
-                &state.step(*next),
-                best.as_ref().map_or(max_edits, |x| x.distance - 1),
-            ) {
-                best = Some(result);
-            };
-        }
-        best
+            best.map_or(Some(max_edits), |x| x.1.checked_sub(1))
+                .and_then(|max_edits| subtrie.find_automaton(&state.step(*next), max_edits))
+                .or(best)
+        })
     }
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
     use std::collections::HashSet;
```

### Comparing `assrs-0.1.0/Cargo.lock` & `assrs-0.1.1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "assrs"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
```

### Comparing `assrs-0.1.0/PKG-INFO` & `assrs-0.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assrs
-Version: 0.1.0
+Version: 0.1.1
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -82,37 +82,53 @@
 
 The above is combined with a reasonably performant implementation of
 Levenshtein distance, using the bitvector algorithm by [Myers][1] for strings
 up to 64 characters long.
 
 ### Performance
 
-Using [rapidfuzz][4] as a reference.
+Using [rapidfuzz][4] as a reference. Results of running `test.py` with Python
+3.11 on a Mac mini 2020 (M1, 16GB RAM).
 
 Taking a dictionary (235,976 words) as index and every 1000th as a query:
-- `Trie.find_one`: 2.28ms
-- `Trie.find_one(..., max_edits=3)`: 1.31ms
-- `BKTree.find_one`: 11.61ms
-- `BKTree.find_one(..., max_edits=3)`: 3.70ms
-- `levenshtein_extract`: 24.06ms
-- `levenshtein` in a Python loop: 36.94ms
-- `rapidfuzz.process.extractOne(..., scorer=rapidfuzz.distance.Levenshtein.distance)`: 4.08ms
-- `rapidfuzz.distance.Levenshtein.distance` in a Python loop: 43.75ms
+- `assrs.Trie.find_one`: 1.00ms
+- `assrs.Trie.find_one(..., max_edits=3)`: 0.43ms
+- `assrs.BKTree.find_one`: 6.35ms
+- `assrs.BKTree.find_one(..., max_edits=3)`: 3.43ms
+- `assrs.levenshtein_extract`: 11.25ms
+- `assrs.levenshtein` in a Python loop: 31.72ms
+- `rapidfuzz.process.extractOne(..., scorer=rapidfuzz.distance.Levenshtein.distance)`: 4.10ms
+- `rapidfuzz.distance.Levenshtein.distance` in a Python loop: 43.32ms
 
 However, with 100,000 random strings of length 10 as index and querying random strings:
-- `Trie.find_one`: 36.44ms
-- `Trie.find_one(..., max_edits=3)`: 15.84ms
-- `BKTree.find_one`: 15.36ms
-- `BKTree.find_one(..., max_edits=3)`: 13.79ms
-- `levenshtein_extract`: 10.89ms
-- `levenshtein` in a Python loop: 16.45ms
-- `rapidfuzz.process.extractOne(..., scorer=rapidfuzz.distance.Levenshtein.distance)`: 4.29ms
-- `rapidfuzz.distance.Levenshtein.distance` in a Python loop: 17.67ms
-
-
+- `assrs.Trie.find_one`: 17.87ms
+- `assrs.Trie.find_one(..., max_edits=3)`: 5.40ms
+- `assrs.BKTree.find_one`: 11.75ms
+- `assrs.BKTree.find_one(..., max_edits=3)`: 11.67ms
+- `assrs.levenshtein_extract`: 8.61ms
+- `assrs.levenshtein` in a Python loop: 14.06ms
+- `rapidfuzz.process.extractOne(..., scorer=rapidfuzz.distance.Levenshtein.distance)`: 4.21ms
+- `rapidfuzz.distance.Levenshtein.distance` in a Python loop: 17.64ms
+
+The tree based structures have a significant advantage if the index is
+relatively low entropy, like a dictionary of words from a natural language.
+However, a random set of strings causes especially poor performance for tries
+due to the excessive branching (e.g. considering that 62^3 is 238,328, it is
+highly likely that the number of explored nodes is roughly the same order of
+magnitude as the size of the index), and limits the benefits from the structure
+of the index. Instead, the overhead from traversing the tree, and extra
+distance calculations, can mean they are slower than straightforwardly
+iterating through the list of choices. Regardless, using a `Trie` with a
+`max_edits` limit remains competitive even in the worst-case scenario and
+offers a significant speedup in case of a nicer index.
+
+The difference between `assrs.levenshtein_extract` and
+`rapidfuzz.process.extractOne` (that notably disappears when the corresponding
+distance functions are called in a Python loop) seems likely attributable to
+this library not using SIMD operations.
 
 ### Limitations
 
 Currently missing features and known issues:
 - poor worst case performance for lookups,
 - not using bitvectors for strings longer than 64 characters,
 - support for segmenting over grapheme clusters rather than codepoints,
```

