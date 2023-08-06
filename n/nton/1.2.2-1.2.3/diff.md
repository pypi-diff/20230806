# Comparing `tmp/nton-1.2.2.tar.gz` & `tmp/nton-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nton-1.2.2.tar", max compression
+gzip compressed data, was "nton-1.2.3.tar", max compression
```

## Comparing `nton-1.2.2.tar` & `nton-1.2.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0    35823 2023-04-20 07:48:40.476933 nton-1.2.2/LICENSE
--rw-r--r--   0        0        0       23 2023-04-20 07:48:40.476933 nton-1.2.2/nton/__init__.py
--rw-r--r--   0        0        0     5669 2023-04-20 07:48:40.476933 nton-1.2.2/nton/assets/control.nacp.xml
--rw-r--r--   0        0        0    54085 2023-04-20 07:48:40.476933 nton-1.2.2/nton/assets/exefs/main
--rw-r--r--   0        0        0     1016 2023-04-20 07:48:40.476933 nton-1.2.2/nton/assets/exefs/main.npdm
--rw-r--r--   0        0        0      262 2023-04-20 07:48:40.476933 nton-1.2.2/nton/assets/logo/NintendoLogo.png
--rw-r--r--   0        0        0    51019 2023-04-20 07:48:40.476933 nton-1.2.2/nton/assets/logo/StartupMovie.gif
--rw-r--r--   0        0        0     1423 2023-04-20 07:48:40.476933 nton-1.2.2/nton/constants.py
--rw-r--r--   0        0        0    15843 2023-04-20 07:48:40.476933 nton-1.2.2/nton/main.py
--rw-r--r--   0        0        0     3339 2023-04-20 07:48:40.476933 nton-1.2.2/nton/nstool.py
--rw-r--r--   0        0        0    22034 2023-04-20 07:48:40.476933 nton-1.2.2/nton/title_ids.py
--rw-r--r--   0        0        0     1123 2023-04-20 07:48:40.476933 nton-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     8263 2023-04-20 07:48:40.476933 nton-1.2.2/README.md
--rw-r--r--   0        0        0     9626 1970-01-01 00:00:00.000000 nton-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-08-06 01:33:02.730366 nton-1.2.3/LICENSE
+-rw-r--r--   0        0        0       23 2023-08-06 01:33:02.730366 nton-1.2.3/nton/__init__.py
+-rw-r--r--   0        0        0     5669 2023-08-06 01:33:02.730366 nton-1.2.3/nton/assets/control.nacp.xml
+-rw-r--r--   0        0        0    54085 2023-08-06 01:33:02.730366 nton-1.2.3/nton/assets/exefs/main
+-rw-r--r--   0        0        0     1016 2023-08-06 01:33:02.730366 nton-1.2.3/nton/assets/exefs/main.npdm
+-rw-r--r--   0        0        0  1346956 2023-08-06 01:33:02.730366 nton-1.2.3/nton/assets/game_title_ids.json
+-rw-r--r--   0        0        0      262 2023-08-06 01:33:02.730366 nton-1.2.3/nton/assets/logo/NintendoLogo.png
+-rw-r--r--   0        0        0    51019 2023-08-06 01:33:02.730366 nton-1.2.3/nton/assets/logo/StartupMovie.gif
+-rw-r--r--   0        0        0     1199 2023-08-06 01:33:02.730366 nton-1.2.3/nton/constants.py
+-rw-r--r--   0        0        0    16102 2023-08-06 01:33:02.746055 nton-1.2.3/nton/main.py
+-rw-r--r--   0        0        0     3339 2023-08-06 01:33:02.746055 nton-1.2.3/nton/nstool.py
+-rw-r--r--   0        0        0    21726 2023-08-06 01:33:02.746055 nton-1.2.3/nton/title_ids.py
+-rw-r--r--   0        0        0     1122 2023-08-06 01:33:02.746055 nton-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0    11129 2023-08-06 01:33:02.730366 nton-1.2.3/README.md
+-rw-r--r--   0        0        0    12453 1970-01-01 00:00:00.000000 nton-1.2.3/PKG-INFO
```

### Comparing `nton-1.2.2/LICENSE` & `nton-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nton-1.2.2/nton/assets/control.nacp.xml` & `nton-1.2.3/nton/assets/control.nacp.xml`

 * *Files identical despite different names*

### Comparing `nton-1.2.2/nton/assets/exefs/main` & `nton-1.2.3/nton/assets/exefs/main`

 * *Files identical despite different names*

### Comparing `nton-1.2.2/nton/assets/exefs/main.npdm` & `nton-1.2.3/nton/assets/exefs/main.npdm`

 * *Files identical despite different names*

### Comparing `nton-1.2.2/nton/assets/logo/StartupMovie.gif` & `nton-1.2.3/nton/assets/logo/StartupMovie.gif`

 * *Files identical despite different names*

### Comparing `nton-1.2.2/nton/constants.py` & `nton-1.2.3/nton/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 import shutil
 import sys
 import tempfile
 from pathlib import Path
 
-from appdirs import AppDirs
-
 
 class Directories:
-    app_dirs = AppDirs("nton", "rlaphoenix")
     root = Path(__file__).resolve().parent  # root of package/src
-    user_configs = Path(app_dirs.user_config_dir)
-    data = Path(app_dirs.user_data_dir)
-    cache = Path(app_dirs.user_cache_dir)
-    logs = Path(app_dirs.user_log_dir)
     temp = Path(tempfile.gettempdir()) / "rlaphoenix-nton"
     output = Path.home() / "Desktop" / "NTON"
     assets = root / "assets"
 
 
 class Binaries:
     nstool = shutil.which("nstool")
     hacbrewpack = shutil.which("hacbrewpack")
     hptnacp = shutil.which("hptnacp")
-    magick = shutil.which("magick")
 
 
 class Files:
     keys_home = (Path.home() / ".switch" / "prod.keys")
     keys_cwd = Path("./prod.keys").absolute()
     keys = keys_cwd if keys_cwd.is_file() else keys_home
