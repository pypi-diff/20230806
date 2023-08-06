# Comparing `tmp/bagbag-0.61.8.tar.gz` & `tmp/bagbag-0.61.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bagbag-0.61.8.tar", max compression
+gzip compressed data, was "bagbag-0.61.9.tar", max compression
```

## Comparing `bagbag-0.61.8.tar` & `bagbag-0.61.9.tar`

### file list

```diff
@@ -1,255 +1,255 @@
--rw-r--r--   0        0        0     1084 2022-07-07 19:24:15.851188 bagbag-0.61.8/LICENSE
--rw-r--r--   0        0        0    16842 2023-06-09 06:25:43.991924 bagbag-0.61.8/README.md
--rw-r--r--   0        0        0     2245 2023-07-25 08:21:28.493642 bagbag-0.61.8/pyproject.toml
--rw-r--r--   0        0        0      353 2023-05-12 12:35:25.861360 bagbag-0.61.8/src/bagbag/Base64/__init__.py
--rw-r--r--   0        0        0      478 2023-05-12 12:35:25.861258 bagbag-0.61.8/src/bagbag/Base64/src.py
--rw-r--r--   0        0        0      499 2023-05-12 12:35:25.861846 bagbag-0.61.8/src/bagbag/Cmd/__init__.py
--rw-r--r--   0        0        0     5769 2023-05-12 12:35:25.861768 bagbag-0.61.8/src/bagbag/Cmd/src.py
--rw-r--r--   0        0        0      361 2023-05-12 12:35:25.866128 bagbag-0.61.8/src/bagbag/Cryptoo/__init__.py
--rw-r--r--   0        0        0     2538 2023-05-12 12:35:25.866065 bagbag-0.61.8/src/bagbag/Cryptoo/src.py
--rw-r--r--   0        0        0      348 2023-06-02 17:02:39.723337 bagbag-0.61.8/src/bagbag/File/__init__.py
--rw-r--r--   0        0        0     4645 2023-06-02 17:04:32.821610 bagbag-0.61.8/src/bagbag/File/src.py
--rw-r--r--   0        0        0    16724 2023-05-12 12:35:25.857941 bagbag-0.61.8/src/bagbag/Funcs/CutSentenceStopWords_src.py
--rw-r--r--   0        0        0      856 2023-05-12 12:35:25.857574 bagbag-0.61.8/src/bagbag/Funcs/CutSentence_src.py
--rw-r--r--   0        0        0     6832 2023-05-12 12:35:25.858214 bagbag-0.61.8/src/bagbag/Funcs/FakeIdentity_src.py
--rw-r--r--   0        0        0      557 2023-05-12 12:35:25.858120 bagbag-0.61.8/src/bagbag/Funcs/FileType_src.py
--rw-r--r--   0        0        0      389 2023-05-12 12:35:25.858488 bagbag-0.61.8/src/bagbag/Funcs/Format/__init__.py
--rw-r--r--   0        0        0      836 2023-05-12 12:35:25.858411 bagbag-0.61.8/src/bagbag/Funcs/Format/src.py
--rw-r--r--   0        0        0      752 2023-05-12 12:35:25.857431 bagbag-0.61.8/src/bagbag/Funcs/GetPublicIP_src.py
--rw-r--r--   0        0        0      295 2023-05-12 12:35:25.857294 bagbag-0.61.8/src/bagbag/Funcs/IPAddressConvert_src.py
--rw-r--r--   0        0        0      473 2023-07-20 18:30:46.438978 bagbag-0.61.8/src/bagbag/Funcs/Markdown_src.py
--rw-r--r--   0        0        0      995 2023-05-12 12:35:25.857504 bagbag-0.61.8/src/bagbag/Funcs/Ping_src.py
--rw-r--r--   0        0        0     1729 2023-05-12 12:35:25.857363 bagbag-0.61.8/src/bagbag/Funcs/ResizeImage_src.py
--rw-r--r--   0        0        0      112 2023-05-12 12:35:25.857802 bagbag-0.61.8/src/bagbag/Funcs/UUID_src.py
--rw-r--r--   0        0        0     1457 2023-05-12 12:35:25.857646 bagbag-0.61.8/src/bagbag/Funcs/Wget_src.py
--rw-r--r--   0        0        0     1120 2023-05-12 12:35:25.857201 bagbag-0.61.8/src/bagbag/Funcs/__init__.py
--rw-r--r--   0        0        0      577 2023-05-12 12:35:25.862318 bagbag-0.61.8/src/bagbag/Hash/__init__.py
--rw-r--r--   0        0        0     1450 2023-05-12 12:35:25.862230 bagbag-0.61.8/src/bagbag/Hash/src.py
--rw-r--r--   0        0        0      683 2023-05-12 12:35:25.862782 bagbag-0.61.8/src/bagbag/Http/__init__.py
--rw-r--r--   0        0        0    12056 2023-07-24 08:20:54.798859 bagbag-0.61.8/src/bagbag/Http/src.py
--rw-r--r--   0        0        0      418 2023-05-12 12:35:25.863142 bagbag-0.61.8/src/bagbag/Json/__init__.py
--rw-r--r--   0        0        0     3271 2023-05-16 06:24:06.059824 bagbag-0.61.8/src/bagbag/Json/src.py
--rw-r--r--   0        0        0    10860 2023-06-16 14:21:52.035937 bagbag-0.61.8/src/bagbag/Lg.py
--rw-r--r--   0        0        0      382 2023-05-12 12:35:25.863851 bagbag-0.61.8/src/bagbag/Math/__init__.py
--rw-r--r--   0        0        0     2075 2023-05-12 12:35:25.863776 bagbag-0.61.8/src/bagbag/Math/src.py
--rw-r--r--   0        0        0      639 2023-05-15 13:18:35.454738 bagbag-0.61.8/src/bagbag/Os/Path/__init__.py
--rw-r--r--   0        0        0     1888 2023-07-20 18:33:32.538591 bagbag-0.61.8/src/bagbag/Os/Path/src.py
--rw-r--r--   0        0        0      917 2023-06-16 05:44:53.093812 bagbag-0.61.8/src/bagbag/Os/__init__.py
--rw-r--r--   0        0        0     3257 2023-06-16 05:44:20.429520 bagbag-0.61.8/src/bagbag/Os/src.py
--rw-r--r--   0        0        0      354 2023-05-12 12:35:25.864309 bagbag-0.61.8/src/bagbag/Process/__init__.py
--rw-r--r--   0        0        0     1239 2023-06-15 09:27:23.720590 bagbag-0.61.8/src/bagbag/Process/src.py
--rw-r--r--   0        0        0      350 2023-05-12 12:35:25.864721 bagbag-0.61.8/src/bagbag/Python/__init__.py
--rw-r--r--   0        0        0      985 2023-06-15 08:44:09.543096 bagbag-0.61.8/src/bagbag/Python/src.py
--rw-r--r--   0        0        0      464 2023-05-12 12:35:25.865128 bagbag-0.61.8/src/bagbag/Random/__init__.py
--rw-r--r--   0        0        0      700 2023-06-01 06:55:49.958227 bagbag-0.61.8/src/bagbag/Random/src.py
--rw-r--r--   0        0        0      510 2023-07-19 13:13:12.245619 bagbag-0.61.8/src/bagbag/Socket/TCP/__init__.py
--rw-r--r--   0        0        0     5127 2023-07-19 13:27:38.761011 bagbag-0.61.8/src/bagbag/Socket/TCP/src.py
--rw-r--r--   0        0        0       17 2023-05-12 12:35:25.860105 bagbag-0.61.8/src/bagbag/Socket/__init__.py
--rw-r--r--   0        0        0      352 2023-05-12 12:35:25.865416 bagbag-0.61.8/src/bagbag/String/__init__.py
--rw-r--r--   0        0        0    16972 2023-07-18 06:50:49.901739 bagbag-0.61.8/src/bagbag/String/src.py
--rw-r--r--   0        0        0      367 2023-05-12 12:35:25.865783 bagbag-0.61.8/src/bagbag/Thread/__init__.py
--rw-r--r--   0        0        0     1127 2023-06-15 09:24:51.853905 bagbag-0.61.8/src/bagbag/Thread/src.py
--rw-r--r--   0        0        0      571 2023-06-15 06:22:08.764134 bagbag-0.61.8/src/bagbag/Time/__init__.py
--rw-r--r--   0        0        0     6061 2023-06-15 06:30:18.558975 bagbag-0.61.8/src/bagbag/Time/src.py
--rw-r--r--   0        0        0     2449 2023-05-12 12:35:25.818366 bagbag-0.61.8/src/bagbag/Tools/Argparser_src.py
--rw-r--r--   0        0        0     2613 2023-05-12 12:35:25.825531 bagbag-0.61.8/src/bagbag/Tools/BlockChain/Binance/CoinsPrice_src.py
--rw-r--r--   0        0        0      350 2023-05-12 12:35:25.826469 bagbag-0.61.8/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/__init__.py
--rw-r--r--   0        0        0      972 2023-05-12 12:35:25.826332 bagbag-0.61.8/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/src.py
--rw-r--r--   0        0        0      509 2023-05-12 12:35:25.825419 bagbag-0.61.8/src/bagbag/Tools/BlockChain/Binance/__init__.py
--rw-r--r--   0        0        0       36 2023-05-12 12:35:25.827257 bagbag-0.61.8/src/bagbag/Tools/BlockChain/Ethereum/__init__.py
--rw-r--r--   0        0        0      325 2023-05-12 12:35:25.827344 bagbag-0.61.8/src/bagbag/Tools/BlockChain/Ethereum/ethereum.py
--rw-r--r--   0        0        0      485 2023-05-12 12:35:25.824938 bagbag-0.61.8/src/bagbag/Tools/BlockChain/Tron/__init__.py
--rw-r--r--   0        0        0    24277 2023-07-06 05:43:43.753694 bagbag-0.61.8/src/bagbag/Tools/BlockChain/Tron/src.py
--rw-r--r--   0        0        0      381 2023-07-04 14:12:42.665691 bagbag-0.61.8/src/bagbag/Tools/BlockChain/__init__.py
--rw-r--r--   0        0        0     3277 2023-06-05 15:36:04.503828 bagbag-0.61.8/src/bagbag/Tools/CSV.py
--rw-r--r--   0        0        0     4615 2023-06-09 06:22:43.542806 bagbag-0.61.8/src/bagbag/Tools/Cache.py
--rw-r--r--   0        0        0     3886 2023-05-12 12:35:25.816327 bagbag-0.61.8/src/bagbag/Tools/Chan_src.py
--rw-r--r--   0        0        0    32941 2023-05-29 11:13:19.619696 bagbag-0.61.8/src/bagbag/Tools/ComputerVision.py
--rw-r--r--   0        0        0     3238 2023-05-29 11:10:20.747420 bagbag-0.61.8/src/bagbag/Tools/Crontab_src.py
--rw-r--r--   0        0        0      644 2023-05-12 12:35:25.856714 bagbag-0.61.8/src/bagbag/Tools/Database/__init__.py
--rw-r--r--   0        0        0      297 2023-05-12 12:35:25.830525 bagbag-0.61.8/src/bagbag/Tools/Database/orator/__init__.py
--rw-r--r--   0        0        0       24 2023-05-12 12:35:25.830659 bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/__init__.py
--rw-r--r--   0        0        0      785 2023-05-12 12:35:25.830739 bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/application.py
--rw-r--r--   0        0        0     3436 2023-05-12 12:35:25.830822 bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/command.py
--rw-r--r--   0        0        0      330 2023-05-12 12:35:25.830964 bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/migrations/__init__.py
--rw-r--r--   0        0        0      186 2023-05-12 12:35:25.831040 bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/migrations/base_command.py
--rw-r--r--   0        0        0      626 2023-05-12 12:35:25.831123 bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/migrations/install_command.py
--rw-r--r--   0        0        0     1301 2023-05-12 12:35:25.831226 bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/migrations/make_command.py
--rw-r--r--   0        0        0     2343 2023-05-12 12:35:25.831313 bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/migrations/migrate_command.py
--rw-r--r--   0        0        0     1886 2023-05-12 12:35:25.831395 bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/migrations/refresh_command.py
--rw-r--r--   0        0        0     1308 2023-05-12 12:35:25.831488 bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/migrations/reset_command.py
--rw-r--r--   0        0        0     1315 2023-05-12 12:35:25.831583 bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/migrations/rollback_command.py
--rw-r--r--   0        0        0     1642 2023-05-12 12:35:25.831666 bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/migrations/status_command.py
--rw-r--r--   0        0        0       68 2023-05-12 12:35:25.831798 bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/models/__init__.py
--rw-r--r--   0        0        0     2217 2023-05-12 12:35:25.831874 bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/models/make_command.py
--rw-r--r--   0        0        0      115 2023-05-12 12:35:25.831968 bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/models/stubs.py
--rw-r--r--   0        0        0      108 2023-05-12 12:35:25.832158 bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/seeds/__init__.py
--rw-r--r--   0        0        0      178 2023-05-12 12:35:25.832248 bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/seeds/base_command.py
--rw-r--r--   0        0        0     2204 2023-05-12 12:35:25.832352 bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/seeds/make_command.py
--rw-r--r--   0        0        0     1923 2023-05-12 12:35:25.832446 bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/seeds/seed_command.py
--rw-r--r--   0        0        0      206 2023-05-12 12:35:25.832590 bagbag-0.61.8/src/bagbag/Tools/Database/orator/connections/__init__.py
--rw-r--r--   0        0        0    15063 2023-05-12 12:35:25.832673 bagbag-0.61.8/src/bagbag/Tools/Database/orator/connections/connection.py
--rw-r--r--   0        0        0     4112 2023-05-12 12:35:25.832759 bagbag-0.61.8/src/bagbag/Tools/Database/orator/connections/connection_interface.py
--rw-r--r--   0        0        0      298 2023-05-12 12:35:25.832861 bagbag-0.61.8/src/bagbag/Tools/Database/orator/connections/connection_resolver_interface.py
--rw-r--r--   0        0        0     2218 2023-05-12 12:35:25.832962 bagbag-0.61.8/src/bagbag/Tools/Database/orator/connections/mysql_connection.py
--rw-r--r--   0        0        0     2056 2023-05-12 12:35:25.833055 bagbag-0.61.8/src/bagbag/Tools/Database/orator/connections/postgres_connection.py
--rw-r--r--   0        0        0     1588 2023-05-12 12:35:25.833159 bagbag-0.61.8/src/bagbag/Tools/Database/orator/connections/sqlite_connection.py
--rw-r--r--   0        0        0      198 2023-05-12 12:35:25.833971 bagbag-0.61.8/src/bagbag/Tools/Database/orator/connectors/__init__.py
--rw-r--r--   0        0        0     3133 2023-05-12 12:35:25.834056 bagbag-0.61.8/src/bagbag/Tools/Database/orator/connectors/connection_factory.py
--rw-r--r--   0        0        0     3106 2023-05-12 12:35:25.834129 bagbag-0.61.8/src/bagbag/Tools/Database/orator/connectors/connector.py
--rw-r--r--   0        0        0     3982 2023-05-12 12:35:25.834204 bagbag-0.61.8/src/bagbag/Tools/Database/orator/connectors/mysql_connector.py
--rw-r--r--   0        0        0     3280 2023-05-12 12:35:25.834291 bagbag-0.61.8/src/bagbag/Tools/Database/orator/connectors/postgres_connector.py
--rw-r--r--   0        0        0     2172 2023-05-12 12:35:25.834370 bagbag-0.61.8/src/bagbag/Tools/Database/orator/connectors/sqlite_connector.py
--rw-r--r--   0        0        0     5089 2023-05-12 12:35:25.835189 bagbag-0.61.8/src/bagbag/Tools/Database/orator/database_manager.py
--rw-r--r--   0        0        0       24 2023-05-12 12:35:25.835796 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/__init__.py
--rw-r--r--   0        0        0     2372 2023-05-12 12:35:25.835903 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/abstract_asset.py
--rw-r--r--   0        0        0     3447 2023-05-12 12:35:25.835999 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/column.py
--rw-r--r--   0        0        0      545 2023-05-12 12:35:25.836087 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/column_diff.py
--rw-r--r--   0        0        0    11219 2023-05-12 12:35:25.836174 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/comparator.py
--rw-r--r--   0        0        0     1943 2023-05-12 12:35:25.836319 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/exceptions/__init__.py
--rw-r--r--   0        0        0     8193 2023-05-12 12:35:25.836678 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/foreign_key_constraint.py
--rw-r--r--   0        0        0      173 2023-05-12 12:35:25.836774 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/identifier.py
--rw-r--r--   0        0        0     7094 2023-05-12 12:35:25.836858 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/index.py
--rw-r--r--   0        0        0     5260 2023-05-12 12:35:25.836935 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/mysql_schema_manager.py
--rw-r--r--   0        0        0      205 2023-05-12 12:35:25.837074 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/platforms/__init__.py
--rw-r--r--   0        0        0       24 2023-05-12 12:35:25.837217 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/__init__.py
--rw-r--r--   0        0        0      209 2023-05-12 12:35:25.837297 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/keyword_list.py
--rw-r--r--   0        0        0     4383 2023-05-12 12:35:25.837375 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/mysql_keywords.py
--rw-r--r--   0        0        0     1730 2023-05-12 12:35:25.837455 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/postgresql_keywords.py
--rw-r--r--   0        0        0     2315 2023-05-12 12:35:25.837531 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/sqlite_keywords.py
--rw-r--r--   0        0        0     1289 2023-05-12 12:35:25.838118 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/platforms/mysql57_platform.py
--rw-r--r--   0        0        0     9489 2023-05-12 12:35:25.838202 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/platforms/mysql_platform.py
--rw-r--r--   0        0        0    21672 2023-05-12 12:35:25.838290 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/platforms/platform.py
--rw-r--r--   0        0        0    14126 2023-05-12 12:35:25.838370 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/platforms/postgres_platform.py
--rw-r--r--   0        0        0    20833 2023-05-12 12:35:25.838457 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/platforms/sqlite_platform.py
--rw-r--r--   0        0        0     6014 2023-05-12 12:35:25.839154 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/postgres_schema_manager.py
--rw-r--r--   0        0        0     4240 2023-05-12 12:35:25.839242 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/schema_manager.py
--rw-r--r--   0        0        0     5458 2023-05-12 12:35:25.839325 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/sqlite_schema_manager.py
--rw-r--r--   0        0        0    17146 2023-05-12 12:35:25.839403 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/table.py
--rw-r--r--   0        0        0     1436 2023-05-12 12:35:25.839495 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/table_diff.py
--rw-r--r--   0        0        0       24 2023-05-12 12:35:25.839639 bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/types/__init__.py
--rw-r--r--   0        0        0      992 2023-05-12 12:35:25.840999 bagbag-0.61.8/src/bagbag/Tools/Database/orator/events/__init__.py
--rw-r--r--   0        0        0       68 2023-05-12 12:35:25.841361 bagbag-0.61.8/src/bagbag/Tools/Database/orator/exceptions/__init__.py
--rw-r--r--   0        0        0      193 2023-05-12 12:35:25.841461 bagbag-0.61.8/src/bagbag/Tools/Database/orator/exceptions/connection.py
--rw-r--r--   0        0        0      822 2023-05-12 12:35:25.841563 bagbag-0.61.8/src/bagbag/Tools/Database/orator/exceptions/connectors.py
--rw-r--r--   0        0        0      551 2023-05-12 12:35:25.841649 bagbag-0.61.8/src/bagbag/Tools/Database/orator/exceptions/orm.py
--rw-r--r--   0        0        0      494 2023-05-12 12:35:25.841746 bagbag-0.61.8/src/bagbag/Tools/Database/orator/exceptions/query.py
--rw-r--r--   0        0        0      208 2023-05-12 12:35:25.842330 bagbag-0.61.8/src/bagbag/Tools/Database/orator/migrations/__init__.py
--rw-r--r--   0        0        0     2730 2023-05-12 12:35:25.842410 bagbag-0.61.8/src/bagbag/Tools/Database/orator/migrations/database_migration_repository.py
--rw-r--r--   0        0        0      425 2023-05-12 12:35:25.842506 bagbag-0.61.8/src/bagbag/Tools/Database/orator/migrations/migration.py
--rw-r--r--   0        0        0     2588 2023-05-12 12:35:25.842583 bagbag-0.61.8/src/bagbag/Tools/Database/orator/migrations/migration_creator.py
--rw-r--r--   0        0        0     7754 2023-05-12 12:35:25.842660 bagbag-0.61.8/src/bagbag/Tools/Database/orator/migrations/migrator.py
--rw-r--r--   0        0        0     1114 2023-05-12 12:35:25.842735 bagbag-0.61.8/src/bagbag/Tools/Database/orator/migrations/stubs.py
--rw-r--r--   0        0        0      419 2023-05-12 12:35:25.842873 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/__init__.py
--rw-r--r--   0        0        0    32311 2023-05-12 12:35:25.842946 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/builder.py
--rw-r--r--   0        0        0      814 2023-05-12 12:35:25.843014 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/collection.py
--rw-r--r--   0        0        0     7481 2023-05-12 12:35:25.843112 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/factory.py
--rw-r--r--   0        0        0     2579 2023-05-12 12:35:25.843207 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/factory_builder.py
--rw-r--r--   0        0        0       63 2023-05-12 12:35:25.843408 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/mixins/__init__.py
--rw-r--r--   0        0        0     3532 2023-05-12 12:35:25.843502 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/mixins/soft_deletes.py
--rw-r--r--   0        0        0    75367 2023-05-12 12:35:25.843880 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/model.py
--rw-r--r--   0        0        0      371 2023-05-12 12:35:25.844072 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/__init__.py
--rw-r--r--   0        0        0     5427 2023-05-12 12:35:25.844163 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/belongs_to.py
--rw-r--r--   0        0        0    23248 2023-05-12 12:35:25.844271 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/belongs_to_many.py
--rw-r--r--   0        0        0     1012 2023-05-12 12:35:25.844373 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/has_many.py
--rw-r--r--   0        0        0     5126 2023-05-12 12:35:25.844473 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/has_many_through.py
--rw-r--r--   0        0        0      955 2023-05-12 12:35:25.844558 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/has_one.py
--rw-r--r--   0        0        0     8617 2023-05-12 12:35:25.844637 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/has_one_or_many.py
--rw-r--r--   0        0        0      899 2023-05-12 12:35:25.844716 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/morph_many.py
--rw-r--r--   0        0        0      843 2023-05-12 12:35:25.844810 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/morph_one.py
--rw-r--r--   0        0        0     5377 2023-05-12 12:35:25.844920 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/morph_one_or_many.py
--rw-r--r--   0        0        0      984 2023-05-12 12:35:25.845022 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/morph_pivot.py
--rw-r--r--   0        0        0     5293 2023-05-12 12:35:25.845127 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/morph_to.py
--rw-r--r--   0        0        0     3555 2023-05-12 12:35:25.845220 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/morph_to_many.py
--rw-r--r--   0        0        0     2978 2023-05-12 12:35:25.845313 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/pivot.py
--rw-r--r--   0        0        0     5956 2023-05-12 12:35:25.845401 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/relation.py
--rw-r--r--   0        0        0      685 2023-05-12 12:35:25.845502 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/result.py
--rw-r--r--   0        0        0     1106 2023-05-12 12:35:25.845583 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/wrapper.py
--rw-r--r--   0        0        0       95 2023-05-12 12:35:25.847154 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/scopes/__init__.py
--rw-r--r--   0        0        0      348 2023-05-12 12:35:25.847229 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/scopes/scope.py
--rw-r--r--   0        0        0     3900 2023-05-12 12:35:25.847308 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/scopes/soft_deleting.py
--rw-r--r--   0        0        0    13642 2023-05-12 12:35:25.847743 bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/utils.py
--rw-r--r--   0        0        0      115 2023-05-12 12:35:25.848559 bagbag-0.61.8/src/bagbag/Tools/Database/orator/pagination/__init__.py
--rw-r--r--   0        0        0     2251 2023-05-12 12:35:25.848628 bagbag-0.61.8/src/bagbag/Tools/Database/orator/pagination/base.py
--rw-r--r--   0        0        0     2426 2023-05-12 12:35:25.848698 bagbag-0.61.8/src/bagbag/Tools/Database/orator/pagination/length_aware_paginator.py
--rw-r--r--   0        0        0     2216 2023-05-12 12:35:25.848764 bagbag-0.61.8/src/bagbag/Tools/Database/orator/pagination/paginator.py
--rw-r--r--   0        0        0       59 2023-05-12 12:35:25.849247 bagbag-0.61.8/src/bagbag/Tools/Database/orator/query/__init__.py
--rw-r--r--   0        0        0    44030 2023-05-12 12:35:25.849322 bagbag-0.61.8/src/bagbag/Tools/Database/orator/query/builder.py
--rw-r--r--   0        0        0      230 2023-05-12 12:35:25.849403 bagbag-0.61.8/src/bagbag/Tools/Database/orator/query/expression.py
--rw-r--r--   0        0        0      202 2023-05-12 12:35:25.849583 bagbag-0.61.8/src/bagbag/Tools/Database/orator/query/grammars/__init__.py
--rw-r--r--   0        0        0    13999 2023-05-12 12:35:25.849662 bagbag-0.61.8/src/bagbag/Tools/Database/orator/query/grammars/grammar.py
--rw-r--r--   0        0        0     3559 2023-05-12 12:35:25.849810 bagbag-0.61.8/src/bagbag/Tools/Database/orator/query/grammars/mysql_grammar.py
--rw-r--r--   0        0        0     4461 2023-05-12 12:35:25.849897 bagbag-0.61.8/src/bagbag/Tools/Database/orator/query/grammars/postgres_grammar.py
--rw-r--r--   0        0        0     4204 2023-05-12 12:35:25.849974 bagbag-0.61.8/src/bagbag/Tools/Database/orator/query/grammars/sqlite_grammar.py
--rw-r--r--   0        0        0     1407 2023-05-12 12:35:25.850460 bagbag-0.61.8/src/bagbag/Tools/Database/orator/query/join_clause.py
--rw-r--r--   0        0        0      218 2023-05-12 12:35:25.850604 bagbag-0.61.8/src/bagbag/Tools/Database/orator/query/processors/__init__.py
--rw-r--r--   0        0        0     1790 2023-05-12 12:35:25.850669 bagbag-0.61.8/src/bagbag/Tools/Database/orator/query/processors/mysql_processor.py
--rw-r--r--   0        0        0     1160 2023-05-12 12:35:25.850732 bagbag-0.61.8/src/bagbag/Tools/Database/orator/query/processors/postgres_processor.py
--rw-r--r--   0        0        0     1423 2023-05-12 12:35:25.850798 bagbag-0.61.8/src/bagbag/Tools/Database/orator/query/processors/processor.py
--rw-r--r--   0        0        0      422 2023-05-12 12:35:25.850863 bagbag-0.61.8/src/bagbag/Tools/Database/orator/query/processors/sqlite_processor.py
--rw-r--r--   0        0        0      166 2023-05-12 12:35:25.851787 bagbag-0.61.8/src/bagbag/Tools/Database/orator/schema/__init__.py
--rw-r--r--   0        0        0    19482 2023-05-12 12:35:25.851871 bagbag-0.61.8/src/bagbag/Tools/Database/orator/schema/blueprint.py
--rw-r--r--   0        0        0     3617 2023-05-12 12:35:25.851961 bagbag-0.61.8/src/bagbag/Tools/Database/orator/schema/builder.py
--rw-r--r--   0        0        0      206 2023-05-12 12:35:25.852130 bagbag-0.61.8/src/bagbag/Tools/Database/orator/schema/grammars/__init__.py
--rw-r--r--   0        0        0     9880 2023-05-12 12:35:25.852215 bagbag-0.61.8/src/bagbag/Tools/Database/orator/schema/grammars/grammar.py
--rw-r--r--   0        0        0     8503 2023-05-12 12:35:25.852316 bagbag-0.61.8/src/bagbag/Tools/Database/orator/schema/grammars/mysql_grammar.py
--rw-r--r--   0        0        0     7103 2023-05-12 12:35:25.852415 bagbag-0.61.8/src/bagbag/Tools/Database/orator/schema/grammars/postgres_grammar.py
--rw-r--r--   0        0        0     8321 2023-05-12 12:35:25.852524 bagbag-0.61.8/src/bagbag/Tools/Database/orator/schema/grammars/sqlite_grammar.py
--rw-r--r--   0        0        0     1229 2023-05-12 12:35:25.853214 bagbag-0.61.8/src/bagbag/Tools/Database/orator/schema/mysql_builder.py
--rw-r--r--   0        0        0      645 2023-05-12 12:35:25.853314 bagbag-0.61.8/src/bagbag/Tools/Database/orator/schema/schema.py
--rw-r--r--   0        0        0       52 2023-05-12 12:35:25.854121 bagbag-0.61.8/src/bagbag/Tools/Database/orator/seeds/__init__.py
--rw-r--r--   0        0        0     1730 2023-05-12 12:35:25.854207 bagbag-0.61.8/src/bagbag/Tools/Database/orator/seeds/seeder.py
--rw-r--r--   0        0        0      203 2023-05-12 12:35:25.854288 bagbag-0.61.8/src/bagbag/Tools/Database/orator/seeds/stubs.py
--rw-r--r--   0        0        0       60 2023-05-12 12:35:25.854476 bagbag-0.61.8/src/bagbag/Tools/Database/orator/support/__init__.py
--rw-r--r--   0        0        0      121 2023-05-12 12:35:25.854566 bagbag-0.61.8/src/bagbag/Tools/Database/orator/support/collection.py
--rw-r--r--   0        0        0     2193 2023-05-12 12:35:25.854656 bagbag-0.61.8/src/bagbag/Tools/Database/orator/support/fluent.py
--rw-r--r--   0        0        0     2614 2023-05-12 12:35:25.854751 bagbag-0.61.8/src/bagbag/Tools/Database/orator/support/grammar.py
--rw-r--r--   0        0        0     2833 2023-05-12 12:35:25.855426 bagbag-0.61.8/src/bagbag/Tools/Database/orator/utils/__init__.py
--rw-r--r--   0        0        0     4398 2023-05-12 12:35:25.855517 bagbag-0.61.8/src/bagbag/Tools/Database/orator/utils/command_formatter.py
--rw-r--r--   0        0        0      749 2023-05-12 12:35:25.855603 bagbag-0.61.8/src/bagbag/Tools/Database/orator/utils/helpers.py
--rw-r--r--   0        0        0      714 2023-05-12 12:35:25.855706 bagbag-0.61.8/src/bagbag/Tools/Database/orator/utils/qmarker.py
--rw-r--r--   0        0        0     7566 2023-05-12 12:35:25.855800 bagbag-0.61.8/src/bagbag/Tools/Database/orator/utils/url.py
--rw-r--r--   0        0        0    33362 2023-07-03 09:42:07.366549 bagbag-0.61.8/src/bagbag/Tools/Database/src.py
--rw-r--r--   0        0        0     5250 2023-05-29 11:10:33.731697 bagbag-0.61.8/src/bagbag/Tools/DistributedLock_src.py
--rw-r--r--   0        0        0     4674 2023-05-29 11:10:40.751258 bagbag-0.61.8/src/bagbag/Tools/Elasticsearch_src.py
--rw-r--r--   0        0        0     4312 2023-05-29 11:10:51.912539 bagbag-0.61.8/src/bagbag/Tools/Github_src.py
--rw-r--r--   0        0        0     1451 2023-05-12 12:35:25.827625 bagbag-0.61.8/src/bagbag/Tools/JavaScript_src.py
--rw-r--r--   0        0        0    10096 2023-06-09 08:35:54.469473 bagbag-0.61.8/src/bagbag/Tools/Kafka_src.py
--rw-r--r--   0        0        0     2028 2023-05-12 12:35:25.815942 bagbag-0.61.8/src/bagbag/Tools/Lock_src.py
--rw-r--r--   0        0        0     6634 2023-05-29 11:11:12.945317 bagbag-0.61.8/src/bagbag/Tools/MatrixBot_src.py
--rw-r--r--   0        0        0      466 2023-05-12 12:35:25.821432 bagbag-0.61.8/src/bagbag/Tools/Nslookup_src.py
--rw-r--r--   0        0        0     2364 2023-05-29 11:11:50.231133 bagbag-0.61.8/src/bagbag/Tools/OCR_src.py
--rw-r--r--   0        0        0     2816 2023-05-12 12:35:25.815348 bagbag-0.61.8/src/bagbag/Tools/ProgressBar_src.py
--rw-r--r--   0        0        0     1660 2023-05-12 12:35:25.821643 bagbag-0.61.8/src/bagbag/Tools/Prometheus/MetricServer.py
--rw-r--r--   0        0        0     3337 2023-06-07 15:52:43.922791 bagbag-0.61.8/src/bagbag/Tools/Prometheus/PushGateway.py
--rw-r--r--   0        0        0      127 2023-05-12 12:35:25.821766 bagbag-0.61.8/src/bagbag/Tools/Prometheus/__init__.py
--rw-r--r--   0        0        0     4670 2023-05-12 12:35:25.821993 bagbag-0.61.8/src/bagbag/Tools/Prometheus/metrics.py
--rw-r--r--   0        0        0     2607 2023-05-29 11:12:14.997684 bagbag-0.61.8/src/bagbag/Tools/Queue_src.py
--rw-r--r--   0        0        0     2490 2023-05-12 12:35:25.821196 bagbag-0.61.8/src/bagbag/Tools/RSS/Feed.py
--rw-r--r--   0        0        0      661 2023-05-12 12:35:25.820920 bagbag-0.61.8/src/bagbag/Tools/RSS/Opml.py
--rw-r--r--   0        0        0      119 2023-05-12 12:35:25.821062 bagbag-0.61.8/src/bagbag/Tools/RSS/__init__.py
--rw-r--r--   0        0        0     3688 2023-05-12 12:35:25.816210 bagbag-0.61.8/src/bagbag/Tools/Ratelimit_src.py
--rw-r--r--   0        0        0    18451 2023-05-29 11:12:03.251797 bagbag-0.61.8/src/bagbag/Tools/Redis_src.py
--rw-r--r--   0        0        0     5609 2023-07-09 07:33:46.935788 bagbag-0.61.8/src/bagbag/Tools/SSH_src.py
--rw-r--r--   0        0        0    34757 2023-07-18 07:42:48.217790 bagbag-0.61.8/src/bagbag/Tools/Selenium.py
--rw-r--r--   0        0        0    14131 2023-05-12 12:35:25.820287 bagbag-0.61.8/src/bagbag/Tools/TelegramAsync.py
--rw-r--r--   0        0        0     5111 2023-05-12 12:35:25.816456 bagbag-0.61.8/src/bagbag/Tools/TelegramBotOfficial_src.py
--rw-r--r--   0        0        0     3069 2023-06-14 11:27:42.444891 bagbag-0.61.8/src/bagbag/Tools/TelegramBot_src.py
--rw-r--r--   0        0        0    24676 2023-06-13 19:08:29.204793 bagbag-0.61.8/src/bagbag/Tools/Telegram_src.py
--rw-r--r--   0        0        0      142 2023-05-12 12:35:25.824483 bagbag-0.61.8/src/bagbag/Tools/Test.py
--rw-r--r--   0        0        0     4276 2023-05-12 12:35:25.819888 bagbag-0.61.8/src/bagbag/Tools/Translater_src.py
--rw-r--r--   0        0        0    14103 2023-06-19 07:22:24.505061 bagbag-0.61.8/src/bagbag/Tools/Twitter/Browser_src.py
--rw-r--r--   0        0        0    12718 2023-07-18 12:42:14.412719 bagbag-0.61.8/src/bagbag/Tools/Twitter/Elevated_src.py
--rw-r--r--   0        0        0     2093 2023-05-26 13:18:47.657372 bagbag-0.61.8/src/bagbag/Tools/Twitter/Essential_src.py
--rw-r--r--   0        0        0    29126 2023-07-25 08:21:12.794106 bagbag-0.61.8/src/bagbag/Tools/Twitter/Nitter_src.py
--rw-r--r--   0        0        0     2744 2023-06-16 08:15:42.223073 bagbag-0.61.8/src/bagbag/Tools/Twitter/Utils.py
--rw-r--r--   0        0        0     1070 2023-07-19 12:53:41.487474 bagbag-0.61.8/src/bagbag/Tools/Twitter/__init__.py
--rw-r--r--   0        0        0     3122 2023-05-12 12:35:25.816080 bagbag-0.61.8/src/bagbag/Tools/URL_src.py
--rw-r--r--   0        0        0      767 2023-05-12 12:35:25.818906 bagbag-0.61.8/src/bagbag/Tools/WaitGroup_src.py
--rw-r--r--   0        0        0     8126 2023-05-12 12:35:25.828462 bagbag-0.61.8/src/bagbag/Tools/WebCrawler_src.py
--rw-r--r--   0        0        0     7040 2023-07-16 17:07:37.080346 bagbag-0.61.8/src/bagbag/Tools/WebServer_src.py
--rw-r--r--   0        0        0     2434 2023-07-19 07:21:05.031779 bagbag-0.61.8/src/bagbag/Tools/XPath_src.py
--rw-r--r--   0        0        0     3235 2023-05-16 08:49:31.768572 bagbag-0.61.8/src/bagbag/Tools/Xlsx.py
--rw-r--r--   0        0        0     3528 2023-07-04 14:13:58.807237 bagbag-0.61.8/src/bagbag/Tools/__init__.py
--rw-r--r--   0        0        0     4555 2023-06-17 10:44:24.595347 bagbag-0.61.8/src/bagbag/__init__.py
--rw-r--r--   0        0        0    19723 1970-01-01 00:00:00.000000 bagbag-0.61.8/PKG-INFO
+-rw-r--r--   0        0        0     1084 2022-07-07 19:24:15.851188 bagbag-0.61.9/LICENSE
+-rw-r--r--   0        0        0    16842 2023-06-09 06:25:43.991924 bagbag-0.61.9/README.md
+-rw-r--r--   0        0        0     2245 2023-07-25 09:09:09.929717 bagbag-0.61.9/pyproject.toml
+-rw-r--r--   0        0        0      353 2023-05-12 12:35:25.861360 bagbag-0.61.9/src/bagbag/Base64/__init__.py
+-rw-r--r--   0        0        0      478 2023-05-12 12:35:25.861258 bagbag-0.61.9/src/bagbag/Base64/src.py
+-rw-r--r--   0        0        0      499 2023-05-12 12:35:25.861846 bagbag-0.61.9/src/bagbag/Cmd/__init__.py
+-rw-r--r--   0        0        0     5769 2023-05-12 12:35:25.861768 bagbag-0.61.9/src/bagbag/Cmd/src.py
+-rw-r--r--   0        0        0      361 2023-05-12 12:35:25.866128 bagbag-0.61.9/src/bagbag/Cryptoo/__init__.py
+-rw-r--r--   0        0        0     2538 2023-05-12 12:35:25.866065 bagbag-0.61.9/src/bagbag/Cryptoo/src.py
+-rw-r--r--   0        0        0      348 2023-06-02 17:02:39.723337 bagbag-0.61.9/src/bagbag/File/__init__.py
+-rw-r--r--   0        0        0     4645 2023-06-02 17:04:32.821610 bagbag-0.61.9/src/bagbag/File/src.py
+-rw-r--r--   0        0        0    16724 2023-05-12 12:35:25.857941 bagbag-0.61.9/src/bagbag/Funcs/CutSentenceStopWords_src.py
+-rw-r--r--   0        0        0      856 2023-05-12 12:35:25.857574 bagbag-0.61.9/src/bagbag/Funcs/CutSentence_src.py
+-rw-r--r--   0        0        0     6832 2023-05-12 12:35:25.858214 bagbag-0.61.9/src/bagbag/Funcs/FakeIdentity_src.py
+-rw-r--r--   0        0        0      557 2023-05-12 12:35:25.858120 bagbag-0.61.9/src/bagbag/Funcs/FileType_src.py
+-rw-r--r--   0        0        0      389 2023-05-12 12:35:25.858488 bagbag-0.61.9/src/bagbag/Funcs/Format/__init__.py
+-rw-r--r--   0        0        0      836 2023-05-12 12:35:25.858411 bagbag-0.61.9/src/bagbag/Funcs/Format/src.py
+-rw-r--r--   0        0        0      752 2023-05-12 12:35:25.857431 bagbag-0.61.9/src/bagbag/Funcs/GetPublicIP_src.py
+-rw-r--r--   0        0        0      295 2023-05-12 12:35:25.857294 bagbag-0.61.9/src/bagbag/Funcs/IPAddressConvert_src.py
+-rw-r--r--   0        0        0      473 2023-07-20 18:30:46.438978 bagbag-0.61.9/src/bagbag/Funcs/Markdown_src.py
+-rw-r--r--   0        0        0      995 2023-05-12 12:35:25.857504 bagbag-0.61.9/src/bagbag/Funcs/Ping_src.py
+-rw-r--r--   0        0        0     1729 2023-05-12 12:35:25.857363 bagbag-0.61.9/src/bagbag/Funcs/ResizeImage_src.py
+-rw-r--r--   0        0        0      112 2023-05-12 12:35:25.857802 bagbag-0.61.9/src/bagbag/Funcs/UUID_src.py
+-rw-r--r--   0        0        0     1457 2023-05-12 12:35:25.857646 bagbag-0.61.9/src/bagbag/Funcs/Wget_src.py
+-rw-r--r--   0        0        0     1120 2023-05-12 12:35:25.857201 bagbag-0.61.9/src/bagbag/Funcs/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-12 12:35:25.862318 bagbag-0.61.9/src/bagbag/Hash/__init__.py
+-rw-r--r--   0        0        0     1450 2023-05-12 12:35:25.862230 bagbag-0.61.9/src/bagbag/Hash/src.py
+-rw-r--r--   0        0        0      683 2023-05-12 12:35:25.862782 bagbag-0.61.9/src/bagbag/Http/__init__.py
+-rw-r--r--   0        0        0    12056 2023-07-24 08:20:54.798859 bagbag-0.61.9/src/bagbag/Http/src.py
+-rw-r--r--   0        0        0      418 2023-05-12 12:35:25.863142 bagbag-0.61.9/src/bagbag/Json/__init__.py
+-rw-r--r--   0        0        0     3271 2023-05-16 06:24:06.059824 bagbag-0.61.9/src/bagbag/Json/src.py
+-rw-r--r--   0        0        0    10860 2023-06-16 14:21:52.035937 bagbag-0.61.9/src/bagbag/Lg.py
+-rw-r--r--   0        0        0      382 2023-05-12 12:35:25.863851 bagbag-0.61.9/src/bagbag/Math/__init__.py
+-rw-r--r--   0        0        0     2075 2023-05-12 12:35:25.863776 bagbag-0.61.9/src/bagbag/Math/src.py
+-rw-r--r--   0        0        0      639 2023-05-15 13:18:35.454738 bagbag-0.61.9/src/bagbag/Os/Path/__init__.py
+-rw-r--r--   0        0        0     1888 2023-07-20 18:33:32.538591 bagbag-0.61.9/src/bagbag/Os/Path/src.py
+-rw-r--r--   0        0        0      917 2023-06-16 05:44:53.093812 bagbag-0.61.9/src/bagbag/Os/__init__.py
+-rw-r--r--   0        0        0     3257 2023-06-16 05:44:20.429520 bagbag-0.61.9/src/bagbag/Os/src.py
+-rw-r--r--   0        0        0      354 2023-05-12 12:35:25.864309 bagbag-0.61.9/src/bagbag/Process/__init__.py
+-rw-r--r--   0        0        0     1239 2023-06-15 09:27:23.720590 bagbag-0.61.9/src/bagbag/Process/src.py
+-rw-r--r--   0        0        0      350 2023-05-12 12:35:25.864721 bagbag-0.61.9/src/bagbag/Python/__init__.py
+-rw-r--r--   0        0        0      985 2023-06-15 08:44:09.543096 bagbag-0.61.9/src/bagbag/Python/src.py
+-rw-r--r--   0        0        0      464 2023-05-12 12:35:25.865128 bagbag-0.61.9/src/bagbag/Random/__init__.py
+-rw-r--r--   0        0        0      700 2023-06-01 06:55:49.958227 bagbag-0.61.9/src/bagbag/Random/src.py
+-rw-r--r--   0        0        0      510 2023-07-19 13:13:12.245619 bagbag-0.61.9/src/bagbag/Socket/TCP/__init__.py
+-rw-r--r--   0        0        0     5127 2023-07-19 13:27:38.761011 bagbag-0.61.9/src/bagbag/Socket/TCP/src.py
+-rw-r--r--   0        0        0       17 2023-05-12 12:35:25.860105 bagbag-0.61.9/src/bagbag/Socket/__init__.py
+-rw-r--r--   0        0        0      352 2023-05-12 12:35:25.865416 bagbag-0.61.9/src/bagbag/String/__init__.py
+-rw-r--r--   0        0        0    16972 2023-07-18 06:50:49.901739 bagbag-0.61.9/src/bagbag/String/src.py
+-rw-r--r--   0        0        0      367 2023-05-12 12:35:25.865783 bagbag-0.61.9/src/bagbag/Thread/__init__.py
+-rw-r--r--   0        0        0     1127 2023-06-15 09:24:51.853905 bagbag-0.61.9/src/bagbag/Thread/src.py
+-rw-r--r--   0        0        0      571 2023-06-15 06:22:08.764134 bagbag-0.61.9/src/bagbag/Time/__init__.py
+-rw-r--r--   0        0        0     6061 2023-06-15 06:30:18.558975 bagbag-0.61.9/src/bagbag/Time/src.py
+-rw-r--r--   0        0        0     2449 2023-05-12 12:35:25.818366 bagbag-0.61.9/src/bagbag/Tools/Argparser_src.py
+-rw-r--r--   0        0        0     2613 2023-05-12 12:35:25.825531 bagbag-0.61.9/src/bagbag/Tools/BlockChain/Binance/CoinsPrice_src.py
+-rw-r--r--   0        0        0      350 2023-05-12 12:35:25.826469 bagbag-0.61.9/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/__init__.py
+-rw-r--r--   0        0        0      972 2023-05-12 12:35:25.826332 bagbag-0.61.9/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/src.py
+-rw-r--r--   0        0        0      509 2023-05-12 12:35:25.825419 bagbag-0.61.9/src/bagbag/Tools/BlockChain/Binance/__init__.py
+-rw-r--r--   0        0        0       36 2023-05-12 12:35:25.827257 bagbag-0.61.9/src/bagbag/Tools/BlockChain/Ethereum/__init__.py
+-rw-r--r--   0        0        0      325 2023-05-12 12:35:25.827344 bagbag-0.61.9/src/bagbag/Tools/BlockChain/Ethereum/ethereum.py
+-rw-r--r--   0        0        0      485 2023-05-12 12:35:25.824938 bagbag-0.61.9/src/bagbag/Tools/BlockChain/Tron/__init__.py
+-rw-r--r--   0        0        0    24277 2023-07-06 05:43:43.753694 bagbag-0.61.9/src/bagbag/Tools/BlockChain/Tron/src.py
+-rw-r--r--   0        0        0      381 2023-07-04 14:12:42.665691 bagbag-0.61.9/src/bagbag/Tools/BlockChain/__init__.py
+-rw-r--r--   0        0        0     3277 2023-06-05 15:36:04.503828 bagbag-0.61.9/src/bagbag/Tools/CSV.py
+-rw-r--r--   0        0        0     4615 2023-06-09 06:22:43.542806 bagbag-0.61.9/src/bagbag/Tools/Cache.py
+-rw-r--r--   0        0        0     3886 2023-05-12 12:35:25.816327 bagbag-0.61.9/src/bagbag/Tools/Chan_src.py
+-rw-r--r--   0        0        0    32941 2023-05-29 11:13:19.619696 bagbag-0.61.9/src/bagbag/Tools/ComputerVision.py
+-rw-r--r--   0        0        0     3238 2023-05-29 11:10:20.747420 bagbag-0.61.9/src/bagbag/Tools/Crontab_src.py
+-rw-r--r--   0        0        0      644 2023-05-12 12:35:25.856714 bagbag-0.61.9/src/bagbag/Tools/Database/__init__.py
+-rw-r--r--   0        0        0      297 2023-05-12 12:35:25.830525 bagbag-0.61.9/src/bagbag/Tools/Database/orator/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-12 12:35:25.830659 bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/__init__.py
+-rw-r--r--   0        0        0      785 2023-05-12 12:35:25.830739 bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/application.py
+-rw-r--r--   0        0        0     3436 2023-05-12 12:35:25.830822 bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/command.py
+-rw-r--r--   0        0        0      330 2023-05-12 12:35:25.830964 bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/migrations/__init__.py
+-rw-r--r--   0        0        0      186 2023-05-12 12:35:25.831040 bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/migrations/base_command.py
+-rw-r--r--   0        0        0      626 2023-05-12 12:35:25.831123 bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/migrations/install_command.py
+-rw-r--r--   0        0        0     1301 2023-05-12 12:35:25.831226 bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/migrations/make_command.py
+-rw-r--r--   0        0        0     2343 2023-05-12 12:35:25.831313 bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/migrations/migrate_command.py
+-rw-r--r--   0        0        0     1886 2023-05-12 12:35:25.831395 bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/migrations/refresh_command.py
+-rw-r--r--   0        0        0     1308 2023-05-12 12:35:25.831488 bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/migrations/reset_command.py
+-rw-r--r--   0        0        0     1315 2023-05-12 12:35:25.831583 bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/migrations/rollback_command.py
+-rw-r--r--   0        0        0     1642 2023-05-12 12:35:25.831666 bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/migrations/status_command.py
+-rw-r--r--   0        0        0       68 2023-05-12 12:35:25.831798 bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/models/__init__.py
+-rw-r--r--   0        0        0     2217 2023-05-12 12:35:25.831874 bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/models/make_command.py
+-rw-r--r--   0        0        0      115 2023-05-12 12:35:25.831968 bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/models/stubs.py
+-rw-r--r--   0        0        0      108 2023-05-12 12:35:25.832158 bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/seeds/__init__.py
+-rw-r--r--   0        0        0      178 2023-05-12 12:35:25.832248 bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/seeds/base_command.py
+-rw-r--r--   0        0        0     2204 2023-05-12 12:35:25.832352 bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/seeds/make_command.py
+-rw-r--r--   0        0        0     1923 2023-05-12 12:35:25.832446 bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/seeds/seed_command.py
+-rw-r--r--   0        0        0      206 2023-05-12 12:35:25.832590 bagbag-0.61.9/src/bagbag/Tools/Database/orator/connections/__init__.py
+-rw-r--r--   0        0        0    15063 2023-05-12 12:35:25.832673 bagbag-0.61.9/src/bagbag/Tools/Database/orator/connections/connection.py
+-rw-r--r--   0        0        0     4112 2023-05-12 12:35:25.832759 bagbag-0.61.9/src/bagbag/Tools/Database/orator/connections/connection_interface.py
+-rw-r--r--   0        0        0      298 2023-05-12 12:35:25.832861 bagbag-0.61.9/src/bagbag/Tools/Database/orator/connections/connection_resolver_interface.py
+-rw-r--r--   0        0        0     2218 2023-05-12 12:35:25.832962 bagbag-0.61.9/src/bagbag/Tools/Database/orator/connections/mysql_connection.py
+-rw-r--r--   0        0        0     2056 2023-05-12 12:35:25.833055 bagbag-0.61.9/src/bagbag/Tools/Database/orator/connections/postgres_connection.py
+-rw-r--r--   0        0        0     1588 2023-05-12 12:35:25.833159 bagbag-0.61.9/src/bagbag/Tools/Database/orator/connections/sqlite_connection.py
+-rw-r--r--   0        0        0      198 2023-05-12 12:35:25.833971 bagbag-0.61.9/src/bagbag/Tools/Database/orator/connectors/__init__.py
+-rw-r--r--   0        0        0     3133 2023-05-12 12:35:25.834056 bagbag-0.61.9/src/bagbag/Tools/Database/orator/connectors/connection_factory.py
+-rw-r--r--   0        0        0     3106 2023-05-12 12:35:25.834129 bagbag-0.61.9/src/bagbag/Tools/Database/orator/connectors/connector.py
+-rw-r--r--   0        0        0     3982 2023-05-12 12:35:25.834204 bagbag-0.61.9/src/bagbag/Tools/Database/orator/connectors/mysql_connector.py
+-rw-r--r--   0        0        0     3280 2023-05-12 12:35:25.834291 bagbag-0.61.9/src/bagbag/Tools/Database/orator/connectors/postgres_connector.py
+-rw-r--r--   0        0        0     2172 2023-05-12 12:35:25.834370 bagbag-0.61.9/src/bagbag/Tools/Database/orator/connectors/sqlite_connector.py
+-rw-r--r--   0        0        0     5089 2023-05-12 12:35:25.835189 bagbag-0.61.9/src/bagbag/Tools/Database/orator/database_manager.py
+-rw-r--r--   0        0        0       24 2023-05-12 12:35:25.835796 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/__init__.py
+-rw-r--r--   0        0        0     2372 2023-05-12 12:35:25.835903 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/abstract_asset.py
+-rw-r--r--   0        0        0     3447 2023-05-12 12:35:25.835999 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/column.py
+-rw-r--r--   0        0        0      545 2023-05-12 12:35:25.836087 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/column_diff.py
+-rw-r--r--   0        0        0    11219 2023-05-12 12:35:25.836174 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/comparator.py
+-rw-r--r--   0        0        0     1943 2023-05-12 12:35:25.836319 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/exceptions/__init__.py
+-rw-r--r--   0        0        0     8193 2023-05-12 12:35:25.836678 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/foreign_key_constraint.py
+-rw-r--r--   0        0        0      173 2023-05-12 12:35:25.836774 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/identifier.py
+-rw-r--r--   0        0        0     7094 2023-05-12 12:35:25.836858 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/index.py
+-rw-r--r--   0        0        0     5260 2023-05-12 12:35:25.836935 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/mysql_schema_manager.py
+-rw-r--r--   0        0        0      205 2023-05-12 12:35:25.837074 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/platforms/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-12 12:35:25.837217 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-12 12:35:25.837297 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/keyword_list.py
+-rw-r--r--   0        0        0     4383 2023-05-12 12:35:25.837375 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/mysql_keywords.py
+-rw-r--r--   0        0        0     1730 2023-05-12 12:35:25.837455 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/postgresql_keywords.py
+-rw-r--r--   0        0        0     2315 2023-05-12 12:35:25.837531 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/sqlite_keywords.py
+-rw-r--r--   0        0        0     1289 2023-05-12 12:35:25.838118 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/platforms/mysql57_platform.py
+-rw-r--r--   0        0        0     9489 2023-05-12 12:35:25.838202 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/platforms/mysql_platform.py
+-rw-r--r--   0        0        0    21672 2023-05-12 12:35:25.838290 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/platforms/platform.py
+-rw-r--r--   0        0        0    14126 2023-05-12 12:35:25.838370 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/platforms/postgres_platform.py
+-rw-r--r--   0        0        0    20833 2023-05-12 12:35:25.838457 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/platforms/sqlite_platform.py
+-rw-r--r--   0        0        0     6014 2023-05-12 12:35:25.839154 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/postgres_schema_manager.py
+-rw-r--r--   0        0        0     4240 2023-05-12 12:35:25.839242 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/schema_manager.py
+-rw-r--r--   0        0        0     5458 2023-05-12 12:35:25.839325 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/sqlite_schema_manager.py
+-rw-r--r--   0        0        0    17146 2023-05-12 12:35:25.839403 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/table.py
+-rw-r--r--   0        0        0     1436 2023-05-12 12:35:25.839495 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/table_diff.py
+-rw-r--r--   0        0        0       24 2023-05-12 12:35:25.839639 bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/types/__init__.py
+-rw-r--r--   0        0        0      992 2023-05-12 12:35:25.840999 bagbag-0.61.9/src/bagbag/Tools/Database/orator/events/__init__.py
+-rw-r--r--   0        0        0       68 2023-05-12 12:35:25.841361 bagbag-0.61.9/src/bagbag/Tools/Database/orator/exceptions/__init__.py
+-rw-r--r--   0        0        0      193 2023-05-12 12:35:25.841461 bagbag-0.61.9/src/bagbag/Tools/Database/orator/exceptions/connection.py
+-rw-r--r--   0        0        0      822 2023-05-12 12:35:25.841563 bagbag-0.61.9/src/bagbag/Tools/Database/orator/exceptions/connectors.py
+-rw-r--r--   0        0        0      551 2023-05-12 12:35:25.841649 bagbag-0.61.9/src/bagbag/Tools/Database/orator/exceptions/orm.py
+-rw-r--r--   0        0        0      494 2023-05-12 12:35:25.841746 bagbag-0.61.9/src/bagbag/Tools/Database/orator/exceptions/query.py
+-rw-r--r--   0        0        0      208 2023-05-12 12:35:25.842330 bagbag-0.61.9/src/bagbag/Tools/Database/orator/migrations/__init__.py
+-rw-r--r--   0        0        0     2730 2023-05-12 12:35:25.842410 bagbag-0.61.9/src/bagbag/Tools/Database/orator/migrations/database_migration_repository.py
+-rw-r--r--   0        0        0      425 2023-05-12 12:35:25.842506 bagbag-0.61.9/src/bagbag/Tools/Database/orator/migrations/migration.py
+-rw-r--r--   0        0        0     2588 2023-05-12 12:35:25.842583 bagbag-0.61.9/src/bagbag/Tools/Database/orator/migrations/migration_creator.py
+-rw-r--r--   0        0        0     7754 2023-05-12 12:35:25.842660 bagbag-0.61.9/src/bagbag/Tools/Database/orator/migrations/migrator.py
+-rw-r--r--   0        0        0     1114 2023-05-12 12:35:25.842735 bagbag-0.61.9/src/bagbag/Tools/Database/orator/migrations/stubs.py
+-rw-r--r--   0        0        0      419 2023-05-12 12:35:25.842873 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/__init__.py
+-rw-r--r--   0        0        0    32311 2023-05-12 12:35:25.842946 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/builder.py
+-rw-r--r--   0        0        0      814 2023-05-12 12:35:25.843014 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/collection.py
+-rw-r--r--   0        0        0     7481 2023-05-12 12:35:25.843112 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/factory.py
+-rw-r--r--   0        0        0     2579 2023-05-12 12:35:25.843207 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/factory_builder.py
+-rw-r--r--   0        0        0       63 2023-05-12 12:35:25.843408 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/mixins/__init__.py
+-rw-r--r--   0        0        0     3532 2023-05-12 12:35:25.843502 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/mixins/soft_deletes.py
+-rw-r--r--   0        0        0    75367 2023-05-12 12:35:25.843880 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/model.py
+-rw-r--r--   0        0        0      371 2023-05-12 12:35:25.844072 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/__init__.py
+-rw-r--r--   0        0        0     5427 2023-05-12 12:35:25.844163 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/belongs_to.py
+-rw-r--r--   0        0        0    23248 2023-05-12 12:35:25.844271 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/belongs_to_many.py
+-rw-r--r--   0        0        0     1012 2023-05-12 12:35:25.844373 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/has_many.py
+-rw-r--r--   0        0        0     5126 2023-05-12 12:35:25.844473 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/has_many_through.py
+-rw-r--r--   0        0        0      955 2023-05-12 12:35:25.844558 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/has_one.py
+-rw-r--r--   0        0        0     8617 2023-05-12 12:35:25.844637 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/has_one_or_many.py
+-rw-r--r--   0        0        0      899 2023-05-12 12:35:25.844716 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/morph_many.py
+-rw-r--r--   0        0        0      843 2023-05-12 12:35:25.844810 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/morph_one.py
+-rw-r--r--   0        0        0     5377 2023-05-12 12:35:25.844920 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/morph_one_or_many.py
+-rw-r--r--   0        0        0      984 2023-05-12 12:35:25.845022 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/morph_pivot.py
+-rw-r--r--   0        0        0     5293 2023-05-12 12:35:25.845127 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/morph_to.py
+-rw-r--r--   0        0        0     3555 2023-05-12 12:35:25.845220 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/morph_to_many.py
+-rw-r--r--   0        0        0     2978 2023-05-12 12:35:25.845313 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/pivot.py
+-rw-r--r--   0        0        0     5956 2023-05-12 12:35:25.845401 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/relation.py
+-rw-r--r--   0        0        0      685 2023-05-12 12:35:25.845502 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/result.py
+-rw-r--r--   0        0        0     1106 2023-05-12 12:35:25.845583 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/wrapper.py
+-rw-r--r--   0        0        0       95 2023-05-12 12:35:25.847154 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/scopes/__init__.py
+-rw-r--r--   0        0        0      348 2023-05-12 12:35:25.847229 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/scopes/scope.py
+-rw-r--r--   0        0        0     3900 2023-05-12 12:35:25.847308 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/scopes/soft_deleting.py
+-rw-r--r--   0        0        0    13642 2023-05-12 12:35:25.847743 bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/utils.py
+-rw-r--r--   0        0        0      115 2023-05-12 12:35:25.848559 bagbag-0.61.9/src/bagbag/Tools/Database/orator/pagination/__init__.py
+-rw-r--r--   0        0        0     2251 2023-05-12 12:35:25.848628 bagbag-0.61.9/src/bagbag/Tools/Database/orator/pagination/base.py
+-rw-r--r--   0        0        0     2426 2023-05-12 12:35:25.848698 bagbag-0.61.9/src/bagbag/Tools/Database/orator/pagination/length_aware_paginator.py
+-rw-r--r--   0        0        0     2216 2023-05-12 12:35:25.848764 bagbag-0.61.9/src/bagbag/Tools/Database/orator/pagination/paginator.py
+-rw-r--r--   0        0        0       59 2023-05-12 12:35:25.849247 bagbag-0.61.9/src/bagbag/Tools/Database/orator/query/__init__.py
+-rw-r--r--   0        0        0    44030 2023-05-12 12:35:25.849322 bagbag-0.61.9/src/bagbag/Tools/Database/orator/query/builder.py
+-rw-r--r--   0        0        0      230 2023-05-12 12:35:25.849403 bagbag-0.61.9/src/bagbag/Tools/Database/orator/query/expression.py
+-rw-r--r--   0        0        0      202 2023-05-12 12:35:25.849583 bagbag-0.61.9/src/bagbag/Tools/Database/orator/query/grammars/__init__.py
+-rw-r--r--   0        0        0    13999 2023-05-12 12:35:25.849662 bagbag-0.61.9/src/bagbag/Tools/Database/orator/query/grammars/grammar.py
+-rw-r--r--   0        0        0     3559 2023-05-12 12:35:25.849810 bagbag-0.61.9/src/bagbag/Tools/Database/orator/query/grammars/mysql_grammar.py
+-rw-r--r--   0        0        0     4461 2023-05-12 12:35:25.849897 bagbag-0.61.9/src/bagbag/Tools/Database/orator/query/grammars/postgres_grammar.py
+-rw-r--r--   0        0        0     4204 2023-05-12 12:35:25.849974 bagbag-0.61.9/src/bagbag/Tools/Database/orator/query/grammars/sqlite_grammar.py
+-rw-r--r--   0        0        0     1407 2023-05-12 12:35:25.850460 bagbag-0.61.9/src/bagbag/Tools/Database/orator/query/join_clause.py
+-rw-r--r--   0        0        0      218 2023-05-12 12:35:25.850604 bagbag-0.61.9/src/bagbag/Tools/Database/orator/query/processors/__init__.py
+-rw-r--r--   0        0        0     1790 2023-05-12 12:35:25.850669 bagbag-0.61.9/src/bagbag/Tools/Database/orator/query/processors/mysql_processor.py
+-rw-r--r--   0        0        0     1160 2023-05-12 12:35:25.850732 bagbag-0.61.9/src/bagbag/Tools/Database/orator/query/processors/postgres_processor.py
+-rw-r--r--   0        0        0     1423 2023-05-12 12:35:25.850798 bagbag-0.61.9/src/bagbag/Tools/Database/orator/query/processors/processor.py
+-rw-r--r--   0        0        0      422 2023-05-12 12:35:25.850863 bagbag-0.61.9/src/bagbag/Tools/Database/orator/query/processors/sqlite_processor.py
+-rw-r--r--   0        0        0      166 2023-05-12 12:35:25.851787 bagbag-0.61.9/src/bagbag/Tools/Database/orator/schema/__init__.py
+-rw-r--r--   0        0        0    19482 2023-05-12 12:35:25.851871 bagbag-0.61.9/src/bagbag/Tools/Database/orator/schema/blueprint.py
+-rw-r--r--   0        0        0     3617 2023-05-12 12:35:25.851961 bagbag-0.61.9/src/bagbag/Tools/Database/orator/schema/builder.py
+-rw-r--r--   0        0        0      206 2023-05-12 12:35:25.852130 bagbag-0.61.9/src/bagbag/Tools/Database/orator/schema/grammars/__init__.py
+-rw-r--r--   0        0        0     9880 2023-05-12 12:35:25.852215 bagbag-0.61.9/src/bagbag/Tools/Database/orator/schema/grammars/grammar.py
+-rw-r--r--   0        0        0     8503 2023-05-12 12:35:25.852316 bagbag-0.61.9/src/bagbag/Tools/Database/orator/schema/grammars/mysql_grammar.py
+-rw-r--r--   0        0        0     7103 2023-05-12 12:35:25.852415 bagbag-0.61.9/src/bagbag/Tools/Database/orator/schema/grammars/postgres_grammar.py
+-rw-r--r--   0        0        0     8321 2023-05-12 12:35:25.852524 bagbag-0.61.9/src/bagbag/Tools/Database/orator/schema/grammars/sqlite_grammar.py
+-rw-r--r--   0        0        0     1229 2023-05-12 12:35:25.853214 bagbag-0.61.9/src/bagbag/Tools/Database/orator/schema/mysql_builder.py
+-rw-r--r--   0        0        0      645 2023-05-12 12:35:25.853314 bagbag-0.61.9/src/bagbag/Tools/Database/orator/schema/schema.py
+-rw-r--r--   0        0        0       52 2023-05-12 12:35:25.854121 bagbag-0.61.9/src/bagbag/Tools/Database/orator/seeds/__init__.py
+-rw-r--r--   0        0        0     1730 2023-05-12 12:35:25.854207 bagbag-0.61.9/src/bagbag/Tools/Database/orator/seeds/seeder.py
+-rw-r--r--   0        0        0      203 2023-05-12 12:35:25.854288 bagbag-0.61.9/src/bagbag/Tools/Database/orator/seeds/stubs.py
+-rw-r--r--   0        0        0       60 2023-05-12 12:35:25.854476 bagbag-0.61.9/src/bagbag/Tools/Database/orator/support/__init__.py
+-rw-r--r--   0        0        0      121 2023-05-12 12:35:25.854566 bagbag-0.61.9/src/bagbag/Tools/Database/orator/support/collection.py
+-rw-r--r--   0        0        0     2193 2023-05-12 12:35:25.854656 bagbag-0.61.9/src/bagbag/Tools/Database/orator/support/fluent.py
+-rw-r--r--   0        0        0     2614 2023-05-12 12:35:25.854751 bagbag-0.61.9/src/bagbag/Tools/Database/orator/support/grammar.py
+-rw-r--r--   0        0        0     2833 2023-05-12 12:35:25.855426 bagbag-0.61.9/src/bagbag/Tools/Database/orator/utils/__init__.py
+-rw-r--r--   0        0        0     4398 2023-05-12 12:35:25.855517 bagbag-0.61.9/src/bagbag/Tools/Database/orator/utils/command_formatter.py
+-rw-r--r--   0        0        0      749 2023-05-12 12:35:25.855603 bagbag-0.61.9/src/bagbag/Tools/Database/orator/utils/helpers.py
+-rw-r--r--   0        0        0      714 2023-05-12 12:35:25.855706 bagbag-0.61.9/src/bagbag/Tools/Database/orator/utils/qmarker.py
+-rw-r--r--   0        0        0     7566 2023-05-12 12:35:25.855800 bagbag-0.61.9/src/bagbag/Tools/Database/orator/utils/url.py
+-rw-r--r--   0        0        0    33362 2023-07-03 09:42:07.366549 bagbag-0.61.9/src/bagbag/Tools/Database/src.py
+-rw-r--r--   0        0        0     5250 2023-05-29 11:10:33.731697 bagbag-0.61.9/src/bagbag/Tools/DistributedLock_src.py
+-rw-r--r--   0        0        0     4674 2023-05-29 11:10:40.751258 bagbag-0.61.9/src/bagbag/Tools/Elasticsearch_src.py
+-rw-r--r--   0        0        0     4312 2023-05-29 11:10:51.912539 bagbag-0.61.9/src/bagbag/Tools/Github_src.py
+-rw-r--r--   0        0        0     1451 2023-05-12 12:35:25.827625 bagbag-0.61.9/src/bagbag/Tools/JavaScript_src.py
+-rw-r--r--   0        0        0    10096 2023-06-09 08:35:54.469473 bagbag-0.61.9/src/bagbag/Tools/Kafka_src.py
+-rw-r--r--   0        0        0     2028 2023-05-12 12:35:25.815942 bagbag-0.61.9/src/bagbag/Tools/Lock_src.py
+-rw-r--r--   0        0        0     6634 2023-05-29 11:11:12.945317 bagbag-0.61.9/src/bagbag/Tools/MatrixBot_src.py
+-rw-r--r--   0        0        0      466 2023-05-12 12:35:25.821432 bagbag-0.61.9/src/bagbag/Tools/Nslookup_src.py
+-rw-r--r--   0        0        0     2364 2023-05-29 11:11:50.231133 bagbag-0.61.9/src/bagbag/Tools/OCR_src.py
+-rw-r--r--   0        0        0     2816 2023-05-12 12:35:25.815348 bagbag-0.61.9/src/bagbag/Tools/ProgressBar_src.py
+-rw-r--r--   0        0        0     1660 2023-05-12 12:35:25.821643 bagbag-0.61.9/src/bagbag/Tools/Prometheus/MetricServer.py
+-rw-r--r--   0        0        0     3337 2023-06-07 15:52:43.922791 bagbag-0.61.9/src/bagbag/Tools/Prometheus/PushGateway.py
+-rw-r--r--   0        0        0      127 2023-05-12 12:35:25.821766 bagbag-0.61.9/src/bagbag/Tools/Prometheus/__init__.py
+-rw-r--r--   0        0        0     4670 2023-05-12 12:35:25.821993 bagbag-0.61.9/src/bagbag/Tools/Prometheus/metrics.py
+-rw-r--r--   0        0        0     2607 2023-05-29 11:12:14.997684 bagbag-0.61.9/src/bagbag/Tools/Queue_src.py
+-rw-r--r--   0        0        0     2490 2023-05-12 12:35:25.821196 bagbag-0.61.9/src/bagbag/Tools/RSS/Feed.py
+-rw-r--r--   0        0        0      661 2023-05-12 12:35:25.820920 bagbag-0.61.9/src/bagbag/Tools/RSS/Opml.py
+-rw-r--r--   0        0        0      119 2023-05-12 12:35:25.821062 bagbag-0.61.9/src/bagbag/Tools/RSS/__init__.py
+-rw-r--r--   0        0        0     3688 2023-05-12 12:35:25.816210 bagbag-0.61.9/src/bagbag/Tools/Ratelimit_src.py
+-rw-r--r--   0        0        0    18451 2023-05-29 11:12:03.251797 bagbag-0.61.9/src/bagbag/Tools/Redis_src.py
+-rw-r--r--   0        0        0     5609 2023-07-09 07:33:46.935788 bagbag-0.61.9/src/bagbag/Tools/SSH_src.py
+-rw-r--r--   0        0        0    34757 2023-07-18 07:42:48.217790 bagbag-0.61.9/src/bagbag/Tools/Selenium.py
+-rw-r--r--   0        0        0    14131 2023-05-12 12:35:25.820287 bagbag-0.61.9/src/bagbag/Tools/TelegramAsync.py
+-rw-r--r--   0        0        0     5111 2023-05-12 12:35:25.816456 bagbag-0.61.9/src/bagbag/Tools/TelegramBotOfficial_src.py
+-rw-r--r--   0        0        0     3069 2023-06-14 11:27:42.444891 bagbag-0.61.9/src/bagbag/Tools/TelegramBot_src.py
+-rw-r--r--   0        0        0    24676 2023-06-13 19:08:29.204793 bagbag-0.61.9/src/bagbag/Tools/Telegram_src.py
+-rw-r--r--   0        0        0      142 2023-05-12 12:35:25.824483 bagbag-0.61.9/src/bagbag/Tools/Test.py
+-rw-r--r--   0        0        0     4276 2023-05-12 12:35:25.819888 bagbag-0.61.9/src/bagbag/Tools/Translater_src.py
+-rw-r--r--   0        0        0    14103 2023-06-19 07:22:24.505061 bagbag-0.61.9/src/bagbag/Tools/Twitter/Browser_src.py
+-rw-r--r--   0        0        0    12718 2023-07-18 12:42:14.412719 bagbag-0.61.9/src/bagbag/Tools/Twitter/Elevated_src.py
+-rw-r--r--   0        0        0     2093 2023-05-26 13:18:47.657372 bagbag-0.61.9/src/bagbag/Tools/Twitter/Essential_src.py
+-rw-r--r--   0        0        0    29231 2023-07-25 09:02:23.817855 bagbag-0.61.9/src/bagbag/Tools/Twitter/Nitter_src.py
+-rw-r--r--   0        0        0     2744 2023-06-16 08:15:42.223073 bagbag-0.61.9/src/bagbag/Tools/Twitter/Utils.py
+-rw-r--r--   0        0        0     1070 2023-07-19 12:53:41.487474 bagbag-0.61.9/src/bagbag/Tools/Twitter/__init__.py
+-rw-r--r--   0        0        0     3122 2023-05-12 12:35:25.816080 bagbag-0.61.9/src/bagbag/Tools/URL_src.py
+-rw-r--r--   0        0        0      767 2023-05-12 12:35:25.818906 bagbag-0.61.9/src/bagbag/Tools/WaitGroup_src.py
+-rw-r--r--   0        0        0     8126 2023-05-12 12:35:25.828462 bagbag-0.61.9/src/bagbag/Tools/WebCrawler_src.py
+-rw-r--r--   0        0        0     7040 2023-07-16 17:07:37.080346 bagbag-0.61.9/src/bagbag/Tools/WebServer_src.py
+-rw-r--r--   0        0        0     2911 2023-07-25 09:08:46.858292 bagbag-0.61.9/src/bagbag/Tools/XPath_src.py
+-rw-r--r--   0        0        0     3235 2023-05-16 08:49:31.768572 bagbag-0.61.9/src/bagbag/Tools/Xlsx.py
+-rw-r--r--   0        0        0     3528 2023-07-04 14:13:58.807237 bagbag-0.61.9/src/bagbag/Tools/__init__.py
+-rw-r--r--   0        0        0     4555 2023-06-17 10:44:24.595347 bagbag-0.61.9/src/bagbag/__init__.py
+-rw-r--r--   0        0        0    19723 1970-01-01 00:00:00.000000 bagbag-0.61.9/PKG-INFO
```

### Comparing `bagbag-0.61.8/LICENSE` & `bagbag-0.61.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/README.md` & `bagbag-0.61.9/README.md`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/pyproject.toml` & `bagbag-0.61.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bagbag"
-version = "0.61.8"
+version = "0.61.9"
 description = "An all in one python library"
 
 license = "MIT"
 
 authors = [
     "Darren"
 ]
```

