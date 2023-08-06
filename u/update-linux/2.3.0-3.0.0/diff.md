# Comparing `tmp/update-linux-2.3.0.tar.gz` & `tmp/update-linux-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "update-linux-2.3.0.tar", last modified: Mon May 15 09:27:41 2023, max compression
+gzip compressed data, was "update-linux-3.0.0.tar", last modified: Sun Aug  6 10:11:26 2023, max compression
```

## Comparing `update-linux-2.3.0.tar` & `update-linux-3.0.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-05-15 09:27:41.671724 update-linux-2.3.0/
--rw-r--r--   0 barry     (1000) barry     (1000)     5714 2023-05-15 09:27:41.671724 update-linux-2.3.0/PKG-INFO
--rw-r--r--   0 barry     (1000) barry     (1000)     5160 2023-05-15 09:27:41.000000 update-linux-2.3.0/README.md
--rw-r--r--   0 barry     (1000) barry     (1000)       38 2023-05-15 09:27:41.671724 update-linux-2.3.0/setup.cfg
--rw-r--r--   0 barry     (1000) barry     (1000)     2127 2023-04-02 12:26:46.000000 update-linux-2.3.0/setup_update_linux.py
-drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-05-15 09:27:41.671724 update-linux-2.3.0/update_linux/
--rwxr-xr-x   0 barry     (1000) barry     (1000)    23940 2023-05-14 11:36:13.000000 update-linux-2.3.0/update_linux/__init__.py
--rw-r--r--   0 barry     (1000) barry     (1000)      144 2023-04-15 15:36:02.000000 update-linux-2.3.0/update_linux/__main__.py
-drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-05-15 09:27:41.671724 update-linux-2.3.0/update_linux.egg-info/
--rw-r--r--   0 barry     (1000) barry     (1000)     5714 2023-05-15 09:27:41.000000 update-linux-2.3.0/update_linux.egg-info/PKG-INFO
--rw-r--r--   0 barry     (1000) barry     (1000)      299 2023-05-15 09:27:41.000000 update-linux-2.3.0/update_linux.egg-info/SOURCES.txt
--rw-r--r--   0 barry     (1000) barry     (1000)        1 2023-05-15 09:27:41.000000 update-linux-2.3.0/update_linux.egg-info/dependency_links.txt
--rw-r--r--   0 barry     (1000) barry     (1000)       60 2023-05-15 09:27:41.000000 update-linux-2.3.0/update_linux.egg-info/entry_points.txt
--rw-r--r--   0 barry     (1000) barry     (1000)       21 2023-05-15 09:27:41.000000 update-linux-2.3.0/update_linux.egg-info/requires.txt
--rw-r--r--   0 barry     (1000) barry     (1000)       13 2023-05-15 09:27:41.000000 update-linux-2.3.0/update_linux.egg-info/top_level.txt
+drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-08-06 10:11:26.339997 update-linux-3.0.0/
+-rw-r--r--   0 barry     (1000) barry     (1000)    11357 2023-07-31 10:07:15.000000 update-linux-3.0.0/LICENSE
+-rw-r--r--   0 barry     (1000) barry     (1000)     6534 2023-08-06 10:11:26.339997 update-linux-3.0.0/PKG-INFO
+-rw-r--r--   0 barry     (1000) barry     (1000)     5894 2023-08-06 10:10:09.000000 update-linux-3.0.0/README.md
+-rw-r--r--   0 barry     (1000) barry     (1000)      992 2023-07-31 11:05:10.000000 update-linux-3.0.0/pyproject.toml
+-rw-r--r--   0 barry     (1000) barry     (1000)       38 2023-08-06 10:11:26.339997 update-linux-3.0.0/setup.cfg
+drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-08-06 10:11:26.339997 update-linux-3.0.0/src/
+drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-08-06 10:11:26.339997 update-linux-3.0.0/src/update_linux/
+-rwxr-xr-x   0 barry     (1000) barry     (1000)    26926 2023-08-06 10:04:41.000000 update-linux-3.0.0/src/update_linux/__init__.py
+-rw-r--r--   0 barry     (1000) barry     (1000)      144 2023-04-15 15:36:02.000000 update-linux-3.0.0/src/update_linux/__main__.py
+drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-08-06 10:11:26.339997 update-linux-3.0.0/src/update_linux.egg-info/
+-rw-r--r--   0 barry     (1000) barry     (1000)     6534 2023-08-06 10:11:26.000000 update-linux-3.0.0/src/update_linux.egg-info/PKG-INFO
+-rw-r--r--   0 barry     (1000) barry     (1000)      332 2023-08-06 10:11:26.000000 update-linux-3.0.0/src/update_linux.egg-info/SOURCES.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)        1 2023-08-06 10:11:26.000000 update-linux-3.0.0/src/update_linux.egg-info/dependency_links.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)       60 2023-08-06 10:11:26.000000 update-linux-3.0.0/src/update_linux.egg-info/entry_points.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)       33 2023-08-06 10:11:26.000000 update-linux-3.0.0/src/update_linux.egg-info/requires.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)       13 2023-08-06 10:11:26.000000 update-linux-3.0.0/src/update_linux.egg-info/top_level.txt
```

### Comparing `update-linux-2.3.0/PKG-INFO` & `update-linux-3.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,38 @@
-Metadata-Version: 2.1
-Name: update-linux
-Version: 2.3.0
-Summary: Update Linux
-Home-page: https://github.com/barry-scott/CLI-tools
-Author: Barry Scott
-Author-email: barry@barrys-emacs.org
-License: Apache 2.0
-Keywords: development
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Topic :: Utilities
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-
 # update-linux command
 
 Command to automate the routine updating of packages and system upgrading for Unix systems.
 
