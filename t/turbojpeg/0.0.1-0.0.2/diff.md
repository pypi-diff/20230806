# Comparing `tmp/turbojpeg-0.0.1-cp39-cp39-win_amd64.whl.zip` & `tmp/turbojpeg-0.0.2-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 434209 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat   197632 b- defN 23-Jun-06 07:45 turbojpeg.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat       47 b- defN 23-Jun-06 07:45 turbojpeg-0.0.1.data/platlib/.load-order-turbojpeg-0.0.1
--rw-rw-rw-  2.0 fat   937472 b- defN 23-Jun-06 07:40 turbojpeg-0.0.1.data/platlib/turbojpeg-9a943270a39656f30bb8d082cd5a8367.dll
--rw-rw-rw-  2.0 fat      504 b- defN 23-Jun-06 07:45 turbojpeg-0.0.1.dist-info/DELVEWHEEL
--rw-rw-rw-  2.0 fat     2185 b- defN 23-Jun-06 07:45 turbojpeg-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      731 b- defN 23-Jun-06 07:45 turbojpeg-0.0.1.dist-info/RECORD
--rw-rw-rw-  2.0 fat       10 b- defN 23-Jun-06 07:45 turbojpeg-0.0.1.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-06 07:45 turbojpeg-0.0.1.dist-info/WHEEL
-8 files, 1138681 bytes uncompressed, 432917 bytes compressed:  62.0%
+Zip file size: 439757 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat   209408 b- defN 23-Aug-06 15:21 turbojpeg.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat       47 b- defN 23-Aug-06 15:21 turbojpeg-0.0.2.data/platlib/.load-order-turbojpeg-0.0.2
+-rw-rw-rw-  2.0 fat   937472 b- defN 23-Aug-06 15:12 turbojpeg-0.0.2.data/platlib/turbojpeg-c526d70e86230491ec9849d550e5d1db.dll
+-rw-rw-rw-  2.0 fat      504 b- defN 23-Aug-06 15:21 turbojpeg-0.0.2.dist-info/DELVEWHEEL
+-rw-rw-rw-  2.0 fat     2243 b- defN 23-Aug-06 15:21 turbojpeg-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      731 b- defN 23-Aug-06 15:21 turbojpeg-0.0.2.dist-info/RECORD
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Aug-06 15:21 turbojpeg-0.0.2.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Aug-06 15:21 turbojpeg-0.0.2.dist-info/WHEEL
+8 files, 1150515 bytes uncompressed, 438465 bytes compressed:  61.9%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: turbojpeg.cp39-win_amd64.pyd
 Comment: 
 
-Filename: turbojpeg-0.0.1.data/platlib/.load-order-turbojpeg-0.0.1
+Filename: turbojpeg-0.0.2.data/platlib/.load-order-turbojpeg-0.0.2
 Comment: 
 
-Filename: turbojpeg-0.0.1.data/platlib/turbojpeg-9a943270a39656f30bb8d082cd5a8367.dll
+Filename: turbojpeg-0.0.2.data/platlib/turbojpeg-c526d70e86230491ec9849d550e5d1db.dll
 Comment: 
 
-Filename: turbojpeg-0.0.1.dist-info/DELVEWHEEL
+Filename: turbojpeg-0.0.2.dist-info/DELVEWHEEL
 Comment: 
 
-Filename: turbojpeg-0.0.1.dist-info/METADATA
+Filename: turbojpeg-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: turbojpeg-0.0.1.dist-info/RECORD
+Filename: turbojpeg-0.0.2.dist-info/RECORD
 Comment: 
 
-Filename: turbojpeg-0.0.1.dist-info/top_level.txt
+Filename: turbojpeg-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: turbojpeg-0.0.1.dist-info/WHEEL
+Filename: turbojpeg-0.0.2.dist-info/WHEEL
 Comment: 
 
 Zip file comment:
```

## Comparing `turbojpeg-0.0.1.data/platlib/turbojpeg-9a943270a39656f30bb8d082cd5a8367.dll` & `turbojpeg-0.0.2.data/platlib/turbojpeg-c526d70e86230491ec9849d550e5d1db.dll`

 * *Files 0% similar despite different names*

### objdump

```diff
@@ -4,20 +4,20 @@
 start address 0x0000000180081460
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Jun  6 07:40:45 2023
+Time/Date		Sun Aug  6 15:12:25 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	35
 SizeOfCode		000000000009ec00