+    game_title_ids = Directories.assets / "game_title_ids.json"
 
 
 for binary, path in vars(Binaries).items():
     if binary.startswith("__"):
         continue
     if not path:
         print(
```

### Comparing `nton-1.2.2/nton/main.py` & `nton-1.2.3/nton/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,21 @@
 import subprocess
 import sys
 from datetime import datetime
 from pathlib import Path
 
 import click as click
 import coloredlogs
+import jsonpickle
+from PIL import Image
 from bs4 import BeautifulSoup
 
 from nton import __version__, nstool, title_ids
 from nton.constants import Directories, Binaries, Files
+from nton.title_ids import get_game_title_ids
 
 
 @click.group(invoke_without_command=True)
 @click.option("-v", "--version", is_flag=True, default=False, help="Print version information.")
 @click.option("-d", "--debug", is_flag=True, default=False, help="Enable DEBUG level logs.")
 def main(version: bool, debug: bool) -> None:
     """nton—Nintendo Switch NRO to NSP Forwarder."""
@@ -281,27 +284,24 @@
                     sys.exit(2)
             else:
                 log.debug("Got the Icon partition")
                 log.debug(base64.b64encode(icon_file.read_bytes()).decode())
 
         if icon_file.exists():
             # We must strip every unnecessary metadata or the icon will be a '?'
-            try:
-                subprocess.check_output([
-                    Binaries.magick, "mogrify",
-                    "-format", "jpg",
-                    "-resize", "256x256",
-                    "-strip", str(icon_file.absolute())
-                ])
-                # magick changes the .dat to .jpg, let's undo that
-                icon_file.unlink()
-                shutil.move(icon_file.with_suffix(".jpg"), icon_file)
-            except subprocess.CalledProcessError as e:
-                log.critical(f"Failed to convert and strip the Icon, {e.output} [{e.returncode}]")
-                sys.exit(2)
+            im = Image.open(icon_file)
+            if im.size != (256, 256):
+                im = im.resize((256, 256))
+            if im.mode != "RGB":
+                im = im.convert("RGB")
+            clean_im = Image.new(im.mode, im.size)
+            clean_im.putdata(list(im.getdata()))
+            clean_im.save(icon_file, format="JPEG")
+            clean_im.close()
+            im.close()
 
         next_nro_path = sdmc
         next_nro_path_file.write_text(next_nro_path)
 
         next_argv = next_nro_path
         if rom:
             next_argv += f' "sdmc:{rom}"'
@@ -332,7 +332,19 @@
 
         log.info(f"Done! The NSP has been saved to {nsp_final_path}")
     finally:
         if build_dir.exists():
             shutil.rmtree(build_dir)
         if hacbrewpack_backup_dir.exists():
             shutil.rmtree(hacbrewpack_backup_dir)
+
+
+@main.command()
+def update_game_ids():
+    """
+    Update the pre-existing Title ID registry.
+
+    Note: This makes calls to Tinfoil.io that may fail.
+    """
+    print("Updating the Game Title ID registry via Tinfoil API, this may take a while...")
+    game_title_ids = get_game_title_ids()
+    Files.game_title_ids.write_text(jsonpickle.dumps(game_title_ids), encoding="utf8")
```

### Comparing `nton-1.2.2/nton/nstool.py` & `nton-1.2.3/nton/nstool.py`

 * *Files identical despite different names*

### Comparing `nton-1.2.2/nton/title_ids.py` & `nton-1.2.3/nton/title_ids.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # Source: https://switchbrew.org/wiki/Title_list
 # Last updated: 2022-11-12 08:00 UTC+0
 # When updating make sure all title IDs are lowercase hex, 16 digits in length (a-z0-9{16}).
+import logging
+import sys
 import time
 
 import jsonpickle
 import requests
 
-from nton.constants import Directories
+from nton.constants import Files
 
 system_modules = (
     # https://switchbrew.org/wiki/Title_list#System_Modules
     "0100000000000000",  # https://switchbrew.org/wiki/Filesystem_services
     "0100000000000001",  # https://switchbrew.org/wiki/Loader_services
     "0100000000000002",  # https://switchbrew.org/wiki/NCM_services
     "0100000000000003",  # https://switchbrew.org/wiki/Process_Manager_services
@@ -443,48 +445,40 @@
             "category": "",
             "region": "ar,at,au,be,bg,br,ca,ch,cl,cn,co,cy,cz,de,dk,ee,es,fi,fr,gb,gr,hk,hr,hu,"
                       "ie,it,jp,kr,lt,lu,lv,mt,mx,nl,no,nz,pe,pl,pt,ro,ru,se,si,sk,us,xx,za,zh",
             "rating": "",
             "_": str(time.time_ns() // 1000000)
         },
         headers={
-            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8",
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0"
+            "Accept": "application/json, text/javascript, */*; q=0.01",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0",
+            "Origin": "https://tinfoil.io",
+            "Referer": "https://tinfoil.io/"
         }
     )
 
     if not res.ok:
         raise requests.ConnectionError(
             f"Failed to get a list of Game Title IDs from Tinfoil's API, [{res.status_code}]")
 
     title_ids = {
-        title["id"].lower(): title["name"].split(">", maxsplit=1)[1].split("</a>", maxsplit=1)[0]
+        title["id"].lower(): title["name"].removeprefix("<a>").removesuffix("</a>")
         for title in res.json()["data"]
     }
 
     return title_ids
 
 
-# get a list of game title ids (cached) via tinfoil's API
-Directories.cache.mkdir(parents=True, exist_ok=True)
-game_title_ids_cache = Directories.cache / "tinfoil_game_ids.json"
-if game_title_ids_cache.exists():
-    if game_title_ids_cache.stat().st_mtime + 43200 < time.time():
-        # expired
-        print("Refreshing the list of Game Title IDs...")
-        game_title_ids = get_game_title_ids()
-        game_title_ids_cache.write_text(jsonpickle.dumps(game_title_ids), encoding="utf8")
-    else:
-        # valid
-        game_title_ids = jsonpickle.loads(game_title_ids_cache.read_text("utf8"))
-else:
-    # no cache
-    print("Downloading a list of Game Title IDs...")
-    game_title_ids = get_game_title_ids()
-    game_title_ids_cache.write_text(jsonpickle.dumps(game_title_ids), encoding="utf8")
+if not Files.game_title_ids.exists():
+    print("[ERROR]: The Game Title ID registry is missing! Please re-add `/assets/game_title_ids.json`!")
+    sys.exit(1)
+if Files.game_title_ids.stat().st_mtime + (60 * 24 * 30) < time.time():
+    log = logging.getLogger()
+    log.warning("Game Title ID registry is quite old, I recommend updating it with `nton update-game-ids`")
+game_title_ids = jsonpickle.loads(Files.game_title_ids.read_text("utf8"))
 
 
 ALL_SYSTEM = (
     *system_modules,
     *system_data_archives,
     *system_applets,
     *development_system_applets,
```

### Comparing `nton-1.2.2/pyproject.toml` & `nton-1.2.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nton"
-version = "1.2.2"
+version = "1.2.3"
 description = "Nintendo Switch NRO to NSP Forwarder."
 authors = ["rlaphoenix <rlaphoenix@pm.me>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/rlaphoenix/nton"
 keywords = ["nintendo", "switch", "homebrew", "forwarder"]
 classifiers = [
@@ -23,17 +23,17 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/rlaphoenix/nton/issues"
 "Forums" = "https://github.com/rlaphoenix/nton/discussions"
 "Changelog" = "https://github.com/rlaphoenix/nton/blob/master/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.12"
-click = "^8.1.3"
-appdirs = "^1.4.4"
-requests = "^2.28.2"
+click = "^8.1.6"
+requests = "^2.31.0"
 jsonpickle = "^3.0.1"
 coloredlogs = "^15.0.1"
 beautifulsoup4 = "^4.12.2"
-lxml = "^4.9.2"
+lxml = "^4.9.3"
+pillow = "^9.5.0"
 
 [tool.poetry.scripts]
 nton = "nton.main:main"
```

### Comparing `nton-1.2.2/README.md` & `nton-1.2.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -15,148 +15,187 @@
 ![Preview](https://user-images.githubusercontent.com/17136956/206882948-4f05cace-16a3-4300-9047-8cba33106a64.jpg)
 *Forwarders made with NTON.*
 
 ## Features
 
 - 🛡️ Safety-first approach; System/Game Title IDs cannot be used and NRO files are validated
 - 🕹️ Boot right into an Emulated Game with Direct RetroArch Game Forwarding
-- 🖼️ Supports any Image file of any resolution or format for the NSP Icon
+- 🎥 Video Capture and Screenshots
+- 🖼️ Custom Forwarder Icon of any resolution or format
 - 🤖 The Title Name, Publisher, Icon, and more are automatically extracted from the NRO
-- 🎥 Supports Video Capture and Screenshots
 - ⚙ Currently Supports Firmware 12.0.0 and up
 - 🧩 Plug-and-play installation via PIP/PyPI
 - ❤️ Forever FOSS!
 
 ## Installation
 
-*Note: Requires [Python] 3.7.0 or newer with PIP installed.*
+> **Note** *Requires [Python] 3.7.0 or newer with PIP installed.*
 
 ```shell
 $ pip install nton
 ```
 
 You now have the `nton` package installed and a `nton` executable is now available.
 Check it out with `nton --help` - Voilà 🎉!
 
-*If you see any warnings about a path not being in your PATH environment variable, add it, or `nton` won't run.*
+> **Warning**<br>
+If pip gives you a warning about a path not being in your PATH environment variable then promptly add that path then
+close all open command prompt Windows, or running `nton` won't work as it will not be recognized as a program.
 
-### Dependencies
+  [Python]: <https://python.org>
+
+### 1. Dependencies
 
-The following is a list of programs required to be installed manually.  
-I recommend installing these with [winget] or [chocolatey] where possible as it automatically adds them to your
-`PATH` environment variable and will be easier to update in the future.
+The following is a list of programs required to be installed manually.
 
 - [hacBrewPack] for packing the NSP.
-- [ImageMagick] for Icon conversion and preparation.
 - [nstool] for NRO extraction and verification.
 - [hptnacp] for creating new NACP partitions if the NRO did not have one.
 
-For portable downloads, make sure you put them in your current working directory, in the installation directory,
-or put the directory path in your `PATH` environment variable. If you do not do this then NTON will not be able to
-find any of the binaries.
+Make sure you put them in your current working directory, in NTON's installation directory, or put the dependency's
+installation folder in your `PATH` environment variable. If you do not do this then NTON will not be able to find said
+dependency and will not be able to continue.
 
-  [winget]: <https://winget.run>
-  [chocolatey]: <https://chocolatey.org>
   [hacBrewPack]: <https://github.com/The-4n/hacBrewPack>
-  [ImageMagick]: <https://imagemagick.org/script/download.php>
   [nstool]: <https://github.com/jakcron/nstool>
   [hptnacp]: <https://github.com/The-4n/hacPack/tree/master/hacPack-Tools/hacPackTools-NACP>
 
-### Keys
-
-NTON requires the use of proprietary key data for use in various ways.
-
-Place your `prod.keys` file at `C:\Users\<User>\.switch\prod.keys` or in your current working directory for
-NTON to be able to find and use your keys.
-
-Make sure your `prod.keys` file is up-to-date for the firmware version your Nintendo Switch is on. It can be extracted
-from your Nintendo Switch with [Lockpick_RCM](https://github.com/shchmue/Lockpick_RCM).
+### 2. Keys
 
-### From Source Code
+Proprietary Keys known as `prod.keys` are required. You can obtain them from your own personal Switch using
+Lockpick_RCM.
 
-The following steps are instructions on downloading, preparing, and running the code under a Poetry environment.
-You can skip steps 3-5 with a simple `pip install .` call instead, but you miss out on a wide array of benefits.
+It must be placed at `C:\Users\<User>\.switch\prod.keys`, in your current working directory, or in
+NTON's installation directory for NTON to be able to find and use the keys.
 
-1. `git clone https://github.com/rlaphoenix/nton`
-2. `cd nton`
-3. (optional) `poetry config virtualenvs.in-project true` 
-4. `poetry install`
-5. `poetry run nton --help`
-
-As seen in Step 5, running the `nton` executable is somewhat different to a normal PIP installation.
-See [Poetry's Docs] on various ways of making calls under the virtual-environment.
+## Usage
 
-  [Python]: <https://python.org>
-  [Poetry]: <https://python-poetry.org>
-  [Poetry's Docs]: <https://python-poetry.org/docs/basic-usage/#using-your-virtual-environment>
+NTON is quite simple, just give it the path to the NRO on your microSD card!
 
-## Usage
+*For example, to create a forwarder for the Daybreak Homebrew included with Atmosphere, it's as simple as:*
 
-Take a look at `nton --help`, specifically `nton build --help`.  
-If you simply want to take an NRO and get an NSP forwarder, simply run `nton build "<nro path>"`.
+```shell
+nton build "D:/switch/daybreak.nro"
+```
 
-Note that the NRO path MUST be on your Switch microSD card. Do not provide a path in your C:/ Drive or such.
-Two different kinds of paths are used based on the initial file path, therefore it must be from your Switch microSD
-card.
+This will build a forwarder with the Title Name, Publisher, Version, and Icon automatically extracted from the NRO.
+The Title ID will be a randomly assigned value within generally conformed bounds. You may manually set a value with
+`--name`, `--publisher`, `--version`, `--icon`, and `--id` respectively.
+
+The Title ID is automatically checked against a periodically updated list of pre-existing System and Software Title IDs
+to ensure a collision does not occur. However, you should still be cautious and verify the Title ID is not already used
+by other Software before using. 
+
+> **Note**<br>
+> While NTON can be used on NRO files stored on your PC, it was designed to be used directly from your Switch's
+> microSD card. If you prefer to create forwarders with NRO files on your PC, or for batch purposes, you can specify
+> the path that the NRO file will reside on your microSD card during generation with `--sdmc`.
 
-E.g., to make a forwarder for the Homebrew Menu that's on your Switch's microSD at `D:\hbmenu.nro`, simply run
-`nton build "D:/hbmenu.nro"`
+For example, to make a forwarder for an NRO that is on your PC:
 
-Take a look at `nton build --help` for advanced usage like changing the Icon, Title Name, and so on.
+```shell
+nton build "C:/Users/rlaphoenix/Downloads/haze.nro" --sdmc "/switch/haze.nro"
+```
 
 ### Direct RetroArch Game forwarding
 
 Use a RetroArch Game Core as the NRO path and provide the path to the ROM on your Switch's microSD card with `--rom`.  
 This will then load the Core directly under RetroArch and provide the path to the ROM as a startup argument to the
 RetroArch Core.
 
-Note:
-
-- You must use a path to a RetroArch Game Core NRO, not the path to the RetroArch NRO itself.
-- Do not move, delete, or rename the ROM or the Core NRO files that are on your microSD card, or it will break.
+> **Note**
+> - You must use a path to a RetroArch Game Core NRO, not the path to the RetroArch NRO itself.
+> - Do not move, delete, or rename the ROM or the Core NRO files that are on your microSD card, or it will break.
 
 ## Troubleshooting
 
 Before continuing try running the homebrew from the Homebrew Launcher and see if it works through there.
-If it does not work through the Homebrew launcher either, then it was never the forwarder's fault and you should
+If it does not work through the Homebrew launcher either, then it was never the forwarder's fault, and you should
 check on your NRO or application installation.
 
 Please note that using Forwarders others have created has a good chance of not working on your system.
 The location of the NRO on their system may differ from the location on your system, hence the NSP won't be able
-to load the homebrew.
+to load the homebrew. I will not provide support if you are having an issue with a Forwarder you did not build
+yourself.
 
 ### The forwarder does not launch, "The software was closed because an error occurred."
 
-You're sigpatches that allow non-signed software to launch is outdated or not set up correctly.
-The `prod.keys` you used to create the NSP may also be outdated. Get new ones with [Lockpick_RCM] and
-make sure you choose to get keys from whichever SysNAND or EmuNAND is actually on the latest firmware.
+Your "sigpatches" (signature patches) that allow unsigned titles to launch is likely outdated or not set up correctly.
+Sigpatches can go outdated from Horizon OS firmware updates, Atmosphere updates (as well as silent updates). It is
+recommended to use the [sys-patch](https://github.com/ITotalJustice/sys-patch) sys-module to automatically patch your
+system from signature checks as well as other useful patches. The default configuration is fine for the majority of
+systems and is a simple copy & paste to your microSD card to install.
+
+It's also possible the `prod.keys` you used with NTON is outdated for your firmware. Get new ones with Lockpick_RCM
+and make sure you choose to get keys from the SysMMC or EmuMMC that you will be installing the forwarder on (or
+whichever has a newer firmware version).
 
 ### The forwarder starts loading but then crashes
 
-If it gets to the black loading screen with the Nintendo Switch logo, but then crashes, you may be setting
-the NRO path wrong when making the NSP. Make sure it starts with `/` and is an absolute path to an existing
-NRO file on your Switch's microSD card. The path you built for must be where the NRO file lies in your Switch's
-microSD card, not your PC.
+The NRO path set when building the forwarder is incorrect or the NRO file is currently missing (or your microSD card is
+not inserted). Make sure the path you choose starts with `/` and is an absolute path to an existing NRO file on your
+Switch's microSD card (not your PC).
 
 ### The forwarder's icon is a '?'
 
-The `icon_AmericanEnglish.dat` is not to the spec that Nintendo likes in some way. This is usually caused by the format of the
-image not being a JPEG, or it has EXIF data or an embedded color space.
-
-I recommend stripping all EXIF metadata and saving without an Embed Color Space. You can do this quickly with ImageMagick,
-`magick mogrify -format jpg -resize 256x256 -strip "C:\Users\John\Downloads\icon.png"`.
+This happens when the `icon_AmericanEnglish.dat` within the built forwarder is not to the spec that Nintendo likes, in
+some way. This is usually caused by the format of the image not being JPEG, or it has EXIF data or other unnecessary
+extra metadata.
+
+> **Note**<br>
+This is considered a bug if it happens to you after using NTON as it should automatically sanitize the
+images when building the forwarder. If this happens to you, please report what image you chose to use, or give
+information on what exact NRO you were making a forwarder from.
+
+### The forwarder's icon is a loading circle, opening fails
+
+The installation of the Forwarder NSP failed in some way and the result is a corrupt title under that Title ID.
+This may have happened when trying to install data to the Title ID you chose or had randomly assigned to your forwarder
+NSP on an unsupported firmware version. This also happens when trying to install DLC to a Title without having the
+minimum required Game Update for that DLC (i.e. Installing the DLC Courses while on Mario Kart 8 Deluxe v1.0). However,
+since this happened on your Forwarder NSP you can likely rule that out.
+
+When this happens deleting and reinstalling the same NSP likely won't fix it or do anything. You may need to reinstall
+the NSP via Goldleaf and hit "Proceed" when it warns yo uthat the title is already installed. Goldleaf will deal with
+the pre-existing files properly unlike Tinfoil (where you likely had the corruption in the first place). DBI may also
+help you resolve this issue as it has tools to remove partial installs and leftover files.
+
+### The forwarder randomly stopped working, I've read everything so far
+
+You most likely updated Atmosphere or Horizon OS's Firmware and need to update your Sigpatches. If that hasn't fixed
+it, make sure you haven't deleted or moved the NRO on your Switch's microSD card. It cannot be moved as the built
+forwarder has a hardcoded file path that it loads the NRO from when launched.
+
+If it still does not work, it's possible a firmware update has broken the [forwarder ROM][ROM] that is used and needs
+to be updated. Both Firmware 9.0.0 and 12.0.0 have previously broken different forwarder ROMs requiring updates. If
+you believe this to be the case then please make an Issue.
+
+## Development
+
+The following steps are basic instructions on downloading and working on the code under a [Poetry] environment.
+
+1. Follow Poetry's Docs to [Install Poetry].
+2. Download NTON's latest code, `git clone https://github.com/rlaphoenix/nton`
+3. Navigate to the downloaded code repository, `cd nton`
+4. _Optionally_ have Poetry install the virtual-env in the project, `poetry config virtualenvs.in-project true` 
+5. Install NTON's dependencies and development tools, `poetry install`
+6. Run NTON from within the Poetry venv, `poetry run nton --help`
+
+As shown, running the `nton` executable is somewhat different to a normal installation. This is because Poetry installs
+all dependencies and the `nton` shim itself within a virtual-environment, which is like a clone of your Python install
+stripped clean, with only NTON's dependencies installed. That way you don't mess around with any dependencies from any
+other installed Python applications, nor the other way around. A secluded environment.
 
-### The forwarder randomly stopped working after a while, I changed nothing!
+I recommend taking a look at [Poetry's Docs] for further information, why not get started by reading Poetry's guide on
+[Using Your Virtual Environment].
 
-You most likely updated your Switch's Firmware and need to update your sigpatches. If not, you may have deleted the NRO from
-your Switch's microSD card or moved the NRO somewhere else. It cannot be moved as the built NSP loads the NRO at the specified
-path when you ran `build`.
-
-It's also possible the firmware update has broken the [forwarder ROM][ROM] that is used and needs to be fixed.
-Firmware 9.0.0 and 12.0.0 are times the firmware has broken different forwarder ROMs in the past.
+  [Poetry]: <https://python-poetry.org>
+  [Install Poetry]: <https://python-poetry.org/docs/#installation>
+  [Poetry's Docs]: <https://python-poetry.org/docs>
+  [Using Your Virtual Environment]: <https://python-poetry.org/docs/basic-usage/#using-your-virtual-environment>
 
 ## Credit
 
 - [meliodas2255] for their [Open-Source forwarder ROM][ROM] supporting v12.0.0+ with both direct RetroArch Forwarding
   and general forwarding both supported.
 - [vgmoose] for the [sdl-hello-world] NRO that is used in CI/CD testing.
```

#### html2text {}

```diff
@@ -6,101 +6,139 @@
 NRO to NSP Forwarder for firmware 12.0.0 and newer. A forwarder lets you open a
 Homebrew NRO file from your SD card through the Nintendo Switch Home Screen
 instead of the Homebrew Launcher. ![Preview](https://user-
 images.githubusercontent.com/17136956/206882948-4f05cace-16a3-4300-9047-
 8cba33106a64.jpg) *Forwarders made with NTON.* ## Features - ð¡ï¸ Safety-
 first approach; System/Game Title IDs cannot be used and NRO files are
 validated - ð¹ï¸ Boot right into an Emulated Game with Direct RetroArch Game
-Forwarding - ð¼ï¸ Supports any Image file of any resolution or format for
-the NSP Icon - ð¤ The Title Name, Publisher, Icon, and more are automatically
-extracted from the NRO - ð¥ Supports Video Capture and Screenshots - â
-Currently Supports Firmware 12.0.0 and up - ð§© Plug-and-play installation via
-PIP/PyPI - â¤ï¸ Forever FOSS! ## Installation *Note: Requires [Python] 3.7.0
-or newer with PIP installed.* ```shell $ pip install nton ``` You now have the
-`nton` package installed and a `nton` executable is now available. Check it out
-with `nton --help` - VoilÃ  ð! *If you see any warnings about a path not
-being in your PATH environment variable, add it, or `nton` won't run.* ###
-Dependencies The following is a list of programs required to be installed
-manually. I recommend installing these with [winget] or [chocolatey] where
-possible as it automatically adds them to your `PATH` environment variable and
-will be easier to update in the future. - [hacBrewPack] for packing the NSP. -
-[ImageMagick] for Icon conversion and preparation. - [nstool] for NRO
+Forwarding - ð¥ Video Capture and Screenshots - ð¼ï¸ Custom Forwarder Icon
+of any resolution or format - ð¤ The Title Name, Publisher, Icon, and more
+are automatically extracted from the NRO - â Currently Supports Firmware
+12.0.0 and up - ð§© Plug-and-play installation via PIP/PyPI - â¤ï¸ Forever
+FOSS! ## Installation > **Note** *Requires [Python] 3.7.0 or newer with PIP
+installed.* ```shell $ pip install nton ``` You now have the `nton` package
+installed and a `nton` executable is now available. Check it out with `nton --
+help` - VoilÃ  ð! > **Warning**
+If pip gives you a warning about a path not being in your PATH environment
+variable then promptly add that path then close all open command prompt
+Windows, or running `nton` won't work as it will not be recognized as a
+program. [Python]:
+python.org> ### 1. Dependencies The following is a list of programs required to
+be installed manually. - [hacBrewPack] for packing the NSP. - [nstool] for NRO
 extraction and verification. - [hptnacp] for creating new NACP partitions if
-the NRO did not have one. For portable downloads, make sure you put them in
-your current working directory, in the installation directory, or put the
-directory path in your `PATH` environment variable. If you do not do this then
-NTON will not be able to find any of the binaries. [winget]:
-winget.run> [chocolatey]:
-chocolatey.org> [hacBrewPack]:
-github.com/The-4n/hacBrewPack> [ImageMagick]:
-imagemagick.org/script/download.php> [nstool]:
+the NRO did not have one. Make sure you put them in your current working
+directory, in NTON's installation directory, or put the dependency's
+installation folder in your `PATH` environment variable. If you do not do this
+then NTON will not be able to find said dependency and will not be able to
+continue. [hacBrewPack]:
+github.com/The-4n/hacBrewPack> [nstool]:
 github.com/jakcron/nstool> [hptnacp]:
-github.com/The-4n/hacPack/tree/master/hacPack-Tools/hacPackTools-NACP> ### Keys
-NTON requires the use of proprietary key data for use in various ways. Place
-your `prod.keys` file at `C:\Users\\.switch\prod.keys` or in your current
-working directory for NTON to be able to find and use your keys. Make sure your
-`prod.keys` file is up-to-date for the firmware version your Nintendo Switch is
-on. It can be extracted from your Nintendo Switch with [Lockpick_RCM](https://
-github.com/shchmue/Lockpick_RCM). ### From Source Code The following steps are
-instructions on downloading, preparing, and running the code under a Poetry
-environment. You can skip steps 3-5 with a simple `pip install .` call instead,
-but you miss out on a wide array of benefits. 1. `git clone https://github.com/
-rlaphoenix/nton` 2. `cd nton` 3. (optional) `poetry config virtualenvs.in-
-project true` 4. `poetry install` 5. `poetry run nton --help` As seen in Step
-5, running the `nton` executable is somewhat different to a normal PIP
-installation. See [Poetry's Docs] on various ways of making calls under the
-virtual-environment. [Python]:
-python.org> [Poetry]:
-python-poetry.org> [Poetry's Docs]:
-python-poetry.org/docs/basic-usage/#using-your-virtual-environment> ## Usage
-Take a look at `nton --help`, specifically `nton build --help`. If you simply
-want to take an NRO and get an NSP forwarder, simply run `nton build ""`. Note
-that the NRO path MUST be on your Switch microSD card. Do not provide a path in
-your C:/ Drive or such. Two different kinds of paths are used based on the
-initial file path, therefore it must be from your Switch microSD card. E.g., to
-make a forwarder for the Homebrew Menu that's on your Switch's microSD at `D:
-\hbmenu.nro`, simply run `nton build "D:/hbmenu.nro"` Take a look at `nton
-build --help` for advanced usage like changing the Icon, Title Name, and so on.
-### Direct RetroArch Game forwarding Use a RetroArch Game Core as the NRO path
-and provide the path to the ROM on your Switch's microSD card with `--rom`.
-This will then load the Core directly under RetroArch and provide the path to
-the ROM as a startup argument to the RetroArch Core. Note: - You must use a
-path to a RetroArch Game Core NRO, not the path to the RetroArch NRO itself. -
-Do not move, delete, or rename the ROM or the Core NRO files that are on your
-microSD card, or it will break. ## Troubleshooting Before continuing try
-running the homebrew from the Homebrew Launcher and see if it works through
-there. If it does not work through the Homebrew launcher either, then it was
-never the forwarder's fault and you should check on your NRO or application
-installation. Please note that using Forwarders others have created has a good
-chance of not working on your system. The location of the NRO on their system
-may differ from the location on your system, hence the NSP won't be able to
-load the homebrew. ### The forwarder does not launch, "The software was closed
-because an error occurred." You're sigpatches that allow non-signed software to
-launch is outdated or not set up correctly. The `prod.keys` you used to create
-the NSP may also be outdated. Get new ones with [Lockpick_RCM] and make sure
-you choose to get keys from whichever SysNAND or EmuNAND is actually on the
-latest firmware. ### The forwarder starts loading but then crashes If it gets
-to the black loading screen with the Nintendo Switch logo, but then crashes,
-you may be setting the NRO path wrong when making the NSP. Make sure it starts
+github.com/The-4n/hacPack/tree/master/hacPack-Tools/hacPackTools-NACP> ### 2.
+Keys Proprietary Keys known as `prod.keys` are required. You can obtain them
+from your own personal Switch using Lockpick_RCM. It must be placed at `C:
+\Users\\.switch\prod.keys`, in your current working directory, or in NTON's
+installation directory for NTON to be able to find and use the keys. ## Usage
+NTON is quite simple, just give it the path to the NRO on your microSD card!
+*For example, to create a forwarder for the Daybreak Homebrew included with
+Atmosphere, it's as simple as:* ```shell nton build "D:/switch/daybreak.nro"
+``` This will build a forwarder with the Title Name, Publisher, Version, and
+Icon automatically extracted from the NRO. The Title ID will be a randomly
+assigned value within generally conformed bounds. You may manually set a value
+with `--name`, `--publisher`, `--version`, `--icon`, and `--id` respectively.
+The Title ID is automatically checked against a periodically updated list of
+pre-existing System and Software Title IDs to ensure a collision does not
+occur. However, you should still be cautious and verify the Title ID is not
+already used by other Software before using. > **Note**
+> While NTON can be used on NRO files stored on your PC, it was designed to be
+used directly from your Switch's > microSD card. If you prefer to create
+forwarders with NRO files on your PC, or for batch purposes, you can specify >
+the path that the NRO file will reside on your microSD card during generation
+with `--sdmc`. For example, to make a forwarder for an NRO that is on your PC:
+```shell nton build "C:/Users/rlaphoenix/Downloads/haze.nro" --sdmc "/switch/
+haze.nro" ``` ### Direct RetroArch Game forwarding Use a RetroArch Game Core as
+the NRO path and provide the path to the ROM on your Switch's microSD card with
+`--rom`. This will then load the Core directly under RetroArch and provide the
+path to the ROM as a startup argument to the RetroArch Core. > **Note** > - You
+must use a path to a RetroArch Game Core NRO, not the path to the RetroArch NRO
+itself. > - Do not move, delete, or rename the ROM or the Core NRO files that
+are on your microSD card, or it will break. ## Troubleshooting Before
+continuing try running the homebrew from the Homebrew Launcher and see if it
+works through there. If it does not work through the Homebrew launcher either,
+then it was never the forwarder's fault, and you should check on your NRO or
+application installation. Please note that using Forwarders others have created
+has a good chance of not working on your system. The location of the NRO on
+their system may differ from the location on your system, hence the NSP won't
+be able to load the homebrew. I will not provide support if you are having an
+issue with a Forwarder you did not build yourself. ### The forwarder does not
+launch, "The software was closed because an error occurred." Your "sigpatches"
+(signature patches) that allow unsigned titles to launch is likely outdated or
+not set up correctly. Sigpatches can go outdated from Horizon OS firmware
+updates, Atmosphere updates (as well as silent updates). It is recommended to
+use the [sys-patch](https://github.com/ITotalJustice/sys-patch) sys-module to
+automatically patch your system from signature checks as well as other useful
+patches. The default configuration is fine for the majority of systems and is a
+simple copy & paste to your microSD card to install. It's also possible the
+`prod.keys` you used with NTON is outdated for your firmware. Get new ones with
+Lockpick_RCM and make sure you choose to get keys from the SysMMC or EmuMMC
+that you will be installing the forwarder on (or whichever has a newer firmware
+version). ### The forwarder starts loading but then crashes The NRO path set
+when building the forwarder is incorrect or the NRO file is currently missing
+(or your microSD card is not inserted). Make sure the path you choose starts
 with `/` and is an absolute path to an existing NRO file on your Switch's
-microSD card. The path you built for must be where the NRO file lies in your
-Switch's microSD card, not your PC. ### The forwarder's icon is a '?' The
-`icon_AmericanEnglish.dat` is not to the spec that Nintendo likes in some way.
-This is usually caused by the format of the image not being a JPEG, or it has
-EXIF data or an embedded color space. I recommend stripping all EXIF metadata
-and saving without an Embed Color Space. You can do this quickly with
-ImageMagick, `magick mogrify -format jpg -resize 256x256 -strip "C:
-\Users\John\Downloads\icon.png"`. ### The forwarder randomly stopped working
-after a while, I changed nothing! You most likely updated your Switch's
-Firmware and need to update your sigpatches. If not, you may have deleted the
-NRO from your Switch's microSD card or moved the NRO somewhere else. It cannot
-be moved as the built NSP loads the NRO at the specified path when you ran
-`build`. It's also possible the firmware update has broken the [forwarder ROM]
-[ROM] that is used and needs to be fixed. Firmware 9.0.0 and 12.0.0 are times
-the firmware has broken different forwarder ROMs in the past. ## Credit -
+microSD card (not your PC). ### The forwarder's icon is a '?' This happens when
+the `icon_AmericanEnglish.dat` within the built forwarder is not to the spec
+that Nintendo likes, in some way. This is usually caused by the format of the
+image not being JPEG, or it has EXIF data or other unnecessary extra metadata.
+> **Note**
+This is considered a bug if it happens to you after using NTON as it should
+automatically sanitize the images when building the forwarder. If this happens
+to you, please report what image you chose to use, or give information on what
+exact NRO you were making a forwarder from. ### The forwarder's icon is a
+loading circle, opening fails The installation of the Forwarder NSP failed in
+some way and the result is a corrupt title under that Title ID. This may have
+happened when trying to install data to the Title ID you chose or had randomly
+assigned to your forwarder NSP on an unsupported firmware version. This also
+happens when trying to install DLC to a Title without having the minimum
+required Game Update for that DLC (i.e. Installing the DLC Courses while on
+Mario Kart 8 Deluxe v1.0). However, since this happened on your Forwarder NSP
+you can likely rule that out. When this happens deleting and reinstalling the
+same NSP likely won't fix it or do anything. You may need to reinstall the NSP
+via Goldleaf and hit "Proceed" when it warns yo uthat the title is already
+installed. Goldleaf will deal with the pre-existing files properly unlike
+Tinfoil (where you likely had the corruption in the first place). DBI may also
+help you resolve this issue as it has tools to remove partial installs and
+leftover files. ### The forwarder randomly stopped working, I've read
+everything so far You most likely updated Atmosphere or Horizon OS's Firmware
+and need to update your Sigpatches. If that hasn't fixed it, make sure you
+haven't deleted or moved the NRO on your Switch's microSD card. It cannot be
+moved as the built forwarder has a hardcoded file path that it loads the NRO
+from when launched. If it still does not work, it's possible a firmware update
+has broken the [forwarder ROM][ROM] that is used and needs to be updated. Both
+Firmware 9.0.0 and 12.0.0 have previously broken different forwarder ROMs
+requiring updates. If you believe this to be the case then please make an
+Issue. ## Development The following steps are basic instructions on downloading
+and working on the code under a [Poetry] environment. 1. Follow Poetry's Docs
+to [Install Poetry]. 2. Download NTON's latest code, `git clone https://
+github.com/rlaphoenix/nton` 3. Navigate to the downloaded code repository, `cd
+nton` 4. _Optionally_ have Poetry install the virtual-env in the project,
+`poetry config virtualenvs.in-project true` 5. Install NTON's dependencies and
+development tools, `poetry install` 6. Run NTON from within the Poetry venv,
+`poetry run nton --help` As shown, running the `nton` executable is somewhat
+different to a normal installation. This is because Poetry installs all
+dependencies and the `nton` shim itself within a virtual-environment, which is
+like a clone of your Python install stripped clean, with only NTON's
+dependencies installed. That way you don't mess around with any dependencies
+from any other installed Python applications, nor the other way around. A
+secluded environment. I recommend taking a look at [Poetry's Docs] for further
+information, why not get started by reading Poetry's guide on [Using Your
+Virtual Environment]. [Poetry]:
+python-poetry.org> [Install Poetry]:
+python-poetry.org/docs/#installation> [Poetry's Docs]:
+python-poetry.org/docs> [Using Your Virtual Environment]:
+python-poetry.org/docs/basic-usage/#using-your-virtual-environment> ## Credit -
 [meliodas2255] for their [Open-Source forwarder ROM][ROM] supporting v12.0.0+
 with both direct RetroArch Forwarding and general forwarding both supported. -
 [vgmoose] for the [sdl-hello-world] NRO that is used in CI/CD testing.
 [meliodas2255]:
 gbatemp.net/members/meliodas2255.410353> [vgmoose]:
 github.com/vgmoose> [ROM]:
 github.com/Skywalker25/Forwarder-Mod> [sdl-hello-world]:
```

### Comparing `nton-1.2.2/PKG-INFO` & `nton-1.2.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nton
-Version: 1.2.2
+Version: 1.2.3
 Summary: Nintendo Switch NRO to NSP Forwarder.
 Home-page: https://github.com/rlaphoenix/nton
 License: GPL-3.0-only
 Keywords: nintendo,switch,homebrew,forwarder
 Author: rlaphoenix
 Author-email: rlaphoenix@pm.me
 Requires-Python: >=3.7,<3.12
@@ -17,21 +17,21 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Utilities
-Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
-Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: click (>=8.1.6,<9.0.0)
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: jsonpickle (>=3.0.1,<4.0.0)
-Requires-Dist: lxml (>=4.9.2,<5.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: lxml (>=4.9.3,<5.0.0)
+Requires-Dist: pillow (>=9.5.0,<10.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/rlaphoenix/nton/issues
 Project-URL: Changelog, https://github.com/rlaphoenix/nton/blob/master/CHANGELOG.md
 Project-URL: Forums, https://github.com/rlaphoenix/nton/discussions
 Project-URL: Repository, https://github.com/rlaphoenix/nton
 Description-Content-Type: text/markdown
 
 # NTON
@@ -51,148 +51,187 @@
 ![Preview](https://user-images.githubusercontent.com/17136956/206882948-4f05cace-16a3-4300-9047-8cba33106a64.jpg)
 *Forwarders made with NTON.*
 
 ## Features
 
 - 🛡️ Safety-first approach; System/Game Title IDs cannot be used and NRO files are validated
 - 🕹️ Boot right into an Emulated Game with Direct RetroArch Game Forwarding
-- 🖼️ Supports any Image file of any resolution or format for the NSP Icon
+- 🎥 Video Capture and Screenshots
+- 🖼️ Custom Forwarder Icon of any resolution or format
 - 🤖 The Title Name, Publisher, Icon, and more are automatically extracted from the NRO
-- 🎥 Supports Video Capture and Screenshots
 - ⚙ Currently Supports Firmware 12.0.0 and up
 - 🧩 Plug-and-play installation via PIP/PyPI
 - ❤️ Forever FOSS!
 
 ## Installation
 
-*Note: Requires [Python] 3.7.0 or newer with PIP installed.*
+> **Note** *Requires [Python] 3.7.0 or newer with PIP installed.*
 
 ```shell
 $ pip install nton
 ```
 
 You now have the `nton` package installed and a `nton` executable is now available.
 Check it out with `nton --help` - Voilà 🎉!
 
-*If you see any warnings about a path not being in your PATH environment variable, add it, or `nton` won't run.*
+> **Warning**<br>
+If pip gives you a warning about a path not being in your PATH environment variable then promptly add that path then
+close all open command prompt Windows, or running `nton` won't work as it will not be recognized as a program.
 
-### Dependencies
+  [Python]: <https://python.org>
+
+### 1. Dependencies
 
-The following is a list of programs required to be installed manually.  
-I recommend installing these with [winget] or [chocolatey] where possible as it automatically adds them to your
-`PATH` environment variable and will be easier to update in the future.
+The following is a list of programs required to be installed manually.
 
 - [hacBrewPack] for packing the NSP.
-- [ImageMagick] for Icon conversion and preparation.
 - [nstool] for NRO extraction and verification.
 - [hptnacp] for creating new NACP partitions if the NRO did not have one.
 
-For portable downloads, make sure you put them in your current working directory, in the installation directory,
-or put the directory path in your `PATH` environment variable. If you do not do this then NTON will not be able to
-find any of the binaries.
+Make sure you put them in your current working directory, in NTON's installation directory, or put the dependency's
+installation folder in your `PATH` environment variable. If you do not do this then NTON will not be able to find said
+dependency and will not be able to continue.
 
-  [winget]: <https://winget.run>
-  [chocolatey]: <https://chocolatey.org>
   [hacBrewPack]: <https://github.com/The-4n/hacBrewPack>
-  [ImageMagick]: <https://imagemagick.org/script/download.php>
   [nstool]: <https://github.com/jakcron/nstool>
   [hptnacp]: <https://github.com/The-4n/hacPack/tree/master/hacPack-Tools/hacPackTools-NACP>
 
-### Keys
-
-NTON requires the use of proprietary key data for use in various ways.
-
-Place your `prod.keys` file at `C:\Users\<User>\.switch\prod.keys` or in your current working directory for
-NTON to be able to find and use your keys.
-
-Make sure your `prod.keys` file is up-to-date for the firmware version your Nintendo Switch is on. It can be extracted
-from your Nintendo Switch with [Lockpick_RCM](https://github.com/shchmue/Lockpick_RCM).
+### 2. Keys
 
-### From Source Code
+Proprietary Keys known as `prod.keys` are required. You can obtain them from your own personal Switch using
+Lockpick_RCM.
 
-The following steps are instructions on downloading, preparing, and running the code under a Poetry environment.
-You can skip steps 3-5 with a simple `pip install .` call instead, but you miss out on a wide array of benefits.
+It must be placed at `C:\Users\<User>\.switch\prod.keys`, in your current working directory, or in
+NTON's installation directory for NTON to be able to find and use the keys.
 
-1. `git clone https://github.com/rlaphoenix/nton`
-2. `cd nton`
-3. (optional) `poetry config virtualenvs.in-project true` 
-4. `poetry install`
-5. `poetry run nton --help`
-
-As seen in Step 5, running the `nton` executable is somewhat different to a normal PIP installation.
-See [Poetry's Docs] on various ways of making calls under the virtual-environment.
+## Usage
 
-  [Python]: <https://python.org>
-  [Poetry]: <https://python-poetry.org>
-  [Poetry's Docs]: <https://python-poetry.org/docs/basic-usage/#using-your-virtual-environment>
+NTON is quite simple, just give it the path to the NRO on your microSD card!
 
-## Usage
+*For example, to create a forwarder for the Daybreak Homebrew included with Atmosphere, it's as simple as:*
 
-Take a look at `nton --help`, specifically `nton build --help`.  
-If you simply want to take an NRO and get an NSP forwarder, simply run `nton build "<nro path>"`.
+```shell
+nton build "D:/switch/daybreak.nro"
+```
 
-Note that the NRO path MUST be on your Switch microSD card. Do not provide a path in your C:/ Drive or such.
-Two different kinds of paths are used based on the initial file path, therefore it must be from your Switch microSD
-card.
+This will build a forwarder with the Title Name, Publisher, Version, and Icon automatically extracted from the NRO.
+The Title ID will be a randomly assigned value within generally conformed bounds. You may manually set a value with
+`--name`, `--publisher`, `--version`, `--icon`, and `--id` respectively.
+
+The Title ID is automatically checked against a periodically updated list of pre-existing System and Software Title IDs
+to ensure a collision does not occur. However, you should still be cautious and verify the Title ID is not already used
+by other Software before using. 
+
+> **Note**<br>
+> While NTON can be used on NRO files stored on your PC, it was designed to be used directly from your Switch's
+> microSD card. If you prefer to create forwarders with NRO files on your PC, or for batch purposes, you can specify
+> the path that the NRO file will reside on your microSD card during generation with `--sdmc`.
 
-E.g., to make a forwarder for the Homebrew Menu that's on your Switch's microSD at `D:\hbmenu.nro`, simply run
-`nton build "D:/hbmenu.nro"`
+For example, to make a forwarder for an NRO that is on your PC:
 
-Take a look at `nton build --help` for advanced usage like changing the Icon, Title Name, and so on.
+```shell
+nton build "C:/Users/rlaphoenix/Downloads/haze.nro" --sdmc "/switch/haze.nro"
+```
 
 ### Direct RetroArch Game forwarding
 
 Use a RetroArch Game Core as the NRO path and provide the path to the ROM on your Switch's microSD card with `--rom`.  
 This will then load the Core directly under RetroArch and provide the path to the ROM as a startup argument to the
 RetroArch Core.
 
-Note:
-
-- You must use a path to a RetroArch Game Core NRO, not the path to the RetroArch NRO itself.
-- Do not move, delete, or rename the ROM or the Core NRO files that are on your microSD card, or it will break.
+> **Note**
+> - You must use a path to a RetroArch Game Core NRO, not the path to the RetroArch NRO itself.
+> - Do not move, delete, or rename the ROM or the Core NRO files that are on your microSD card, or it will break.
 
 ## Troubleshooting
 
 Before continuing try running the homebrew from the Homebrew Launcher and see if it works through there.
-If it does not work through the Homebrew launcher either, then it was never the forwarder's fault and you should
+If it does not work through the Homebrew launcher either, then it was never the forwarder's fault, and you should
 check on your NRO or application installation.
 
 Please note that using Forwarders others have created has a good chance of not working on your system.
 The location of the NRO on their system may differ from the location on your system, hence the NSP won't be able
-to load the homebrew.
+to load the homebrew. I will not provide support if you are having an issue with a Forwarder you did not build
+yourself.
 
 ### The forwarder does not launch, "The software was closed because an error occurred."
 
-You're sigpatches that allow non-signed software to launch is outdated or not set up correctly.
-The `prod.keys` you used to create the NSP may also be outdated. Get new ones with [Lockpick_RCM] and
-make sure you choose to get keys from whichever SysNAND or EmuNAND is actually on the latest firmware.
+Your "sigpatches" (signature patches) that allow unsigned titles to launch is likely outdated or not set up correctly.
+Sigpatches can go outdated from Horizon OS firmware updates, Atmosphere updates (as well as silent updates). It is
+recommended to use the [sys-patch](https://github.com/ITotalJustice/sys-patch) sys-module to automatically patch your
+system from signature checks as well as other useful patches. The default configuration is fine for the majority of
+systems and is a simple copy & paste to your microSD card to install.
+
+It's also possible the `prod.keys` you used with NTON is outdated for your firmware. Get new ones with Lockpick_RCM
+and make sure you choose to get keys from the SysMMC or EmuMMC that you will be installing the forwarder on (or
+whichever has a newer firmware version).
 
 ### The forwarder starts loading but then crashes
 
-If it gets to the black loading screen with the Nintendo Switch logo, but then crashes, you may be setting
-the NRO path wrong when making the NSP. Make sure it starts with `/` and is an absolute path to an existing
-NRO file on your Switch's microSD card. The path you built for must be where the NRO file lies in your Switch's
-microSD card, not your PC.
+The NRO path set when building the forwarder is incorrect or the NRO file is currently missing (or your microSD card is
+not inserted). Make sure the path you choose starts with `/` and is an absolute path to an existing NRO file on your
+Switch's microSD card (not your PC).
 
 ### The forwarder's icon is a '?'
 
-The `icon_AmericanEnglish.dat` is not to the spec that Nintendo likes in some way. This is usually caused by the format of the
-image not being a JPEG, or it has EXIF data or an embedded color space.
-
-I recommend stripping all EXIF metadata and saving without an Embed Color Space. You can do this quickly with ImageMagick,
-`magick mogrify -format jpg -resize 256x256 -strip "C:\Users\John\Downloads\icon.png"`.
+This happens when the `icon_AmericanEnglish.dat` within the built forwarder is not to the spec that Nintendo likes, in
+some way. This is usually caused by the format of the image not being JPEG, or it has EXIF data or other unnecessary
+extra metadata.
+
+> **Note**<br>
+This is considered a bug if it happens to you after using NTON as it should automatically sanitize the
+images when building the forwarder. If this happens to you, please report what image you chose to use, or give
+information on what exact NRO you were making a forwarder from.
+
+### The forwarder's icon is a loading circle, opening fails
+
+The installation of the Forwarder NSP failed in some way and the result is a corrupt title under that Title ID.
+This may have happened when trying to install data to the Title ID you chose or had randomly assigned to your forwarder
+NSP on an unsupported firmware version. This also happens when trying to install DLC to a Title without having the
+minimum required Game Update for that DLC (i.e. Installing the DLC Courses while on Mario Kart 8 Deluxe v1.0). However,
+since this happened on your Forwarder NSP you can likely rule that out.
+
+When this happens deleting and reinstalling the same NSP likely won't fix it or do anything. You may need to reinstall
+the NSP via Goldleaf and hit "Proceed" when it warns yo uthat the title is already installed. Goldleaf will deal with
+the pre-existing files properly unlike Tinfoil (where you likely had the corruption in the first place). DBI may also
+help you resolve this issue as it has tools to remove partial installs and leftover files.
+
+### The forwarder randomly stopped working, I've read everything so far
+
+You most likely updated Atmosphere or Horizon OS's Firmware and need to update your Sigpatches. If that hasn't fixed
+it, make sure you haven't deleted or moved the NRO on your Switch's microSD card. It cannot be moved as the built
+forwarder has a hardcoded file path that it loads the NRO from when launched.
+
+If it still does not work, it's possible a firmware update has broken the [forwarder ROM][ROM] that is used and needs
+to be updated. Both Firmware 9.0.0 and 12.0.0 have previously broken different forwarder ROMs requiring updates. If
+you believe this to be the case then please make an Issue.
+
+## Development
+
+The following steps are basic instructions on downloading and working on the code under a [Poetry] environment.
+
+1. Follow Poetry's Docs to [Install Poetry].
+2. Download NTON's latest code, `git clone https://github.com/rlaphoenix/nton`
+3. Navigate to the downloaded code repository, `cd nton`
+4. _Optionally_ have Poetry install the virtual-env in the project, `poetry config virtualenvs.in-project true` 
+5. Install NTON's dependencies and development tools, `poetry install`
+6. Run NTON from within the Poetry venv, `poetry run nton --help`
+
+As shown, running the `nton` executable is somewhat different to a normal installation. This is because Poetry installs
+all dependencies and the `nton` shim itself within a virtual-environment, which is like a clone of your Python install
+stripped clean, with only NTON's dependencies installed. That way you don't mess around with any dependencies from any
+other installed Python applications, nor the other way around. A secluded environment.
 
-### The forwarder randomly stopped working after a while, I changed nothing!
+I recommend taking a look at [Poetry's Docs] for further information, why not get started by reading Poetry's guide on
+[Using Your Virtual Environment].
 
-You most likely updated your Switch's Firmware and need to update your sigpatches. If not, you may have deleted the NRO from
-your Switch's microSD card or moved the NRO somewhere else. It cannot be moved as the built NSP loads the NRO at the specified
-path when you ran `build`.
-
-It's also possible the firmware update has broken the [forwarder ROM][ROM] that is used and needs to be fixed.
-Firmware 9.0.0 and 12.0.0 are times the firmware has broken different forwarder ROMs in the past.
+  [Poetry]: <https://python-poetry.org>
+  [Install Poetry]: <https://python-poetry.org/docs/#installation>
+  [Poetry's Docs]: <https://python-poetry.org/docs>
+  [Using Your Virtual Environment]: <https://python-poetry.org/docs/basic-usage/#using-your-virtual-environment>
 
 ## Credit
 
 - [meliodas2255] for their [Open-Source forwarder ROM][ROM] supporting v12.0.0+ with both direct RetroArch Forwarding
   and general forwarding both supported.
 - [vgmoose] for the [sdl-hello-world] NRO that is used in CI/CD testing.
```

#### html2text {}

```diff
@@ -1,126 +1,164 @@
-Metadata-Version: 2.1 Name: nton Version: 1.2.2 Summary: Nintendo Switch NRO to
+Metadata-Version: 2.1 Name: nton Version: 1.2.3 Summary: Nintendo Switch NRO to
 NSP Forwarder. Home-page: https://github.com/rlaphoenix/nton License: GPL-3.0-
 only Keywords: nintendo,switch,homebrew,forwarder Author: rlaphoenix Author-
 email: rlaphoenix@pm.me Requires-Python: >=3.7,<3.12 Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Topic :: Games/Entertainment Classifier: Topic ::
-Utilities Requires-Dist: appdirs (>=1.4.4,<2.0.0) Requires-Dist: beautifulsoup4
-(>=4.12.2,<5.0.0) Requires-Dist: click (>=8.1.3,<9.0.0) Requires-Dist:
-coloredlogs (>=15.0.1,<16.0.0) Requires-Dist: jsonpickle (>=3.0.1,<4.0.0)
-Requires-Dist: lxml (>=4.9.2,<5.0.0) Requires-Dist: requests (>=2.28.2,<3.0.0)
-Project-URL: Bug Tracker, https://github.com/rlaphoenix/nton/issues Project-
-URL: Changelog, https://github.com/rlaphoenix/nton/blob/master/CHANGELOG.md
-Project-URL: Forums, https://github.com/rlaphoenix/nton/discussions Project-
-URL: Repository, https://github.com/rlaphoenix/nton Description-Content-Type:
-text/markdown # NTON [![Build status](https://github.com/rlaphoenix/nton/
-actions/workflows/ci.yml/badge.svg)](https://github.com/rlaphoenix/nton/
-actions/workflows/ci.yml) [![PyPI version](https://img.shields.io/pypi/v/nton)]
-(https://pypi.python.org/pypi/nton) [![Python versions](https://img.shields.io/
-pypi/pyversions/nton)](https://pypi.python.org/pypi/nton) [License_(GPLv3)]
-NTON is a Nintendo Switch NRO to NSP Forwarder for firmware 12.0.0 and newer. A
-forwarder lets you open a Homebrew NRO file from your SD card through the
-Nintendo Switch Home Screen instead of the Homebrew Launcher. ![Preview](https:
-//user-images.githubusercontent.com/17136956/206882948-4f05cace-16a3-4300-9047-
+Utilities Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0) Requires-Dist: click
+(>=8.1.6,<9.0.0) Requires-Dist: coloredlogs (>=15.0.1,<16.0.0) Requires-Dist:
+jsonpickle (>=3.0.1,<4.0.0) Requires-Dist: lxml (>=4.9.3,<5.0.0) Requires-Dist:
+pillow (>=9.5.0,<10.0.0) Requires-Dist: requests (>=2.31.0,<3.0.0) Project-URL:
+Bug Tracker, https://github.com/rlaphoenix/nton/issues Project-URL: Changelog,
+https://github.com/rlaphoenix/nton/blob/master/CHANGELOG.md Project-URL:
+Forums, https://github.com/rlaphoenix/nton/discussions Project-URL: Repository,
+https://github.com/rlaphoenix/nton Description-Content-Type: text/markdown #
+NTON [![Build status](https://github.com/rlaphoenix/nton/actions/workflows/
+ci.yml/badge.svg)](https://github.com/rlaphoenix/nton/actions/workflows/ci.yml)
+[![PyPI version](https://img.shields.io/pypi/v/nton)](https://pypi.python.org/
+pypi/nton) [![Python versions](https://img.shields.io/pypi/pyversions/nton)]
+(https://pypi.python.org/pypi/nton) [License_(GPLv3)] NTON is a Nintendo Switch
+NRO to NSP Forwarder for firmware 12.0.0 and newer. A forwarder lets you open a
+Homebrew NRO file from your SD card through the Nintendo Switch Home Screen
+instead of the Homebrew Launcher. ![Preview](https://user-
+images.githubusercontent.com/17136956/206882948-4f05cace-16a3-4300-9047-
 8cba33106a64.jpg) *Forwarders made with NTON.* ## Features - ð¡ï¸ Safety-
 first approach; System/Game Title IDs cannot be used and NRO files are
 validated - ð¹ï¸ Boot right into an Emulated Game with Direct RetroArch Game
-Forwarding - ð¼ï¸ Supports any Image file of any resolution or format for
-the NSP Icon - ð¤ The Title Name, Publisher, Icon, and more are automatically
-extracted from the NRO - ð¥ Supports Video Capture and Screenshots - â
-Currently Supports Firmware 12.0.0 and up - ð§© Plug-and-play installation via
-PIP/PyPI - â¤ï¸ Forever FOSS! ## Installation *Note: Requires [Python] 3.7.0
-or newer with PIP installed.* ```shell $ pip install nton ``` You now have the
-`nton` package installed and a `nton` executable is now available. Check it out
-with `nton --help` - VoilÃ  ð! *If you see any warnings about a path not
-being in your PATH environment variable, add it, or `nton` won't run.* ###
-Dependencies The following is a list of programs required to be installed
-manually. I recommend installing these with [winget] or [chocolatey] where
-possible as it automatically adds them to your `PATH` environment variable and
-will be easier to update in the future. - [hacBrewPack] for packing the NSP. -
-[ImageMagick] for Icon conversion and preparation. - [nstool] for NRO
+Forwarding - ð¥ Video Capture and Screenshots - ð¼ï¸ Custom Forwarder Icon
+of any resolution or format - ð¤ The Title Name, Publisher, Icon, and more
+are automatically extracted from the NRO - â Currently Supports Firmware
+12.0.0 and up - ð§© Plug-and-play installation via PIP/PyPI - â¤ï¸ Forever
+FOSS! ## Installation > **Note** *Requires [Python] 3.7.0 or newer with PIP
+installed.* ```shell $ pip install nton ``` You now have the `nton` package
+installed and a `nton` executable is now available. Check it out with `nton --
+help` - VoilÃ  ð! > **Warning**
+If pip gives you a warning about a path not being in your PATH environment
+variable then promptly add that path then close all open command prompt
+Windows, or running `nton` won't work as it will not be recognized as a
+program. [Python]:
+python.org> ### 1. Dependencies The following is a list of programs required to
+be installed manually. - [hacBrewPack] for packing the NSP. - [nstool] for NRO
 extraction and verification. - [hptnacp] for creating new NACP partitions if
-the NRO did not have one. For portable downloads, make sure you put them in
-your current working directory, in the installation directory, or put the
-directory path in your `PATH` environment variable. If you do not do this then
-NTON will not be able to find any of the binaries. [winget]:
-winget.run> [chocolatey]:
-chocolatey.org> [hacBrewPack]:
-github.com/The-4n/hacBrewPack> [ImageMagick]:
-imagemagick.org/script/download.php> [nstool]:
+the NRO did not have one. Make sure you put them in your current working
+directory, in NTON's installation directory, or put the dependency's
+installation folder in your `PATH` environment variable. If you do not do this
+then NTON will not be able to find said dependency and will not be able to
+continue. [hacBrewPack]:
+github.com/The-4n/hacBrewPack> [nstool]:
 github.com/jakcron/nstool> [hptnacp]:
-github.com/The-4n/hacPack/tree/master/hacPack-Tools/hacPackTools-NACP> ### Keys
-NTON requires the use of proprietary key data for use in various ways. Place
-your `prod.keys` file at `C:\Users\\.switch\prod.keys` or in your current
-working directory for NTON to be able to find and use your keys. Make sure your
-`prod.keys` file is up-to-date for the firmware version your Nintendo Switch is
-on. It can be extracted from your Nintendo Switch with [Lockpick_RCM](https://
-github.com/shchmue/Lockpick_RCM). ### From Source Code The following steps are
-instructions on downloading, preparing, and running the code under a Poetry
-environment. You can skip steps 3-5 with a simple `pip install .` call instead,
-but you miss out on a wide array of benefits. 1. `git clone https://github.com/
-rlaphoenix/nton` 2. `cd nton` 3. (optional) `poetry config virtualenvs.in-
-project true` 4. `poetry install` 5. `poetry run nton --help` As seen in Step
-5, running the `nton` executable is somewhat different to a normal PIP
-installation. See [Poetry's Docs] on various ways of making calls under the
-virtual-environment. [Python]:
-python.org> [Poetry]:
-python-poetry.org> [Poetry's Docs]:
-python-poetry.org/docs/basic-usage/#using-your-virtual-environment> ## Usage
-Take a look at `nton --help`, specifically `nton build --help`. If you simply
-want to take an NRO and get an NSP forwarder, simply run `nton build ""`. Note
-that the NRO path MUST be on your Switch microSD card. Do not provide a path in
-your C:/ Drive or such. Two different kinds of paths are used based on the
-initial file path, therefore it must be from your Switch microSD card. E.g., to
-make a forwarder for the Homebrew Menu that's on your Switch's microSD at `D:
-\hbmenu.nro`, simply run `nton build "D:/hbmenu.nro"` Take a look at `nton
-build --help` for advanced usage like changing the Icon, Title Name, and so on.
-### Direct RetroArch Game forwarding Use a RetroArch Game Core as the NRO path
-and provide the path to the ROM on your Switch's microSD card with `--rom`.
-This will then load the Core directly under RetroArch and provide the path to
-the ROM as a startup argument to the RetroArch Core. Note: - You must use a
-path to a RetroArch Game Core NRO, not the path to the RetroArch NRO itself. -
-Do not move, delete, or rename the ROM or the Core NRO files that are on your
-microSD card, or it will break. ## Troubleshooting Before continuing try
-running the homebrew from the Homebrew Launcher and see if it works through
-there. If it does not work through the Homebrew launcher either, then it was
-never the forwarder's fault and you should check on your NRO or application
-installation. Please note that using Forwarders others have created has a good
-chance of not working on your system. The location of the NRO on their system
-may differ from the location on your system, hence the NSP won't be able to
-load the homebrew. ### The forwarder does not launch, "The software was closed
-because an error occurred." You're sigpatches that allow non-signed software to
-launch is outdated or not set up correctly. The `prod.keys` you used to create
-the NSP may also be outdated. Get new ones with [Lockpick_RCM] and make sure
-you choose to get keys from whichever SysNAND or EmuNAND is actually on the
-latest firmware. ### The forwarder starts loading but then crashes If it gets
-to the black loading screen with the Nintendo Switch logo, but then crashes,
-you may be setting the NRO path wrong when making the NSP. Make sure it starts
+github.com/The-4n/hacPack/tree/master/hacPack-Tools/hacPackTools-NACP> ### 2.
+Keys Proprietary Keys known as `prod.keys` are required. You can obtain them
+from your own personal Switch using Lockpick_RCM. It must be placed at `C:
+\Users\\.switch\prod.keys`, in your current working directory, or in NTON's
+installation directory for NTON to be able to find and use the keys. ## Usage
+NTON is quite simple, just give it the path to the NRO on your microSD card!
+*For example, to create a forwarder for the Daybreak Homebrew included with
+Atmosphere, it's as simple as:* ```shell nton build "D:/switch/daybreak.nro"
+``` This will build a forwarder with the Title Name, Publisher, Version, and
+Icon automatically extracted from the NRO. The Title ID will be a randomly
+assigned value within generally conformed bounds. You may manually set a value
+with `--name`, `--publisher`, `--version`, `--icon`, and `--id` respectively.
+The Title ID is automatically checked against a periodically updated list of
+pre-existing System and Software Title IDs to ensure a collision does not
+occur. However, you should still be cautious and verify the Title ID is not
+already used by other Software before using. > **Note**
+> While NTON can be used on NRO files stored on your PC, it was designed to be
+used directly from your Switch's > microSD card. If you prefer to create
+forwarders with NRO files on your PC, or for batch purposes, you can specify >
+the path that the NRO file will reside on your microSD card during generation
+with `--sdmc`. For example, to make a forwarder for an NRO that is on your PC:
+```shell nton build "C:/Users/rlaphoenix/Downloads/haze.nro" --sdmc "/switch/
+haze.nro" ``` ### Direct RetroArch Game forwarding Use a RetroArch Game Core as
+the NRO path and provide the path to the ROM on your Switch's microSD card with
+`--rom`. This will then load the Core directly under RetroArch and provide the
+path to the ROM as a startup argument to the RetroArch Core. > **Note** > - You
+must use a path to a RetroArch Game Core NRO, not the path to the RetroArch NRO
+itself. > - Do not move, delete, or rename the ROM or the Core NRO files that
+are on your microSD card, or it will break. ## Troubleshooting Before
+continuing try running the homebrew from the Homebrew Launcher and see if it
+works through there. If it does not work through the Homebrew launcher either,
+then it was never the forwarder's fault, and you should check on your NRO or
+application installation. Please note that using Forwarders others have created
+has a good chance of not working on your system. The location of the NRO on
+their system may differ from the location on your system, hence the NSP won't
+be able to load the homebrew. I will not provide support if you are having an
+issue with a Forwarder you did not build yourself. ### The forwarder does not
+launch, "The software was closed because an error occurred." Your "sigpatches"
+(signature patches) that allow unsigned titles to launch is likely outdated or
+not set up correctly. Sigpatches can go outdated from Horizon OS firmware
+updates, Atmosphere updates (as well as silent updates). It is recommended to
+use the [sys-patch](https://github.com/ITotalJustice/sys-patch) sys-module to
+automatically patch your system from signature checks as well as other useful
+patches. The default configuration is fine for the majority of systems and is a
+simple copy & paste to your microSD card to install. It's also possible the
+`prod.keys` you used with NTON is outdated for your firmware. Get new ones with
+Lockpick_RCM and make sure you choose to get keys from the SysMMC or EmuMMC
+that you will be installing the forwarder on (or whichever has a newer firmware
+version). ### The forwarder starts loading but then crashes The NRO path set
+when building the forwarder is incorrect or the NRO file is currently missing
+(or your microSD card is not inserted). Make sure the path you choose starts
 with `/` and is an absolute path to an existing NRO file on your Switch's
-microSD card. The path you built for must be where the NRO file lies in your
-Switch's microSD card, not your PC. ### The forwarder's icon is a '?' The
-`icon_AmericanEnglish.dat` is not to the spec that Nintendo likes in some way.
-This is usually caused by the format of the image not being a JPEG, or it has
-EXIF data or an embedded color space. I recommend stripping all EXIF metadata
-and saving without an Embed Color Space. You can do this quickly with
-ImageMagick, `magick mogrify -format jpg -resize 256x256 -strip "C:
-\Users\John\Downloads\icon.png"`. ### The forwarder randomly stopped working
-after a while, I changed nothing! You most likely updated your Switch's
-Firmware and need to update your sigpatches. If not, you may have deleted the
-NRO from your Switch's microSD card or moved the NRO somewhere else. It cannot
-be moved as the built NSP loads the NRO at the specified path when you ran
-`build`. It's also possible the firmware update has broken the [forwarder ROM]
-[ROM] that is used and needs to be fixed. Firmware 9.0.0 and 12.0.0 are times
-the firmware has broken different forwarder ROMs in the past. ## Credit -
+microSD card (not your PC). ### The forwarder's icon is a '?' This happens when
+the `icon_AmericanEnglish.dat` within the built forwarder is not to the spec
+that Nintendo likes, in some way. This is usually caused by the format of the
+image not being JPEG, or it has EXIF data or other unnecessary extra metadata.
+> **Note**
+This is considered a bug if it happens to you after using NTON as it should
+automatically sanitize the images when building the forwarder. If this happens
+to you, please report what image you chose to use, or give information on what
+exact NRO you were making a forwarder from. ### The forwarder's icon is a
+loading circle, opening fails The installation of the Forwarder NSP failed in
+some way and the result is a corrupt title under that Title ID. This may have
+happened when trying to install data to the Title ID you chose or had randomly
+assigned to your forwarder NSP on an unsupported firmware version. This also
+happens when trying to install DLC to a Title without having the minimum
+required Game Update for that DLC (i.e. Installing the DLC Courses while on
+Mario Kart 8 Deluxe v1.0). However, since this happened on your Forwarder NSP
+you can likely rule that out. When this happens deleting and reinstalling the
+same NSP likely won't fix it or do anything. You may need to reinstall the NSP
+via Goldleaf and hit "Proceed" when it warns yo uthat the title is already
+installed. Goldleaf will deal with the pre-existing files properly unlike
+Tinfoil (where you likely had the corruption in the first place). DBI may also
+help you resolve this issue as it has tools to remove partial installs and
+leftover files. ### The forwarder randomly stopped working, I've read
+everything so far You most likely updated Atmosphere or Horizon OS's Firmware
+and need to update your Sigpatches. If that hasn't fixed it, make sure you
+haven't deleted or moved the NRO on your Switch's microSD card. It cannot be
+moved as the built forwarder has a hardcoded file path that it loads the NRO
+from when launched. If it still does not work, it's possible a firmware update
+has broken the [forwarder ROM][ROM] that is used and needs to be updated. Both
+Firmware 9.0.0 and 12.0.0 have previously broken different forwarder ROMs
+requiring updates. If you believe this to be the case then please make an
+Issue. ## Development The following steps are basic instructions on downloading
+and working on the code under a [Poetry] environment. 1. Follow Poetry's Docs
+to [Install Poetry]. 2. Download NTON's latest code, `git clone https://
+github.com/rlaphoenix/nton` 3. Navigate to the downloaded code repository, `cd
+nton` 4. _Optionally_ have Poetry install the virtual-env in the project,
+`poetry config virtualenvs.in-project true` 5. Install NTON's dependencies and
+development tools, `poetry install` 6. Run NTON from within the Poetry venv,
+`poetry run nton --help` As shown, running the `nton` executable is somewhat
+different to a normal installation. This is because Poetry installs all
+dependencies and the `nton` shim itself within a virtual-environment, which is
+like a clone of your Python install stripped clean, with only NTON's
+dependencies installed. That way you don't mess around with any dependencies
+from any other installed Python applications, nor the other way around. A
+secluded environment. I recommend taking a look at [Poetry's Docs] for further
+information, why not get started by reading Poetry's guide on [Using Your
+Virtual Environment]. [Poetry]:
+python-poetry.org> [Install Poetry]:
+python-poetry.org/docs/#installation> [Poetry's Docs]:
+python-poetry.org/docs> [Using Your Virtual Environment]:
+python-poetry.org/docs/basic-usage/#using-your-virtual-environment> ## Credit -
 [meliodas2255] for their [Open-Source forwarder ROM][ROM] supporting v12.0.0+
 with both direct RetroArch Forwarding and general forwarding both supported. -
 [vgmoose] for the [sdl-hello-world] NRO that is used in CI/CD testing.
 [meliodas2255]:
 gbatemp.net/members/meliodas2255.410353> [vgmoose]:
 github.com/vgmoose> [ROM]:
 github.com/Skywalker25/Forwarder-Mod> [sdl-hello-world]:
```

