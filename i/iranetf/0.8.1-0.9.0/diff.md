# Comparing `tmp/iranetf-0.8.1.tar.gz` & `tmp/iranetf-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iranetf-0.8.1.tar", last modified: Thu Apr 13 06:22:29 2023, max compression
+gzip compressed data, was "iranetf-0.9.0.tar", last modified: Thu Apr 13 11:22:22 2023, max compression
```

## Comparing `iranetf-0.8.1.tar` & `iranetf-0.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 06:22:29.244557 iranetf-0.8.1/
--rw-rw-rw-   0        0        0    35149 2021-12-03 06:39:06.000000 iranetf-0.8.1/LICENSE
--rw-rw-rw-   0        0        0       44 2022-08-14 15:03:12.000000 iranetf-0.8.1/MANIFEST.in
--rw-rw-rw-   0        0        0      725 2023-04-13 06:22:29.244557 iranetf-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0      152 2023-01-13 07:19:37.000000 iranetf-0.8.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-13 06:22:29.228936 iranetf-0.8.1/iranetf/
--rw-rw-rw-   0        0        0      860 2023-04-13 06:22:26.000000 iranetf-0.8.1/iranetf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:22:29.244557 iranetf-0.8.1/iranetf/sites/
--rw-rw-rw-   0        0        0    10775 2023-04-13 05:38:47.000000 iranetf-0.8.1/iranetf/sites/__init__.py
--rw-rw-rw-   0        0        0    10967 2023-04-13 05:45:10.000000 iranetf-0.8.1/iranetf/sites/dataset.csv
-drwxrwxrwx   0        0        0        0 2023-04-13 06:22:29.244557 iranetf-0.8.1/iranetf.egg-info/
--rw-rw-rw-   0        0        0      725 2023-04-13 06:22:29.000000 iranetf-0.8.1/iranetf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-04-13 06:22:29.000000 iranetf-0.8.1/iranetf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 06:22:29.000000 iranetf-0.8.1/iranetf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-08-14 14:54:43.000000 iranetf-0.8.1/iranetf.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       70 2023-04-13 06:22:29.000000 iranetf-0.8.1/iranetf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 06:22:29.000000 iranetf-0.8.1/iranetf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1068 2023-04-13 06:06:07.000000 iranetf-0.8.1/pyproject.toml
--rw-rw-rw-   0        0        0       67 2023-04-13 06:04:35.000000 iranetf-0.8.1/pytest.ini
--rw-rw-rw-   0        0        0       42 2023-04-13 06:22:29.244557 iranetf-0.8.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 11:22:22.085372 iranetf-0.9.0/
+-rw-rw-rw-   0        0        0    35149 2021-12-03 06:39:06.000000 iranetf-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0       44 2022-08-14 15:03:12.000000 iranetf-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      725 2023-04-13 11:22:22.085372 iranetf-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0      152 2023-01-13 07:19:37.000000 iranetf-0.9.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-13 11:22:22.069749 iranetf-0.9.0/iranetf/
+-rw-rw-rw-   0        0        0      882 2023-04-13 11:22:19.000000 iranetf-0.9.0/iranetf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:22:22.085372 iranetf-0.9.0/iranetf/sites/
+-rw-rw-rw-   0        0        0    12068 2023-04-13 11:20:53.000000 iranetf-0.9.0/iranetf/sites/__init__.py
+-rw-rw-rw-   0        0        0    11880 2023-04-13 11:01:05.000000 iranetf-0.9.0/iranetf/sites/dataset.csv
+drwxrwxrwx   0        0        0        0 2023-04-13 11:22:22.085372 iranetf-0.9.0/iranetf.egg-info/
+-rw-rw-rw-   0        0        0      725 2023-04-13 11:22:21.000000 iranetf-0.9.0/iranetf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-04-13 11:22:21.000000 iranetf-0.9.0/iranetf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 11:22:21.000000 iranetf-0.9.0/iranetf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-08-14 14:54:43.000000 iranetf-0.9.0/iranetf.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       70 2023-04-13 11:22:21.000000 iranetf-0.9.0/iranetf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 11:22:21.000000 iranetf-0.9.0/iranetf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1068 2023-04-13 06:06:07.000000 iranetf-0.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0       67 2023-04-13 06:04:35.000000 iranetf-0.9.0/pytest.ini
+-rw-rw-rw-   0        0        0       42 2023-04-13 11:22:22.085372 iranetf-0.9.0/setup.cfg
```

### Comparing `iranetf-0.8.1/LICENSE` & `iranetf-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iranetf-0.8.1/PKG-INFO` & `iranetf-0.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iranetf
-Version: 0.8.1
+Version: 0.9.0
 Summary: a library to fetch data from iranetf.org
 Author-email: 5j9 <5j9@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/5j9/fipiran
 Project-URL: Bug Tracker, https://github.com/5j9/fipiran/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `iranetf-0.8.1/iranetf/__init__.py` & `iranetf-0.9.0/iranetf/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.8.1'