### Comparing `bagbag-0.61.8/src/bagbag/Cmd/src.py` & `bagbag-0.61.9/src/bagbag/Cmd/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Cryptoo/src.py` & `bagbag-0.61.9/src/bagbag/Cryptoo/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/File/src.py` & `bagbag-0.61.9/src/bagbag/File/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Funcs/CutSentenceStopWords_src.py` & `bagbag-0.61.9/src/bagbag/Funcs/CutSentenceStopWords_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Funcs/CutSentence_src.py` & `bagbag-0.61.9/src/bagbag/Funcs/CutSentence_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Funcs/FakeIdentity_src.py` & `bagbag-0.61.9/src/bagbag/Funcs/FakeIdentity_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Funcs/FileType_src.py` & `bagbag-0.61.9/src/bagbag/Funcs/FileType_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Funcs/Format/src.py` & `bagbag-0.61.9/src/bagbag/Funcs/Format/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Funcs/GetPublicIP_src.py` & `bagbag-0.61.9/src/bagbag/Funcs/GetPublicIP_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Funcs/Ping_src.py` & `bagbag-0.61.9/src/bagbag/Funcs/Ping_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Funcs/ResizeImage_src.py` & `bagbag-0.61.9/src/bagbag/Funcs/ResizeImage_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Funcs/Wget_src.py` & `bagbag-0.61.9/src/bagbag/Funcs/Wget_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Funcs/__init__.py` & `bagbag-0.61.9/src/bagbag/Funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Hash/__init__.py` & `bagbag-0.61.9/src/bagbag/Hash/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Hash/src.py` & `bagbag-0.61.9/src/bagbag/Hash/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Http/__init__.py` & `bagbag-0.61.9/src/bagbag/Http/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Http/src.py` & `bagbag-0.61.9/src/bagbag/Http/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Json/src.py` & `bagbag-0.61.9/src/bagbag/Json/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Lg.py` & `bagbag-0.61.9/src/bagbag/Lg.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Math/src.py` & `bagbag-0.61.9/src/bagbag/Math/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Os/Path/__init__.py` & `bagbag-0.61.9/src/bagbag/Os/Path/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Os/Path/src.py` & `bagbag-0.61.9/src/bagbag/Os/Path/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Os/__init__.py` & `bagbag-0.61.9/src/bagbag/Os/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Os/src.py` & `bagbag-0.61.9/src/bagbag/Os/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Process/src.py` & `bagbag-0.61.9/src/bagbag/Process/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Python/src.py` & `bagbag-0.61.9/src/bagbag/Python/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Random/src.py` & `bagbag-0.61.9/src/bagbag/Random/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Socket/TCP/src.py` & `bagbag-0.61.9/src/bagbag/Socket/TCP/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/String/src.py` & `bagbag-0.61.9/src/bagbag/String/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Thread/src.py` & `bagbag-0.61.9/src/bagbag/Thread/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Time/__init__.py` & `bagbag-0.61.9/src/bagbag/Time/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Time/src.py` & `bagbag-0.61.9/src/bagbag/Time/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Argparser_src.py` & `bagbag-0.61.9/src/bagbag/Tools/Argparser_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/BlockChain/Binance/CoinsPrice_src.py` & `bagbag-0.61.9/src/bagbag/Tools/BlockChain/Binance/CoinsPrice_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/src.py` & `bagbag-0.61.9/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/BlockChain/Tron/src.py` & `bagbag-0.61.9/src/bagbag/Tools/BlockChain/Tron/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/CSV.py` & `bagbag-0.61.9/src/bagbag/Tools/CSV.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Cache.py` & `bagbag-0.61.9/src/bagbag/Tools/Cache.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Chan_src.py` & `bagbag-0.61.9/src/bagbag/Tools/Chan_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/ComputerVision.py` & `bagbag-0.61.9/src/bagbag/Tools/ComputerVision.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Crontab_src.py` & `bagbag-0.61.9/src/bagbag/Tools/Crontab_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/__init__.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/application.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/application.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/command.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/migrations/install_command.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/migrations/install_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/migrations/make_command.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/migrations/make_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/migrations/migrate_command.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/migrations/migrate_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/migrations/refresh_command.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/migrations/refresh_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/migrations/reset_command.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/migrations/reset_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/migrations/rollback_command.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/migrations/rollback_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/migrations/status_command.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/migrations/status_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/models/make_command.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/models/make_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/seeds/make_command.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/seeds/make_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/commands/seeds/seed_command.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/commands/seeds/seed_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/connections/connection.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/connections/connection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/connections/connection_interface.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/connections/connection_interface.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/connections/mysql_connection.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/connections/mysql_connection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/connections/postgres_connection.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/connections/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/connections/sqlite_connection.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/connections/sqlite_connection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/connectors/connection_factory.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/connectors/connection_factory.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/connectors/connector.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/connectors/connector.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/connectors/mysql_connector.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/connectors/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/connectors/postgres_connector.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/connectors/postgres_connector.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/connectors/sqlite_connector.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/connectors/sqlite_connector.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/database_manager.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/database_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/abstract_asset.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/abstract_asset.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/column.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/column.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/column_diff.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/column_diff.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/comparator.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/comparator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/exceptions/__init__.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/foreign_key_constraint.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/foreign_key_constraint.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/index.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/index.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/mysql_schema_manager.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/mysql_schema_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/mysql_keywords.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/mysql_keywords.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/postgresql_keywords.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/postgresql_keywords.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/sqlite_keywords.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/sqlite_keywords.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/platforms/mysql57_platform.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/platforms/mysql57_platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/platforms/mysql_platform.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/platforms/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/platforms/platform.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/platforms/platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/platforms/postgres_platform.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/platforms/postgres_platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/platforms/sqlite_platform.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/platforms/sqlite_platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/postgres_schema_manager.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/postgres_schema_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/schema_manager.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/schema_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/sqlite_schema_manager.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/sqlite_schema_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/table.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/table.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/dbal/table_diff.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/dbal/table_diff.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/events/__init__.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/events/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/exceptions/connectors.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/exceptions/connectors.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/exceptions/orm.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/exceptions/orm.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/migrations/database_migration_repository.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/migrations/database_migration_repository.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/migrations/migration_creator.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/migrations/migration_creator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/migrations/migrator.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/migrations/migrator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/migrations/stubs.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/migrations/stubs.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/builder.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/collection.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/collection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/factory.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/factory.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/factory_builder.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/factory_builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/mixins/soft_deletes.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/mixins/soft_deletes.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/model.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/model.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/belongs_to.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/belongs_to.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/belongs_to_many.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/belongs_to_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/has_many.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/has_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/has_many_through.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/has_many_through.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/has_one.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/has_one.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/has_one_or_many.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/has_one_or_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/morph_many.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/morph_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/morph_one.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/morph_one.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/morph_one_or_many.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/morph_one_or_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/morph_pivot.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/morph_pivot.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/morph_to.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/morph_to.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/morph_to_many.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/morph_to_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/pivot.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/pivot.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/relation.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/relation.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/result.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/result.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/relations/wrapper.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/relations/wrapper.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/scopes/soft_deleting.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/scopes/soft_deleting.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/orm/utils.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/orm/utils.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/pagination/base.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/pagination/base.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/pagination/length_aware_paginator.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/pagination/length_aware_paginator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/pagination/paginator.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/pagination/paginator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/query/builder.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/query/builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/query/grammars/grammar.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/query/grammars/grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/query/grammars/mysql_grammar.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/query/grammars/mysql_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/query/grammars/postgres_grammar.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/query/grammars/postgres_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/query/grammars/sqlite_grammar.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/query/grammars/sqlite_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/query/join_clause.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/query/join_clause.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/query/processors/mysql_processor.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/query/processors/mysql_processor.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/query/processors/postgres_processor.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/query/processors/postgres_processor.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/query/processors/processor.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/query/processors/processor.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/schema/blueprint.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/schema/blueprint.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/schema/builder.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/schema/builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/schema/grammars/grammar.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/schema/grammars/grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/schema/grammars/mysql_grammar.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/schema/grammars/mysql_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/schema/grammars/postgres_grammar.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/schema/grammars/postgres_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/schema/grammars/sqlite_grammar.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/schema/grammars/sqlite_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/schema/mysql_builder.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/schema/mysql_builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/schema/schema.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/schema/schema.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/seeds/seeder.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/seeds/seeder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/support/fluent.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/support/fluent.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/support/grammar.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/support/grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/utils/__init__.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/utils/command_formatter.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/utils/command_formatter.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/utils/helpers.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/utils/qmarker.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/utils/qmarker.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/orator/utils/url.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/orator/utils/url.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Database/src.py` & `bagbag-0.61.9/src/bagbag/Tools/Database/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/DistributedLock_src.py` & `bagbag-0.61.9/src/bagbag/Tools/DistributedLock_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Elasticsearch_src.py` & `bagbag-0.61.9/src/bagbag/Tools/Elasticsearch_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Github_src.py` & `bagbag-0.61.9/src/bagbag/Tools/Github_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/JavaScript_src.py` & `bagbag-0.61.9/src/bagbag/Tools/JavaScript_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Kafka_src.py` & `bagbag-0.61.9/src/bagbag/Tools/Kafka_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Lock_src.py` & `bagbag-0.61.9/src/bagbag/Tools/Lock_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/MatrixBot_src.py` & `bagbag-0.61.9/src/bagbag/Tools/MatrixBot_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/OCR_src.py` & `bagbag-0.61.9/src/bagbag/Tools/OCR_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/ProgressBar_src.py` & `bagbag-0.61.9/src/bagbag/Tools/ProgressBar_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Prometheus/MetricServer.py` & `bagbag-0.61.9/src/bagbag/Tools/Prometheus/MetricServer.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Prometheus/PushGateway.py` & `bagbag-0.61.9/src/bagbag/Tools/Prometheus/PushGateway.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Prometheus/metrics.py` & `bagbag-0.61.9/src/bagbag/Tools/Prometheus/metrics.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Queue_src.py` & `bagbag-0.61.9/src/bagbag/Tools/Queue_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/RSS/Feed.py` & `bagbag-0.61.9/src/bagbag/Tools/RSS/Feed.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/RSS/Opml.py` & `bagbag-0.61.9/src/bagbag/Tools/RSS/Opml.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Ratelimit_src.py` & `bagbag-0.61.9/src/bagbag/Tools/Ratelimit_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Redis_src.py` & `bagbag-0.61.9/src/bagbag/Tools/Redis_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/SSH_src.py` & `bagbag-0.61.9/src/bagbag/Tools/SSH_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Selenium.py` & `bagbag-0.61.9/src/bagbag/Tools/Selenium.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/TelegramAsync.py` & `bagbag-0.61.9/src/bagbag/Tools/TelegramAsync.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/TelegramBotOfficial_src.py` & `bagbag-0.61.9/src/bagbag/Tools/TelegramBotOfficial_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/TelegramBot_src.py` & `bagbag-0.61.9/src/bagbag/Tools/TelegramBot_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Telegram_src.py` & `bagbag-0.61.9/src/bagbag/Tools/Telegram_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Translater_src.py` & `bagbag-0.61.9/src/bagbag/Tools/Translater_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Twitter/Browser_src.py` & `bagbag-0.61.9/src/bagbag/Tools/Twitter/Browser_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Twitter/Elevated_src.py` & `bagbag-0.61.9/src/bagbag/Tools/Twitter/Elevated_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Twitter/Essential_src.py` & `bagbag-0.61.9/src/bagbag/Tools/Twitter/Essential_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Twitter/Nitter_src.py` & `bagbag-0.61.9/src/bagbag/Tools/Twitter/Nitter_src.py`

 * *Files 1% similar despite different names*

