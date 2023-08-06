# Comparing `tmp/wangticketyes24-1.1-py3-none-any.whl.zip` & `tmp/wangticketyes24-1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 28276 bytes, number of entries: 12
--rw-r--r--  2.0 unx      114 b- defN 23-Jun-27 12:19 wangticketyes24/__init__.py
--rw-r--r--  2.0 unx    28280 b- defN 23-Jun-27 12:19 wangticketyes24/selenium_yes24.py
--rw-r--r--  2.0 unx    43080 b- defN 23-Jun-20 11:13 wangticketyes24/yes24.py
+Zip file size: 28354 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      114 b- defN 23-Aug-06 04:12 wangticketyes24/__init__.py
+-rw-r--r--  2.0 unx    28886 b- defN 23-Aug-06 04:12 wangticketyes24/selenium_yes24.py
+-rw-r--r--  2.0 unx    43119 b- defN 23-Aug-06 04:08 wangticketyes24/yes24.py
 -rw-r--r--  2.0 unx       94 b- defN 18-Dec-12 13:54 yes24ticket/__init__.py
 -rw-r--r--  2.0 unx     7490 b- defN 18-Dec-12 14:11 yes24ticket/selenium_yes24.py
 -rw-r--r--  2.0 unx    15460 b- defN 18-Dec-12 14:12 yes24ticket/yes24test.py
--rw-r--r--  2.0 unx       61 b- defN 23-Jun-27 12:20 wangticketyes24-1.1.dist-info/DESCRIPTION.rst
--rw-r--r--  2.0 unx      690 b- defN 23-Jun-27 12:20 wangticketyes24-1.1.dist-info/metadata.json
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-27 12:20 wangticketyes24-1.1.dist-info/top_level.txt
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 12:20 wangticketyes24-1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx      575 b- defN 23-Jun-27 12:20 wangticketyes24-1.1.dist-info/METADATA
--rw-r--r--  2.0 unx     1034 b- defN 23-Jun-27 12:20 wangticketyes24-1.1.dist-info/RECORD
-12 files, 96986 bytes uncompressed, 26542 bytes compressed:  72.6%
+-rw-r--r--  2.0 unx       61 b- defN 23-Aug-06 04:13 wangticketyes24-1.2.dist-info/DESCRIPTION.rst
+-rw-r--r--  2.0 unx      690 b- defN 23-Aug-06 04:13 wangticketyes24-1.2.dist-info/metadata.json
+-rw-r--r--  2.0 unx       16 b- defN 23-Aug-06 04:13 wangticketyes24-1.2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-06 04:13 wangticketyes24-1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx      575 b- defN 23-Aug-06 04:13 wangticketyes24-1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx     1034 b- defN 23-Aug-06 04:13 wangticketyes24-1.2.dist-info/RECORD
+12 files, 97631 bytes uncompressed, 26620 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: yes24ticket/selenium_yes24.py
 Comment: 
 
 Filename: yes24ticket/yes24test.py
 Comment: 
 
-Filename: wangticketyes24-1.1.dist-info/DESCRIPTION.rst
+Filename: wangticketyes24-1.2.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: wangticketyes24-1.1.dist-info/metadata.json
+Filename: wangticketyes24-1.2.dist-info/metadata.json
 Comment: 
 
-Filename: wangticketyes24-1.1.dist-info/top_level.txt
+Filename: wangticketyes24-1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: wangticketyes24-1.1.dist-info/WHEEL
+Filename: wangticketyes24-1.2.dist-info/WHEEL
 Comment: 
 
-Filename: wangticketyes24-1.1.dist-info/METADATA
+Filename: wangticketyes24-1.2.dist-info/METADATA
 Comment: 
 
-Filename: wangticketyes24-1.1.dist-info/RECORD
+Filename: wangticketyes24-1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wangticketyes24/__init__.py

```diff
@@ -1,5 +1,5 @@
 name = "wangticketyes24"
-__version__ = "1.1"
+__version__ = "1.2"
 
 from .yes24 import Yes24
 from .selenium_yes24 import Selenium_yes24
```

## wangticketyes24/selenium_yes24.py