-SizeOfInitializedData	0000000000045e00
+SizeOfInitializedData	0000000000047000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000081460
 BaseOfCode		0000000000001000
 ImageBase		0000000180000000
 SectionAlignment	00001000
 FileAlignment		00000200
 MajorOSystemVersion	6
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	3
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		000e9000
 SizeOfHeaders		00000400
-CheckSum		000f3339
+CheckSum		00000000
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -41,15 +41,15 @@
 SizeOfHeapCommit	0000000000001000
 LoaderFlags		00000000
 NumberOfRvaAndSizes	00000010
 
 The Data Directory
 Entry 0 00000000000dcf40 000007c8 Export Directory [.edata (or where ever we found it)]
 Entry 1 00000000000dd708 00000028 Import Directory [parts of .idata]
-Entry 2 00000000000e7000 00000534 Resource Directory [.rsrc]
+Entry 2 00000000000e7000 00000558 Resource Directory [.rsrc]
 Entry 3 00000000000e0000 00005c40 Exception Directory [.pdata]
 Entry 4 0000000000000000 00000000 Security Directory
 Entry 5 00000000000e8000 0000088c Base Relocation Directory [.reloc]
 Entry 6 00000000000d5cd0 0000001c Debug Directory
 Entry 7 0000000000000000 00000000 Description Directory
 Entry 8 0000000000000000 00000000 Special Directory
 Entry 9 00000000000d5d00 00000028 Thread Storage Directory [.tls]
@@ -17650,42 +17650,42 @@
 
 There is a debug directory in .rdata at 0x1800d5cd0
 
 Type                Size     Rva      Offset
  13         CoffGrp 00000360 000d61e0 000d51e0
 
 The .rsrc Resource Directory section:
-000  Type Table: Char: 0, Time: 00000000, Ver: 4/0, Num Names: 0, IDs: 2
+000  Type Table: Char: 0, Time: 00000000, Ver: 0/0, Num Names: 0, IDs: 2
 010   Entry: ID: 0x000010, Value: 0x80000020
-020    Name Table: Char: 0, Time: 00000000, Ver: 4/0, Num Names: 0, IDs: 1
+020    Name Table: Char: 0, Time: 00000000, Ver: 0/0, Num Names: 0, IDs: 1
 030     Entry: ID: 0x000001, Value: 0x80000050
-050      Language Table: Char: 0, Time: 00000000, Ver: 4/0, Num Names: 0, IDs: 1
+050      Language Table: Char: 0, Time: 00000000, Ver: 0/0, Num Names: 0, IDs: 1
 060       Entry: ID: 0x000409, Value: 0x000080
-080        Leaf: Addr: 0x0e70a0, Size: 0x000338, Codepage: 1252
+080        Leaf: Addr: 0x0e70a0, Size: 0x000338, Codepage: 0
 018   Entry: ID: 0x000018, Value: 0x80000038
-038    Name Table: Char: 0, Time: 00000000, Ver: 4/0, Num Names: 0, IDs: 1
+038    Name Table: Char: 0, Time: 00000000, Ver: 0/0, Num Names: 0, IDs: 1
 048     Entry: ID: 0x000002, Value: 0x80000068
-068      Language Table: Char: 0, Time: 00000000, Ver: 4/0, Num Names: 0, IDs: 1
+068      Language Table: Char: 0, Time: 00000000, Ver: 0/0, Num Names: 0, IDs: 1
 078       Entry: ID: 0x000409, Value: 0x000090
-090        Leaf: Addr: 0x0e73d8, Size: 0x00015a, Codepage: 1252
+090        Leaf: Addr: 0x0e73d8, Size: 0x00017d, Codepage: 0
  Resources start at offset: 0xa0
 
 Sections:
 Idx Name          Size      VMA               LMA               File off  Algn
   0 .text         0009eac0  0000000180001000  0000000180001000  00000400  2**4
                   CONTENTS, ALLOC, LOAD, READONLY, CODE
   1 .rdata        0003df62  00000001800a0000  00000001800a0000  0009f000  2**4
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
   2 .data         00000e00  00000001800de000  00000001800de000  000dd000  2**4
                   CONTENTS, ALLOC, LOAD, DATA
   3 .pdata        00005c40  00000001800e0000  00000001800e0000  000dde00  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
   4 _RDATA        0000015c  00000001800e6000  00000001800e6000  000e3c00  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  5 .rsrc         00000534  00000001800e7000  00000001800e7000  000e3e00  2**2
