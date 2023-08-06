# Comparing `tmp/mapfile_parser-1.3.1.tar.gz` & `tmp/mapfile_parser-2.0.0.tar.gz`

## Comparing `mapfile_parser-1.3.1.tar` & `mapfile_parser-2.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mapfile_parser-1.3.1/.gitattributes
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 mapfile_parser-1.3.1/mypy.ini
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 mapfile_parser-1.3.1/requirements.txt
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 mapfile_parser-1.3.1/.github/workflows/mypy.yml
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 mapfile_parser-1.3.1/.github/workflows/upload_pypi.yml
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 mapfile_parser-1.3.1/src/mapfile_parser/__init__.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 mapfile_parser-1.3.1/src/mapfile_parser/__main__.py
--rw-r--r--   0        0        0    18204 2020-02-02 00:00:00.000000 mapfile_parser-1.3.1/src/mapfile_parser/mapfile.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 mapfile_parser-1.3.1/src/mapfile_parser/progress_stats.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 mapfile_parser-1.3.1/src/mapfile_parser/utils.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 mapfile_parser-1.3.1/src/mapfile_parser/frontends/__init__.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 mapfile_parser-1.3.1/src/mapfile_parser/frontends/first_diff.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 mapfile_parser-1.3.1/src/mapfile_parser/frontends/jsonify.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 mapfile_parser-1.3.1/src/mapfile_parser/frontends/pj64_syms.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 mapfile_parser-1.3.1/src/mapfile_parser/frontends/progress.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 mapfile_parser-1.3.1/src/mapfile_parser/frontends/sym_info.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 mapfile_parser-1.3.1/src/mapfile_parser/frontends/symbol_sizes_csv.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 mapfile_parser-1.3.1/src/mapfile_parser/frontends/upload_frogress.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 mapfile_parser-1.3.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mapfile_parser-1.3.1/LICENSE
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 mapfile_parser-1.3.1/README.md
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 mapfile_parser-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 mapfile_parser-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/.gitattributes
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/mypy.ini
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/requirements.txt
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/.github/workflows/mypy.yml
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/.github/workflows/upload_pypi.yml
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/src/mapfile_parser/__init__.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/src/mapfile_parser/__main__.py
+-rw-r--r--   0        0        0    21625 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/src/mapfile_parser/mapfile.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/src/mapfile_parser/progress_stats.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/src/mapfile_parser/utils.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/src/mapfile_parser/frontends/__init__.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/src/mapfile_parser/frontends/first_diff.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/src/mapfile_parser/frontends/jsonify.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/src/mapfile_parser/frontends/pj64_syms.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/src/mapfile_parser/frontends/progress.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/src/mapfile_parser/frontends/sym_info.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/src/mapfile_parser/frontends/symbol_sizes_csv.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/src/mapfile_parser/frontends/upload_frogress.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/README.md
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/PKG-INFO
```

### Comparing `mapfile_parser-1.3.1/.github/workflows/mypy.yml` & `mapfile_parser-2.0.0/.github/workflows/mypy.yml`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.3.1/.github/workflows/upload_pypi.yml` & `mapfile_parser-2.0.0/.github/workflows/upload_pypi.yml`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.3.1/src/mapfile_parser/__init__.py` & `mapfile_parser-2.0.0/src/mapfile_parser/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #!/usr/bin/env python3
 
 # SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
-__version_info__ = (1, 3, 1)
+__version_info__ = (2, 0, 0)
 __version__ = ".".join(map(str, __version_info__))
 __author__ = "Decompollaborate"
 
 from . import utils as utils
 
 from .mapfile import MapFile as MapFile
 from .mapfile import Symbol as Symbol
 from .mapfile import File as File
+from .mapfile import Segment as Segment
 from .mapfile import FoundSymbolInfo as FoundSymbolInfo
 
 from .progress_stats import ProgressStats as ProgressStats
 
 from . import frontends as frontends
```

### Comparing `mapfile_parser-1.3.1/src/mapfile_parser/__main__.py` & `mapfile_parser-2.0.0/src/mapfile_parser/__main__.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.3.1/src/mapfile_parser/mapfile.py` & `mapfile_parser-2.0.0/src/mapfile_parser/mapfile.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,100 +3,105 @@
 # SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import dataclasses
 import re
-from typing import Any, Generator
+from typing import Generator
 from pathlib import Path
 
 from .progress_stats import ProgressStats
 from . import utils
 
 
 regex_fileDataEntry = re.compile(r"^\s+(?P<section>\.[^\s]+)\s+(?P<vram>0x[^\s]+)\s+(?P<size>0x[^\s]+)\s+(?P<name>[^\s]+)$")
 regex_functionEntry = re.compile(r"^\s+(?P<vram>0x[^\s]+)\s+(?P<name>[^\s]+)$")
 regex_label = re.compile(r"^(?P<name>\.?L[0-9A-F]{8})$")
 regex_fill = re.compile(r"^\s+(?P<fill>\*[^\s\*]+\*)\s+(?P<vram>0x[^\s]+)\s+(?P<size>0x[^\s]+)\s*$")