+update-linuk can check for updates (--check), install updates (--update) and do a system upgrade (--system-upgrade).
+
 Supports Fedora like and Debian Like OS.
 
 Fedora like includes Fedora, RHEL, Centos, Rocky etc that use DNF.
 
 Debian like includes Dedian, Ubuntu etc that use apt.
 
-update-linux uses ssh to run commands on the hosts being worked.
+update-linux uses ssh to run commands on the hosts being worked on.
 
 It assumes that it can `ssh root@<host>` without a password prompt.
 
+However when using the --self option to update localhost sudo will be used if not running as root. This will prompt for the sudo password as necessary.
+Normally update-linux will reboot a host if that is required, but when working on --self no reboot is done unless --force-reboot is used.
+
 If running update-linux on a macOS system it is necessary to flush DNS so that freshly booted hosts can be accessed by host-name.
 
 This is done with the command `sudo killall -HUP mDNSResponder`.
 
-update-linux will refuse to update the host it is running on.
+update-linux will refuse to update the host it is running on unless the -self options is used.
+
+Normally a reboot is done at the conclusion of an update unless update-linux can determine that the reboot is not required.
 
 ## update-linux update process
 
 ```
-$ update-linux host
+$ update-linux --update host
 ```
 
 For an update the following steps are performed:
 
 1. Update packages  - if there is nothing to update stop here
 
     Fedora: `dnf -vy update --refresh`
@@ -51,14 +41,18 @@
 
 1. Wait until all systemd jobs have finished
 
     `systemctl list-jobs`
 
     For example akmod building nvidia drivers for a new kernel
 
+1. Check if a reboot is needed.
+
+    `dnf needs-restart -r`
+
 1. Reboot the host
 
     `reboot`
 
 1. Report on state of any failed services
 
     `systemctl --failed`
@@ -73,15 +67,15 @@
 
 1. Check if there are packages to update
 
     Fedora: `dnf check-update --refresh`
 
     Debian: `apt-get update --assume-yes` then `apt-get upgrade --assume-no`
 
-1. Report on state of any failed services
+1. Report on state of any failed services. Not possible upgrading localhost with --self.
 
     `systemctl --failed`
 
 ## update-linux system-upgrade process
 
 ```
 $ update-linux --system-upgrade=38 host
@@ -109,15 +103,15 @@
 
     `dnf system-upgrade reboot`
 
 1. Wait for the system to reboot
 
     There is a limit of 45 minutes to wait for the reboot
 
-1. Report on state of any failed services
+1. Report on state of any failed services. Not possible upgrading localhost with --self.
 
     `systemctl --failed`
 
 ## update-linux command
 
 ```
 Usage: update-linux <options> <group>|<host>...
```

### Comparing `update-linux-2.3.0/update_linux/__init__.py` & `update-linux-3.0.0/src/update_linux/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import sys
+import os
 import datetime
 import subprocess
 import time
 import socket
 import platform
 import tempfile
 import json
 from config_path import ConfigPath  # type: ignore
 
