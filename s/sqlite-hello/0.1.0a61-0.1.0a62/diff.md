# Comparing `tmp/sqlite_hello-0.1.0a61-py3-none-win_amd64.whl.zip` & `tmp/sqlite_hello-0.1.0a62-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 33707 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-24 01:16 noop.cp311-win_amd64.pyd
--rw-rw-rw-  2.0 fat      316 b- defN 23-Jul-24 01:15 sqlite_hello/__init__.py
--rw-rw-rw-  2.0 fat    47925 b- defN 23-Jul-24 01:15 sqlite_hello/hello0.dll
--rw-rw-rw-  2.0 fat    47923 b- defN 23-Jul-24 01:15 sqlite_hello/hola0.dll
--rw-rw-rw-  2.0 fat       82 b- defN 23-Jul-24 01:15 sqlite_hello/version.py
--rw-rw-rw-  2.0 fat      521 b- defN 23-Jul-24 01:16 sqlite_hello-0.1.0a61.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-Jul-24 01:16 sqlite_hello-0.1.0a61.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Jul-24 01:16 sqlite_hello-0.1.0a61.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      727 b- defN 23-Jul-24 01:16 sqlite_hello-0.1.0a61.dist-info/RECORD
-9 files, 97614 bytes uncompressed, 32449 bytes compressed:  66.8%
+Zip file size: 33704 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Aug-06 08:49 noop.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      316 b- defN 23-Aug-06 08:49 sqlite_hello/__init__.py
+-rw-rw-rw-  2.0 fat    47925 b- defN 23-Aug-06 08:49 sqlite_hello/hello0.dll
+-rw-rw-rw-  2.0 fat    47923 b- defN 23-Aug-06 08:49 sqlite_hello/hola0.dll
+-rw-rw-rw-  2.0 fat       82 b- defN 23-Aug-06 08:49 sqlite_hello/version.py
+-rw-rw-rw-  2.0 fat      521 b- defN 23-Aug-06 08:49 sqlite_hello-0.1.0a62.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-Aug-06 08:49 sqlite_hello-0.1.0a62.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Aug-06 08:49 sqlite_hello-0.1.0a62.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      727 b- defN 23-Aug-06 08:49 sqlite_hello-0.1.0a62.dist-info/RECORD
+9 files, 97614 bytes uncompressed, 32446 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: sqlite_hello/hola0.dll
 Comment: 
 
 Filename: sqlite_hello/version.py
 Comment: 
 
-Filename: sqlite_hello-0.1.0a61.dist-info/METADATA
+Filename: sqlite_hello-0.1.0a62.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_hello-0.1.0a61.dist-info/WHEEL
+Filename: sqlite_hello-0.1.0a62.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_hello-0.1.0a61.dist-info/top_level.txt
+Filename: sqlite_hello-0.1.0a62.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_hello-0.1.0a61.dist-info/RECORD
+Filename: sqlite_hello-0.1.0a62.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_hello/hello0.dll

### objdump