+  5 .rsrc         00000558  00000001800e7000  00000001800e7000  000e3e00  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
   6 .reloc        0000088c  00000001800e8000  00000001800e8000  000e4400  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
 SYMBOL TABLE:
 no symbols
 
 
@@ -244387,15 +244387,15 @@
    1800b3445:	and    %dh,0x65(%rsi)
    1800b3448:	jb     0x1800b34bd
    1800b344a:	imul   $0x312e3220,0x6e(%rdi),%ebp
    1800b3451:	cs cmp %esi,(%rdx)
    1800b3454:	and    %ch,(%rax)
    1800b3456:	(bad)
    1800b3458:	imul   $0x33323032,0x20(%rsp,%riz,2),%ebp
-   1800b3460:	xor    %dh,(%rsi)
+   1800b3460:	xor    %bh,(%rax)
    1800b3462:	xor    %dh,(%rsi)
    1800b3464:	sub    %eax,(%rax)
 	...
    1800b346e:	add    %al,(%rax)
    1800b3470:	(bad)
    1800b3471:	(bad)
    1800b3472:	(bad)
@@ -321831,16 +321831,16 @@
    1800d5cbd:	add    %al,(%rax)
    1800d5cbf:	add    %ch,0x1800a02(%rax)
    1800d5cc5:	add    %al,(%rax)
    1800d5cc7:	add    %dh,0x1800a02(%rax)
    1800d5ccd:	add    %al,(%rax)
    1800d5ccf:	add    %al,(%rax)
    1800d5cd1:	add    %al,(%rax)
-   1800d5cd3:	add    %bh,%ch
-   1800d5cd5:	loop   0x1800d5d55
+   1800d5cd3:	add    %bl,-0x48(%rcx)
+   1800d5cd6:	iret
    1800d5cd7:	add    %al,%fs:(%rax)
    1800d5cda:	add    %al,(%rax)
    1800d5cdc:	or     $0x60000000,%eax
    1800d5ce1:	add    (%rax),%eax
    1800d5ce3:	add    %ah,%al
    1800d5ce5:	(bad)
    1800d5ce6:	or     $0xd51e000,%eax
@@ -322666,25 +322666,22 @@
    1800d6508:	add    %ah,0xe(%rax)
    1800d650b:	add    %bl,0x0(%rcx,%rax,1)
    1800d650f:	add    %bl,0x52(%rdi)
    1800d6512:	rex.R
    1800d6513:	push   %r12
    1800d6515:	add    %al,(%r8)
    1800d6518:	add    %dh,0xe(%rax)
-   1800d651b:	add    %ah,0x0(%rax)
-   1800d651e:	add    %al,(%rax)
-   1800d6520:	jb,pn  0x1800d6596
+   1800d651b:	add    %ah,0x2e000000(%rax)
+   1800d6521:	jb     0x1800d6596
    1800d6523:	jb     0x1800d6588
    1800d6525:	and    $0x30,%al
    1800d6527:	xor    %eax,(%rax)
    1800d6529:	add    %al,(%rax)
-   1800d652b:	add    %ah,0x70(%rax)
-   1800d652e:	(bad)
-   1800d652f:	add    %bh,(%rax)
-   1800d6531:	add    (%rax),%eax
+   1800d652b:	add    %ah,-0x47fff190(%rax)
+   1800d6531:	add    $0x0,%al
    1800d6533:	add    %ch,(%rsi)
    1800d6535:	jb     0x1800d65aa
    1800d6537:	jb     0x1800d659c
    1800d6539:	and    $0x30,%al
    1800d653b:	xor    (%rax),%al
 	...
    1800d656d:	add    %al,(%rax)
@@ -343372,77 +343369,53 @@
    1800e6159:	and    $0x8,%al
 	...
 
 Disassembly of section .rsrc:
 
 00000001800e7000 <.rsrc>:
 	...
-   1800e7008:	add    $0x0,%al
-   1800e700a:	add    %al,(%rax)
    1800e700c:	add    %al,(%rax)
    1800e700e:	add    (%rax),%al
    1800e7010:	adc    %al,(%rax)
    1800e7012:	add    %al,(%rax)
    1800e7014:	and    %al,(%rax)
    1800e7016:	add    %al,0x18(%rax)
    1800e701c:	cmp    %al,(%rax)
    1800e701e:	add    %al,0x0(%rax)