-VERSION = '2.3.0'
+VERSION = '3.0.0'
 
 default_json_config_template = u'''{
     "group":
         {"all": []},
     "logdir":   "%(logdir)s"
 }
 '''
@@ -71,21 +72,26 @@
 
     def __call__( self ):
         return self.value
 
     def help( self ):
         all_help = []
         if self.value_type is not None:
-            all_help.append( '%s=%s default %s' %
-                (self.name
-                ,self.value_name
-                ,{True: 'On', False: 'Off'}.get( self.default, self.default ) ))
+            if self.default is None:
+                all_help.append( '%s=%s' %
+                    (self.name
+                    ,self.value_name))
+            else:
+                all_help.append( '%s=%s (default %s)' %
+                    (self.name
+                    ,self.value_name
+                    ,{True: 'On', False: 'Off'}.get( self.default, self.default ) ))
 
         else:
-            all_help.append( '%s default %s' %
+            all_help.append( '%s (default %s)' %
                 (self.name
                 ,{True: 'On', False: 'Off'}.get( self.default, self.default ) ))
 
         if self.description:
             for line in self.description.split('\n'):
                 all_help.append( '    %s' % (line,) )
 
@@ -124,29 +130,35 @@
         self.all_hosts = []
         self.opt_help = Option( '--help', False,
                             description='print this help' )
         self.opt_debug = Option( '--debug', False,
                             description='print debug messages' )
         self.opt_check = Option( '--check', False,
                             description='check if update is required' )
-        self.opt_exclude = Option( '--exclude', None, value_type=str, value_name='<host>',
-                            description='exclude the <host> from being updated'  )
+        self.opt_update = Option( '--update', False,
+                            description='perform update of installed packages' )
         self.opt_system_upgrade = Option( '--system-upgrade', None, value_type=int, value_name='<version>',
                             description='perform a system upgrade to version <version>' )
+        self.opt_exclude = Option( '--exclude', None, value_type=str, value_name='<host>',
+                            description='exclude the <host> from being updated'  )
         self.opt_force_reboot = Option( '--force-reboot', False,
-                            description='always reboot host even if no packages where updated' )
+                            description='reboot if required for --update --self.\n'
+                                        'For remote system --update always reboot host even if no packages where updated' )
         self.opt_install_package = Option( '--install-package', None, value_type=str, value_name='<package>',
                             description='install <package> only' )
         self.opt_list_config = Option( '--list-config', False,
                             description='list the configuration from the JSON config file' )
+        self.opt_update_self = Option( '--self', False,
+                            description='apply command to this computer')
 
         self.ct = ColourText()
         self.ct.initTerminal()
         self.ct.define( 'host', 'lightblue' )
         self.ct.define( 'proc', 'magenta' )
+        self.ct.define( 'file', 'magenta' )
 
         t = datetime.datetime.now()
         self.ts = t.strftime( '%Y-%m-%d' )
         self.summary_log_name = None
         self.summary_log = None
         self.all_summary_lines = []
 