+__version__ = '0.9.0'
 
 from datetime import datetime as _datetime
 
 from aiohttp import (
     ClientResponse as _ClientResponse,
     ClientSession as _ClientSession,
     ClientTimeout as _ClientTimeout,
@@ -19,16 +19,19 @@
         if 'timeout' not in kwargs:
             kwargs['timeout'] = _ClientTimeout(
                 total=60., sock_connect=10., sock_read=10.)
         SESSION = _ClientSession(**kwargs)
         return SESSION
 
 
+SSL = None
+
+
 async def _get(url: str) -> _ClientResponse:
-    return await SESSION.get(url)
+    return await SESSION.get(url, ssl=SSL)
 
 
 async def _read(url: str) -> bytes:
     return await (await _get(url)).read()
 
 
 def _j2g(s: str) -> _datetime:
```

### Comparing `iranetf-0.8.1/iranetf/sites/__init__.py` & `iranetf-0.9.0/iranetf/sites/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 from abc import ABC as _ABC, abstractmethod as _abstractmethod
 from asyncio import gather as _gather
 from json import JSONDecodeError as _JSONDecodeError, loads as _loads
-from logging import warning
+from logging import error as _error, warning as _warning
 from pathlib import Path as _Path
 from typing import TypedDict as _TypedDict
 
 from aiohttp import (
     ClientConnectorError as _ClientConnectorError,
     ClientOSError as _ClientOSError,
     ServerTimeoutError as _ServerTimeoutError,
+    TooManyRedirects as _TooManyRedirects,
 )
 from pandas import (
     DataFrame as _DataFrame,
     Series as _Series,
     concat as _concat,
     read_csv as _read_csv,
     to_datetime as _to_datetime,
 )
 
+import iranetf
 from iranetf import _datetime, _get, _j2g, _jdatetime
 
+_ETF_TYPES = {  # numbers are according to fipiran
+    6: 'Stock', 4: 'Fixed', 7: 'Mixed',
+    5: 'Commodity', 17: 'FOF', 18: 'REIT',
+}
 
 class _LiveNAV(_TypedDict, total=True):
     issue: int
     cancel: int
     date: _datetime
 
 
@@ -214,30 +220,45 @@
     )
     if site:
         df['site'] = df[df.site_type.notna()].apply(_make_site, axis=1)
         df.drop(columns=['url', 'site_type'], inplace=True)
     return df
 
 
+async def _check_validity(site: BaseSite) -> tuple[str, str] | None:
+    try:
+        await site.live_navps()
+    except (
+        _JSONDecodeError,
+        _ClientConnectorError,
+        _ServerTimeoutError,
+        _ClientOSError,
+        _TooManyRedirects,
+    ):
+        return None
+    last_url = site.last_response.url  # to avoid redirected URLs
+    return f'{last_url.scheme}://{last_url.host}/', type(site).__name__
+
+
+SITE_TYPES = (RayanHamafza, TadbirPardaz, MabnaDP, LeveragedTadbirPardaz)
+
+
 async def _url_type(domain: str) -> tuple:
-    for protocol in ('https', 'http'):
-        for SiteType in (RayanHamafza, TadbirPardaz):
-            url = f'{protocol}://{domain}/'
-            site = SiteType(url)
-            try:
-                await site.live_navps()
-            except (
-                _JSONDecodeError,
-                _ClientConnectorError,
-                _ServerTimeoutError,
-                _ClientOSError,
-            ):
-                continue
-            last_url = site.last_response.url  # to avoid redirected URLs
-            return f'{last_url.scheme}://{last_url.host}/', SiteType.__name__
+    coros = [
+        _check_validity(SiteType(f'{protocol}://{domain}/'))
+        for protocol in ('https', 'http')
+        for SiteType in SITE_TYPES
+    ]
+
+    results = await _gather(*coros)
+
+    for result in results:
+        if result is not None:
+            return result
+
     return None, None
 
 
 async def _url_type_columns(domains):
     list_of_tuples = await _gather(*[_url_type(d) for d in domains])
     return zip(*list_of_tuples)
 