-   1800e7024:	add    %al,(%rax)
-   1800e7026:	add    %al,(%rax)
-   1800e7028:	add    $0x0,%al
-   1800e702a:	add    %al,(%rax)
+	...
    1800e702c:	add    %al,(%rax)
    1800e702e:	add    %eax,(%rax)
    1800e7030:	add    %eax,(%rax)
    1800e7032:	add    %al,(%rax)
    1800e7034:	push   %rax
    1800e7035:	add    %al,(%rax)
    1800e7037:	addb   $0x0,(%rax)
-   1800e703a:	add    %al,(%rax)
-   1800e703c:	add    %al,(%rax)
-   1800e703e:	add    %al,(%rax)
-   1800e7040:	add    $0x0,%al
-   1800e7042:	add    %al,(%rax)
-   1800e7044:	add    %al,(%rax)
+	...
    1800e7046:	add    %eax,(%rax)
    1800e7048:	add    (%rax),%al
    1800e704a:	add    %al,(%rax)
    1800e704c:	push   $0x800000
-   1800e7051:	add    %al,(%rax)
-   1800e7053:	add    %al,(%rax)
-   1800e7055:	add    %al,(%rax)
-   1800e7057:	add    %al,(%rax,%rax,1)
-   1800e705a:	add    %al,(%rax)
-   1800e705c:	add    %al,(%rax)
-   1800e705e:	add    %eax,(%rax)
-   1800e7060:	or     %eax,(%rax,%rax,1)
+	...
+   1800e705d:	add    %al,(%rcx)
+   1800e705f:	add    %cl,(%rcx)
+   1800e7061:	add    $0x0,%al
    1800e7063:	add    %al,0x0(%rax)
-   1800e7069:	add    %al,(%rax)
-   1800e706b:	add    %al,(%rax)
-   1800e706d:	add    %al,(%rax)
-   1800e706f:	add    %al,(%rax,%rax,1)
-   1800e7072:	add    %al,(%rax)
-   1800e7074:	add    %al,(%rax)
-   1800e7076:	add    %eax,(%rax)
-   1800e7078:	or     %eax,(%rax,%rax,1)
+	...
+   1800e7075:	add    %al,(%rcx)
+   1800e7077:	add    %cl,(%rcx)
+   1800e7079:	add    $0x0,%al
    1800e707b:	add    %dl,-0x60000000(%rax)
    1800e7081:	jo     0x1800e7091
    1800e7083:	add    %bh,(%rax)
    1800e7085:	add    (%rax),%eax
-   1800e7087:	add    %ah,%ah
-   1800e7089:	add    $0x0,%al
-   1800e708b:	add    %al,(%rax)
-   1800e708d:	add    %al,(%rax)
+	...
    1800e708f:	add    %bl,%al
    1800e7091:	jae    0x1800e70a1
-   1800e7093:	add    %bl,0x1(%rdx)
-   1800e7096:	add    %al,(%rax)
-   1800e7098:	in     $0x4,%al
-   1800e709a:	add    %al,(%rax)
-   1800e709c:	add    %al,(%rax)
+   1800e7093:	add    %bh,0x1(%rbp)
+	...
    1800e709e:	add    %al,(%rax)
    1800e70a0:	cmp    %al,(%rbx)
    1800e70a2:	xor    $0x0,%al
    1800e70a4:	add    %al,(%rax)
    1800e70a6:	push   %rsi
    1800e70a7:	add    %dl,0x0(%rbx)
    1800e70aa:	pop    %rdi
@@ -343759,140 +343732,152 @@
    1800e73c8:	je     0x1800e73ca
    1800e73ca:	imul   $0x6e006f,(%rax),%eax
    1800e73d0:	add    %al,(%rax)
    1800e73d2:	add    %al,(%rax)
    1800e73d4:	or     %eax,(%rax,%rsi,4)
    1800e73d7:	add    $0x3c,%al
    1800e73d9:	(bad)