@@ -164,24 +176,32 @@
 
         except OptionError as e:
             self.error( '', str(e) )
             return 1
 
         if self.opt_help:
             print(
-'''Usage: %(appname)s <options> <group>|<host>...
+'''Usage: %(appname)s <options> <group>|<host>|--self...
 
     %(appname)s version %(version)s
 
+    Run one of the commands --check, --update, --system-upgrade
+    or --install-package on a group of hosts.
+
     group - read from the JSON config file:
             %(config_file)s
 
-        each group is a list of hosts to be updated
+        each group is a list of hosts to act on
+
+    host - host to on
 
-    host - host to be updated
+    --self - commands apply to this computer.
+             By default on reboot is done.
+             Use --force-reboot to reboot when required
+             to complete the command.
 
     options:''' % {'appname': appname.name
                   ,'version': VERSION
                   ,'config_file': self.config.readFilePath()} )
 
             printOptionsHelp( self )
             return 0
@@ -198,15 +218,18 @@
             print( 'Log directory: %s' % (self.logdir,) )
             return 0
 
         all_to_exclude = []
         if self.opt_exclude:
             all_to_exclude = self.all_groups.get( self.opt_exclude(), self.opt_exclude() )
 
-        self.all_hosts = list( self.hostIter( positional_args ) )
+        if self.opt_update_self:
+            self.all_hosts = [None]
+        else:
+            self.all_hosts = list( self.hostIter( positional_args ) )
 
         if len(self.all_hosts) == 0:
             self.error( '', 'No hosts to update' )
             print('''
 For help:
     %s --help
 ''' % (appname.name,))
@@ -218,51 +241,56 @@
             t = datetime.datetime.now()
             self.header( 'Update summary %s' % (t.strftime( '%Y-%m-%d %H:%M:%S' ),) )
 
             for host in self.all_hosts:
                 if host in all_to_exclude:
                     continue
 
-                os_plugin_type, os_id = self.detectOperatingSystem( host )
+                os_plugin_type, os_id, os_version = self.detectOperatingSystem( host )
                 if os_plugin_type is None:
                     if os_id is not None:
-                        self.warn( host, 'Unsupported OS type %s' % (os_id,) )
+                        self.warn( host, 'Unsupported OS type %s %s' % (os_id, os_version) )
                     continue
 
-                self.info( host, 'OS is %s. Using OS plugin %s' % (os_id, os_plugin_type) )
+                self.info( host, 'OS is %s %s. Using OS plugin %s' % (os_id, os_version, os_plugin_type) )
 
                 plugin = os_id_to_plugin[ os_plugin_type ]( self )
 
                 self.flushDns()
                 if self.opt_check:
                     plugin.check( host,
-                        check_log_name=self.logdir / ('check-update-%s-%s.log' % (host, self.ts)) )
+                        check_log_name=self.logdir / ('check-update-%s-%s.log' % (host or 'localhost', self.ts)) )
 
                 elif self.opt_install_package() is not None:
-                    self.installPackage( host, self.opt_install_package,
-                        update_log_name=self.logdir / ('install-%s-%s.log' % (host, self.ts)) )
+                    plugin.installPackage( host, self.opt_install_package(),
+                        install_log_name=self.logdir / ('install-%s-%s.log' % (host or 'localhost', self.ts)) )
 
                 else:
-                    if self.isThisHost( host ):
+                    if host is not None and self.isThisHost( host ):
                         self.warn( host, 'Refusing to update this host' )
 
                     elif self.opt_system_upgrade:
-                        plugin.systemUpgrade( host, self.opt_system_upgrade,
-                            upgrade_log_name=self.logdir / ('upgrade-%s-%s.log' % (host, self.ts)) )
+                        plugin.systemUpgrade( host, self.opt_system_upgrade(),
+                            upgrade_log_name=self.logdir / ('upgrade-%s-%s.log' % (host or 'localhost', self.ts)) )
 
-                    else:
+                    elif self.opt_update:
                         plugin.update( host,
-                            update_log_name=self.logdir / ('update-%s-%s.log' % (host, self.ts)),
-                            status_log_name=self.logdir / ('status-%s-%s.log' % (host, self.ts)) )
+                            update_log_name=self.logdir / ('update-%s-%s.log' % (host or 'localhost', self.ts)),
+                            status_log_name=self.logdir / ('status-%s-%s.log' % (host or 'localhost', self.ts)) )
+
+                    else:
+                        self.error( host, 'What action do you wish performed? --check --update or --system-upgrade' )
+                        return 1
 
-        print( '-' * 60 )
-        for line in self.all_summary_lines:
-            print( line )
+        if not self.opt_check:
+            print( '-' * 60 )
+            for line in self.all_summary_lines:
+                print( line )
 
-        return 0
+            return 0
 
     def hostIter( self, all_groups_or_hosts, _handled=None ):
         if _handled is None:
             _handled = set()
 
         for group_or_host in all_groups_or_hosts:
             # deal with recursive groups and duplicate host
@@ -338,44 +366,50 @@
 
         # mac often needs its DNS cache flushing as it will
         # not notice newly booted hosts
         cmd = ['sudo', 'killall', '-HUP', 'mDNSResponder']
         self.runAndLog( None, cmd, log=False )
 
     def detectOperatingSystem( self, host ):
-        rc = ssh_wait( host, wait=False, log_fn=None )
-        if rc != 0:
-            self.warn( host, 'Is not reachable' )
-            return None, None
+        if host is not None:
+            rc = ssh_wait( host, wait=False, log_fn=None )
+            if rc != 0:
+                self.warn( host, 'Is not reachable' )
+                return None, None, None
 
         os_release = {}
 
-        cmd = ['cat', '/etc/os-release']
-        rc, stdout = self.runAndLog( host, cmd, log=False )
-        for line in stdout:
-            line = line.strip()
-            if line == '' or '=' not in line:
-                continue
-
-            key, value = line.split( '=', 1 )
-            if value.startswith('"') and value.endswith('"'):
-                value = value[1:-1]
-            os_release[key] = value
+        try:
+            with open( '/etc/os-release' ) as f:
+                for line in f:
+                    line = line.strip()
+                    if line == '' or '=' not in line:
+                        continue
+
+                    key, value = line.split( '=', 1 )
+                    if value.startswith('"') and value.endswith('"'):
+                        value = value[1:-1]
+                    os_release[key] = value
+
+        except IOError as e:
+            self.error( host, str(e) )
+            return None, None, None
 
         os_main_id = os_release.get('ID', None)
         os_id_set = set([os_main_id])
+        os_version_id = os_release.get('VERSION_ID', 'Unknown')
         if 'ID_LIKE' in os_release:
             for ID in os_release['ID_LIKE'].split():
                 os_id_set.add( ID )
 
         for os_id in os_id_set:
             if os_id in os_id_to_plugin:
-                return os_id, os_main_id
+                return os_id, os_main_id, os_version_id
 
-        return None, os_main_id
+        return None, os_main_id, os_version_id
 
     def reboot( self, host, cmd, wait_limit=600 ):
         while True:
             rc, stdout = self.runAndLog( host, cmd )
             if len(stdout) == 0:
                 # no messages assume ok
                 break
@@ -403,15 +437,15 @@
         cmd = ['systemctl', '--failed']
         rc, stdout = self.runAndLog( host, cmd, log=False )
         if log_name is not None:
             self.writeLines( log_name, stdout )
 
         if len(stdout) < 1 and not stdout[0].startswith( '0 loaded units listed.' ):
             for line in stdout:
-                print( self.ct( '<>proc %s<>: %s' % (host, line.rstrip()) ) )
+                print( self.ct( '<>proc %s<>: %s' % (host or 'localhost', line.rstrip()) ) )
 
             self.error( host, 'Some services failed' )
             return False
 
         self.info( host, 'All services running' )
         return True
 
@@ -431,25 +465,28 @@
 
             time.sleep( 10 )
 
     def runAndLog( self, host, cmd, log=True ):
         if host is not None:
             cmd = ['ssh', 'root@%s' % (host,)] + cmd
 
+        elif os.getuid() != 0:
+            cmd = ['sudo'] + cmd
+
         self.debug( 'runAndLog( %s )' % (' '.join( cmd ),) )
         stdout = []
         p = subprocess.Popen( cmd, stderr=subprocess.STDOUT, stdout=subprocess.PIPE )
         while True:
             line = p.stdout.readline()
             if line == b'':
                 break
 
             line = line.decode( 'utf-8' )
             if log:
-                print( self.ct( '<>proc %s<>: %s' % (host, line.rstrip()) ) )
+                print( self.ct( '<>proc %s<>: %s' % (host or 'localhost', line.rstrip()) ) )
 
             stdout.append( line )
 
         p.wait( 5 )
         self.debug( 'runAndLog rc=%d' % (p.returncode,) )
         return p.returncode, stdout
 
@@ -460,21 +497,21 @@
 
     # log functions
     def debug( self, msg ):
         if self.opt_debug:
             print( self.ct( '<>red Debug:<> %s' % (msg,) ), flush=True )
 
     def info( self, host, msg ):
-        self._log( '<>info %(TIME)s<> <>host %(HOST)10s<> %(MSG)s', host, msg )
+        self._log( '<>info %(TIME)s<> <>host %(HOST)10s<> %(MSG)s', host or 'localhost', msg )
 
     def error( self, host, msg ):
-        self._log( '<>error %(TIME)s<> <>host %(HOST)10s<> <>error %(MSG)s<>', host, msg )
+        self._log( '<>error %(TIME)s<> <>host %(HOST)10s<> <>error %(MSG)s<>', host or 'localhost', msg )
 
     def warn( self, host, msg ):
-        self._log( '<>em %(TIME)s<> <>host %(HOST)10s<> <>em %(MSG)s<>', host, msg )
+        self._log( '<>em %(TIME)s<> <>host %(HOST)10s<> <>em %(MSG)s<>', host or 'localhost', msg )
 
     def header( self, msg ):
         self._log( '<>em %(MSG)s<>', '', msg )
 
     def _log( self, fmt, host, msg ):
         t = datetime.datetime.now()
         log_line = self.ct( fmt % {'HOST': host
@@ -500,44 +537,46 @@
         rc, stdout = self.app.runAndLog( host, cmd, log=False )
         self.app.writeLines( check_log_name, stdout )
 
         if rc == 0:
             self.app.info( host, 'Already up to date' )
 
         elif rc == 100:
-            self.app.warn( host, 'Updates available' )
+            self.app.warn( host, 'Updates available. See<> <>file %s<> <>em for details' % (check_log_name,) )
 
         else:
             self.app.error( host, 'check-update failed' )
 
         self.app.checkServices( host, check_log_name )
 
         release = self.releaseInfo( host )
         self.app.info( host, 'Running on release %s' % (release,) )
 
     def installPackage( self, host, package, install_log_name ):
-        rc = ssh_wait( host, wait=False, log_fn=None )
-        if rc != 0:
-            self.app.warn( host, 'Is not reachable' )
-            return
+        if host is not None:
+            rc = ssh_wait( host, wait=False, log_fn=None )
+            if rc != 0:
+                self.app.warn( host, 'Is not reachable' )
+                return
 
         cmd = ['dnf', '-y', 'install', '--refresh', package]
         rc, stdout = self.app.runAndLog( host, cmd )
 
         self.app.writeLines( install_log_name, stdout )
 
         if rc != 0:
             self.app.error( host, 'Install failed' )
             return
 
     def update( self, host, update_log_name, status_log_name ):
-        rc = ssh_wait( host, wait=False, log_fn=None )
-        if rc != 0:
-            self.app.warn( host, 'Is not reachable' )
-            return
+        if host is not None:
+            rc = ssh_wait( host, wait=False, log_fn=None )
+            if rc != 0:
+                self.app.warn( host, 'Is not reachable' )
+                return
 
         self.app.info( host, 'Starting Update' )
 
         cmd = ['dnf', '-vy', 'update', '--refresh']
         rc, stdout = self.app.runAndLog( host, cmd )
 
         self.app.writeLines( update_log_name, stdout )
@@ -547,26 +586,53 @@
             return
 
         if 'Nothing to do.\n' in stdout:
             self.app.info( host, 'Already up to date' )
             if not self.app.opt_force_reboot:
                 return
 
+        # look for reasons to reboot
+        reboot_required = False
+
+        for line in stdout:
+            if line.startswith( 'Installed: kernel-' ):
+                self.app.info( 'Reboot required to install new kernel' )
+                reboot_required = True
+
+            elif( line.startswith( 'Installed: akmod-nvidia' )
+            or line.startswith( 'Upgraded: akmod-nvidia' ) ):
+                self.app.info( 'Reboot required to install new akmod-nvidia' )
+                reboot_required = True
+
         self.app.waitAllSystemdJobsFinished( host, update_log_name )
 
-        self.app.info( host, 'Rebooting' )
-        if self.app.reboot( host, ['reboot'] ):
-            self.app.checkServices( host, status_log_name )
+        # see if there are an services that need a restart
+        cmd = ['dnf', 'needs-restarting', '-r']
+        rc, stdout = self.app.runAndLog( host, cmd )
+        if rc != 0:
+            self.app.info( host, 'Reboot required to restart services' )
+            reboot_required = True
+
+        if reboot_required:
+            if host is None and not self.opt.opt_force_reboot:
+                self.app.info( host, 'Reboot is required - reboot at your convenience to complete update' )
+
+            else:
+                self.app.info( host, 'Rebooting' )
+                if self.app.reboot( host, ['reboot'] ):
+                    self.app.checkServices( host, status_log_name )
 
     def systemUpgrade( self, host, target_release, upgrade_log_name ):
-        current_release = self.app.releaseInfo( host )
-        if current_release == target_release:
-            self.app.info( host, 'Already running release %d' % (target_release,) )
+        current_release = self.releaseInfo( host )
+        if current_release >= target_release:
+            self.app.info( host, 'Already running release %d' % (current_release,) )
             return
 
+        return
+
         self.app.info( host, 'Currently release %d' % (current_release,) )
 
         # only update by one release at a time
         next_release = current_release + 1
 
         cmd = ['dnf', 'system-upgrade', 'download', '--releasever=%d' % (next_release,), '--assumeyes']
         rc, stdout = self.app.runAndLog( host, cmd )
@@ -577,15 +643,15 @@
             return
 
         self.app.info( host, 'Rebooting to install system-upgrade' )
         # upgrades of lots of packages can be slow - wait for 45 minutes
         if self.app.reboot( host, ['dnf', 'system-upgrade', 'reboot'], wait_limit=45*60 ):
             self.app.checkServices( host, upgrade_log_name )
 
-        self.app.info( host, 'Now running release %d' % (self.app.releaseInfo( host ),) )
+        self.app.info( host, 'Now running release %d' % (self.releaseInfo( host ),) )
 
     def releaseInfo( self, host ):
         cmd = ['cat', '/etc/system-release-cpe']
         rc, stdout = self.app.runAndLog( host, cmd, log=False )
         cpe_parts = stdout[0].strip().split( ':' )
         if len(cpe_parts) >= 4:
             return int( cpe_parts[4] )
```

### Comparing `update-linux-2.3.0/update_linux.egg-info/PKG-INFO` & `update-linux-3.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 Metadata-Version: 2.1
 Name: update-linux
-Version: 2.3.0
-Summary: Update Linux
-Home-page: https://github.com/barry-scott/CLI-tools
-Author: Barry Scott
-Author-email: barry@barrys-emacs.org
+Version: 3.0.0
+Summary: Command to automate the routine updating of packages and system upgrading for Unix systems.
+Author-email: Barry Scott <barry@barrys-emacs.org>
 License: Apache 2.0
+Project-URL: Homepage, https://github.com/barry-scott/CLI-tools
+Project-URL: Bug Tracker, https://github.com/barry-scott/CLI-tools/issues
 Keywords: development
-Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Utilities
 Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # update-linux command
 
 Command to automate the routine updating of packages and system upgrading for Unix systems.
 
+update-linuk can check for updates (--check), install updates (--update) and do a system upgrade (--system-upgrade).
+
 Supports Fedora like and Debian Like OS.
 
 Fedora like includes Fedora, RHEL, Centos, Rocky etc that use DNF.
 
 Debian like includes Dedian, Ubuntu etc that use apt.
 
-update-linux uses ssh to run commands on the hosts being worked.
+update-linux uses ssh to run commands on the hosts being worked on.
 
 It assumes that it can `ssh root@<host>` without a password prompt.
 
+However when using the --self option to update localhost sudo will be used if not running as root. This will prompt for the sudo password as necessary.
+Normally update-linux will reboot a host if that is required, but when working on --self no reboot is done unless --force-reboot is used.
+
 If running update-linux on a macOS system it is necessary to flush DNS so that freshly booted hosts can be accessed by host-name.
 
 This is done with the command `sudo killall -HUP mDNSResponder`.
 
-update-linux will refuse to update the host it is running on.
+update-linux will refuse to update the host it is running on unless the -self options is used.
+
+Normally a reboot is done at the conclusion of an update unless update-linux can determine that the reboot is not required.
 
 ## update-linux update process
 
 ```
-$ update-linux host
+$ update-linux --update host
 ```
 
 For an update the following steps are performed:
 
 1. Update packages  - if there is nothing to update stop here
 
     Fedora: `dnf -vy update --refresh`
@@ -51,14 +58,18 @@
 
 1. Wait until all systemd jobs have finished
 
     `systemctl list-jobs`
 
     For example akmod building nvidia drivers for a new kernel
 
+1. Check if a reboot is needed.
+
+    `dnf needs-restart -r`
+
 1. Reboot the host
 
     `reboot`
 
 1. Report on state of any failed services
 
     `systemctl --failed`
@@ -73,15 +84,15 @@
 
 1. Check if there are packages to update
 
     Fedora: `dnf check-update --refresh`
 
     Debian: `apt-get update --assume-yes` then `apt-get upgrade --assume-no`
 
-1. Report on state of any failed services
+1. Report on state of any failed services. Not possible upgrading localhost with --self.
 
     `systemctl --failed`
 
 ## update-linux system-upgrade process
 
 ```
 $ update-linux --system-upgrade=38 host
@@ -109,15 +120,15 @@
 
     `dnf system-upgrade reboot`
 
 1. Wait for the system to reboot
 
     There is a limit of 45 minutes to wait for the reboot
 
-1. Report on state of any failed services
+1. Report on state of any failed services. Not possible upgrading localhost with --self.
 
     `systemctl --failed`
 
 ## update-linux command
 
 ```
 Usage: update-linux <options> <group>|<host>...
```

