# Comparing `tmp/sqlite_http-0.1.0a9-py3-none-win_amd64.whl.zip` & `tmp/sqlite_http-0.1.1a1-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5033566 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat        0 b- defN 23-Aug-05 01:39 noop.cp311-win_amd64.pyd
--rw-rw-rw-  2.0 fat      556 b- defN 23-Aug-05 01:38 sqlite_http/__init__.py
--rw-rw-rw-  2.0 fat 15831410 b- defN 23-Aug-05 01:39 sqlite_http/http0.dll
--rw-rw-rw-  2.0 fat       81 b- defN 23-Aug-05 01:38 sqlite_http/version.py
--rw-rw-rw-  2.0 fat      515 b- defN 23-Aug-05 01:39 sqlite_http-0.1.0a9.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-Aug-05 01:39 sqlite_http-0.1.0a9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Aug-05 01:39 sqlite_http-0.1.0a9.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      638 b- defN 23-Aug-05 01:39 sqlite_http-0.1.0a9.dist-info/RECORD
-8 files, 15833319 bytes uncompressed, 5032452 bytes compressed:  68.2%
+Zip file size: 5033570 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Aug-06 00:42 noop.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      556 b- defN 23-Aug-06 00:41 sqlite_http/__init__.py
+-rw-rw-rw-  2.0 fat 15831410 b- defN 23-Aug-06 00:41 sqlite_http/http0.dll
+-rw-rw-rw-  2.0 fat       81 b- defN 23-Aug-06 00:41 sqlite_http/version.py
+-rw-rw-rw-  2.0 fat      515 b- defN 23-Aug-06 00:42 sqlite_http-0.1.1a1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-Aug-06 00:42 sqlite_http-0.1.1a1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Aug-06 00:42 sqlite_http-0.1.1a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      638 b- defN 23-Aug-06 00:42 sqlite_http-0.1.1a1.dist-info/RECORD
+8 files, 15833319 bytes uncompressed, 5032456 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: sqlite_http/http0.dll
 Comment: 
 
 Filename: sqlite_http/version.py
 Comment: 
 
-Filename: sqlite_http-0.1.0a9.dist-info/METADATA
+Filename: sqlite_http-0.1.1a1.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_http-0.1.0a9.dist-info/WHEEL
+Filename: sqlite_http-0.1.1a1.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_http-0.1.0a9.dist-info/top_level.txt
+Filename: sqlite_http-0.1.1a1.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_http-0.1.0a9.dist-info/RECORD
+Filename: sqlite_http-0.1.1a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_http/http0.dll

### objdump