```diff
@@ -481,35 +481,51 @@
 	def handleBookSuccess(self):
 		content = self.driver.find_elements_by_xpath("//div[@id='SuccessBoard']")
 
 		if len(content)>0 and content[0].is_displayed():
 			print("SuccessBoard is displayed")
 
 			while True:
-				#OLD:<strong id="bk_bookno" class="big">Y1532880152</strong>
-				#NEW:<strong id="bk_bookno" class="big">1532880152</strong>
-				bookno_xpath = "//strong[@id='bk_bookno']"
-				bookno_e = self.driver.find_element_by_xpath(bookno_xpath)
-				bookno = bookno_e.get_attribute('innerHTML')
-				if len(bookno) < 10:
-					print("bookno not displayed yet.. ", bookno)
-					time.sleep(1)
-					continue
+				try:
+					#OLD:<strong id="bk_bookno" class="big">Y1532880152</strong>
+					#NEW:<strong id="bk_bookno" class="big">1532880152</strong>
+					bookno_xpath = "//strong[@id='bk_bookno']"
+					bookno_e = self.driver.find_element_by_xpath(bookno_xpath)
+					bookno = bookno_e.get_attribute('innerHTML')
+					if len(bookno) < 10:
+						print("bookno not displayed yet.. ", bookno)
+						time.sleep(1)
+						continue
+
+					if not bookno.isdigit():
+						bookno = bookno[1:]
+					break
+				except UnexpectedAlertPresentException as e:
+					print(traceback.format_exc())
+					# alert text check
+					# 주문이 완료되었습니다.
+					# 이용해 주셔서 감사합니다.
 
-				if not bookno.isdigit():
-					bookno = bookno[1:]
+					alert = self.driver.switch_to.alert
+					alertText = alert.text
 
-				break
+					msg = "[{}] alert:{} (seat:{})".format(self.userid, alertText, self.trying_seat)
+					print(msg)
+					self.notifyTelegram(message=msg)
+					bookno = ""
+					tkseat = self.trying_seat
+					break
 
-			tkseat_xpath = "//div[@id='bk_tkseat']"
-			tkseat_e = self.driver.find_element_by_xpath(tkseat_xpath)
-			tkseat = tkseat_e.get_attribute('innerText')
-			self.bookno = bookno
-			self.tkseat = tkseat
-			#print("seat:", tkseat)
+			if bookno != "":
+				tkseat_xpath = "//div[@id='bk_tkseat']"
+				tkseat_e = self.driver.find_element_by_xpath(tkseat_xpath)
+				tkseat = tkseat_e.get_attribute('innerText')
+				self.bookno = bookno
+				self.tkseat = tkseat
+				#print("seat:", tkseat)
 			print("[{}][{}] {}".format(self.userid, bookno, tkseat))
 
 			# register bookingno
 			playdatetime = '{}_{}'.format(self.playdate, self.playtime)
 			URL = "http://wangticket.com/yes24/new_booking.php?yes24id={}&pcid={}&bookingno={}&datetime={}&seats={}".format(self.userid, self.pcid, bookno, playdatetime, tkseat)
 			headers = {"User-Agent":"Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.102 Safari/537.36"}
 			r = requests.get(URL, headers=headers)
@@ -557,15 +573,16 @@
 		print(msg)
 		self.notifyTelegram(message=msg)
 
 	def payHyundaiCard(self):
 		iframe = self.driver.find_element_by_id("iframe")
 		self.driver.switch_to.frame(iframe)
 
-		e = retry_find_element_by_xpath(self.driver, "//a[@id='cardCode22']")
+		#e = retry_find_element_by_xpath(self.driver, "//a[@id='cardCode10']")
+		e = retry_find_element_by_xpath(self.driver, "//a[contains(@title,'현대카드')]")
 		self.driver.execute_script("arguments[0].click();", e)
 
 		# OFF POPUP
 		self.driver.execute_script("overlayPopupOnOff2(false);")
 
 		# if agr_utilzr exist, inputAll exist
 		es = self.driver.find_elements_by_xpath("//div[contains(@class,'agr_utilzr')]")
@@ -621,15 +638,15 @@
 			totalprice = payprice + giftuse
 			print("totalprice:", totalprice)
 			print("giftuse:", giftuse)
 			if giftuse > 0 and totalprice != giftuse:
 				print("totalprice and giftuse is different! need to change")
 				self.fixGiftAmount(money=totalprice)
 
-			trying_seat = self.driver.execute_script("return document.getElementById('tk_seat').innerText;")
+			self.trying_seat = self.driver.execute_script("return document.getElementById('tk_seat').innerText;")
 
 			## checkout button
 			e = self.driver.find_element_by_xpath("//img[@id='imgPayEnd']")
 			self.driver.execute_script("arguments[0].click();", e)
 
 			self.driver.implicitly_wait(1)
 
@@ -703,15 +720,15 @@
 					alertText = alert.text
 
 					if '자동주문방지 문자를 잘못 입력하셨습니다' in alertText:
 						alert.accept()
 						print("alert accepted")
 						break
 					else:
-						msg = "[{}] alert:{} (seat:{})".format(self.userid, alertText, trying_seat)
+						msg = "[{}] alert:{} (seat:{})".format(self.userid, alertText, self.trying_seat)
 						print(msg)
 						self.notifyTelegram(message=msg)
 						time.sleep(10)
 
 				except WebDriverException as e:
 					print(traceback.format_exc())
 					print("This error temporarily happens in Windows..")
```