```diff
@@ -651,15 +651,15 @@
 
         quota = mtx.Find("//div[@class='tweet-stats']/span[3]").Text().strip().replace(',', '')
         quota = int(quota) if String(quota).IsDigit() else 0
 
         like = mtx.Find("//div[@class='tweet-stats']/span[4]").Text().strip().replace(",", "")
         like = int(like) if String(like).IsDigit() else 0
 
-        # ipdb.set_trace()
+        ipdb.set_trace()
 
         # Lg.Trace({
         #     # "tid": tid,
         #     "username": username,
         #     "screenname": screenname,
         #     "text": text,
         #     "time": time,
@@ -752,20 +752,20 @@
 
     # # 只有一页
     # html = Http.Get("https://nitter.kavin.rocks/RDelaney/status/1679898053631782924#m").Content
     # File("tweet.detail.single.html").Write(html)
 
     # html = File("tweet.detail.html").Read()
 
-    # n = Nitter("nitter.kavin.rocks")
+    n = Nitter("nitter.kavin.rocks")
     # # t = n.getMainThreadInTweetPage(html)
 
-    # t = n.Tweet("cz_binance", 1681734275589189634)
+    t = n.Tweet(1651414032925204480)
 
-    # Lg.Trace(t)
+    Lg.Trace(t)
 
     # --- 测试获取服务器列表
 
     # n = Nitter()
     # servers = n.getServers()
     # n.selectServer(servers)
 
@@ -807,28 +807,28 @@
     # for t in n.Search("psychologist a paradox"):
     #     Lg.Trace(t.ID)
 
     # Lg.Trace(t.User)
 
     # ---- 调试 NitterTwitterUser - info 
 
-    n = Nitter("nitter.kavin.rocks")
+    # n = Nitter("nitter.kavin.rocks")
 
-    # Lg.Trace(ntu)
-    ntu = n.User("blahlaja")
+    # # Lg.Trace(ntu)
+    # ntu = n.User("blahlaja")
 
-    # html = File("user.4.verified.html").Read()
-    html = File("user.html").Read()
+    # # html = File("user.4.verified.html").Read()
+    # html = File("user.html").Read()
 
-    # ntu = n.User("binsingha")
-    # html = File("user.1.html").Read()
+    # # ntu = n.User("binsingha")
+    # # html = File("user.1.html").Read()
 
-    ntu.setInfoByHtml(html)
+    # ntu.setInfoByHtml(html)
 
-    Lg.Trace(ntu)
+    # Lg.Trace(ntu)
 
     # ---- 调试 NitterTwitterUser - info
 
     # 活动频繁, 好多转推
     # html = Http.Get("https://nitter.kavin.rocks/blahlaja").Content
     # File("user.html").Write(html)
 
@@ -861,8 +861,9 @@
     # for i in n.getTweetInHtml(html):
     #     Lg.Trace(i)
 
     # 其他
 
     # html = Http.Get("https://nitter.kavin.rocks/search?f=tweets&q=Si+on+prend+l%27argent+de+Musk%2C+Bezos+et+Arnault+et+qu%27on+le+redistribue+entre").Content
     # html = Http.Get("https://nitter.kavin.rocks/blahlaja").Content
-    # File("user.html").Write(html)
+    html = Http.Get("https://nitter.kavin.rocks/cz_binance/status/1651414032925204480#m").Content
+    File("tweet.url.in.text.html").Write(html)
```

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Twitter/Utils.py` & `bagbag-0.61.9/src/bagbag/Tools/Twitter/Utils.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Twitter/__init__.py` & `bagbag-0.61.9/src/bagbag/Tools/Twitter/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/URL_src.py` & `bagbag-0.61.9/src/bagbag/Tools/URL_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/WaitGroup_src.py` & `bagbag-0.61.9/src/bagbag/Tools/WaitGroup_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/WebCrawler_src.py` & `bagbag-0.61.9/src/bagbag/Tools/WebCrawler_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/WebServer_src.py` & `bagbag-0.61.9/src/bagbag/Tools/WebServer_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/Xlsx.py` & `bagbag-0.61.9/src/bagbag/Tools/Xlsx.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/Tools/__init__.py` & `bagbag-0.61.9/src/bagbag/Tools/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/src/bagbag/__init__.py` & `bagbag-0.61.9/src/bagbag/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.61.8/PKG-INFO` & `bagbag-0.61.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bagbag
-Version: 0.61.8
+Version: 0.61.9
 Summary: An all in one python library
 Home-page: https://github.com/darren2046/bagbag
 License: MIT
 Keywords: base,library
 Author: Darren
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
```

