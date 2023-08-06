# Comparing `tmp/sqlite_html-0.1.2a8-py3-none-win_amd64.whl.zip` & `tmp/sqlite_html-0.1.3a1-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3906386 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat        0 b- defN 23-Aug-05 03:36 noop.cp311-win_amd64.pyd
--rw-rw-rw-  2.0 fat      315 b- defN 23-Aug-05 03:35 sqlite_html/__init__.py
--rw-rw-rw-  2.0 fat 12358681 b- defN 23-Aug-05 03:35 sqlite_html/html0.dll
--rw-rw-rw-  2.0 fat       81 b- defN 23-Aug-05 03:35 sqlite_html/version.py
--rw-rw-rw-  2.0 fat      515 b- defN 23-Aug-05 03:36 sqlite_html-0.1.2a8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-Aug-05 03:36 sqlite_html-0.1.2a8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Aug-05 03:36 sqlite_html-0.1.2a8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      638 b- defN 23-Aug-05 03:36 sqlite_html-0.1.2a8.dist-info/RECORD
-8 files, 12360349 bytes uncompressed, 3905272 bytes compressed:  68.4%
+Zip file size: 3906378 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Aug-06 01:11 noop.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      315 b- defN 23-Aug-06 01:10 sqlite_html/__init__.py
+-rw-rw-rw-  2.0 fat 12358681 b- defN 23-Aug-06 01:10 sqlite_html/html0.dll
+-rw-rw-rw-  2.0 fat       81 b- defN 23-Aug-06 01:10 sqlite_html/version.py
+-rw-rw-rw-  2.0 fat      515 b- defN 23-Aug-06 01:11 sqlite_html-0.1.3a1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-Aug-06 01:11 sqlite_html-0.1.3a1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Aug-06 01:11 sqlite_html-0.1.3a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      638 b- defN 23-Aug-06 01:11 sqlite_html-0.1.3a1.dist-info/RECORD
+8 files, 12360349 bytes uncompressed, 3905264 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: sqlite_html/html0.dll
 Comment: 
 
 Filename: sqlite_html/version.py
 Comment: 
 
-Filename: sqlite_html-0.1.2a8.dist-info/METADATA
+Filename: sqlite_html-0.1.3a1.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_html-0.1.2a8.dist-info/WHEEL
+Filename: sqlite_html-0.1.3a1.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_html-0.1.2a8.dist-info/top_level.txt
+Filename: sqlite_html-0.1.3a1.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_html-0.1.2a8.dist-info/RECORD
+Filename: sqlite_html-0.1.3a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_html/html0.dll

### objdump