@@ -256,15 +277,15 @@
 async def _fipiran_data(ds):
     import fipiran.funds
     async with fipiran.Session():
         fipiran_df = await fipiran.funds.funds()
 
     dataset_ids_not_on_fipiran = ds[~ds.fipiran_id.isin(fipiran_df.regNo)]
     if not dataset_ids_not_on_fipiran.empty:
-        warning('some dataset rows were not found on fipiran')
+        _warning('some dataset rows were not found on fipiran')
 
     df = fipiran_df[
         (fipiran_df['typeOfInvest'] == 'Negotiable')
         # 11: 'Market Maker', 12: 'VC', 13: 'Project', 14: 'Land and building',
         # 16: 'PE'
         & ~(fipiran_df['fundType'].isin((11, 12, 13, 14, 16)))
         & fipiran_df['isCompleted']
@@ -276,20 +297,15 @@
         columns={
             'regNo': 'fipiran_id',
             'fundType': 'type',
             'websiteAddress': 'domain',
         }, copy=False, inplace=True, errors='raise'
     )
 
-    df.type.replace(
-        {
-            6: 'Stock', 4: 'Fixed', 7: 'Mixed',
-            5: 'Commodity', 17: 'FOF'
-        }, inplace=True
-    )
+    df.type.replace(_ETF_TYPES, inplace=True)
 
     return df
 
 
 async def _tsetmc_dataset() -> _DataFrame:
     import tsetmc.dataset
 
@@ -322,23 +338,59 @@
 
     new_fipiran_df = fipiran_df[~fipiran_ids_existing_in_ds].copy()
 
     new_fipiran_df['tsetmc_id'] = await _inscodes(new_fipiran_df.name)
 
     new_with_tsetmcid = new_fipiran_df[new_fipiran_df.tsetmc_id.notna()]
 
-    tsetmc_df = await _tsetmc_dataset()
-    new_with_tsetmcid = new_with_tsetmcid.merge(
-        tsetmc_df, 'left', on='tsetmc_id'
-    )
+    if not new_with_tsetmcid.empty:
+        tsetmc_df = await _tsetmc_dataset()
+        new_with_tsetmcid = new_with_tsetmcid.merge(
+            tsetmc_df, 'left', on='tsetmc_id'
+        )
+
+        ds = _concat([ds, new_with_tsetmcid]).sort_values('symbol')
 