-   1800e73da:	jae    0x1800e744f
-   1800e73dc:	gs insl (%dx),%es:(%rdi)
-   1800e73de:	(bad)
-   1800e73df:	insb   (%dx),%es:(%rdi)
-   1800e73e0:	jns    0x1800e7402
-   1800e73e2:	js     0x1800e7451
-   1800e73e4:	insb   (%dx),%es:(%rdi)
-   1800e73e5:	outsb  %ds:(%rsi),(%dx)
-   1800e73e6:	jae    0x1800e7425
-   1800e73e8:	and    0x72(%rbp),%dh
-   1800e73eb:	outsb  %ds:(%rsi),(%dx)
-   1800e73ec:	cmp    0x63(%rbx),%dh
-   1800e73ef:	push   $0x73616d65
-   1800e73f4:	sub    $0x7263696d,%eax
-   1800e73f9:	outsl  %ds:(%rsi),(%dx)
-   1800e73fa:	jae    0x1800e746b
-   1800e73fc:	data16 je 0x1800e742c
-   1800e73ff:	movsxd 0x6d(%rdi),%ebp
-   1800e7402:	cmp    0x73(%rcx),%ah
-   1800e7405:	insl   (%dx),%es:(%rdi)
-   1800e7406:	jbe,pn 0x1800e743a
-   1800e7409:	and    (%rax),%ah
-   1800e740b:	insl   (%dx),%es:(%rdi)
+   1800e73da:	js     0x1800e7449
+   1800e73dc:	insb   (%dx),%es:(%rdi)
+   1800e73dd:	and    %dh,0x65(%rsi)
+   1800e73e0:	jb     0x1800e7455
+   1800e73e2:	imul   $0x2e31273d,0x6e(%rdi),%ebp
+   1800e73e9:	xor    %ah,(%rdi)
+   1800e73eb:	and    %ah,0x6e(%rbp)
+   1800e73ee:	movsxd 0x64(%rdi),%ebp
+   1800e73f1:	imul   $0x5455273d,0x67(%rsi),%ebp
+   1800e73f8:	rex.RX sub $0x73202738,%eax
+   1800e73fe:	je     0x1800e7461
+   1800e7400:	outsb  %ds:(%rsi),(%dx)
+   1800e7401:	fs (bad)
+   1800e7403:	insb   (%dx),%es:(%rdi)
+   1800e7404:	outsl  %ds:(%rsi),(%dx)
+   1800e7405:	outsb  %ds:(%rsi),(%dx)
+   1800e7406:	gs cmp $0x73657927,%eax
    1800e740c:	(bad)