```diff
@@ -5,15 +5,15 @@
 
 Characteristics 0x2026
 	executable
 	line numbers stripped
 	large address aware
 	DLL
 
-Time/Date		Mon Jul 24 01:15:00 2023
+Time/Date		Sun Aug  6 08:48:22 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	2
 MinorLinkerVersion	30
 SizeOfCode		0000000000001c00
 SizeOfInitializedData	0000000000003600
 SizeOfUninitializedData	0000000000000a00
 AddressOfEntryPoint	0000000000001330
@@ -26,15 +26,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	5
 MinorSubsystemVersion	2
 Win32Version		00000000
 SizeOfImage		00014000
 SizeOfHeaders		00000600
-CheckSum		000144ae
+CheckSum		00016155
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00000000
 SizeOfStackReserve	0000000000200000
 SizeOfStackCommit	0000000000001000
 SizeOfHeapReserve	0000000000100000
 SizeOfHeapCommit	0000000000001000
 LoaderFlags		00000000
@@ -112,15 +112,15 @@
  00009028	00000000 00000000 00000000 00000000 00000000
 
 There is an export table in .edata at 0x6e408000
 
 The Export Tables (interpreted .edata section contents)
 
 Export Flags 			0
-Time/Date stamp 		64bdd094
+Time/Date stamp 		64cf5e56
 Major/Minor 			0/0
 Name 				0000000000008032 hello0.dll
 Ordinal Base 			1
 Number in:
 	Export Address Table 		00000001
 	[Name Pointer/Ordinal] Table	00000001
 Table Addresses
@@ -3785,15 +3785,15 @@
     6e404004:	outsl  %ds:(%rsi),(%dx)
     6e404005:	sub    $0x20,%al
     6e404007:	and    $0x76002173,%eax
     6e40400c:	xor    %ch,(%rsi)
     6e40400e:	xor    %ebp,(%rsi)
     6e404010:	xor    %ch,0x68706c61(%rip)        # d6b0ac77 <.debug_str+0x686f7c77>
     6e404016:	(bad)
-    6e404017:	cs ss xor %eax,(%rax)
+    6e404017:	cs ss xor (%rax),%al
     6e40401b:	push   $0x6f6c6c65
     6e404020:	add    %ch,0x65(%rax)
     6e404023:	insb   (%dx),%es:(%rdi)
     6e404024:	insb   (%dx),%es:(%rdi)
     6e404025:	outsl  %ds:(%rsi),(%dx)
     6e404026:	pop    %rdi
     6e404027:	jbe    6e40408e <_tls_used+0x2e>
@@ -4603,19 +4603,20 @@
 	...
 
 Disassembly of section .edata:
 
 000000006e408000 <.edata>:
     6e408000:	add    %al,(%rax)
     6e408002:	add    %al,(%rax)
-    6e408004:	xchg   %eax,%esp
-    6e408005:	sarb   0x64(%rbp)
-    6e40800b:	add    %dh,(%rdx)
-    6e40800d:	addb   $0x0,(%rax)
-    6e408010:	add    %eax,(%rax)
+    6e408004:	push   %rsi
+    6e408005:	pop    %rsi
+    6e408006:	iret
+    6e408007:	add    %al,%fs:(%rax)
+    6e40800a:	add    %al,(%rax)
+    6e40800c:	xor    0x10000(%rax),%al
     6e408012:	add    %al,(%rax)
     6e408014:	add    %eax,(%rax)
     6e408016:	add    %al,(%rax)
     6e408018:	add    %eax,(%rax)
     6e40801a:	add    %al,(%rax)
     6e40801c:	sub    %al,-0x7fd40000(%rax)
     6e408022:	add    %al,(%rax)
```

## sqlite_hello/hola0.dll

### objdump

```diff
@@ -5,15 +5,15 @@
 
 Characteristics 0x2026
 	executable
 	line numbers stripped
 	large address aware
 	DLL
 
-Time/Date		Mon Jul 24 01:15:00 2023
+Time/Date		Sun Aug  6 08:48:22 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	2
 MinorLinkerVersion	30
 SizeOfCode		0000000000001c00
 SizeOfInitializedData	0000000000003600
 SizeOfUninitializedData	0000000000000a00
 AddressOfEntryPoint	0000000000001330
@@ -26,15 +26,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	5
 MinorSubsystemVersion	2
 Win32Version		00000000
 SizeOfImage		00014000
 SizeOfHeaders		00000600
-CheckSum		0000bf1f
+CheckSum		0000dac7
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00000000
 SizeOfStackReserve	0000000000200000
 SizeOfStackCommit	0000000000001000
 SizeOfHeapReserve	0000000000100000
 SizeOfHeapCommit	0000000000001000
 LoaderFlags		00000000
@@ -112,15 +112,15 @@
  00009028	00000000 00000000 00000000 00000000 00000000
 
 There is an export table in .edata at 0x68748000
 
 The Export Tables (interpreted .edata section contents)
 
 Export Flags 			0
-Time/Date stamp 		64bdd094
+Time/Date stamp 		64cf5e56
 Major/Minor 			0/0
 Name 				0000000000008032 hola0.dll
 Ordinal Base 			1
 Number in:
 	Export Address Table 		00000001
 	[Name Pointer/Ordinal] Table	00000001
 Table Addresses
@@ -3785,15 +3785,15 @@
     68744005:	(bad)
     68744006:	sub    $0x20,%al
     68744008:	and    $0x76002173,%eax
     6874400d:	xor    %ch,(%rsi)
     6874400f:	xor    %ebp,(%rsi)
     68744011:	xor    %ch,0x68706c61(%rip)        # d0e4ac78 <.debug_str+0x686f7c78>
     68744017:	(bad)
-    68744018:	cs ss xor %eax,(%rax)
+    68744018:	cs ss xor (%rax),%al
     6874401c:	push   $0x616c6f
     68744021:	push   $0x5f616c6f
     68744026:	jbe    6874408d <_tls_used+0x2d>
     68744028:	jb     6874409d <_tls_used+0x3d>
     6874402a:	imul   $0x20000000,0x6e(%rdi),%ebp
 
 0000000068744030 <GS_ExceptionPointers>:
@@ -4592,19 +4592,20 @@
 	...
 
 Disassembly of section .edata:
 
 0000000068748000 <.edata>:
     68748000:	add    %al,(%rax)
     68748002:	add    %al,(%rax)
-    68748004:	xchg   %eax,%esp
-    68748005:	sarb   0x64(%rbp)
-    6874800b:	add    %dh,(%rdx)
-    6874800d:	addb   $0x0,(%rax)
-    68748010:	add    %eax,(%rax)
+    68748004:	push   %rsi
+    68748005:	pop    %rsi
+    68748006:	iret
+    68748007:	add    %al,%fs:(%rax)
+    6874800a:	add    %al,(%rax)
+    6874800c:	xor    0x10000(%rax),%al
     68748012:	add    %al,(%rax)
     68748014:	add    %eax,(%rax)
     68748016:	add    %al,(%rax)
     68748018:	add    %eax,(%rax)
     6874801a:	add    %al,(%rax)
     6874801c:	sub    %al,-0x7fd40000(%rax)
     68748022:	add    %al,(%rax)
```