-regex_loadAddress = re.compile(r"\s+(?P<vram>0x[^\s]+)\s+(?P<size>0x[^\s]+)\s+(?P<loadaddress>load address)\s+(?P<vrom>0x[^\s]+)$")
+regex_segmentEntry = re.compile(r"(?P<name>([^\s]+)?)\s+(?P<vram>0x[^\s]+)\s+(?P<size>0x[^\s]+)\s+(?P<loadaddress>(load address)?)\s+(?P<vrom>0x[^\s]+)$")
+
 
 @dataclasses.dataclass
-class LoadAddressData:
-    vram: int
-    size: int
-    vrom: int
+class FoundSymbolInfo:
+    file: File
+    symbol: Symbol
+    offset: int = 0
+
+    def getAsStr(self) -> str:
+        return f"'{self.symbol.name}' (VRAM: {self.symbol.getVramStr()}, VROM: {self.symbol.getVromStr()}, SIZE: {self.symbol.getSizeStr()}, {self.file.filepath})"
+
+    def getAsStrPlusOffset(self, symName: str|None=None) -> str:
+        if self.offset != 0:
+            if symName is not None:
+                message = symName
+            else:
+                message = f"0x{self.symbol.vram + self.offset:X}"
+            message += f" is at 0x{self.offset:X} bytes inside"
+        else:
+            message = "Symbol"
+        return f"{message} {self.getAsStr()}"
 
 @dataclasses.dataclass
 class Symbol:
     name: str
     vram: int
-    size: int = -1 # in bytes
+    size: int|None = None # in bytes
     vrom: int|None = None
 
     def getVramStr(self) -> str:
         return f"0x{self.vram:08X}"
 
     def getSizeStr(self) -> str:
-        if self.size < 0:
+        if self.size is None:
             return "None"
         return f"0x{self.size:X}"
 
     def getVromStr(self) -> str:
         if self.vrom is None:
             return "None"
         return f"0x{self.vrom:06X}"
 
     def serializeSize(self) -> str|None:
-        if self.size < 0:
+        if self.size is None:
             return None
         return f"0x{self.size:X}"
 
 
     @staticmethod
     def printCsvHeader():
         print("Symbol name,VRAM,Size in bytes")
 
     def printAsCsv(self):
         print(f"{self.name},{self.vram:08X},{self.size}")
 
 