-    new_dataset = _concat([ds, new_with_tsetmcid]).sort_values('symbol')
-    new_dataset[[  # resort columns (order was changed by the ds.reset_index)
+    ds[[  # resort columns (order was changed by the ds.reset_index)
         'symbol', 'name', 'type', 'tsetmc_id', 'fipiran_id', 'url', 'site_type'
     ]].to_csv(
         _DATASET_PATH,
         lineterminator='\n',
         encoding='utf-8-sig',
         index=False
     )
 
-    return new_fipiran_df[new_fipiran_df.tsetmc_id.notna()]
+    return new_fipiran_df[new_fipiran_df.tsetmc_id.isna()]
+
+
+async def _check_live_site(site: BaseSite):
+    if site != site:  # na
+        return
+
+    try:
+        navps = await site.live_navps()
+    except Exception as e:
+        _error(f'exception during checking of {site}: {e}')
+    else:
+        assert type(navps['issue']) is int
+
+
+async def check_dataset(live=False):
+    ds = load_dataset(site=False)
+    assert ds.symbol.is_unique
+    assert ds.name.is_unique
+    assert ds.type.unique().isin(_ETF_TYPES.values()).all()
+    assert ds.tsetmc_id.is_unique
+    assert ds.fipiran_id.is_unique
+
+    if not live:
+        return
+
+    ds['site'] = ds[ds.site_type.notna()].apply(_make_site, axis=1)
+    iranetf.SSL = False  # many sites fail ssl verification
+    coros = ds.site.apply(_check_live_site)
+    await _gather(*coros)
+
+    if not (no_site := ds[ds.site.isna()]).empty:
+        _warning(
+            f'some dataset entries have no associated site:\n{no_site.symbol}'
+        )
```

### Comparing `iranetf-0.8.1/iranetf/sites/dataset.csv` & `iranetf-0.9.0/iranetf/sites/dataset.csv`

 * *Files 4% similar despite different names*

```diff
@@ -2,100 +2,107 @@
 آتیمس,آرمان آتیه درخشان مس,Stock,22839330962768817,11378,http://armanmesetf.ir/,RayanHamafza
 آرام,شاخصی آرام مفید,Stock,14230681955555738,11939,https://arametf.com/,TadbirPardaz
 آساس,آسمان آرمانی سهام,Stock,66682662312253625,11195,https://asasfund.ir/,TadbirPardaz
 آسام,آرمان سپهر آشنا,Mixed,36592972482259020,11172,https://asaetf.ir/,TadbirPardaz
 آسامید,مشترک آسمان امید,Fixed,24869832924911721,11626,https://asamidfund.ir/,TadbirPardaz
 آفاق,نوع دوم افق آتی,Fixed,37073830945037165,11976,https://ofoghati.ir/,TadbirPardaz
 آوا,آوای معیار,Stock,18007109712724189,11729,http://avayemeyar.ir/,RayanHamafza
-آکورد,آرمان آتی کوثر,Fixed,30282299500988269,11409,http://aaketf.com/,RayanHamafza
+آکورد,آرمان آتی کوثر,Fixed,30282299500988269,11409,https://aaketf.com/,RayanHamafza
 آگاس,هستی بخش آگاه,Stock,33887145736684266,11341,https://hbagahfund.com/,RayanHamafza
-ارزش,ارزش آفرین بیدار,Stock,43443105991896600,11712,http://arzesh.ebb.ir/,RayanHamafza
-ارمغان,ارمغان ایرانیان,Fixed,31366347648583654,10920,http://armaghanfund.ir/,RayanHamafza
+ارزش,ارزش آفرین بیدار,Stock,43443105991896600,11712,https://arzesh.ebb.ir/,RayanHamafza
+ارزش مسکن,املاک و مستغلات مدیریت ارزش مسکن,REIT,71945594172117613,12027,https://reit1.cvpf.ir/,TadbirPardaz
+ارمغان,ارمغان ایرانیان,Fixed,31366347648583654,10920,https://armaghanfund.ir/,RayanHamafza
 اطلس,توسعه اطلس مفید,Stock,11427939669935844,11215,https://atlasetf.com/,TadbirPardaz
-اعتبار,نوع دوم اعتبار,Fixed,35163287528816137,12031,http://etebaretf2.com/,RayanHamafza
+اعتبار,نوع دوم اعتبار,Fixed,35163287528816137,12031,https://etebaretf2.com/,RayanHamafza
 اعتماد,اعتماد آفرین پارسیان,Fixed,66818022341772870,11315,http://eap-fund.com/,RayanHamafza
 افران,افرا نماد پایدار,Fixed,3846143218462419,11692,https://afra.fund/,RayanHamafza
 افق ملت,افق ملت,Stock,15451317146134956,11233,https://ofoghmellat.ir/,TadbirPardaz
-الماس,امین تدبیرگران فردا,Stock,28788598290160782,11260,http://fardaetf.tadbirfunds.ir/,RayanHamafza
+الماس,امین تدبیرگران فردا,Stock,28788598290160782,11260,https://fardaetf.tadbirfunds.ir/,RayanHamafza
 امین یکم,امین یکم فردا,Fixed,45728383369147894,11460,http://aminfarda.ir/,TadbirPardaz
 انار,انار نماد ارزش,Stock,30215634246748564,11900,https://anar.fund/,RayanHamafza
-اهرم,سهامی اهرمی کاریزما,Stock,17914401175772326,11912,http://ahrom.charisma.ir/,LeveragedTadbirPardaz
-اوج,اوج دماوند,Stock,62575434414985179,11886,http://oujdamavandfund.ir/,RayanHamafza
+اهرم,سهامی اهرمی کاریزما,Stock,17914401175772326,11912,https://ahrom.charisma.ir/,LeveragedTadbirPardaz
+اوج,اوج دماوند,Stock,62575434414985179,11886,https://oujdamavandfund.ir/,RayanHamafza
 اوصتا,اندیشه ورزان صبا تامین,Fixed,57761388729898548,11588,https://sast.sabaamc.ir/,RayanHamafza
-اکسیژن,سهامی اکسیژن,Stock,50094941173290382,12035,http://oxygen.o2am.ir/,
+اکسیژن,سهامی اکسیژن,Stock,50094941173290382,12035,https://oxygen.o2am.ir/,RayanHamafza
+برلیان,در سهام برلیان,Stock,4216536645718658,11985,https://berelianfund.ir/,RayanHamafza
+دیبا,بازده پایه بازار صبا,Fixed,70698996132397388,12045,https://payeh.sabaamc.ir/,RayanHamafza
 بذر,بذر امید آفرین,Stock,37222720235819361,11197,http://bazreomidfund.ir/,RayanHamafza
-تاراز,آوای تاراز زاگرس,Stock,24651394045981418,11922,http://tarazfund.ir/,RayanHamafza
+تاراز,آوای تاراز زاگرس,Stock,24651394045981418,11922,https://tarazfund.ir/,RayanHamafza
+ترمه,ترمه ایساتیس پویا,Stock,42705920381780437,12018,https://termeh.isatispm.com/,RayanHamafza
 تصمیم,در اوراق بهادار با درآمد ثابت تصمیم,Fixed,53419976284977130,11569,http://tasmim-sabet.ir/,RayanHamafza
 تمشک,تمشک نماد رشد,FOF,53145304508578701,12057,https://tameshk.fund/,RayanHamafza
 توان,سهامی اهرمی مفید,Stock,41927452991671109,12033,https://tavanfund.com/,LeveragedTadbirPardaz
-ثبات,ثبات ویستا,Fixed,26780282166315918,11874,http://sobatvista.ir/,RayanHamafza
-ثروتم,ثروت آفرین پارسیان,Stock,71672399601682259,11327,http://sap-fund.com/,RayanHamafza
-ثمین,ثروت افزون ثمین,Stock,66721204145017523,11889,http://saminfund.ir/,RayanHamafza
-ثنا,زرین نهال ثنا,Stock,32112121249636248,12023,https://zarinnahal.sanaamc.com/,
+ثبات,ثبات ویستا,Fixed,26780282166315918,11874,https://sobatvista.ir/,RayanHamafza
+ثروتم,ثروت آفرین پارسیان,Stock,71672399601682259,11327,https://sap-fund.com/,RayanHamafza
+ثمین,ثروت افزون ثمین,Stock,66721204145017523,11889,https://saminfund.ir/,RayanHamafza
+ثنا,زرین نهال ثنا,Stock,32112121249636248,12023,https://zarinnahal.sanaamc.com/,MabnaDP
 ثهام,ثروت هامرز,Stock,38713440086361985,11823,https://servat.hummers.ir/,TadbirPardaz
-خاتم,خاتم ایساتیس پویا,Fixed,18865325633315847,11753,http://etf.isatispm.com/,RayanHamafza
-دارا,دارا الگوریتم,Fixed,62012736978844991,11660,http://darafund.ir/,RayanHamafza
-دارا یکم,واسطه گری مالی یکم,Stock,62235397452612911,11709,http://fi1fund.com/,RayanHamafza
+خاتم,خاتم ایساتیس پویا,Fixed,18865325633315847,11753,https://etf.isatispm.com/,RayanHamafza
+دارا,دارا الگوریتم,Fixed,62012736978844991,11660,https://darafund.ir/,RayanHamafza
+دارا یکم,واسطه گری مالی یکم,Stock,62235397452612911,11709,https://fi1fund.com/,RayanHamafza
 داریوش,ثروت داریوش,Stock,58789178087946067,11878,http://servat.dariush.fund/,RayanHamafza
 داریک,اعتماد داریک,Fixed,71076372178147339,11725,http://etemaddarik.ir/,RayanHamafza
-درسا,قابل معامله سهامی درسا,Stock,34581754264880199,11962,http://dorsaetf.com/,RayanHamafza
+درسا,قابل معامله سهامی درسا,Stock,34581754264880199,11962,https://dorsaetf.com/,RayanHamafza
 دریا,دریای آبی فیروزه,Stock,11285885633824855,12039,https://daryaetf.ir/,TadbirPardaz
-درین,درین بها بازار,Fixed,21077182490095731,12086,http://dorinfund.com/,RayanHamafza
+درین,درین بها بازار,Fixed,21077182490095731,12086,https://dorinfund.com/,RayanHamafza
 رابین,توسعه افق رابین,Fixed,33527290777160784,12052,http://rabinetf.ir/,RayanHamafza
-رایکا,نوع دوم رایکا,Fixed,66105959479616770,12024,http://raykaetf.com/,RayanHamafza
+رایکا,نوع دوم رایکا,Fixed,66105959479616770,12024,https://raykaetf.com/,RayanHamafza
 رشد,رشد پایدار آبان,Fixed,48287767791629523,11667,https://rpfund.ir/,TadbirPardaz
-رماس,راهبرد ممتاز ابن سینا,Stock,22002589755112021,11803,http://emacofund.ir/,RayanHamafza
-زر,پشتوانه سکه طلای زرافشان امید ایرانیان,Commodity,33254899395816171,11530,http://omidgoldfund.ir/,RayanHamafza
+رماس,راهبرد ممتاز ابن سینا,Stock,22002589755112021,11803,https://emacofund.ir/,RayanHamafza
+زر,پشتوانه سکه طلای زرافشان امید ایرانیان,Commodity,33254899395816171,11530,https://omidgoldfund.ir/,RayanHamafza
 زرفام,زرفام آشنا,Commodity,33144542989832366,11967,https://goldfund.ir/,RayanHamafza
-زرین,زرین کوروش,Stock,50139638026536387,11774,http://zarinfunds.com/,RayanHamafza
+زرین,زرین کوروش,Stock,50139638026536387,11774,https://zarinfunds.com/,RayanHamafza
 زیتون,زیتون نماد پایا,Mixed,28551661889797217,11888,https://zeytoon.fund/,RayanHamafza
+ساحل,مختص اوراق دولتی خلیج فارس,Fixed,62708526880913292,11990,https://sahel.pgibc.ir/,RayanHamafza
 سحرخیز,گروه زعفران سحرخیز,Commodity,51200575796028449,11780,http://saharkhizfund.com/,RayanHamafza
-سخند,سپهر خبرگان نفت,Fixed,59598536122397373,11340,http://khobregan-etf.com/,RayanHamafza
+سخند,سپهر خبرگان نفت,Fixed,59598536122397373,11340,https://khobregan-etf.com/,RayanHamafza
 سرو,سرو سودمند مدبران,Stock,64942549055019553,11649,https://sarv.fund/,RayanHamafza
 سلام,سلام فارابی,Stock,70541934393301867,11951,https://salam.irfarabi.ir/,TadbirPardaz
 سپاس,پاداش سهامداری توسعه یکم,Fixed,39453972158399542,11367,https://sepasetf.ir/,TadbirPardaz
-سپر,سپر سرمایه بیدار,Fixed,17226661368470120,11722,http://separ.ebb.ir/,RayanHamafza
-سپیدما,سپید دماوند,Fixed,2161110547458064,11820,http://sepiddamavandfund.ir/,RayanHamafza
+سپر,سپر سرمایه بیدار,Fixed,17226661368470120,11722,https://separ.ebb.ir/,RayanHamafza
+سپیدما,سپید دماوند,Fixed,2161110547458064,11820,https://sepiddamavandfund.ir/,RayanHamafza
 سیناد,سپهر سودمند سینا,Fixed,31913287805282551,11841,https://sinaetf.ir/,TadbirPardaz
-صایند,گنجینه آینده روشن,Fixed,45205530868811305,11323,http://ayandehfund.com/,RayanHamafza
-صنم,صندوق در صندوق صنم,FOF,47125023640770480,11927,http://sanam.charisma.ir/,RayanHamafza
-صنوین,سپهر اندیشه نوین,Mixed,68203878405672734,11196,http://sepehrnovin.ir/,RayanHamafza
-طلا,پشتوانه طلای لوتوس,Commodity,46700660505281786,11509,http://lotusgoldfund.capital/,RayanHamafza
+صایند,گنجینه آینده روشن,Fixed,45205530868811305,11323,https://ayandehfund.com/,RayanHamafza
+صنم,صندوق در صندوق صنم,FOF,47125023640770480,11927,https://sanam.charisma.ir/,RayanHamafza
+صنوین,سپهر اندیشه نوین,Mixed,68203878405672734,11196,https://sepehrnovin.ir/,RayanHamafza
+طلا,پشتوانه طلای لوتوس,Commodity,46700660505281786,11509,https://lotusgoldfund.capital/,RayanHamafza
 عیار,طلای عیار مفید,Commodity,34144395039913458,11586,https://ayaretf.com/,TadbirPardaz
-فراز,فراز داریک,Stock,13666407494621646,11773,http://farazdarik.ir/,RayanHamafza
+فراز,فراز داریک,Stock,13666407494621646,11773,https://farazdarik.ir/,RayanHamafza
 فردا,آوای فردای زاگرس,Fixed,65249046611427924,11776,https://afzfund.ir/,TadbirPardaz
 فیروزا,ارمغان فیروزه آسیا,Fixed,10795723506538053,11518,https://firouzehfixetf.com/,TadbirPardaz
 فیروزه,شاخص سی شرکت بزرگ فیروزه,Stock,66036975502302203,11308,https://iranetf.ir/,TadbirPardaz
 لبخند,لبخند فارابی,Fixed,31569200988534548,12002,https://labkhand.irfarabi.ir/,TadbirPardaz
 مانی,ثابت مانی,Fixed,61265100181977543,11859,https://manifunds.ir/,TadbirPardaz
-مثقال,در اوراق بهادار مبتنی بر طلای زرین آگاه,Commodity,32469128621155736,11899,http://zarinagahfund.com/,RayanHamafza
+مثقال,در اوراق بهادار مبتنی بر طلای زرین آگاه,Commodity,32469128621155736,11899,https://zarinagahfund.com/,RayanHamafza
 مدیر,مدیریت ثروت صندوق بازنشستگی کشوری,Stock,65576885779918210,11736,https://modirfund.ir/,TadbirPardaz
-مروارید,مروارید بها بازار,Stock,31248540252187559,11929,http://morvaridfund.ir/,RayanHamafza
-نخل,در اوراق بهادار با درآمد ثابت خلیج فارس,Fixed,27797446447955609,11989,http://nakhl.pgibc.ir/,RayanHamafza
-نهال,طلای سرخ نو ویرا,Commodity,12913156843322499,11772,http://ngmf.ir/,RayanHamafza
-نیلی,نوع دوم نیلی دماوند,Fixed,31188566503248753,12070,http://nilidamavandfund.ir/,RayanHamafza
+مروارید,مروارید بها بازار,Stock,31248540252187559,11929,https://morvaridfund.ir/,RayanHamafza
+نخل,در اوراق بهادار با درآمد ثابت خلیج فارس,Fixed,27797446447955609,11989,https://nakhl.pgibc.ir/,RayanHamafza
+نشان,مختص اوراق دولتی نشان هامرز,Fixed,1241998328504490,11959,https://neshan.hummers.ir/,TadbirPardaz
+نهال,طلای سرخ نو ویرا,Commodity,12913156843322499,11772,https://ngmf.ir/,RayanHamafza
+نیلی,نوع دوم نیلی دماوند,Fixed,31188566503248753,12070,https://nilidamavandfund.ir/,RayanHamafza
 هامرز,اعتماد هامرز,Fixed,50503654866742146,11920,https://hummersfund.ir/,TadbirPardaz
-هم وزن,قابل معامله شاخصی کیان,Stock,47041908051542008,11924,http://kianfunds6.ir/,MabnaDP
+هم وزن,قابل معامله شاخصی کیان,Stock,47041908051542008,11924,https://kianfunds6.ir/,MabnaDP
 همای,همای آگاه,Fixed,15494954332657697,11767,https://homayeagah.ir/,RayanHamafza
 هیوا,ثروت هیوا,Stock,62845384302495432,11998,http://hiwafund.ir/,RayanHamafza
-وبازار,شاخصی بازار آشنا,Stock,41286608288791633,11763,http://indexfund.ir/,RayanHamafza
-ویستا,سهام ویستا,Stock,58852293795036597,11885,http://vistasahm.ir/,RayanHamafza
-پادا,پاداش سرمایه پارس,Stock,67522512921942106,11470,http://padashparsfund.com/,RayanHamafza
-پاداش,ارزش پاداش,Fixed,43267179898797137,11955,http://arzeshpadash.com/,RayanHamafza
+وبازار,شاخصی بازار آشنا,Stock,41286608288791633,11763,https://indexfund.ir/,RayanHamafza
+ویستا,سهام ویستا,Stock,58852293795036597,11885,https://vistasahm.ir/,RayanHamafza
+پادا,پاداش سرمایه پارس,Stock,67522512921942106,11470,https://padashparsfund.com/,RayanHamafza
+پاداش,ارزش پاداش,Fixed,43267179898797137,11955,https://arzeshpadash.com/,RayanHamafza
 پارند,پارند پایدار سپهر,Fixed,70595828753641750,11416,https://parandfund.ir/,RayanHamafza
-پالایش,پالایشی یکم,Stock,67675656072510693,11745,http://p1fund.ir/,RayanHamafza
-پتروآگاه,بخشی پتروشیمی آگاه,Stock,37828981835497620,12093,http://petroagahfund.ir/,RayanHamafza
+پالایش,پالایشی یکم,Stock,67675656072510693,11745,https://p1fund.ir/,RayanHamafza
+پتروآگاه,بخشی پتروشیمی آگاه,Stock,37828981835497620,12093,https://petroagahfund.ir/,RayanHamafza
 پرتو,پرتو پایش پیشرو,Stock,48818952524587858,12048,http://partofund.ir/,
-کارا,نوع دوم کارا,Fixed,71843282162462661,11883,http://kara.charisma.ir/,RayanHamafza
+کاج,نوع دوم پایدار نو ویرا,Fixed,42670427020727409,12017,https://vira-fund.ir/,RayanHamafza
+کارا,نوع دوم کارا,Fixed,71843282162462661,11883,https://kara.charisma.ir/,RayanHamafza
 کاردان,تجارت شاخصی کاردان,Stock,65023851436340574,11312,https://iran-kfunds3.ir/,TadbirPardaz
-کاریس,سهامی سپند کاریزما,Stock,69067576215760005,11183,http://scetf.ir/,RayanHamafza
+کاریس,سهامی سپند کاریزما,Stock,69067576215760005,11183,https://scetf.ir/,RayanHamafza
 کارین,با درآمد ثابت نگین سامان,Fixed,16056283141617755,11500,https://iran-kfunds4.ir/,TadbirPardaz
-کامیاب,کامیاب آشنا,Fixed,16040900750729921,11838,http://kamyabfund.ir/,RayanHamafza
-کمند,با درآمد ثابت کمند,Fixed,34718633636164421,11513,http://kamandfixedincome.com/,RayanHamafza
-کهربا,در اوراق بهادار مبتنی بر گواهی سپرده سکه طلا کهربا,Commodity,25559236668122210,11856,http://kahroba.charisma.ir/,RayanHamafza
+کامیاب,کامیاب آشنا,Fixed,16040900750729921,11838,https://kamyabfund.ir/,RayanHamafza
+کمند,با درآمد ثابت کمند,Fixed,34718633636164421,11513,https://kamandfixedincome.com/,RayanHamafza
+کهربا,در اوراق بهادار مبتنی بر گواهی سپرده سکه طلا کهربا,Commodity,25559236668122210,11856,https://kahroba.charisma.ir/,RayanHamafza
 کیان,با درآمد ثابت کیان,Fixed,53251602435454519,11459,https://kianfunds1.ir/,RayanHamafza
-گنبد,گنبد مینای دماوند,Mixed,7670135462634715,11907,http://gonbadminafund.ir/,RayanHamafza
+گنبد,گنبد مینای دماوند,Mixed,7670135462634715,11907,https://gonbadminafund.ir/,RayanHamafza
 گنجین,گنجینه یکم آوید,Fixed,57728534324022361,11499,https://ganjinehavid.ir/,TadbirPardaz
 گنجینه,گنجینه داریوش,Fixed,47101579271117172,11673,http://ganjineh.dariush.fund/,RayanHamafza
 گوهر,در اوراق بهادار مبتنی بر سکه طلای کیان,Commodity,12390706505809150,11556,https://kianfunds3.ir/,RayanHamafza
 یارا,در اوراق بهادار با درآمد ثابت آریا,Fixed,45284811973404357,11916,https://fund1.ariaamc.ir/,RayanHamafza
 یاقوت,یاقوت آگاه,Fixed,1438514795814416,11698,https://yaghootfund.ir/,RayanHamafza
```

### Comparing `iranetf-0.8.1/iranetf.egg-info/PKG-INFO` & `iranetf-0.9.0/iranetf.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iranetf
-Version: 0.8.1
+Version: 0.9.0
 Summary: a library to fetch data from iranetf.org
 Author-email: 5j9 <5j9@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/5j9/fipiran
 Project-URL: Bug Tracker, https://github.com/5j9/fipiran/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `iranetf-0.8.1/pyproject.toml` & `iranetf-0.9.0/pyproject.toml`

 * *Files identical despite different names*