```diff
@@ -26,15 +26,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	1
 Win32Version		00000000
 SizeOfImage		00baf000
 SizeOfHeaders		00000600
-CheckSum		00bd130e
+CheckSum		00bd69e3
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00008160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 					TERMINAL_SERVICE_AWARE
 SizeOfStackReserve	0000000000200000
@@ -62555,55 +62555,64 @@
    2de54159a:	nopw   0x0(%rax,%rax,1)
 
 00000002de5415a0 <go:buildid>:
    2de5415a0:	jmp    *(%rax)
    2de5415a2:	rex.RXB outsl %ds:(%rsi),(%dx)
    2de5415a4:	and    %ah,0x75(%rdx)
    2de5415a7:	imul   $0x203a4449,0x20(%rsp,%riz,2),%ebp
-   2de5415af:	and    0x76(%rbx),%ch
-   2de5415b2:	outsb  %ds:(%rsi),(%dx)
-   2de5415b3:	rex.XB push $0x46
-   2de5415b6:	(bad)
-   2de5415bb:	push   %rdi
-   2de5415bc:	push   $0x5a
-   2de5415be:	ja     2de541637 <internal/cpu.Initialize+0x17>
-   2de5415c0:	rex.RB
-   2de5415c1:	push   %si
-   2de5415c3:	ja     2de5415f4 <go:buildid+0x54>
-   2de5415c5:	xor    0x69(%rsi),%edx
-   2de5415c8:	rex.X jae 2de541615 <go:buildid+0x75>
-   2de5415cb:	ss push $0x5939374f
-   2de5415d1:	pop    %rdi
-   2de5415d2:	push   %rax
-   2de5415d3:	xor    0x6b(%rax),%r9b
-   2de5415d7:	rex.RB jae 2de541609 <go:buildid+0x69>
+   2de5415af:	and    0x52(%rax),%bl
+   2de5415b2:	sub    $0x4c38795f,%eax
+   2de5415b7:	rex.RB push %r12
+   2de5415b9:	rex.XB
+   2de5415ba:	addr32 push %rsi
+   2de5415bc:	rex.WX
+   2de5415bd:	rex.RX push %rbx
+   2de5415bf:	insb   (%dx),%es:(%rdi)
+   2de5415c0:	push   %rax
+   2de5415c1:	imul   $0x55,0x4d452f6a(%rip),%esi        # 32b994532 <.debug_line_str+0x4c8a64e8>
+   2de5415c8:	push   %rsp
+   2de5415c9:	outsl  %ds:(%rsi),(%dx)
+   2de5415ca:	insl   (%dx),%es:(%rdi)
+   2de5415cb:	push   %rbx
+   2de5415cc:	pop    %rdi
+   2de5415cd:	xor    %dh,(%rdi)
+   2de5415cf:	jb     2de54163b <internal/cpu.Initialize+0x1b>
+   2de5415d1:	ja     2de541621 <internal/cpu.Initialize+0x1>
+   2de5415d3:	jae    2de54162c <internal/cpu.Initialize+0xc>
+   2de5415d5:	rex.B jae 2de54162c <internal/cpu.Initialize+0xc>
+   2de5415d8:	push   %rcx
+   2de5415d9:	(bad)
    2de5415da:	insl   (%dx),%es:(%rdi)
    2de5415db:	push   %rcx
    2de5415dc:	xor    $0x67,%al
    2de5415de:	(bad)
    2de5415df:	rex.R outsl %ds:(%rsi),(%dx)
    2de5415e1:	xor    $0x39,%al
    2de5415e3:	push   %rbp
    2de5415e4:	rex.RXB
    2de5415e5:	rex.WR jne 2de541658 <internal/cpu.Initialize+0x38>
    2de5415e8:	pop    %rax
    2de5415e9:	outsl  %ds:(%rsi),(%dx)
    2de5415ea:	xor    0x34(%rdx),%ecx
    2de5415ed:	rex.WRB (bad)
-   2de5415ef:	rex.WXB jns 2de541644 <internal/cpu.Initialize+0x24>
-   2de5415f2:	data16 jae 2de541625 <internal/cpu.Initialize+0x5>
+   2de5415ef:	jbe    2de541622 <internal/cpu.Initialize+0x2>
+   2de5415f1:	rex.WX pop %rax
+   2de5415f3:	insl   (%dx),%es:(%rdi)
+   2de5415f4:	pop    %rdi
    2de5415f5:	push   %rdi
-   2de5415f6:	jae    2de54166d <internal/cpu.Initialize+0x4d>
-   2de5415f8:	rex.WRX xor 0x38(%rdx),%r9b
-   2de5415fc:	push   %rbp
-   2de5415fd:	pop    %rdi
-   2de5415fe:	xor    $0x38345064,%eax
-   2de541603:	and    (%rdx),%cl
-   2de541605:	and    %bh,%bh
-   2de541607:	int3
+   2de5415f6:	xor    (%r8),%sil
+   2de5415f9:	rex.WR
+   2de5415fa:	rex.WB
+   2de5415fb:	rex.RX
+   2de5415fc:	rex.WXB (bad)
+   2de5415fe:	rex.WRXB pop %r15
+   2de541600:	push   %rdx
+   2de541601:	cmp    %esp,0x22(%rdx)
+   2de541604:	or     (%rax),%ah
+   2de541606:	dec    %esp
    2de541608:	int3
    2de541609:	int3
    2de54160a:	int3
    2de54160b:	int3
    2de54160c:	int3
    2de54160d:	int3
    2de54160e:	int3
@@ -886953,41 +886962,47 @@
    2de77b378:	insb   (%dx),%es:(%rdi)
    2de77b379:	(bad)
    2de77b37a:	addr32 jae 2de77b3ba <go:buildinfo+0x39a>
    2de77b37d:	and    0x616d2058(%rip),%ch        # 33fe4d3db <.debug_line_str+0x60d5f391>
    2de77b383:	imul   $0x73726556,0x2e(%rsi),%ebp
    2de77b38a:	imul   $0x2e30763d,0x6e(%rdi),%ebp
    2de77b391:	xor    %ebp,(%rsi)
-   2de77b393:	xor    0x68706c61(%rip),%ch        # 346e81ffa <.debug_line_str+0x67d93fb0>
+   2de77b393:	xor    0x68706c61(%rip),%ebp        # 346e81ffa <.debug_line_str+0x67d93fb0>
    2de77b399:	(bad)
-   2de77b39a:	cs cmp %ah,(%rax)
+   2de77b39a:	cs xor %esp,(%rax)
    2de77b39d:	sub    $0x616d2058,%eax
    2de77b3a2:	imul   $0x6d6d6f43,0x2e(%rsi),%ebp
-   2de77b3a9:	imul   $0x65623734,0x30(%rbp,%rdi,1),%esi
-   2de77b3b1:	(bad)
-   2de77b3b2:	(bad)
+   2de77b3a9:	imul   $0x31393031,0x62(%rbp,%rdi,1),%esi
+   2de77b3b1:	cmp    %dh,(%rdi)
    2de77b3b3:	(bad)
-   2de77b3b4:	xor    %esi,(%rbx)
-   2de77b3b6:	xor    %esi,(%rdx,%riz,2)
-   2de77b3b9:	xor    (%rdx),%dh
-   2de77b3bb:	movsxd 0x36346336(%rip),%esi        # 314ac16f7 <.debug_line_str+0x359d36ad>
-   2de77b3c1:	(bad)
-   2de77b3c2:	(bad)
-   2de77b3c7:	cmp    %ah,%fs:0x33(%rbp)
-   2de77b3cb:	(bad)
+   2de77b3b4:	xor    (%rcx),%esi
+   2de77b3b6:	xor    0x39(%rdx),%esp
+   2de77b3b9:	xor    %dh,(%rcx)
+   2de77b3bb:	xor    (%rcx),%esi
+   2de77b3bd:	cmp    %esp,0x37(%rcx)
+   2de77b3c0:	gs data16 (bad)
+   2de77b3c3:	(bad)
+   2de77b3c4:	(bad)
+   2de77b3c5:	xor    %esp,0x61(%rbp)
+   2de77b3c8:	movsxd (%rbx),%esi
+   2de77b3ca:	cmp    %esi,(%rbx)
    2de77b3cc:	(bad)
-   2de77b3cd:	xor    %ah,0x30(%rax,%rsi,1)
-   2de77b3d1:	xor    0x65(%rsi),%esp
-   2de77b3d4:	and    %ch,0x616d2058(%rip)        # 33fe4d432 <.debug_line_str+0x60d5f3e8>
+   2de77b3cd:	(bad)
+   2de77b3ce:	cmp    %esi,%fs:(%rax)
+   2de77b3d1:	cmp    %dh,(%rdx)
+   2de77b3d3:	movsxd (%rax),%esp
+   2de77b3d5:	sub    $0x616d2058,%eax
    2de77b3da:	imul   $0x65746144,0x2e(%rsi),%ebp
    2de77b3e1:	cmp    $0x33323032,%eax
    2de77b3e6:	sub    $0x302d3830,%eax
-   2de77b3eb:	xor    $0x3a333054,%eax
-   2de77b3f0:	xor    (%rdx,%rdi,1),%esi
-   2de77b3f3:	xor    %esi,(%rdx)
+   2de77b3eb:	ss push %rsp
+   2de77b3ed:	xor    %dh,(%rcx)
+   2de77b3ef:	cmp    (%rax),%dh
+   2de77b3f1:	cmp    %edi,(%rdx)
+   2de77b3f3:	xor    %dh,(%rdi)
    2de77b3f5:	pop    %rdx
    2de77b3f6:	sub    (%rax),%esi
    2de77b3f8:	xor    %dh,(%rax)
    2de77b3fa:	xor    %ah,(%rdx)
    2de77b3fc:	or     0x75(%rdx),%ah
    2de77b3ff:	imul   $0x6761742d,0x9(%rsp,%riz,2),%ebp
    2de77b407:	jae    2de77b446 <go:buildinfo+0x426>
@@ -887080,40 +887095,47 @@
    2de77b4eb:	or     %esi,0x63(%rsi)
    2de77b4ee:	jae    2de77b51e <go:buildinfo+0x4fe>
    2de77b4f0:	jb     2de77b557 <go:buildinfo+0x537>
    2de77b4f2:	jbe    2de77b55d <go:buildinfo+0x53d>
    2de77b4f4:	jae    2de77b55f <go:buildinfo+0x53f>
    2de77b4f6:	outsl  %ds:(%rsi),(%dx)
    2de77b4f7:	outsb  %ds:(%rsi),(%dx)
-   2de77b4f8:	cmp    $0x62373430,%eax
-   2de77b4fd:	gs (bad)
+   2de77b4f8:	cmp    $0x39303162,%eax
+   2de77b4fd:	xor    %edi,(%rax)
    2de77b4ff:	(bad)
    2de77b500:	(bad)
-   2de77b501:	xor    %esi,(%rbx)
-   2de77b503:	xor    %esi,(%rdx,%riz,2)
-   2de77b506:	xor    (%rdx),%dh
-   2de77b508:	movsxd 0x36346336(%rip),%esi        # 314ac1844 <.debug_line_str+0x359d37fa>
-   2de77b50e:	(bad)
-   2de77b50f:	(bad)
-   2de77b514:	cmp    %ah,%fs:0x33(%rbp)
-   2de77b518:	(bad)
+   2de77b501:	xor    (%rcx),%esi
+   2de77b503:	xor    0x39(%rdx),%esp
+   2de77b506:	xor    %dh,(%rcx)
+   2de77b508:	xor    (%rcx),%esi
+   2de77b50a:	cmp    %esp,0x37(%rcx)
+   2de77b50d:	gs data16 (bad)
+   2de77b510:	(bad)
+   2de77b511:	(bad)
+   2de77b512:	xor    %esp,0x61(%rbp)
+   2de77b515:	movsxd (%rbx),%esi
+   2de77b517:	cmp    %esi,(%rbx)
    2de77b519:	(bad)
-   2de77b51a:	xor    %ah,0x30(%rax,%rsi,1)
-   2de77b51e:	xor    0x65(%rsi),%esp
-   2de77b521:	or     0x75(%rdx),%ah
+   2de77b51a:	(bad)
+   2de77b51b:	cmp    %esi,%fs:(%rax)
+   2de77b51e:	cmp    %dh,(%rdx)
+   2de77b520:	movsxd (%rdx),%ecx
+   2de77b522:	(bad)
    2de77b524:	imul   $0x2e736376,0x9(%rsp,%riz,2),%ebp
    2de77b52c:	je     2de77b597 <encoding/json..gobytes.1+0x3>
    2de77b52e:	insl   (%dx),%es:(%rdi)
    2de77b52f:	gs cmp $0x33323032,%eax
    2de77b535:	sub    $0x302d3830,%eax
-   2de77b53a:	xor    $0x3a333054,%eax
-   2de77b53f:	xor    (%rdx),%esi
-   2de77b541:	cmp    (%rbx),%dh
-   2de77b543:	cmp    %bl,0xa(%rdx)
-   2de77b546:	(bad)
+   2de77b53a:	ss push %rsp
+   2de77b53c:	xor    %dh,(%rcx)
+   2de77b53e:	cmp    (%rax),%dh
+   2de77b540:	cmp    %bh,(%rdx)
+   2de77b542:	xor    %dh,(%rcx)
+   2de77b544:	pop    %rdx
+   2de77b545:	or     0x75(%rdx),%ah
    2de77b548:	imul   $0x2e736376,0x9(%rsp,%riz,2),%ebp
    2de77b550:	insl   (%dx),%es:(%rdi)
    2de77b551:	outsl  %ds:(%rsi),(%dx)
    2de77b552:	imul   $0x663d6465,%fs:0x69(%rsi),%esp
    2de77b55a:	(bad)
    2de77b55b:	insb   (%dx),%es:(%rdi)
    2de77b55c:	jae    2de77b5c3 <runtime.finalizer1+0x3>
@@ -1325592,17 +1325614,17 @@
    2de891ada:	add    %al,(%rax)
    2de891adc:	add    %al,(%rax)
 	...
 
 00000002de891ae0 <main.Version.str>:
    2de891ae0:	jbe    2de891b12 <main..stmp_9+0x2>
    2de891ae2:	cs xor %ebp,(%rsi)
-   2de891ae5:	xor    0x68706c61(%rip),%ch        # 346f9874c <.debug_line_str+0x67eaa702>
+   2de891ae5:	xor    0x68706c61(%rip),%ebp        # 346f9874c <.debug_line_str+0x67eaa702>
    2de891aeb:	(bad)
-   2de891aec:	cs cmp %al,(%rax)
+   2de891aec:	cs xor %eax,(%rax)
 	...
 
 00000002de891af0 <main..stmp_5>:
    2de891af0:	fiaddl -0x7d(%rdx)
    2de891af3:	fiadds (%rdx)
    2de891af5:	add    %al,(%rax)
    2de891af7:	add    %dh,(%rbx)
@@ -1327937,17 +1327959,19 @@
    2de892a7d:	add    %al,(%rax)
 	...
 
 00000002de892a80 <main.Date.str>:
    2de892a80:	xor    (%rax),%dh
    2de892a82:	xor    (%rbx),%dh
    2de892a84:	sub    $0x302d3830,%eax
-   2de892a89:	xor    $0x3a333054,%eax
-   2de892a8e:	xor    (%rdx,%rdi,1),%esi
-   2de892a91:	xor    %esi,(%rdx)
+   2de892a89:	ss push %rsp
+   2de892a8b:	xor    %dh,(%rcx)
+   2de892a8d:	cmp    (%rax),%dh
+   2de892a8f:	cmp    %edi,(%rdx)
+   2de892a91:	xor    %dh,(%rdi)
    2de892a93:	pop    %rdx
    2de892a94:	sub    (%rax),%esi
    2de892a96:	xor    %dh,(%rax)
    2de892a98:	xor    %al,(%rax)
    2de892a9a:	add    %al,(%rax)
    2de892a9c:	add    %al,(%rax)
 	...
@@ -1329682,31 +1329706,36 @@
 00000002de8939a0 <vendor/golang.org/x/text/unicode/norm..stmp_12>:
    2de8939a0:	(bad)
    2de8939a2:	sbb    $0x2,%esi
    2de8939a8:	add    (%rax),%al
 	...
 
 00000002de8939e0 <main.Commit.str>:
-   2de8939e0:	xor    %dh,(%rdi,%rsi,1)
-   2de8939e3:	(bad)
-   2de8939e5:	(bad)
+   2de8939e0:	(bad)
+   2de8939e2:	xor    %bh,(%rcx)
+   2de8939e4:	xor    %edi,(%rax)
    2de8939e6:	(bad)
    2de8939e7:	(bad)
-   2de8939e8:	xor    %esi,(%rbx)
-   2de8939ea:	xor    %esi,(%rdx,%riz,2)
-   2de8939ed:	xor    (%rdx),%dh
-   2de8939ef:	movsxd 0x36346336(%rip),%esi        # 314bd9d2b <.debug_line_str+0x35aebce1>
-   2de8939f5:	(bad)
-   2de8939f6:	(bad)
-   2de8939fb:	cmp    %ah,%fs:0x33(%rbp)
-   2de8939ff:	(bad)
+   2de8939e8:	xor    (%rcx),%esi
+   2de8939ea:	xor    0x39(%rdx),%esp
+   2de8939ed:	xor    %dh,(%rcx)
+   2de8939ef:	xor    (%rcx),%esi
+   2de8939f1:	cmp    %esp,0x37(%rcx)
+   2de8939f4:	gs data16 (bad)
+   2de8939f7:	(bad)
+   2de8939f8:	(bad)
+   2de8939f9:	xor    %esp,0x61(%rbp)
+   2de8939fc:	movsxd (%rbx),%esi
+   2de8939fe:	cmp    %esi,(%rbx)
    2de893a00:	(bad)
-   2de893a01:	xor    %ah,0x30(%rax,%rsi,1)
-   2de893a05:	xor    0x65(%rsi),%esp
-   2de893a08:	add    %al,(%rax)
+   2de893a01:	(bad)
+   2de893a02:	cmp    %esi,%fs:(%rax)
+   2de893a05:	cmp    %dh,(%rdx)
+   2de893a07:	movsxd (%rax),%eax
+   2de893a09:	add    %al,(%rax)
 	...
 
 00000002de893a0c <golang.org/x/net/html..stmp_41>:
    2de893a0c:	add    %eax,(%rcx)
    2de893a0e:	add    %eax,(%rcx)
    2de893a10:	add    %eax,(%rcx)
    2de893a12:	add    %eax,(%rcx)
@@ -1339753,41 +1339782,47 @@
    2de899bec:	insb   (%dx),%es:(%rdi)
    2de899bed:	(bad)
    2de899bee:	addr32 jae 2de899c2e <runtime.modinfo.str+0x36e>
    2de899bf1:	and    0x616d2058(%rip),%ch        # 33ff6bc4f <.debug_line_str+0x60e7dc05>
    2de899bf7:	imul   $0x73726556,0x2e(%rsi),%ebp
    2de899bfe:	imul   $0x2e30763d,0x6e(%rdi),%ebp
    2de899c05:	xor    %ebp,(%rsi)
-   2de899c07:	xor    0x68706c61(%rip),%ch        # 346fa086e <.debug_line_str+0x67eb2824>
+   2de899c07:	xor    0x68706c61(%rip),%ebp        # 346fa086e <.debug_line_str+0x67eb2824>
    2de899c0d:	(bad)
-   2de899c0e:	cs cmp %ah,(%rax)
+   2de899c0e:	cs xor %esp,(%rax)
    2de899c11:	sub    $0x616d2058,%eax
    2de899c16:	imul   $0x6d6d6f43,0x2e(%rsi),%ebp
-   2de899c1d:	imul   $0x65623734,0x30(%rbp,%rdi,1),%esi
-   2de899c25:	(bad)
-   2de899c26:	(bad)
+   2de899c1d:	imul   $0x31393031,0x62(%rbp,%rdi,1),%esi
+   2de899c25:	cmp    %dh,(%rdi)
    2de899c27:	(bad)
-   2de899c28:	xor    %esi,(%rbx)
-   2de899c2a:	xor    %esi,(%rdx,%riz,2)
-   2de899c2d:	xor    (%rdx),%dh
-   2de899c2f:	movsxd 0x36346336(%rip),%esi        # 314bdff6b <.debug_line_str+0x35af1f21>
-   2de899c35:	(bad)
-   2de899c36:	(bad)
-   2de899c3b:	cmp    %ah,%fs:0x33(%rbp)
-   2de899c3f:	(bad)
+   2de899c28:	xor    (%rcx),%esi
+   2de899c2a:	xor    0x39(%rdx),%esp
+   2de899c2d:	xor    %dh,(%rcx)
+   2de899c2f:	xor    (%rcx),%esi
+   2de899c31:	cmp    %esp,0x37(%rcx)
+   2de899c34:	gs data16 (bad)
+   2de899c37:	(bad)
+   2de899c38:	(bad)
+   2de899c39:	xor    %esp,0x61(%rbp)
+   2de899c3c:	movsxd (%rbx),%esi
+   2de899c3e:	cmp    %esi,(%rbx)
    2de899c40:	(bad)
-   2de899c41:	xor    %ah,0x30(%rax,%rsi,1)
-   2de899c45:	xor    0x65(%rsi),%esp
-   2de899c48:	and    %ch,0x616d2058(%rip)        # 33ff6bca6 <.debug_line_str+0x60e7dc5c>
+   2de899c41:	(bad)
+   2de899c42:	cmp    %esi,%fs:(%rax)
+   2de899c45:	cmp    %dh,(%rdx)
+   2de899c47:	movsxd (%rax),%esp
+   2de899c49:	sub    $0x616d2058,%eax
    2de899c4e:	imul   $0x65746144,0x2e(%rsi),%ebp
    2de899c55:	cmp    $0x33323032,%eax
    2de899c5a:	sub    $0x302d3830,%eax
-   2de899c5f:	xor    $0x3a333054,%eax
-   2de899c64:	xor    (%rdx,%rdi,1),%esi
-   2de899c67:	xor    %esi,(%rdx)
+   2de899c5f:	ss push %rsp
+   2de899c61:	xor    %dh,(%rcx)
+   2de899c63:	cmp    (%rax),%dh
+   2de899c65:	cmp    %edi,(%rdx)
+   2de899c67:	xor    %dh,(%rdi)
    2de899c69:	pop    %rdx
    2de899c6a:	sub    (%rax),%esi
    2de899c6c:	xor    %dh,(%rax)
    2de899c6e:	xor    %ah,(%rdx)
    2de899c70:	or     0x75(%rdx),%ah
    2de899c73:	imul   $0x6761742d,0x9(%rsp,%riz,2),%ebp
    2de899c7b:	jae    2de899cba <runtime.modinfo.str+0x3fa>
@@ -1339880,40 +1339915,47 @@
    2de899d5f:	or     %esi,0x63(%rsi)
    2de899d62:	jae    2de899d92 <runtime.modinfo.str+0x4d2>
    2de899d64:	jb     2de899dcb <runtime.modinfo.str+0x50b>
    2de899d66:	jbe    2de899dd1 <runtime.modinfo.str+0x511>
    2de899d68:	jae    2de899dd3 <runtime.modinfo.str+0x513>
    2de899d6a:	outsl  %ds:(%rsi),(%dx)
    2de899d6b:	outsb  %ds:(%rsi),(%dx)
-   2de899d6c:	cmp    $0x62373430,%eax
-   2de899d71:	gs (bad)
+   2de899d6c:	cmp    $0x39303162,%eax
+   2de899d71:	xor    %edi,(%rax)
    2de899d73:	(bad)
    2de899d74:	(bad)
-   2de899d75:	xor    %esi,(%rbx)
-   2de899d77:	xor    %esi,(%rdx,%riz,2)
-   2de899d7a:	xor    (%rdx),%dh
-   2de899d7c:	movsxd 0x36346336(%rip),%esi        # 314be00b8 <.debug_line_str+0x35af206e>
-   2de899d82:	(bad)
-   2de899d83:	(bad)
-   2de899d88:	cmp    %ah,%fs:0x33(%rbp)
-   2de899d8c:	(bad)
+   2de899d75:	xor    (%rcx),%esi
+   2de899d77:	xor    0x39(%rdx),%esp
+   2de899d7a:	xor    %dh,(%rcx)
+   2de899d7c:	xor    (%rcx),%esi
+   2de899d7e:	cmp    %esp,0x37(%rcx)
+   2de899d81:	gs data16 (bad)
+   2de899d84:	(bad)
+   2de899d85:	(bad)
+   2de899d86:	xor    %esp,0x61(%rbp)
+   2de899d89:	movsxd (%rbx),%esi
+   2de899d8b:	cmp    %esi,(%rbx)
    2de899d8d:	(bad)
-   2de899d8e:	xor    %ah,0x30(%rax,%rsi,1)
-   2de899d92:	xor    0x65(%rsi),%esp
-   2de899d95:	or     0x75(%rdx),%ah
+   2de899d8e:	(bad)
+   2de899d8f:	cmp    %esi,%fs:(%rax)
+   2de899d92:	cmp    %dh,(%rdx)
+   2de899d94:	movsxd (%rdx),%ecx
+   2de899d96:	(bad)
    2de899d98:	imul   $0x2e736376,0x9(%rsp,%riz,2),%ebp
    2de899da0:	je     2de899e0b <golang.org/x/net/html..stmp_38+0x23>
    2de899da2:	insl   (%dx),%es:(%rdi)
    2de899da3:	gs cmp $0x33323032,%eax
    2de899da9:	sub    $0x302d3830,%eax
-   2de899dae:	xor    $0x3a333054,%eax
-   2de899db3:	xor    (%rdx),%esi
-   2de899db5:	cmp    (%rbx),%dh
-   2de899db7:	cmp    %bl,0xa(%rdx)
-   2de899dba:	(bad)
+   2de899dae:	ss push %rsp
+   2de899db0:	xor    %dh,(%rcx)
+   2de899db2:	cmp    (%rax),%dh
+   2de899db4:	cmp    %bh,(%rdx)
+   2de899db6:	xor    %dh,(%rcx)
+   2de899db8:	pop    %rdx
+   2de899db9:	or     0x75(%rdx),%ah
    2de899dbc:	imul   $0x2e736376,0x9(%rsp,%riz,2),%ebp
    2de899dc4:	insl   (%dx),%es:(%rdi)
    2de899dc5:	outsl  %ds:(%rsi),(%dx)
    2de899dc6:	imul   $0x663d6465,%fs:0x69(%rsi),%esp
    2de899dce:	(bad)
    2de899dcf:	insb   (%dx),%es:(%rdi)
    2de899dd0:	jae    2de899e37 <golang.org/x/net/html..stmp_38+0x4f>
@@ -4194253,50 +4194295,8 @@
    2defa226e:	(bad)
    2defa226f:	(bad)
    2defa2270:	jmp    *(%rax)
    2defa2272:	and    %esp,-0x22(%rdi)
    2defa2275:	add    (%rax),%al
    2defa2277:	add    %al,(%rax)
    2defa2279:	jnp    2defa227f <.debug_loc+0x22227f>
-   2defa227b:	add    %al,(%rax)
-   2defa227d:	add    %al,(%rax)
-   2defa227f:	add    %al,(%rax)
-   2defa2281:	(bad)
-   2defa2282:	add    $0x0,%al
-   2defa2284:	add    %al,(%rax)
-   2defa2286:	add    %al,(%rax)
-   2defa2288:	add    %al,(%rcx)
-   2defa228a:	add    %bl,-0x49(%rdx)
-   2defa228d:	add    $0x0,%al
-   2defa228f:	add    %al,(%rax)
-   2defa2291:	add    %al,(%rax)
-   2defa2293:	add    %bh,0x4(%rdi)
-   2defa2299:	add    %al,(%rax)
-   2defa229b:	add    %al,(%rcx)
-   2defa229d:	add    %bl,0x0(%rdx)
-	...
-   2defa22ac:	add    %al,(%rax)
-   2defa22ae:	add    %bh,%bh
-   2defa22b0:	(bad)
-   2defa22b1:	(bad)
-   2defa22b2:	(bad)
-   2defa22b3:	(bad)
-   2defa22b4:	(bad)
-   2defa22b5:	(bad)
-   2defa22b6:	jmp    *(%rax)
-   2defa22b8:	and    %esp,-0x22(%rdi)
-   2defa22bb:	add    (%rax),%al
-   2defa22bd:	add    %al,(%rax)
-   2defa22bf:	movsl  %ds:(%rsi),%es:(%rdi)
-   2defa22c0:	add    $0x0,%al
-   2defa22c2:	add    %al,(%rax)
-   2defa22c4:	add    %al,(%rax)
-   2defa22c6:	add    %dh,0x4(%rdi)
-   2defa22cc:	add    %al,(%rax)
-   2defa22ce:	add    %al,(%rcx)
-   2defa22d0:	add    %bl,-0x49(%rbx)
-   2defa22d3:	add    $0x0,%al
-   2defa22d5:	add    %al,(%rax)
-   2defa22d7:	add    %al,(%rax)
-   2defa22d9:	add    %bh,0x4(%rdi)
-   2defa22df:	add    %al,(%rax)
-[ Too much input for diff (SHA256: 530265b12ab80a3c491dc043ecefdc026211f4d5f439c6130faed9d6cdb3854c) ]
+[ Too much input for diff (SHA256: 4ab522ead08a20b8932bd76e6f9ddc64ace099f9da9f286b6677ecb97c027a82) ]
```

## sqlite_html/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.2-alpha.8"
+__version__ = "0.1.3-alpha.1"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_html-0.1.2a8.dist-info/METADATA` & `sqlite_html-0.1.3a1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-html
-Version: 0.1.2a8
+Version: 0.1.3a1
 Home-page: https://github.com/asg017/sqlite-html
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-html/issues
 Project-URL: CI, https://github.com/asg017/sqlite-html/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-html/releases
 Requires-Python: >=3.7
```