```diff
@@ -26,15 +26,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	1
 Win32Version		00000000
 SizeOfImage		00ef4000
 SizeOfHeaders		00000600
-CheckSum		00f23b04
+CheckSum		00f26135
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00008160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 					TERMINAL_SERVICE_AWARE
 SizeOfStackReserve	0000000000200000
@@ -75026,56 +75026,58 @@
    377b6159a:	nopw   0x0(%rax,%rax,1)
 
 0000000377b615a0 <go:buildid>:
    377b615a0:	jmp    *(%rax)
    377b615a2:	rex.RXB outsl %ds:(%rsi),(%dx)
    377b615a4:	and    %ah,0x75(%rdx)
    377b615a7:	imul   $0x203a4449,0x20(%rsp,%riz,2),%ebp
-   377b615af:	and    0x72(%rdi),%bl
-   377b615b2:	rex.WRB jo 377b6161e <go:buildid+0x7e>
-   377b615b5:	push   %rsi
-   377b615b6:	data16 rex.RXB
-   377b615b8:	rex.WRXB push %r9
-   377b615ba:	cmp    %edx,0x34(%rbx)
-   377b615bd:	outsl  %ds:(%rsi),(%dx)
-   377b615be:	rex.RX pop %rdi
-   377b615c0:	jns    377b615f8 <go:buildid+0x58>
-   377b615c2:	pop    %rdi
-   377b615c3:	push   %rbx
+   377b615af:	and    0x65(%rdx),%bl
+   377b615b2:	rex.X
+   377b615b3:	data16 rex.XB insb (%dx),%es:(%rdi)
+   377b615b6:	rex.X
+   377b615b7:	rex.WRB jns 377b61607 <go:buildid+0x67>
+   377b615ba:	rex.WB
+   377b615bb:	rex.WXB jb 377b61623 <internal/abi.(*RegArgs).Dump+0x3>
+   377b615be:	rex.WXB
+   377b615bf:	rex.WRB push %r15
+   377b615c1:	rex.WRXB js 377b61607 <go:buildid+0x67>
    377b615c4:	(bad)
-   377b615c5:	rex.WXB xor %rbx,0x44(%r10)
-   377b615c9:	rex.RX push $0x42
-   377b615cc:	jae    377b61604 <go:buildid+0x64>
-   377b615ce:	imul   $0x4e,0x31(%rbx),%ebp
-   377b615d2:	rex.RB
-   377b615d3:	rex.RXB outsl %ds:(%rsi),(%dx)
-   377b615d5:	rex.WB
-   377b615d6:	data16 rex.W
-   377b615d8:	data16 (bad)
+   377b615c5:	pop    %rdi
+   377b615c6:	jbe    377b61619 <go:buildid+0x79>
+   377b615c8:	jb     377b61640 <internal/abi.(*RegArgs).Dump+0x20>
+   377b615ca:	push   $0x31
+   377b615cc:	rex.W push $0x63
+   377b615cf:	xor    0x30(%rdx),%cl
+   377b615d2:	outsb  %ds:(%rsi),(%dx)
+   377b615d3:	pop    %rcx
+   377b615d4:	rex.XB
+   377b615d5:	rex.R push $0x50
+   377b615d8:	xor    %ch,(%rdi)
    377b615da:	xor    0x64(%rsi),%dh
    377b615dd:	rex.X sub $0x6a4a6243,%eax
    377b615e3:	push   %rcx
    377b615e4:	je     377b6165b <internal/abi.(*RegArgs).Dump+0x3b>
    377b615e6:	rex.WRX push %rsi
    377b615e8:	rex.WR
    377b615e9:	rex.WRX outsl %ds:(%rsi),(%dx)
    377b615eb:	push   %dx
    377b615ed:	gs (bad)
-   377b615ef:	js     377b61665 <internal/abi.(*RegArgs).Dump+0x45>
-   377b615f1:	rex.WB jno 377b61669 <internal/abi.(*RegArgs).Dump+0x49>
-   377b615f4:	insb   (%dx),%es:(%rdi)
-   377b615f5:	xor    %eax,0x76(%rcx)
-   377b615f8:	push   %rsp
-   377b615f9:	push   $0x6a537366
-   377b615fe:	rex.WR insl (%dx),%es:(%rdi)
-   377b61600:	rex.X
-   377b61601:	fs insl (%dx),%es:(%rdi)
-   377b61603:	and    (%rdx),%cl
-   377b61605:	and    %bh,%bh
-   377b61607:	int3
+   377b615ef:	insl   (%dx),%es:(%rdi)
+   377b615f0:	rex.XB sub $0x3757667a,%eax
+   377b615f6:	pop    %rdi
+   377b615f7:	outsl  %ds:(%rsi),(%dx)
+   377b615f8:	(bad)
+   377b615f9:	outsl  %gs:(%rsi),(%dx)
+   377b615fb:	pop    %rcx
+   377b615fc:	jb     377b6166a <internal/abi.(*RegArgs).Dump+0x4a>
+   377b615fe:	rex.RXB pop %r10
+   377b61600:	jbe    377b6167b <internal/abi.(*RegArgs).Dump+0x5b>
+   377b61602:	xor    (%rdx),%ah
+   377b61604:	or     (%rax),%ah
+   377b61606:	dec    %esp
    377b61608:	int3
    377b61609:	int3
    377b6160a:	int3
    377b6160b:	int3
    377b6160c:	int3
    377b6160d:	int3
    377b6160e:	int3
@@ -1130212,41 +1130214,43 @@
    377e5125b:	insb   (%dx),%es:(%rdi)
    377e5125c:	(bad)
    377e5125d:	addr32 jae 377e5129d <go:buildinfo+0x27d>
    377e51260:	and    0x616d2058(%rip),%ch        # 3d95232be <.debug_line_str+0x60ad0274>
    377e51266:	imul   $0x73726556,0x2e(%rsi),%ebp
    377e5126d:	imul   $0x2e30763d,0x6e(%rdi),%ebp
    377e51274:	xor    %ebp,(%rsi)
-   377e51276:	xor    %ch,0x68706c61(%rip)        # 3e0557edd <.debug_line_str+0x67b04e93>
+   377e51276:	xor    %ebp,0x68706c61(%rip)        # 3e0557edd <.debug_line_str+0x67b04e93>
    377e5127c:	(bad)
-   377e5127d:	cs cmp %esp,(%rax)
+   377e5127d:	cs xor %esp,(%rax)
    377e51280:	sub    $0x616d2058,%eax
    377e51285:	imul   $0x6d6d6f43,0x2e(%rsi),%ebp
-   377e5128c:	imul   $0x35623631,0x32(%rbp,%rdi,1),%esi
-   377e51294:	xor    $0x31,%al
-   377e51296:	(bad)
-   377e51298:	xor    (%rsi),%esi
-   377e5129a:	cmp    %bh,(%rcx)
-   377e5129c:	xor    $0x38,%al
-   377e5129e:	gs xor $0x33,%al
-   377e512a1:	gs xor $0x31626130,%eax
-   377e512a7:	xor    0x30(%rbx),%esp
-   377e512aa:	xor    %esp,0x34(%rsi)
-   377e512ad:	(bad)
-   377e512ae:	cmp    %esp,0x66(%rbp)
-   377e512b1:	xor    $0x34,%al
-   377e512b3:	ss ss xor $0x582d2039,%eax
-   377e512ba:	and    %ch,0x61(%rbp)
+   377e5128c:	imul   $0x64633839,0x37(%rbp,%rdi,1),%esi
+   377e51294:	ss cmp %dh,(%rdi)
+   377e51297:	ss gs xor $0x64,%al
+   377e5129b:	xor    0x62(%rbp),%ah
+   377e5129e:	gs (bad)
+   377e512a0:	(bad)
+   377e512a1:	cmp    %esp,0x36(%rbp)
+   377e512a4:	gs (bad)
+   377e512a6:	xor    %ah,0x35(%rsi)
+   377e512a9:	xor    %ah,0x36(%rcx)
+   377e512ac:	xor    %si,(%rcx)
+   377e512af:	xor    $0x31,%al
+   377e512b1:	cmp    %bh,%gs:(%rcx)
+   377e512b4:	(bad)
+   377e512b5:	cmp    %bh,(%rcx)
+   377e512b7:	and    %ch,0x616d2058(%rip)        # 3d9523315 <.debug_line_str+0x60ad02cb>
    377e512bd:	imul   $0x65746144,0x2e(%rsi),%ebp
    377e512c4:	cmp    $0x33323032,%eax
    377e512c9:	sub    $0x302d3830,%eax
-   377e512ce:	xor    $0x3a313054,%eax
-   377e512d3:	xor    (%rdi),%esi
-   377e512d5:	cmp    (%rdx),%dh
-   377e512d7:	xor    %ebx,0x2b(%rdx)
+   377e512ce:	ss push %rsp
+   377e512d0:	xor    %dh,(%rax)
+   377e512d2:	cmp    (%rax,%rsi,1),%dh
+   377e512d5:	cmp    (%rcx),%dh
+   377e512d7:	xor    0x2b(%rdx),%ebx
    377e512da:	xor    %dh,(%rax)
    377e512dc:	xor    %dh,(%rax)
    377e512de:	and    (%rdx),%cl
    377e512e0:	(bad)
    377e512e2:	imul   $0x6761742d,0x9(%rsp,%riz,2),%ebp
    377e512ea:	jae    377e51329 <go:buildinfo+0x309>
    377e512ec:	jae    377e51356 <go:buildinfo+0x336>
@@ -1130338,34 +1130342,41 @@
    377e513ce:	or     %esi,0x63(%rsi)
    377e513d1:	jae    377e51401 <go:buildinfo+0x3e1>
    377e513d3:	jb     377e5143a <go:buildinfo+0x41a>
    377e513d5:	jbe    377e51440 <go:buildinfo+0x420>
    377e513d7:	jae    377e51442 <go:buildinfo+0x422>
    377e513d9:	outsl  %ds:(%rsi),(%dx)
    377e513da:	outsb  %ds:(%rsi),(%dx)
-   377e513db:	cmp    $0x62363132,%eax
-   377e513e0:	xor    $0x36623134,%eax
-   377e513e5:	xor    (%rsi),%esi
-   377e513e7:	cmp    %bh,(%rcx)
-   377e513e9:	xor    $0x38,%al
-   377e513eb:	gs xor $0x33,%al
-   377e513ee:	gs xor $0x31626130,%eax
-   377e513f4:	xor    0x30(%rbx),%esp
-   377e513f7:	xor    %esp,0x34(%rsi)
-   377e513fa:	(bad)
-   377e513fb:	cmp    %esp,0x66(%rbp)
-   377e513fe:	xor    $0x34,%al
-   377e51400:	ss ss xor $0x75620a39,%eax
+   377e513db:	cmp    $0x63383937,%eax
+   377e513e0:	fs cmp %dh,%fs:(%rdi)
+   377e513e4:	ss gs xor $0x64,%al
+   377e513e8:	xor    0x62(%rbp),%ah
+   377e513eb:	gs (bad)
+   377e513ed:	(bad)
+   377e513ee:	cmp    %esp,0x36(%rbp)
+   377e513f1:	gs (bad)
+   377e513f3:	xor    %ah,0x35(%rsi)
+   377e513f6:	xor    %ah,0x36(%rcx)
+   377e513f9:	xor    %si,(%rcx)
+   377e513fc:	xor    $0x31,%al
+   377e513fe:	cmp    %bh,%gs:(%rcx)
+   377e51401:	(bad)
+   377e51402:	cmp    %bh,(%rcx)
+   377e51404:	or     0x75(%rdx),%ah
    377e51407:	imul   $0x2e736376,0x9(%rsp,%riz,2),%ebp
    377e5140f:	je     377e5147a <text/template..gobytes.6+0x2>
    377e51411:	insl   (%dx),%es:(%rdi)
    377e51412:	gs cmp $0x33323032,%eax
    377e51418:	sub    $0x302d3830,%eax
-   377e5141d:	xor    $0x3a313054,%eax
-   377e51422:	xor    0x5a32353a(%rip),%esi        # 3d2174962 <.debug_line_str+0x59721918>
+   377e5141d:	ss push %rsp
+   377e5141f:	xor    %dh,(%rax)
+   377e51421:	cmp    (%rbx),%dh
+   377e51423:	cmp    %bh,(%rdx)
+   377e51425:	xor    $0x32,%al
+   377e51427:	pop    %rdx
    377e51428:	or     0x75(%rdx),%ah
    377e5142b:	imul   $0x2e736376,0x9(%rsp,%riz,2),%ebp
    377e51433:	insl   (%dx),%es:(%rdi)
    377e51434:	outsl  %ds:(%rsi),(%dx)
    377e51435:	imul   $0x663d6465,%fs:0x69(%rsi),%esp
    377e5143d:	(bad)
    377e5143e:	insb   (%dx),%es:(%rdi)
@@ -1681332,17 +1681343,17 @@
    377fa8e3a:	add    %al,(%rax)
    377fa8e3c:	add    %al,(%rax)
 	...
 
 0000000377fa8e40 <main.Version.str>:
    377fa8e40:	jbe    377fa8e72 <vendor/golang.org/x/crypto/chacha20poly1305.sseIncMask+0x2>
    377fa8e42:	cs xor %ebp,(%rsi)
-   377fa8e45:	xor    %ch,0x68706c61(%rip)        # 3e06afaac <.debug_line_str+0x67c5ca62>
+   377fa8e45:	xor    %ebp,0x68706c61(%rip)        # 3e06afaac <.debug_line_str+0x67c5ca62>
    377fa8e4b:	(bad)
-   377fa8e4c:	cs cmp %eax,(%rax)
+   377fa8e4c:	cs xor %eax,(%rax)
 	...
 
 0000000377fa8e50 <bswapMask>:
    377fa8e50:	femms
    377fa8e52:	or     $0x90a0b0c,%eax
    377fa8e57:	or     %al,(%rdi)
    377fa8e59:	(bad)
@@ -1684512,18 +1684523,19 @@
    377faa37f:	add    %ah,0x377b615(%rax)
 	...
 
 0000000377faa390 <main.Date.str>:
    377faa390:	xor    (%rax),%dh
    377faa392:	xor    (%rbx),%dh
    377faa394:	sub    $0x302d3830,%eax
-   377faa399:	xor    $0x3a313054,%eax
-   377faa39e:	xor    (%rdi),%esi
-   377faa3a0:	cmp    (%rdx),%dh
-   377faa3a2:	xor    %ebx,0x2b(%rdx)
+   377faa399:	ss push %rsp
+   377faa39b:	xor    %dh,(%rax)
+   377faa39d:	cmp    (%rax,%rsi,1),%dh
+   377faa3a0:	cmp    (%rcx),%dh
+   377faa3a2:	xor    0x2b(%rdx),%ebx
    377faa3a5:	xor    %dh,(%rax)
    377faa3a7:	xor    %dh,(%rax)
 	...
 
 0000000377faa3c0 <BSWAP_SHUFB_CTL>:
    377faa3c0:	add    (%rdx),%eax
    377faa3c2:	add    %eax,(%rax)
@@ -1689052,27 +1689064,31 @@
    377fac7c2:	int1
    377fac7c3:	ja     377fac7c8 <vendor/golang.org/x/text/unicode/norm..stmp_12+0x8>
    377fac7c5:	add    %al,(%rax)
    377fac7c7:	add    %al,(%rdx)
 	...
 
 0000000377fac800 <main.Commit.str>:
-   377fac800:	xor    (%rcx),%dh
-   377fac802:	(bad)
-   377fac808:	ss xor (%rsi),%esi
-   377fac80b:	cmp    %bh,(%rcx)
-   377fac80d:	xor    $0x38,%al
-   377fac80f:	gs xor $0x33,%al
-   377fac812:	gs xor $0x31626130,%eax
-   377fac818:	xor    0x30(%rbx),%esp
-   377fac81b:	xor    %esp,0x34(%rsi)
-   377fac81e:	(bad)
-   377fac81f:	cmp    %esp,0x66(%rbp)
-   377fac822:	xor    $0x34,%al
-   377fac824:	ss ss xor $0x39,%eax
+   377fac800:	(bad)
+   377fac801:	cmp    %edi,(%rax)
+   377fac803:	movsxd 0x38(%rsi,%rsi,1),%esp
+   377fac807:	(bad)
+   377fac808:	ss gs xor $0x64,%al
+   377fac80c:	xor    0x62(%rbp),%ah
+   377fac80f:	gs (bad)
+   377fac811:	(bad)
+   377fac812:	cmp    %esp,0x36(%rbp)
+   377fac815:	gs (bad)
+   377fac817:	xor    %ah,0x35(%rsi)
+   377fac81a:	xor    %ah,0x36(%rcx)
+   377fac81d:	xor    %si,(%rcx)
+   377fac820:	xor    $0x31,%al
+   377fac822:	cmp    %bh,%gs:(%rcx)
+   377fac825:	(bad)
+   377fac826:	cmp    %bh,(%rcx)
 	...
 
 0000000377fac840 <zeroTLS>:
 	...
 
 0000000377fac870 <go:itab.encoding/json.byIndex,sort.Interface>:
    377fac870:	add    %bh,(%rdx)
@@ -1698338,41 +1698354,43 @@
    377fb298f:	insb   (%dx),%es:(%rdi)
    377fb2990:	(bad)
    377fb2991:	addr32 jae 377fb29d1 <runtime.modinfo.str+0x251>
    377fb2994:	and    0x616d2058(%rip),%ch        # 3d96849f2 <.debug_line_str+0x60c319a8>
    377fb299a:	imul   $0x73726556,0x2e(%rsi),%ebp
    377fb29a1:	imul   $0x2e30763d,0x6e(%rdi),%ebp
    377fb29a8:	xor    %ebp,(%rsi)
-   377fb29aa:	xor    %ch,0x68706c61(%rip)        # 3e06b9611 <.debug_line_str+0x67c665c7>
+   377fb29aa:	xor    %ebp,0x68706c61(%rip)        # 3e06b9611 <.debug_line_str+0x67c665c7>
    377fb29b0:	(bad)
-   377fb29b1:	cs cmp %esp,(%rax)
+   377fb29b1:	cs xor %esp,(%rax)
    377fb29b4:	sub    $0x616d2058,%eax
    377fb29b9:	imul   $0x6d6d6f43,0x2e(%rsi),%ebp
-   377fb29c0:	imul   $0x35623631,0x32(%rbp,%rdi,1),%esi
-   377fb29c8:	xor    $0x31,%al
-   377fb29ca:	(bad)
-   377fb29cc:	xor    (%rsi),%esi
-   377fb29ce:	cmp    %bh,(%rcx)
-   377fb29d0:	xor    $0x38,%al
-   377fb29d2:	gs xor $0x33,%al
-   377fb29d5:	gs xor $0x31626130,%eax
-   377fb29db:	xor    0x30(%rbx),%esp
-   377fb29de:	xor    %esp,0x34(%rsi)
-   377fb29e1:	(bad)
-   377fb29e2:	cmp    %esp,0x66(%rbp)
-   377fb29e5:	xor    $0x34,%al
-   377fb29e7:	ss ss xor $0x582d2039,%eax
-   377fb29ee:	and    %ch,0x61(%rbp)
+   377fb29c0:	imul   $0x64633839,0x37(%rbp,%rdi,1),%esi
+   377fb29c8:	ss cmp %dh,(%rdi)
+   377fb29cb:	ss gs xor $0x64,%al
+   377fb29cf:	xor    0x62(%rbp),%ah
+   377fb29d2:	gs (bad)
+   377fb29d4:	(bad)
+   377fb29d5:	cmp    %esp,0x36(%rbp)
+   377fb29d8:	gs (bad)
+   377fb29da:	xor    %ah,0x35(%rsi)
+   377fb29dd:	xor    %ah,0x36(%rcx)
+   377fb29e0:	xor    %si,(%rcx)
+   377fb29e3:	xor    $0x31,%al
+   377fb29e5:	cmp    %bh,%gs:(%rcx)
+   377fb29e8:	(bad)
+   377fb29e9:	cmp    %bh,(%rcx)
+   377fb29eb:	and    %ch,0x616d2058(%rip)        # 3d9684a49 <.debug_line_str+0x60c319ff>
    377fb29f1:	imul   $0x65746144,0x2e(%rsi),%ebp
    377fb29f8:	cmp    $0x33323032,%eax
    377fb29fd:	sub    $0x302d3830,%eax
-   377fb2a02:	xor    $0x3a313054,%eax
-   377fb2a07:	xor    (%rdi),%esi
-   377fb2a09:	cmp    (%rdx),%dh
-   377fb2a0b:	xor    %ebx,0x2b(%rdx)
+   377fb2a02:	ss push %rsp
+   377fb2a04:	xor    %dh,(%rax)
+   377fb2a06:	cmp    (%rax,%rsi,1),%dh
+   377fb2a09:	cmp    (%rcx),%dh
+   377fb2a0b:	xor    0x2b(%rdx),%ebx
    377fb2a0e:	xor    %dh,(%rax)
    377fb2a10:	xor    %dh,(%rax)
    377fb2a12:	and    (%rdx),%cl
    377fb2a14:	(bad)
    377fb2a16:	imul   $0x6761742d,0x9(%rsp,%riz,2),%ebp
    377fb2a1e:	jae    377fb2a5d <runtime.modinfo.str+0x2dd>
    377fb2a20:	jae    377fb2a8a <runtime.modinfo.str+0x30a>
@@ -1698464,34 +1698482,41 @@
    377fb2b02:	or     %esi,0x63(%rsi)
    377fb2b05:	jae    377fb2b35 <runtime.modinfo.str+0x3b5>
    377fb2b07:	jb     377fb2b6e <runtime.modinfo.str+0x3ee>
    377fb2b09:	jbe    377fb2b74 <runtime.modinfo.str+0x3f4>
    377fb2b0b:	jae    377fb2b76 <runtime.modinfo.str+0x3f6>
    377fb2b0d:	outsl  %ds:(%rsi),(%dx)
    377fb2b0e:	outsb  %ds:(%rsi),(%dx)
-   377fb2b0f:	cmp    $0x62363132,%eax
-   377fb2b14:	xor    $0x36623134,%eax
-   377fb2b19:	xor    (%rsi),%esi
-   377fb2b1b:	cmp    %bh,(%rcx)
-   377fb2b1d:	xor    $0x38,%al
-   377fb2b1f:	gs xor $0x33,%al
-   377fb2b22:	gs xor $0x31626130,%eax
-   377fb2b28:	xor    0x30(%rbx),%esp
-   377fb2b2b:	xor    %esp,0x34(%rsi)
-   377fb2b2e:	(bad)
-   377fb2b2f:	cmp    %esp,0x66(%rbp)
-   377fb2b32:	xor    $0x34,%al
-   377fb2b34:	ss ss xor $0x75620a39,%eax
+   377fb2b0f:	cmp    $0x63383937,%eax
+   377fb2b14:	fs cmp %dh,%fs:(%rdi)
+   377fb2b18:	ss gs xor $0x64,%al
+   377fb2b1c:	xor    0x62(%rbp),%ah
+   377fb2b1f:	gs (bad)
+   377fb2b21:	(bad)
+   377fb2b22:	cmp    %esp,0x36(%rbp)
+   377fb2b25:	gs (bad)
+   377fb2b27:	xor    %ah,0x35(%rsi)
+   377fb2b2a:	xor    %ah,0x36(%rcx)
+   377fb2b2d:	xor    %si,(%rcx)
+   377fb2b30:	xor    $0x31,%al
+   377fb2b32:	cmp    %bh,%gs:(%rcx)
+   377fb2b35:	(bad)
+   377fb2b36:	cmp    %bh,(%rcx)
+   377fb2b38:	or     0x75(%rdx),%ah
    377fb2b3b:	imul   $0x2e736376,0x9(%rsp,%riz,2),%ebp
    377fb2b43:	je     377fb2bae <vendor/golang.org/x/sys/cpu..stmp_1+0x26>
    377fb2b45:	insl   (%dx),%es:(%rdi)
    377fb2b46:	gs cmp $0x33323032,%eax
    377fb2b4c:	sub    $0x302d3830,%eax
-   377fb2b51:	xor    $0x3a313054,%eax
-   377fb2b56:	xor    0x5a32353a(%rip),%esi        # 3d22d6096 <.debug_line_str+0x5988304c>
+   377fb2b51:	ss push %rsp
+   377fb2b53:	xor    %dh,(%rax)
+   377fb2b55:	cmp    (%rbx),%dh
+   377fb2b57:	cmp    %bh,(%rdx)
+   377fb2b59:	xor    $0x32,%al
+   377fb2b5b:	pop    %rdx
    377fb2b5c:	or     0x75(%rdx),%ah
    377fb2b5f:	imul   $0x2e736376,0x9(%rsp,%riz,2),%ebp
    377fb2b67:	insl   (%dx),%es:(%rdi)
    377fb2b68:	outsl  %ds:(%rsi),(%dx)
    377fb2b69:	imul   $0x663d6465,%fs:0x69(%rsi),%esp
    377fb2b71:	(bad)
    377fb2b72:	insb   (%dx),%es:(%rdi)
@@ -4194270,33 +4194295,8 @@
    3785f810f:	add    %al,(%rax)
    3785f8111:	add    %al,(%rax)
    3785f8113:	add    %al,(%rax)
    3785f8115:	(bad)
    3785f8116:	add    %dl,-0x6d(%rbx)
    3785f8119:	or     %dl,0x63089308(%rbx)
    3785f811f:	add    %eax,(%rax)
-   3785f8121:	add    %al,(%rax)
-   3785f8123:	add    %al,(%rax)
-   3785f8125:	add    %al,0x1(%rbp)
-   3785f812b:	add    %al,(%rax)
-   3785f812d:	add    %cl,(%rdx)
-   3785f812f:	add    %dl,-0x6d(%rbx)
-   3785f8132:	or     %dl,0x55089348(%rcx)
-   3785f8138:	xchg   %eax,%ebx
-   3785f8139:	or     %al,0x1(%rbp)
-   3785f813f:	add    %al,(%rax)
-   3785f8141:	add    %bl,0x1(%rcx)
-   3785f8147:	add    %al,(%rax)
-   3785f8149:	add    %cl,(%rcx)
-   3785f814b:	add    %dl,-0x6d(%rbx)
-   3785f814e:	or     %dl,-0x6d(%rdx)
-   3785f8151:	or     %dl,-0x6d(%rbp)
-   3785f8154:	or     %dl,%ch
-   3785f8156:	add    %eax,(%rax)
-   3785f8158:	add    %al,(%rax)
-   3785f815a:	add    %al,(%rax)
-   3785f815c:	add    %bl,%cl
-   3785f815e:	add    %eax,(%rax)
-   3785f8160:	add    %al,(%rax)
-   3785f8162:	add    %al,(%rax)
-   3785f8164:	add    %cl,(%rax)
-[ Too much input for diff (SHA256: 5f24e43ac3605c3a8de321df0ee034a2ca0bf02a4c7b8bc45ae399e17a524e3f) ]
+[ Too much input for diff (SHA256: ead3bb03143c8e73118f20c90285fdd2759a8aaa3f416368dbaa62b159449557) ]
```

## sqlite_http/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.9"
+__version__ = "0.1.1-alpha.1"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_http-0.1.0a9.dist-info/METADATA` & `sqlite_http-0.1.1a1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-http
-Version: 0.1.0a9
+Version: 0.1.1a1
 Home-page: https://github.com/asg017/sqlite-http
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-http/issues
 Project-URL: CI, https://github.com/asg017/sqlite-http/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-http/releases
 Requires-Python: >=3.7
```

