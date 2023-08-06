# Comparing `tmp/sqlite_vss-0.1.2a2-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip` & `tmp/sqlite_vss-0.1.2a3-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 1553958 bytes, number of entries: 9
--rwxr-xr-x  2.0 unx    15784 b- defN 23-Jul-24 21:14 noop.cpython-311-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      572 b- defN 23-Jul-24 21:14 sqlite_vss/__init__.py
--rw-r--r--  2.0 unx   187896 b- defN 23-Jul-24 21:14 sqlite_vss/vector0.so
--rw-r--r--  2.0 unx       79 b- defN 23-Jul-24 21:14 sqlite_vss/version.py
--rw-r--r--  2.0 unx  5135704 b- defN 23-Jul-24 21:14 sqlite_vss/vss0.so
--rw-r--r--  2.0 unx      496 b- defN 23-Jul-24 21:14 sqlite_vss-0.1.2a2.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 23-Jul-24 21:14 sqlite_vss-0.1.2a2.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jul-24 21:14 sqlite_vss-0.1.2a2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      724 b- defN 23-Jul-24 21:14 sqlite_vss-0.1.2a2.dist-info/RECORD
+-rwxr-xr-x  2.0 unx    15784 b- defN 23-Aug-06 02:15 noop.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      572 b- defN 23-Aug-06 02:15 sqlite_vss/__init__.py
+-rw-r--r--  2.0 unx   187896 b- defN 23-Aug-06 02:15 sqlite_vss/vector0.so
+-rw-r--r--  2.0 unx       79 b- defN 23-Aug-06 02:15 sqlite_vss/version.py
+-rw-r--r--  2.0 unx  5135704 b- defN 23-Aug-06 02:15 sqlite_vss/vss0.so
+-rw-r--r--  2.0 unx      496 b- defN 23-Aug-06 02:15 sqlite_vss-0.1.2a3.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 23-Aug-06 02:15 sqlite_vss-0.1.2a3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Aug-06 02:15 sqlite_vss-0.1.2a3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      724 b- defN 23-Aug-06 02:15 sqlite_vss-0.1.2a3.dist-info/RECORD
 9 files, 5341376 bytes uncompressed, 1552720 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: sqlite_vss/version.py
 Comment: 
 
 Filename: sqlite_vss/vss0.so
 Comment: 
 
-Filename: sqlite_vss-0.1.2a2.dist-info/METADATA
+Filename: sqlite_vss-0.1.2a3.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_vss-0.1.2a2.dist-info/WHEEL
+Filename: sqlite_vss-0.1.2a3.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_vss-0.1.2a2.dist-info/top_level.txt
+Filename: sqlite_vss-0.1.2a3.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_vss-0.1.2a2.dist-info/RECORD
+Filename: sqlite_vss-0.1.2a3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_vss/vector0.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 0ffcbb8f006c2500a82debae3de01f55f4b65341
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: aeaf3f32915386ffb494cab0f53afaf47943ea86
```

### strings --all --bytes=8 {}

```diff
@@ -331,15 +331,15 @@
 AWAVAUATUH
 []A\A]A^A_
 []A\A]A^A_
 AWAVAUATL
 []A\A]A^A_
 AVAUATUH
 []A\A]A^A_
-v0.1.2-alpha.2
+v0.1.2-alpha.3
 vector0_api_ptr
 Blob type not right
 vector_fvecs_each
 %d out of range: %s
 Value not a vector
 size: %lld [
 vector_version
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -1,10 +1,10 @@
 
 Hex dump of section '.rodata':
-  0x0001f000 76302e31 2e322d61 6c706861 2e320076 v0.1.2-alpha.2.v
+  0x0001f000 76302e31 2e322d61 6c706861 2e330076 v0.1.2-alpha.3.v
   0x0001f010 6563746f 72305f61 70695f70 74720042 ector0_api_ptr.B
   0x0001f020 6c6f6220 74797065 206e6f74 20726967 lob type not rig
   0x0001f030 68740076 6563746f 72300025 733a2025 ht.vector0.%s: %
   0x0001f040 73007665 63746f72 5f667665 63735f65 s.vector_fvecs_e
   0x0001f050 61636800 2564206f 7574206f 66207261 ach.%d out of ra
   0x0001f060 6e67653a 20257300 56616c75 65206e6f nge: %s.Value no
   0x0001f070 74206120 76656374 6f720073 697a653a t a vector.size:
```

## sqlite_vss/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.2-alpha.2"
+__version__ = "0.1.2-alpha.3"
 __version_info__ = tuple(__version__.split("."))
```

## sqlite_vss/vss0.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 56fcc6b1668cf0da7fa5c7101b42fd985913bcc5
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 358b1f93dc739facb7b66baeb01bbb00561f8db8
```

### strings --all --bytes=8 {}

```diff
@@ -7406,15 +7406,15 @@
 AWAVAUATUSH
 L$ H9L$8
 []A\A]A^A_
 AWAVAUATUSH
 []A\A]A^A_
 AWAVAUATI
 [A\A]A^A_]