## wangticketyes24/yes24.py

```diff
@@ -810,14 +810,17 @@
 			self.myOrderList()
 			return True
 		else:
 			print("Finding another seat!!!!!!!!")
 			return False
 
 	def myOrderList(self):
+		if self.sel.bookno == "":
+			return
+
 		for i in range(0,100):
 			try:
 				isfound = self.myOrderList_ex()
 				if isfound:
 					break
 				time.sleep(1)
 				continue
```

## Comparing `wangticketyes24-1.1.dist-info/metadata.json` & `wangticketyes24-1.2.dist-info/metadata.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'1.2'"}*

```diff
@@ -33,9 +33,9 @@
                 "beautifulsoup4",
                 "requests",
                 "selenium"
             ]
         }
     ],
     "summary": "wangticket for y",
-    "version": "1.1"
+    "version": "1.2"
 }
```

## Comparing `wangticketyes24-1.1.dist-info/METADATA` & `wangticketyes24-1.2.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: wangticketyes24
-Version: 1.1
+Version: 1.2
 Summary: wangticket for y
 Home-page: https://gitlab.com/wangticket/yes24-ticket
 Author: Wangticket
 Author-email: wangticket77@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `wangticketyes24-1.1.dist-info/RECORD` & `wangticketyes24-1.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-wangticketyes24/__init__.py,sha256=YZQUcg13IKwXC967Qex1luYqg5sTy7nUXzOla43EpKo,114
-wangticketyes24/selenium_yes24.py,sha256=35zOyqWwbwMV4grxUnene8qJ48VGSlQkS642wW-Kyfg,28280
-wangticketyes24/yes24.py,sha256=iCopqbnuryIMeVs0ygUNEl7vXh2xh6onFLBKlDwT2i0,43080
-wangticketyes24-1.1.dist-info/DESCRIPTION.rst,sha256=iA1-u5zGsM2eQRcqv1-vqBiJevH0U-KhtkZxpjzmfx4,61
-wangticketyes24-1.1.dist-info/METADATA,sha256=ZnvukDyGyhypiBuMCNDyfzm7DTeFC0XbqMjdsDud0kc,575
-wangticketyes24-1.1.dist-info/RECORD,,
-wangticketyes24-1.1.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
-wangticketyes24-1.1.dist-info/metadata.json,sha256=K_EpQGM13BNvieB5nJtz84Ee1TWh53yDGeIOEvDK4R8,690
-wangticketyes24-1.1.dist-info/top_level.txt,sha256=gHGxU_Wfy3Ly7zkKLxm67DoXktNcwN0ImDzlhzNaiW4,16
+wangticketyes24/__init__.py,sha256=7Ecq9qr_TkOarzadELi4kaE_vGV-Yhc3nhQMLtnpbP8,114
+wangticketyes24/selenium_yes24.py,sha256=TXMfy5gNQbloZcF-7HZnBmS6b4PhhbjHiD-278BLcgU,28886
+wangticketyes24/yes24.py,sha256=AM_6AzV6OspRG8CYt5JV3oQa1caFSzdR0M1XL5FGPeM,43119
+wangticketyes24-1.2.dist-info/DESCRIPTION.rst,sha256=iA1-u5zGsM2eQRcqv1-vqBiJevH0U-KhtkZxpjzmfx4,61
+wangticketyes24-1.2.dist-info/METADATA,sha256=5cDIoT7Iz0OIxKqJVD1eYbzuIhRywIF_YlNfahEOuFg,575
+wangticketyes24-1.2.dist-info/RECORD,,
+wangticketyes24-1.2.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
+wangticketyes24-1.2.dist-info/metadata.json,sha256=IL6gkwIVJ3UqKMUvGiLZcSbRBBvd05_Q2Gbbc15QZb0,690
+wangticketyes24-1.2.dist-info/top_level.txt,sha256=gHGxU_Wfy3Ly7zkKLxm67DoXktNcwN0ImDzlhzNaiW4,16
 yes24ticket/__init__.py,sha256=amffzfln3WNiLWWyUul39xXObS4TmQRza8OBgfN24M8,94
 yes24ticket/selenium_yes24.py,sha256=z6ataHl-e3AVhQTZFSYPdn1OfSOklBTizd2mLA57DAM,7490
 yes24ticket/yes24test.py,sha256=6my-oQh4NITv3IkaT_W_v61Z5iPDqNmDU6b3Qx9N5l8,15460
```