-    def toJson(self) -> dict[str, Any]:
-        result: dict[str, Any] = {
+    def toJson(self) -> dict:
+        result = {
             "name": self.name,
             "vram": self.getVramStr(),
             "size": self.serializeSize(),
             "vrom": self.getVromStr(),
         }
 
         return result
 
 
-    def __eq__(self, other: object) -> bool:
-        if not isinstance(other, Symbol):
-            return False
-        return self.name == other.name and self.vram == other.vram
-
-    # https://stackoverflow.com/a/56915493/6292472
-    def __hash__(self):
-        return hash((self.name, self.vram))
-
-
 @dataclasses.dataclass
 class File:
     filepath: Path
     vram: int
     size: int # in bytes
-    segmentType: str
-    symbols: list[Symbol] = dataclasses.field(default_factory=list)
+    sectionType: str
     vrom: int|None = None
+    _symbols: list[Symbol] = dataclasses.field(default_factory=list)
 
     @property
-    def isNoloadSegment(self) -> bool:
-        return self.segmentType == ".bss"
+    def isNoloadSection(self) -> bool:
+        return self.sectionType == ".bss"
 
 
     def serializeVram(self) -> str|None:
         return f"0x{self.vram:08X}"
 
     def serializeSize(self) -> str|None:
         return f"0x{self.size:X}"
@@ -107,27 +112,27 @@
         return f"0x{self.vrom:06X}"
 
 
     def getName(self) -> Path:
         return Path(*self.filepath.with_suffix("").parts[2:])
 
     def findSymbolByName(self, symName: str) -> Symbol|None:
-        for sym in self.symbols:
+        for sym in self._symbols:
             if sym.name == symName:
                 return sym
         return None
 
     def findSymbolByVramOrVrom(self, address: int) -> tuple[Symbol, int]|None:
         prevVram = self.vram
         prevVrom = self.vrom
         prevSym: Symbol|None = None
 
         isVram = address >= 0x1000000
 
-        for sym in self.symbols:
+        for sym in self._symbols:
             if sym.vram == address:
                 return sym, 0
             if sym.vrom == address:
                 return sym, 0
 
             if prevSym is not None:
                 if (sym.vrom is not None and sym.vrom > address) or (isVram and sym.vram > address):
@@ -141,15 +146,15 @@
                     return prevSym, offset
 
             prevVram = sym.vram
             prevVrom = sym.vrom
             prevSym = sym
 
         if prevSym is not None:
-            if (prevSym.vrom is not None and prevSym.vrom + prevSym.size > address) or (isVram and prevSym.vram + prevSym.size > address):
+            if (prevSym.vrom is not None and prevSym.size is not None and prevSym.vrom + prevSym.size > address) or (isVram and prevSym.size is not None and prevSym.vram + prevSym.size > address):
                 if isVram:
                     offset = address - prevVram
                 else:
                     assert isinstance(prevVrom, int)
                     offset = address - prevVrom
                 if offset < 0:
                     return None
@@ -157,93 +162,198 @@
 
         return None
 
     @staticmethod
     def printCsvHeader(printVram: bool=True):
         if printVram:
             print("VRAM,", end="")
-        print("File,Segment type,Num symbols,Max size,Total size,Average size")
+        print("File,Section type,Num symbols,Max size,Total size,Average size")
 
     def printAsCsv(self, printVram: bool=True):
         # Calculate stats
-        symCount = len(self.symbols)
+        symCount = len(self._symbols)
         maxSize = 0
         averageSize = self.size / (symCount or 1)
-        for sym in self.symbols:
-            symSize = sym.size
-            if symSize > maxSize:
-                maxSize = symSize
+        for sym in self._symbols:
+            if sym.size is not None and sym.size > maxSize:
+                maxSize = sym.size
 
         if printVram:
             print(f"{self.vram:08X},", end="")
-        print(f"{self.filepath},{self.segmentType},{symCount},{maxSize},{self.size},{averageSize:0.2f}")
+        print(f"{self.filepath},{self.sectionType},{symCount},{maxSize},{self.size},{averageSize:0.2f}")
 
 
-    def toJson(self) -> dict[str, Any]:
-        fileDict: dict[str, Any] = {
+    def toJson(self) -> dict:
+        fileDict: dict = {
             "filepath": str(self.filepath),
-            "segmentType": self.segmentType,
+            "sectionType": self.sectionType,
             "vram": self.serializeVram(),
             "size": self.serializeSize(),
             "vrom": self.serializeVrom(),
         }
 
         symbolsList = []
-        for symbol in self.symbols:
+        for symbol in self._symbols:
             symbolsList.append(symbol.toJson())
 
         fileDict["symbols"] = symbolsList
         return fileDict
 
 
     def __iter__(self) -> Generator[Symbol, None, None]:
-        for sym in self.symbols:
+        for sym in self._symbols:
             yield sym
 
     def __getitem__(self, index) -> Symbol:
-        return self.symbols[index]
+        return self._symbols[index]
 
-    def __eq__(self, other: object) -> bool:
-        if not isinstance(other, File):
-            return False
-        return self.filepath == other.filepath
-
-    # https://stackoverflow.com/a/56915493/6292472
-    def __hash__(self):
-        return hash((self.filepath,))
+    def __setitem__(self, index, sym: Symbol):
+        self._symbols[index] = sym
+
+    def __len__(self) -> int:
+        return len(self._symbols)
 
 
 @dataclasses.dataclass
-class FoundSymbolInfo:
-    file: File
-    symbol: Symbol
-    offset: int = 0
+class Segment:
+    name: str
+    vram: int
+    size: int
+    vrom: int
+    _filesList: list[File] = dataclasses.field(default_factory=list)
 
-    def getAsStr(self) -> str:
-        return f"'{self.symbol.name}' (VRAM: {self.symbol.getVramStr()}, VROM: {self.symbol.getVromStr()}, SIZE: {self.symbol.getSizeStr()}, {self.file.filepath})"
+    def serializeVram(self) -> str|None:
+        return f"0x{self.vram:08X}"
+
+    def serializeSize(self) -> str|None:
+        return f"0x{self.size:X}"
+
+    def serializeVrom(self) -> str|None:
+        return f"0x{self.vrom:06X}"
+
+
+    def filterBySectionType(self, sectionType: str) -> Segment:
+        newSegment = Segment(self.name, self.vram, self.size, self.vrom)
+
+        for file in self._filesList:
+            if file.sectionType == sectionType:
+                newSegment._filesList.append(file)
+        return newSegment
+
+    def getEveryFileExceptSectionType(self, sectionType: str) -> Segment:
+        newSegment = Segment(self.name, self.vram, self.size, self.vrom)
+
+        for file in self._filesList:
+            if file.sectionType != sectionType:
+                newSegment._filesList.append(file)
+        return newSegment
+
+
+    def findSymbolByName(self, symName: str) -> FoundSymbolInfo|None:
+        for file in self._filesList:
+            sym = file.findSymbolByName(symName)
+            if sym is not None:
+                return FoundSymbolInfo(file, sym)
+        return None
+
+    def findSymbolByVramOrVrom(self, address: int) -> FoundSymbolInfo|None:
+        for file in self._filesList:
+            pair = file.findSymbolByVramOrVrom(address)
+            if pair is not None:
+                sym, offset = pair
+                return FoundSymbolInfo(file, sym, offset)
+        return None
+
+
+    def mixFolders(self) -> Segment:
+        newSegment = Segment(self.name, self.vram, self.size, self.vrom)
+
+        auxDict: dict[Path, list[File]] = dict()
+
+        # Put files in the same folder together
+        for file in self._filesList:
+            path = Path(*file.getName().parts[:-1])
+            if path not in auxDict:
+                auxDict[path] = list()
+            auxDict[path].append(file)
+
+        # Pretend files in the same folder are one huge file
+        for folderPath, filesInFolder in auxDict.items():
+            firstFile = filesInFolder[0]
+
+            vram = firstFile.vram
+            size = 0
+            vrom = firstFile.vrom
+            sectionType = firstFile.sectionType
+
+            symbols = list()
+            for file in filesInFolder:
+                size += file.size
+                for sym in file:
+                    symbols.append(sym)
+
+            newSegment._filesList.append(File(folderPath, vram, size, sectionType, vrom, symbols))
+
+        return newSegment
+
+    def printAsCsv(self, printVram: bool=True, skipWithoutSymbols: bool=True):
+        for file in self._filesList:
+            if skipWithoutSymbols and len(file) == 0:
+                continue
+
+            file.printAsCsv(printVram)
+        return
+
+    def printSymbolsCsv(self):
+        for file in self._filesList:
+            if len(file) == 0:
+                continue
+
+            for sym in file:
+                print(f"{file.filepath},", end="")
+                sym.printAsCsv()
+        return
+
+
+    def toJson(self) -> dict:
+        segmentDict: dict = {
+            "name": self.name,
+            "vram": self.serializeVram(),
+            "size": self.serializeSize(),
+            "vrom": self.serializeVrom(),
+        }
+
+        filesList = []
+        for file in self._filesList:
+            filesList.append(file.toJson())
+
+        segmentDict["files"] = filesList
+
+        return segmentDict
+
+
+    def __iter__(self) -> Generator[File, None, None]:
+        for file in self._filesList:
+            yield file
+
+    def __getitem__(self, index) -> File:
+        return self._filesList[index]
+
+    def __len__(self) -> int:
+        return len(self._filesList)
 
-    def getAsStrPlusOffset(self, symName: str|None=None) -> str:
-        if self.offset != 0:
-            if symName is not None:
-                message = symName
-            else:
-                message = f"0x{self.symbol.vram + self.offset:X}"
-            message += f" is at 0x{self.offset:X} bytes inside"
-        else:
-            message = "Symbol"
-        return f"{message} {self.getAsStr()}"
 
 class MapFile:
     def __init__(self):
-        self.filesList: list[File] = list()
+        self._segmentsList: list[Segment] = list()
         self.debugging: bool = False
 
     def readMapFile(self, mapPath: Path):
-        tempFilesList: list[File] = list()
-        loadAddressData: LoadAddressData|None = None
+        tempSegmentsList: list[Segment] = list()
+        tempFilesListList: list[list[File]] = list()
 
         with mapPath.open("r") as f:
             mapData = f.read()
 
             # Skip the stuff we don't care about
             startIndex = 0
             auxVar = 0
@@ -254,291 +364,282 @@
             if auxVar != -1:
                 startIndex = auxVar
             mapData = mapData[startIndex:]
         # print(len(mapData))
 
         inFile = False
 
+        prevLine = ""
         mapLines = mapData.split("\n")
         for line in mapLines:
             if inFile:
                 if line.startswith("                "):
                     entryMatch = regex_functionEntry.search(line)
 
                     # Find function
                     if entryMatch is not None:
                         funcName = entryMatch["name"]
                         funcVram = int(entryMatch["vram"], 16)
 
                         # Filter out jump table's labels
                         labelMatch = regex_label.search(funcName)
                         if labelMatch is None:
-                            tempFilesList[-1].symbols.append(Symbol(funcName, funcVram))
+                            tempFilesListList[-1][-1]._symbols.append(Symbol(funcName, funcVram))
                         # print(hex(funcVram), funcName)
 
                 else:
                     inFile = False
 
             if not inFile:
                 fillMatch = regex_fill.search(line)
                 entryMatch = regex_fileDataEntry.search(line)
-                loadAddressMatch = regex_loadAddress.search(line)
+                loadAddressMatch = regex_segmentEntry.search(line)
 
                 if fillMatch is not None:
                     # Add *fill* size to last file
                     size = int(fillMatch["size"], 16)
-                    tempFilesList[-1].size += size
+                    tempFilesListList[-1][-1].size += size
                 elif entryMatch is not None:
                     # Find file
                     filepath = Path(entryMatch["name"])
                     size = int(entryMatch["size"], 16)
                     vram = int(entryMatch["vram"], 16)
-                    segmentType = entryMatch["section"]
+                    sectionType = entryMatch["section"]
 
                     if size > 0:
                         inFile = True
-                        tempFile = File(filepath, vram, size, segmentType)
-                        if loadAddressData is not None and loadAddressData.vram == vram and not tempFile.isNoloadSegment:
-                            tempFile.vrom = loadAddressData.vrom
-                        tempFilesList.append(tempFile)
+                        tempFile = File(filepath, vram, size, sectionType)
+                        tempFilesListList[-1].append(tempFile)
 
                 elif loadAddressMatch is not None:
+                    name = loadAddressMatch["name"]
                     vram = int(loadAddressMatch["vram"], 0)
                     size = int(loadAddressMatch["size"], 0)
                     vrom = int(loadAddressMatch["vrom"], 0)
 
-                    loadAddressData = LoadAddressData(vram, size, vrom)
-
-        vromOffset = 0
-        for file in tempFilesList:
-            acummulatedSize = 0
-            symbolsCount = len(file.symbols)
-
-            if file.vrom is not None:
-                vromOffset = file.vrom
-
-            isNoloadSegment = file.isNoloadSegment
-            if not isNoloadSegment:
-                file.vrom = vromOffset
-
-            if symbolsCount > 0:
-                symVrom = vromOffset
-
-                # Calculate size of each symbol
-                for index in range(symbolsCount-1):
-                    func = file.symbols[index]
-                    nextFunc = file.symbols[index+1]
-
-                    size = (nextFunc.vram - func.vram)
-                    acummulatedSize += size
-
-                    file.symbols[index] = Symbol(func.name, func.vram, size)
-
-                    if not isNoloadSegment:
-                        # Only set vrom of non bss variables
-                        file.symbols[index].vrom = symVrom
+                    if name == "":
+                        # If the segment name is too long then this line gets break in two lines
+                        name = prevLine
+
+                    tempSegment = Segment(name, vram, size, vrom)
+                    tempSegmentsList.append(tempSegment)
+                    tempFilesListList.append([])
+
+            prevLine = line
+
+        for i, segment in enumerate(tempSegmentsList):
+            filesList = tempFilesListList[i]
+
+            vromOffset = segment.vrom
+            for file in filesList:
+                acummulatedSize = 0
+                symbolsCount = len(file)
+
+                if file.vrom is not None:
+                    vromOffset = file.vrom
+
+                isNoloadSection = file.isNoloadSection
+                if not isNoloadSection:
+                    file.vrom = vromOffset
+
+                if symbolsCount > 0:
+                    symVrom = vromOffset
+
+                    # Calculate size of each symbol
+                    for index in range(symbolsCount-1):
+                        func = file[index]
+                        nextFunc = file[index+1]
+
+                        size = (nextFunc.vram - func.vram)
+                        acummulatedSize += size
+
+                        file[index] = Symbol(func.name, func.vram, size)
+
+                        if not isNoloadSection:
+                            # Only set vrom of non bss variables
+                            file[index].vrom = symVrom
+                            symVrom += size
+
+                    # Calculate size of last symbol of the file
+                    func = file[symbolsCount-1]
+                    size = file.size - acummulatedSize
+                    file[symbolsCount-1] = Symbol(func.name, func.vram, size)
+                    if not isNoloadSection:
+                        file[symbolsCount-1].vrom = symVrom
                         symVrom += size
 
-                # Calculate size of last symbol of the file
-                func = file.symbols[symbolsCount-1]
-                size = file.size - acummulatedSize
-                file.symbols[symbolsCount-1] = Symbol(func.name, func.vram, size)
-                if not isNoloadSegment:
-                    file.symbols[symbolsCount-1].vrom = symVrom
-                    symVrom += size
-
-            if not isNoloadSegment:
-                # Only increment vrom offset for non bss segments
-                vromOffset += file.size
+                if not isNoloadSection:
+                    # Only increment vrom offset for non bss sections
+                    vromOffset += file.size
 
-            self.filesList.append(file)
+                segment._filesList.append(file)
+            self._segmentsList.append(segment)
         return
 
-    def filterBySegmentType(self, segmentType: str) -> MapFile:
+    def filterBySectionType(self, sectionType: str) -> MapFile:
         newMapFile = MapFile()
 
         newMapFile.debugging = self.debugging
 
-        for file in self.filesList:
-            if file.segmentType == segmentType:
-                newMapFile.filesList.append(file)
+        for segment in self._segmentsList:
+            newSegment = segment.filterBySectionType(sectionType)
+            if len(newSegment) != 0:
+                newMapFile._segmentsList.append(newSegment)
         return newMapFile
 
-    def getEveryFileExceptSegmentType(self, segmentType: str) -> MapFile:
+    def getEveryFileExceptSectionType(self, sectionType: str) -> MapFile:
         newMapFile = MapFile()
 
         newMapFile.debugging = self.debugging
 
-        for file in self.filesList:
-            if file.segmentType != segmentType:
-                newMapFile.filesList.append(file)
+        for segment in self._segmentsList:
+            newSegment = segment.getEveryFileExceptSectionType(sectionType)
+            if len(newSegment) != 0:
+                newMapFile._segmentsList.append(newSegment)
         return newMapFile
 
 
     def findSymbolByName(self, symName: str) -> FoundSymbolInfo|None:
-        for file in self.filesList:
-            sym = file.findSymbolByName(symName)
-            if sym is not None:
-                return FoundSymbolInfo(file, sym)
+        for segment in self._segmentsList:
+            info = segment.findSymbolByName(symName)
+            if info is not None:
+                return info
         return None
 
     def findSymbolByVramOrVrom(self, address: int) -> FoundSymbolInfo|None:
-        for file in self.filesList:
-            pair = file.findSymbolByVramOrVrom(address)
-            if pair is not None:
-                sym, offset = pair
-                return FoundSymbolInfo(file, sym, offset)
+        for segment in self._segmentsList:
+            info = segment.findSymbolByVramOrVrom(address)
+            if info is not None:
+                return info
         return None
 
     def findLowestDifferingSymbol(self, otherMapFile: MapFile) -> tuple[Symbol, File, Symbol|None]|None:
         minVram = None
         found = None
-        for builtFile in self.filesList:
-            for i, builtSym in enumerate(builtFile):
-                expectedSymInfo = otherMapFile.findSymbolByName(builtSym.name)
-                if expectedSymInfo is None:
-                    continue
-
-                expectedSym = expectedSymInfo.symbol
-                if builtSym.vram != expectedSym.vram:
-                    if minVram is None or builtSym.vram < minVram:
-                        minVram = builtSym.vram
-                        prevSym = None
-                        if i > 0:
-                            prevSym = builtFile[i-1]
-                        found = (builtSym, builtFile, prevSym)
+        for builtSegement in self._segmentsList:
+            for builtFile in builtSegement:
+                for i, builtSym in enumerate(builtFile):
+                    expectedSymInfo = otherMapFile.findSymbolByName(builtSym.name)
+                    if expectedSymInfo is None:
+                        continue
+
+                    expectedSym = expectedSymInfo.symbol
+                    if builtSym.vram != expectedSym.vram:
+                        if minVram is None or builtSym.vram < minVram:
+                            minVram = builtSym.vram
+                            prevSym = None
+                            if i > 0:
+                                prevSym = builtFile[i-1]
+                            found = (builtSym, builtFile, prevSym)
         return found
 
 
     def mixFolders(self) -> MapFile:
         newMapFile = MapFile()
 
         newMapFile.debugging = self.debugging
 
-        auxDict: dict[Path, list[File]] = dict()
-
-        # Put files in the same folder together
-        for file in self.filesList:
-            path = Path(*file.getName().parts[:-1])
-            if path not in auxDict:
-                auxDict[path] = list()
-            auxDict[path].append(file)
-
-        # Pretend files in the same folder are one huge file
-        for folderPath, filesInFolder in auxDict.items():
-            firstFile = filesInFolder[0]
-
-            vram = firstFile.vram
-            size = 0
-            segmentType = firstFile.segmentType
-
-            symbols = list()
-            for file in filesInFolder:
-                size += file.size
-                for sym in file.symbols:
-                    symbols.append(sym)
-
-            newMapFile.filesList.append(File(folderPath, vram, size, segmentType, symbols))
+        for segment in self._segmentsList:
+            newMapFile._segmentsList.append(segment.mixFolders())
 
         return newMapFile
 
     def getProgress(self, asmPath: Path, nonmatchings: Path, aliases: dict[str, str]=dict(), pathIndex: int=2) -> tuple[ProgressStats, dict[str, ProgressStats]]:
         totalStats = ProgressStats()
         progressPerFolder: dict[str, ProgressStats] = dict()
 
         if self.debugging:
             utils.eprint(f"getProgress():")
 
-        for file in self.filesList:
-            if len(file.symbols) == 0:
-                continue
-
-            folder = file.filepath.parts[pathIndex]
-            if folder in aliases:
-                folder = aliases[folder]
-
-            if folder not in progressPerFolder:
-                progressPerFolder[folder] = ProgressStats()
+        for segment in self._segmentsList:
+            for file in segment:
+                if len(file) == 0:
+                    continue
 
-            if self.debugging:
-                utils.eprint(f"  folder path: {folder}")
+                folder = file.filepath.parts[pathIndex]
+                if folder in aliases:
+                    folder = aliases[folder]
 
-            originalFilePath = Path(*file.filepath.parts[pathIndex:])
+                if folder not in progressPerFolder:
+                    progressPerFolder[folder] = ProgressStats()
 
-            extensionlessFilePath = originalFilePath
-            while extensionlessFilePath.suffix:
-                extensionlessFilePath = extensionlessFilePath.with_suffix("")
+                if self.debugging:
+                    utils.eprint(f"  folder path: {folder}")
 
-            fullAsmFile = asmPath / extensionlessFilePath.with_suffix(".s")
-            wholeFileIsUndecomped = fullAsmFile.exists()
+                originalFilePath = Path(*file.filepath.parts[pathIndex:])
 
-            if self.debugging:
-                utils.eprint(f"  original file path: {originalFilePath}")
-                utils.eprint(f"  extensionless file path: {extensionlessFilePath}")
-                utils.eprint(f"  full asm file: {fullAsmFile}")
-                utils.eprint(f"  whole file is undecomped: {wholeFileIsUndecomped}")
+                extensionlessFilePath = originalFilePath
+                while extensionlessFilePath.suffix:
+                    extensionlessFilePath = extensionlessFilePath.with_suffix("")
 
-            for func in file.symbols:
-                funcAsmPath = nonmatchings / extensionlessFilePath / f"{func.name}.s"
+                fullAsmFile = asmPath / extensionlessFilePath.with_suffix(".s")
+                wholeFileIsUndecomped = fullAsmFile.exists()
 
                 if self.debugging:
-                    utils.eprint(f"    Checking function '{funcAsmPath}' (size 0x{func.size:X}) ... ", end="")
+                    utils.eprint(f"  original file path: {originalFilePath}")
+                    utils.eprint(f"  extensionless file path: {extensionlessFilePath}")
+                    utils.eprint(f"  full asm file: {fullAsmFile}")
+                    utils.eprint(f"  whole file is undecomped: {wholeFileIsUndecomped}")
+
+                for func in file:
+                    funcAsmPath = nonmatchings / extensionlessFilePath / f"{func.name}.s"
+
+                    symSize = 0
+                    if func.size is not None:
+                        symSize = func.size
 
-                if wholeFileIsUndecomped:
-                    totalStats.undecompedSize += func.size
-                    progressPerFolder[folder].undecompedSize += func.size
-                    if self.debugging:
-                        utils.eprint(f" the whole file is undecomped (no individual function files exist yet)")
-                elif funcAsmPath.exists():
-                    totalStats.undecompedSize += func.size
-                    progressPerFolder[folder].undecompedSize += func.size
                     if self.debugging:
-                        utils.eprint(f" the function hasn't been matched yet (the function file still exists)")
-                else:
-                    totalStats.decompedSize += func.size
-                    progressPerFolder[folder].decompedSize += func.size
-                    if self.debugging:
-                        utils.eprint(f" the function is matched! (the function file was not found)")
+                        utils.eprint(f"    Checking function '{funcAsmPath}' (size 0x{symSize:X}) ... ", end="")
+
+                    if wholeFileIsUndecomped:
+                        totalStats.undecompedSize += symSize
+                        progressPerFolder[folder].undecompedSize += symSize
+                        if self.debugging:
+                            utils.eprint(f" the whole file is undecomped (no individual function files exist yet)")
+                    elif funcAsmPath.exists():
+                        totalStats.undecompedSize += symSize
+                        progressPerFolder[folder].undecompedSize += symSize
+                        if self.debugging:
+                            utils.eprint(f" the function hasn't been matched yet (the function file still exists)")
+                    else:
+                        totalStats.decompedSize += symSize
+                        progressPerFolder[folder].decompedSize += symSize
+                        if self.debugging:
+                            utils.eprint(f" the function is matched! (the function file was not found)")
 
         return totalStats, progressPerFolder
 
     def printAsCsv(self, printVram: bool=True, skipWithoutSymbols: bool=True):
         File.printCsvHeader(printVram)
-        for file in self.filesList:
-            if skipWithoutSymbols and len(file.symbols) == 0:
-                continue
-
-            file.printAsCsv(printVram)
+        for segment in self._segmentsList:
+            segment.printAsCsv(printVram=printVram, skipWithoutSymbols=skipWithoutSymbols)
         return
 
     def printSymbolsCsv(self):
         print(f"File,", end="")
         Symbol.printCsvHeader()
 
-        for file in self.filesList:
-            if len(file.symbols) == 0:
-                continue
-
-            for sym in file.symbols:
-                print(f"{file.filepath},", end="")
-                sym.printAsCsv()
+        for segment in self._segmentsList:
+            segment.printSymbolsCsv()
         return
 
 
-    def toJson(self) -> dict[str, Any]:
-        filesList = []
+    def toJson(self) -> dict:
+        segmentsList = []
+        for segment in self._segmentsList:
+            segmentsList.append(segment.toJson())
 
-        for file in self.filesList:
-            filesList.append(file.toJson())
-
-        result: dict[str, Any] = {
-            "files": filesList
+        result = {
+            "segments": segmentsList
         }
         return result
 
 
-    def __iter__(self) -> Generator[File, None, None]:
-        for file in self.filesList:
+    def __iter__(self) -> Generator[Segment, None, None]:
+        for file in self._segmentsList:
             yield file
 
-    def __getitem__(self, index) -> File:
-        return self.filesList[index]
+    def __getitem__(self, index) -> Segment:
+        return self._segmentsList[index]
+
+    def __len__(self) -> int:
+        return len(self._segmentsList)
```

### Comparing `mapfile_parser-1.3.1/src/mapfile_parser/progress_stats.py` & `mapfile_parser-2.0.0/src/mapfile_parser/progress_stats.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.3.1/src/mapfile_parser/utils.py` & `mapfile_parser-2.0.0/src/mapfile_parser/utils.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.3.1/src/mapfile_parser/frontends/first_diff.py` & `mapfile_parser-2.0.0/src/mapfile_parser/frontends/first_diff.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.3.1/src/mapfile_parser/frontends/jsonify.py` & `mapfile_parser-2.0.0/src/mapfile_parser/frontends/jsonify.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.3.1/src/mapfile_parser/frontends/pj64_syms.py` & `mapfile_parser-2.0.0/src/mapfile_parser/frontends/pj64_syms.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 from typing import TextIO
 import sys
 
 from .. import mapfile
 
 
 def writePj64SymsToFile(mapFile: mapfile.MapFile, outFile: TextIO):
-    for file in mapFile:
-        for sym in file:
-            symType = "code" if file.segmentType == ".text" else "data"
-            outFile.write(f"{sym.vram:08X},{symType},{sym.name}\n")
+    for segment in mapFile:
+        for file in segment:
+            for sym in file:
+                symType = "code" if file.sectionType == ".text" else "data"
+                outFile.write(f"{sym.vram:08X},{symType},{sym.name}\n")
 
 def doPj64Syms(mapPath: Path, outputPath: Path|None) -> int:
     mapFile = mapfile.MapFile()
     mapFile.readMapFile(mapPath)
 
     if outputPath is None:
         writePj64SymsToFile(mapFile, sys.stdout)
```

### Comparing `mapfile_parser-1.3.1/src/mapfile_parser/frontends/progress.py` & `mapfile_parser-2.0.0/src/mapfile_parser/frontends/progress.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 def getProgress(mapPath: Path, asmPath: Path, nonmatchingsPath: Path, pathIndex: int=2, debugging: bool=False) -> tuple[progress_stats.ProgressStats, dict[str, progress_stats.ProgressStats]]:
     mapFile = mapfile.MapFile()
 
     mapFile.debugging = debugging
     mapFile.readMapFile(mapPath)
 
-    return mapFile.filterBySegmentType(".text").getProgress(asmPath, nonmatchingsPath, pathIndex=pathIndex)
+    return mapFile.filterBySectionType(".text").getProgress(asmPath, nonmatchingsPath, pathIndex=pathIndex)
 
 def doProgress(mapPath: Path, asmPath: Path, nonmatchingsPath: Path, pathIndex: int=2, debugging: bool=False) -> int:
     totalStats, progressPerFolder = getProgress(mapPath, asmPath, nonmatchingsPath, pathIndex=pathIndex, debugging=debugging)
 
     progress_stats.printStats(totalStats, progressPerFolder)
     return 0
```

### Comparing `mapfile_parser-1.3.1/src/mapfile_parser/frontends/sym_info.py` & `mapfile_parser-2.0.0/src/mapfile_parser/frontends/sym_info.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.3.1/src/mapfile_parser/frontends/symbol_sizes_csv.py` & `mapfile_parser-2.0.0/src/mapfile_parser/frontends/symbol_sizes_csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .. import mapfile
 
 
 def processArguments(args: argparse.Namespace):
     mapFile = mapfile.MapFile()
     mapFile.readMapFile(args.mapfile)
     if args.filter_section is not None:
-        mapFile = mapFile.filterBySegmentType(args.filter_section)
+        mapFile = mapFile.filterBySectionType(args.filter_section)
 
     if args.same_folder:
         mapFile = mapFile.mixFolders()
 
     if args.symbols:
         mapFile.printSymbolsCsv()
     else:
```

### Comparing `mapfile_parser-1.3.1/src/mapfile_parser/frontends/upload_frogress.py` & `mapfile_parser-2.0.0/src/mapfile_parser/frontends/upload_frogress.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.3.1/.gitignore` & `mapfile_parser-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.3.1/LICENSE` & `mapfile_parser-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.3.1/README.md` & `mapfile_parser-2.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 pip install mapfile-parser
 ```
 
 In case you want to mess with the latest development version without wanting to clone the repository, then you could use the following command:
 
 ```bash
 pip uninstall mapfile-parser
-pip install git+https://github.com/Decompollaborate/mapfile_parser.git@1.x
+pip install git+https://github.com/Decompollaborate/mapfile_parser.git@develop
 ```
 
 NOTE: Installing the development version is not recommended. Proceed at your own risk.
 
 ## Examples
 
 Various cli examples are provided in the [frontends folder](src/mapfile_parser/frontends). Most of them are re-implementations of already existing tools using this library to show how to use this library and inspire new ideas.
```

### Comparing `mapfile_parser-1.3.1/pyproject.toml` & `mapfile_parser-2.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 [project]
 name = "mapfile_parser"
-version = "1.3.1"
+version = "2.0.0"
 description = "Map file parser library focusing decompilation projects"
 readme = "README.md"
 requires-python = ">=3.7"
 dynamic = ["dependencies"]
 
 [project.urls]
 "Homepage" = "https://github.com/Decompollaborate/mapfile_parser"
```

### Comparing `mapfile_parser-1.3.1/PKG-INFO` & `mapfile_parser-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapfile_parser
-Version: 1.3.1
+Version: 2.0.0
 Summary: Map file parser library focusing decompilation projects
 Project-URL: Homepage, https://github.com/Decompollaborate/mapfile_parser
 Project-URL: Bug Tracker, https://github.com/Decompollaborate/mapfile_parser/issues
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: requests
 Description-Content-Type: text/markdown
@@ -27,15 +27,15 @@
 pip install mapfile-parser
 ```
 
 In case you want to mess with the latest development version without wanting to clone the repository, then you could use the following command:
 
 ```bash
 pip uninstall mapfile-parser
-pip install git+https://github.com/Decompollaborate/mapfile_parser.git@1.x
+pip install git+https://github.com/Decompollaborate/mapfile_parser.git@develop
 ```
 
 NOTE: Installing the development version is not recommended. Proceed at your own risk.
 
 ## Examples
 
 Various cli examples are provided in the [frontends folder](src/mapfile_parser/frontends). Most of them are re-implementations of already existing tools using this library to show how to use this library and inspire new ideas.
```