-v0.1.2-alpha.2
+v0.1.2-alpha.3
 fullscan
 vss_search
 vss_range_search
 drop table "%w_index";
 drop table "%w_data";
 1st argument is not a vector
 vss0_rangesearchparams
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -1,10 +1,10 @@
 
 Hex dump of section '.rodata':
-  0x00382000 76302e31 2e322d61 6c706861 2e320066 v0.1.2-alpha.2.f
+  0x00382000 76302e31 2e322d61 6c706861 2e330066 v0.1.2-alpha.3.f
   0x00382010 756c6c73 63616e00 7673735f 73656172 ullscan.vss_sear
   0x00382020 63680076 73735f72 616e6765 5f736561 ch.vss_range_sea
   0x00382030 72636800 64726f70 20746162 6c652022 rch.drop table "
   0x00382040 25775f69 6e646578 223b0064 726f7020 %w_index";.drop 
   0x00382050 7461626c 65202225 775f6461 7461223b table "%w_data";
   0x00382060 00317374 20617267 756d656e 74206973 .1st argument is
   0x00382070 206e6f74 20612076 6563746f 72007673  not a vector.vs
```

## Comparing `sqlite_vss-0.1.2a2.dist-info/RECORD` & `sqlite_vss-0.1.2a3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 noop.cpython-311-x86_64-linux-gnu.so,sha256=0B-BA9FfREBugvBZIP1k-N0_MdSZEIJz-NPv0WPM5Ro,15784
 sqlite_vss/__init__.py,sha256=5PIhAIaJ1cVKtzSV9eZaymWS4CjRHUjkJ6y8VXyaG8Y,572
-sqlite_vss/vector0.so,sha256=1NzqwOniCiuFzlUZJM6N7YpHevtGpiYTnUB_el6JE4E,187896
-sqlite_vss/version.py,sha256=QtWzHtwser_tDr8xgVfTu8zKUY8Ber-BRSaYl66-oMs,79
-sqlite_vss/vss0.so,sha256=D0DflZ_KPV6PTsFO_J_sg3d2cdjGv49ga2DDjbJuerw,5135704
-sqlite_vss-0.1.2a2.dist-info/METADATA,sha256=SB3bnjJgGiUiiQRPudR64K3du_9XT0tX8wwmbNQ-QdM,496
-sqlite_vss-0.1.2a2.dist-info/WHEEL,sha256=bc9AIvLXnt_uk1DFAs9A9G48iq3HERrVzvuB4WpotO8,105
-sqlite_vss-0.1.2a2.dist-info/top_level.txt,sha256=Z2PPuSp9qvLljXNaO4Jwv8wSXtVhLIU2qBu5OEgZxGQ,16
-sqlite_vss-0.1.2a2.dist-info/RECORD,,
+sqlite_vss/vector0.so,sha256=V9wJ8LUXzQXNZRCadvJoJNFT3qIcA-o81XM3hYbqf68,187896
+sqlite_vss/version.py,sha256=aYFLTc4xifpUVIcK816d0Vo1HmRkuLxyzmu6XZ8FUG8,79
+sqlite_vss/vss0.so,sha256=rSf3DPID5byhv_gcQPKKD3KxaIwyq1bljPXv0B90jko,5135704
+sqlite_vss-0.1.2a3.dist-info/METADATA,sha256=E2e6bmebT1wtB8mgpZNtop-MiVltgrJ48Lg0CSZVf1Y,496
+sqlite_vss-0.1.2a3.dist-info/WHEEL,sha256=68SEJEGPnJA0YZmC4OXopTXD7FTwySrluDuL_hzv51w,105
+sqlite_vss-0.1.2a3.dist-info/top_level.txt,sha256=Z2PPuSp9qvLljXNaO4Jwv8wSXtVhLIU2qBu5OEgZxGQ,16
+sqlite_vss-0.1.2a3.dist-info/RECORD,,
```