## sqlite_hello/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.61"
+__version__ = "0.1.0-alpha.62"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_hello-0.1.0a61.dist-info/METADATA` & `sqlite_hello-0.1.0a62.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-hello
-Version: 0.1.0a61
+Version: 0.1.0a62
 Home-page: https://github.com/asg017/sqlite-hello
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-hello/issues
 Project-URL: CI, https://github.com/asg017/sqlite-hello/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-hello/releases
 Requires-Python: >=3.6
```

## Comparing `sqlite_hello-0.1.0a61.dist-info/RECORD` & `sqlite_hello-0.1.0a62.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 noop.cp311-win_amd64.pyd,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sqlite_hello/__init__.py,sha256=_SH5dbQOWvHZs14Mu6FCjaNhOleuM2Z9mTPoPkZaopE,316
-sqlite_hello/hello0.dll,sha256=ReNVIP-8W90KWLTSu0hKHmoX4wwP2Y-5SDiUR-FT-uo,47925
-sqlite_hello/hola0.dll,sha256=SBA8a0nElQEsbTdLWyIQAuD0zhyKufgGQrtoQpVeStI,47923
-sqlite_hello/version.py,sha256=MW2ry8IcjY4xwb0nJW-iXqiJhZ9WgpZAPXvGROQ5XKA,82
-sqlite_hello-0.1.0a61.dist-info/METADATA,sha256=v8j8VYKQqneP3jO7xdA3rzeJitAnaK9wTTqzbGAwW-4,521
-sqlite_hello-0.1.0a61.dist-info/WHEEL,sha256=_7p9Q7gln4IKfQKAaNeimlWk5nRt3CeHwqN-V03Bs0E,102
-sqlite_hello-0.1.0a61.dist-info/top_level.txt,sha256=KjVnaNCiS11UOKhSHnqZUwUFlrCeCQv89AtVw-JnynI,18
-sqlite_hello-0.1.0a61.dist-info/RECORD,,
+sqlite_hello/hello0.dll,sha256=UoULRlQzRk6zMkk0IBrc0F-vN7IQ_jpBFeR-RfsjgLM,47925
+sqlite_hello/hola0.dll,sha256=yq3L8vo2u4DaZmQ78lUj2UJUudhjGBNC-peKLBmg7F4,47923
+sqlite_hello/version.py,sha256=WnZph3UNvevJelH_NR5tEN_D1NyQiswAjdmtB88lBdE,82
+sqlite_hello-0.1.0a62.dist-info/METADATA,sha256=HGTyI4pnyGnMAWPc2BRdl_eEZ5vFH61pvqJZEMuScq0,521
+sqlite_hello-0.1.0a62.dist-info/WHEEL,sha256=viuncpH_EfvQZWqmP28y3RsBnRoE49Wb1vcMVyR8XUI,102
+sqlite_hello-0.1.0a62.dist-info/top_level.txt,sha256=KjVnaNCiS11UOKhSHnqZUwUFlrCeCQv89AtVw-JnynI,18
+sqlite_hello-0.1.0a62.dist-info/RECORD,,
```