-   1800e740d:	outsb  %ds:(%rsi),(%dx)
-   1800e740e:	imul   $0x65567473,0x65(%rsi),%esp
-   1800e7415:	jb     0x1800e748a
-   1800e7417:	imul   $0x2e31223d,0x6e(%rdi),%ebp
-   1800e741e:	xor    %ah,(%rdx)
-   1800e7420:	ds or  $0x3c20200a,%eax
-   1800e7426:	je     0x1800e749a
-   1800e7428:	jne    0x1800e749d
-   1800e742a:	je     0x1800e7475
-   1800e742c:	outsb  %ds:(%rsi),(%dx)
-   1800e742d:	outsw  %ds:(%rsi),(%dx)
-   1800e742f:	and    %bh,0x6d(%rax)
-   1800e7432:	insb   (%dx),%es:(%rdi)
-   1800e7433:	outsb  %ds:(%rsi),(%dx)
-   1800e7434:	jae    0x1800e7473
-   1800e7436:	and    0x72(%rbp),%dh
-   1800e7439:	outsb  %ds:(%rsi),(%dx)
-   1800e743a:	cmp    0x63(%rbx),%dh
-   1800e743d:	push   $0x73616d65
-   1800e7442:	sub    $0x7263696d,%eax
-   1800e7447:	outsl  %ds:(%rsi),(%dx)
-   1800e7448:	jae    0x1800e74b9
-   1800e744a:	data16 je 0x1800e747a
-   1800e744d:	movsxd 0x6d(%rdi),%ebp
-   1800e7450:	cmp    0x73(%rcx),%ah
-   1800e7453:	insl   (%dx),%es:(%rdi)
-   1800e7454:	jbe,pn 0x1800e748a
-   1800e7457:	and    (%rsi),%bh
-   1800e7459:	or     $0x2020200a,%eax
-   1800e745e:	and    %bh,(%rbx,%rsi,2)
-   1800e7461:	movsxd %gs:0x72(%rbp),%esi
-   1800e7465:	imul   $0x20200a0d,0x3e(%rcx,%rdi,2),%esi
-   1800e746d:	and    %ah,(%rax)
-   1800e746f:	and    %ah,(%rax)
-   1800e7471:	cmp    $0x72,%al
-   1800e7473:	gs jno 0x1800e74eb
-   1800e7476:	gs jae 0x1800e74ed
-   1800e7479:	gs fs push %rax
-   1800e747c:	jb     0x1800e74e7
-   1800e747e:	jbe    0x1800e74e9
-   1800e7480:	insb   (%dx),%es:(%rdi)
-   1800e7481:	gs addr32 gs jae 0x1800e74c4
-   1800e7486:	or     $0x2020200a,%eax
-   1800e748b:	and    %ah,(%rax)
-   1800e748d:	and    %ah,(%rax)
-   1800e748f:	and    %bh,(%rdx,%rsi,2)
-   1800e7492:	gs jno 0x1800e750a
-   1800e7495:	gs jae 0x1800e750c
-   1800e7498:	gs fs rex.RB js 0x1800e7502
-   1800e749d:	movsxd 0x74(%rbp),%esi
-   1800e74a0:	imul   $0x6576654c,0x6e(%rdi),%ebp
-   1800e74a7:	insb   (%dx),%es:(%rdi)
-   1800e74a8:	and    %ch,0x76(%rbp,%riz,2)
-   1800e74ac:	gs insb (%dx),%es:(%rdi)
-   1800e74ae:	cmp    $0x49736122,%eax
-   1800e74b3:	outsb  %ds:(%rsi),(%dx)
-   1800e74b4:	jbe    0x1800e7525
-   1800e74b6:	imul   $0x22,0x72(%rbp),%esp
-   1800e74ba:	and    %dh,0x69(%rbp)
-   1800e74bd:	movsxd 0x65(%r11),%esp
-   1800e74c1:	jae    0x1800e7536
-   1800e74c3:	cmp    $0x6c616622,%eax
-   1800e74c8:	jae    0x1800e752f
-   1800e74ca:	and    (%rsi),%bh
-   1800e74cc:	cmp    $0x2f,%al
-   1800e74ce:	jb     0x1800e7535
-   1800e74d0:	jno    0x1800e7547
-   1800e74d2:	gs jae 0x1800e7549
-   1800e74d5:	gs fs rex.RB js 0x1800e753f
-   1800e74da:	movsxd 0x74(%rbp),%esi
-   1800e74dd:	imul   $0x6576654c,0x6e(%rdi),%ebp
-   1800e74e4:	insb   (%dx),%es:(%rdi)
-   1800e74e5:	ds or  $0x2020200a,%eax
-   1800e74eb:	and    %ah,(%rax)
-   1800e74ed:	and    %bh,(%rdi,%rbp,1)
-   1800e74f0:	jb     0x1800e7557
-   1800e74f2:	jno    0x1800e7569
-   1800e74f4:	gs jae 0x1800e756b
-   1800e74f7:	gs fs push %rax
-   1800e74fa:	jb     0x1800e7565
-   1800e74fc:	jbe    0x1800e7567
-   1800e74fe:	insb   (%dx),%es:(%rdi)
-   1800e74ff:	gs addr32 gs jae 0x1800e7542
-   1800e7504:	or     $0x2020200a,%eax
-   1800e7509:	and    %bh,(%rdi,%rbp,1)
-   1800e750c:	jae    0x1800e7573
-   1800e750e:	movsxd 0x72(%rbp),%esi
-   1800e7511:	imul   $0x20200a0d,0x3e(%rcx,%rdi,2),%esi
-   1800e7519:	cmp    $0x2f,%al
-   1800e751b:	je     0x1800e758f
-   1800e751d:	jne    0x1800e7592
-   1800e751f:	je     0x1800e756a
-   1800e7521:	outsb  %ds:(%rsi),(%dx)
-   1800e7522:	outsw  %ds:(%rsi),(%dx)
-   1800e7524:	ds or  $0x612f3c0a,%eax
-   1800e752a:	jae    0x1800e759f
-   1800e752c:	gs insl (%dx),%es:(%rdi)
-   1800e752e:	(bad)
-   1800e752f:	insb   (%dx),%es:(%rdi)
-   1800e7530:	jns    0x1800e7570
-   1800e7532:	push   %rax
-   1800e7533:	rex.B
+   1800e740d:	(bad)
+   1800e740e:	ds or  $0x73613c0a,%eax
+   1800e7414:	jae    0x1800e747b
+   1800e7416:	insl   (%dx),%es:(%rdi)
+   1800e7417:	(bad)
+   1800e7418:	insb   (%dx),%es:(%rdi)
+   1800e7419:	jns    0x1800e743b
+   1800e741b:	js     0x1800e748a
+   1800e741d:	insb   (%dx),%es:(%rdi)
+   1800e741e:	outsb  %ds:(%rsi),(%dx)
+   1800e741f:	jae    0x1800e745e
+   1800e7421:	(bad)
+   1800e7422:	jne    0x1800e7496
+   1800e7424:	outsb  %ds:(%rsi),(%dx)
+   1800e7425:	cmp    0x63(%rbx),%dh
+   1800e7428:	push   $0x73616d65
+   1800e742d:	sub    $0x7263696d,%eax
+   1800e7432:	outsl  %ds:(%rsi),(%dx)
+   1800e7433:	jae    0x1800e74a4
+   1800e7435:	data16 je 0x1800e7465
+   1800e7438:	movsxd 0x6d(%rdi),%ebp
+   1800e743b:	cmp    0x73(%rcx),%ah
+   1800e743e:	insl   (%dx),%es:(%rdi)
+   1800e743f:	jbe,pn 0x1800e7473
+   1800e7442:	(bad)
+   1800e7443:	and    %ch,0x61(%rbp)
+   1800e7446:	outsb  %ds:(%rsi),(%dx)
+   1800e7447:	imul   $0x65567473,0x65(%rsi),%esp
+   1800e744e:	jb     0x1800e74c3
+   1800e7450:	imul   $0x2e31273d,0x6e(%rdi),%ebp
+   1800e7457:	xor    %ah,(%rdi)
+   1800e7459:	ds or  $0x3c20200a,%eax
+   1800e745f:	je     0x1800e74d3
+   1800e7461:	jne    0x1800e74d6
+   1800e7463:	je     0x1800e74ae
+   1800e7465:	outsb  %ds:(%rsi),(%dx)
+   1800e7466:	outsw  %ds:(%rsi),(%dx)
+   1800e7468:	and    %bh,0x6d(%rax)
+   1800e746b:	insb   (%dx),%es:(%rdi)
+   1800e746c:	outsb  %ds:(%rsi),(%dx)
+   1800e746d:	jae    0x1800e74ac
+   1800e746f:	and    0x72(%rbp),%dh
+   1800e7472:	outsb  %ds:(%rsi),(%dx)
+   1800e7473:	cmp    0x63(%rbx),%dh
+   1800e7476:	push   $0x73616d65
+   1800e747b:	sub    $0x7263696d,%eax
+   1800e7480:	outsl  %ds:(%rsi),(%dx)
+   1800e7481:	jae    0x1800e74f2
+   1800e7483:	data16 je 0x1800e74b3
+   1800e7486:	movsxd 0x6d(%rdi),%ebp
+   1800e7489:	cmp    0x73(%rcx),%ah
+   1800e748c:	insl   (%dx),%es:(%rdi)
+   1800e748d:	jbe,pn 0x1800e74c3
+   1800e7490:	and    (%rsi),%bh
+   1800e7492:	or     $0x2020200a,%eax
+   1800e7497:	and    %bh,(%rbx,%rsi,2)
+   1800e749a:	movsxd %gs:0x72(%rbp),%esi
+   1800e749e:	imul   $0x20200a0d,0x3e(%rcx,%rdi,2),%esi
+   1800e74a6:	and    %ah,(%rax)
+   1800e74a8:	and    %ah,(%rax)
+   1800e74aa:	cmp    $0x72,%al
+   1800e74ac:	gs jno 0x1800e7524
+   1800e74af:	gs jae 0x1800e7526
+   1800e74b2:	gs fs push %rax
+   1800e74b5:	jb     0x1800e7520
+   1800e74b7:	jbe    0x1800e7522
+   1800e74b9:	insb   (%dx),%es:(%rdi)
+   1800e74ba:	gs addr32 gs jae 0x1800e74fd
+   1800e74bf:	or     $0x2020200a,%eax
+   1800e74c4:	and    %ah,(%rax)
+   1800e74c6:	and    %ah,(%rax)
+   1800e74c8:	and    %bh,(%rdx,%rsi,2)
+   1800e74cb:	gs jno 0x1800e7543
+   1800e74ce:	gs jae 0x1800e7545
+   1800e74d1:	gs fs rex.RB js 0x1800e753b
+   1800e74d6:	movsxd 0x74(%rbp),%esi
+   1800e74d9:	imul   $0x6576654c,0x6e(%rdi),%ebp
+   1800e74e0:	insb   (%dx),%es:(%rdi)
+   1800e74e1:	and    %ch,0x76(%rbp,%riz,2)
+   1800e74e5:	gs insb (%dx),%es:(%rdi)
+   1800e74e7:	cmp    $0x49736127,%eax
+   1800e74ec:	outsb  %ds:(%rsi),(%dx)
+   1800e74ed:	jbe    0x1800e755e
+   1800e74ef:	imul   $0x27,0x72(%rbp),%esp
+   1800e74f3:	and    %dh,0x69(%rbp)
+   1800e74f6:	movsxd 0x65(%r11),%esp
+   1800e74fa:	jae    0x1800e756f
+   1800e74fc:	cmp    $0x6c616627,%eax
+   1800e7501:	jae    0x1800e7568
+   1800e7503:	(bad)
+   1800e7504:	and    %ch,(%rdi)
+   1800e7506:	ds or  $0x2020200a,%eax
+   1800e750c:	and    %ah,(%rax)
+   1800e750e:	and    %bh,(%rdi,%rbp,1)
+   1800e7511:	jb     0x1800e7578
+   1800e7513:	jno    0x1800e758a
+   1800e7515:	gs jae 0x1800e758c
+   1800e7518:	gs fs push %rax
+   1800e751b:	jb     0x1800e7586
+   1800e751d:	jbe    0x1800e7588
+   1800e751f:	insb   (%dx),%es:(%rdi)
+   1800e7520:	gs addr32 gs jae 0x1800e7563
+   1800e7525:	or     $0x2020200a,%eax
+   1800e752a:	and    %bh,(%rdi,%rbp,1)
+   1800e752d:	jae    0x1800e7594
+   1800e752f:	movsxd 0x72(%rbp),%esi
+   1800e7532:	imul   $0x20200a0d,0x3e(%rcx,%rdi,2),%esi
+   1800e753a:	cmp    $0x2f,%al
+   1800e753c:	je     0x1800e75b0
+   1800e753e:	jne    0x1800e75b3
+   1800e7540:	je     0x1800e758b
+   1800e7542:	outsb  %ds:(%rsi),(%dx)
+   1800e7543:	outsw  %ds:(%rsi),(%dx)
+   1800e7545:	ds or  $0x612f3c0a,%eax
+   1800e754b:	jae    0x1800e75c0
+   1800e754d:	gs insl (%dx),%es:(%rdi)
+   1800e754f:	(bad)
+   1800e7550:	insb   (%dx),%es:(%rdi)
+   1800e7551:	jns    0x1800e7591
+   1800e7553:	or     $0xa,%eax
 
 Disassembly of section .reloc:
 
 00000001800e8000 <.reloc>:
    1800e8000:	add    %al,(%rax)
    1800e8002:	or     (%rax),%al
    1800e8004:	and    $0x0,%al
```

## Comparing `turbojpeg-0.0.1.dist-info/METADATA` & `turbojpeg-0.0.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbojpeg
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python bindungs for libjpeg-turbo using pybind11
 Home-page: https://github.com/Dobatymo/turbojpeg-python
 Author: Dobatymo
 Author-email: Dobatymo@users.noreply.github.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -53,7 +53,11 @@
 ```
 
 ## Build
 
 The Python `setup.py` expects the `libjpeg-turbo` binaries in `libjpeg-turbo-build`. You can either build it yourself or download precompiled binaries. For more details see <https://github.com/libjpeg-turbo/libjpeg-turbo/blob/main/BUILDING.md>.
 
 GitHub actions CI builds wheels for Windows 32 and 64-bit, manylinux 64-bit, musllinux 64-bit and MacOS 64-bit. 32-bit Linux builds fail due some weird NASM error. Not all wheels are tested, since some of the test dependencies are not available for all platforms.
+
+## Run tests
+
+`python -m unittest discover -s tests`
```

