# Comparing `tmp/pyjs8call-0.2.2.tar.gz` & `tmp/pyjs8call-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjs8call-0.2.2.tar", last modified: Fri Jan 26 15:45:26 2024, max compression
+gzip compressed data, was "pyjs8call-0.2.3.tar", last modified: Fri May 31 19:57:31 2024, max compression
```

## Comparing `pyjs8call-0.2.2.tar` & `pyjs8call-0.2.3.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 otisbyron  (1000) otisbyron  (1000)        0 2024-01-26 15:45:26.198984 pyjs8call-0.2.2/
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)     1119 2022-12-26 14:28:50.000000 pyjs8call-0.2.2/LICENSE
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    17075 2024-01-26 15:45:26.198984 pyjs8call-0.2.2/PKG-INFO
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    16502 2024-01-26 15:44:42.000000 pyjs8call-0.2.2/README.md
-drwxr-xr-x   0 otisbyron  (1000) otisbyron  (1000)        0 2024-01-26 15:45:26.188984 pyjs8call-0.2.2/pyjs8call/
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)     2092 2024-01-26 15:44:42.000000 pyjs8call-0.2.2/pyjs8call/__init__.py
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    11133 2024-01-26 15:44:42.000000 pyjs8call-0.2.2/pyjs8call/appmonitor.py
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    98621 2024-01-26 15:44:42.000000 pyjs8call-0.2.2/pyjs8call/client.py
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    17847 2024-01-26 15:44:42.000000 pyjs8call-0.2.2/pyjs8call/confighandler.py
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)     7869 2024-01-26 15:44:42.000000 pyjs8call-0.2.2/pyjs8call/hbnetwork.py
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    15759 2024-01-26 15:44:42.000000 pyjs8call-0.2.2/pyjs8call/inboxmonitor.py
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    36118 2024-01-26 15:44:42.000000 pyjs8call-0.2.2/pyjs8call/js8call.py
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    28322 2024-01-26 15:44:42.000000 pyjs8call-0.2.2/pyjs8call/message.py
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    11368 2024-01-26 15:44:42.000000 pyjs8call-0.2.2/pyjs8call/notifications.py
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    17080 2024-01-26 15:44:42.000000 pyjs8call-0.2.2/pyjs8call/offsetmonitor.py
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)     7660 2024-01-26 15:44:42.000000 pyjs8call-0.2.2/pyjs8call/outgoingmonitor.py
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    15147 2024-01-26 15:44:42.000000 pyjs8call-0.2.2/pyjs8call/propagation.py
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    14103 2024-01-26 15:44:42.000000 pyjs8call-0.2.2/pyjs8call/schedulemonitor.py
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)     9209 2024-01-26 15:44:42.000000 pyjs8call-0.2.2/pyjs8call/spotmonitor.py
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    21157 2023-06-25 19:49:03.000000 pyjs8call-0.2.2/pyjs8call/timemonitor.py
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    10682 2024-01-26 15:44:42.000000 pyjs8call-0.2.2/pyjs8call/windowmonitor.py
-drwxr-xr-x   0 otisbyron  (1000) otisbyron  (1000)        0 2024-01-26 15:45:26.188984 pyjs8call-0.2.2/pyjs8call.egg-info/
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    17075 2024-01-26 15:45:25.000000 pyjs8call-0.2.2/pyjs8call.egg-info/PKG-INFO
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)      659 2024-01-26 15:45:25.000000 pyjs8call-0.2.2/pyjs8call.egg-info/SOURCES.txt
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)        1 2024-01-26 15:45:25.000000 pyjs8call-0.2.2/pyjs8call.egg-info/dependency_links.txt
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)       12 2024-01-26 15:45:25.000000 pyjs8call-0.2.2/pyjs8call.egg-info/requires.txt
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)       10 2024-01-26 15:45:25.000000 pyjs8call-0.2.2/pyjs8call.egg-info/top_level.txt
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)       38 2024-01-26 15:45:26.198984 pyjs8call-0.2.2/setup.cfg
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)      823 2024-01-26 15:44:42.000000 pyjs8call-0.2.2/setup.py
-drwxr-xr-x   0 otisbyron  (1000) otisbyron  (1000)        0 2024-01-26 15:45:26.198984 pyjs8call-0.2.2/tests/
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)     3971 2023-06-25 19:49:03.000000 pyjs8call-0.2.2/tests/test_cross_platform.py
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)     1672 2023-02-25 18:49:44.000000 pyjs8call-0.2.2/tests/test_helpers.py
--rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)     1222 2023-06-25 19:49:03.000000 pyjs8call-0.2.2/tests/test_start.py
+drwxr-xr-x   0 otisbyron  (1000) otisbyron  (1000)        0 2024-05-31 19:57:31.475439 pyjs8call-0.2.3/
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)     1119 2022-12-26 14:28:50.000000 pyjs8call-0.2.3/LICENSE
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    19946 2024-05-31 19:57:31.475439 pyjs8call-0.2.3/PKG-INFO
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    19346 2024-05-31 19:56:24.000000 pyjs8call-0.2.3/README.md
+drwxr-xr-x   0 otisbyron  (1000) otisbyron  (1000)        0 2024-05-31 19:57:31.465438 pyjs8call-0.2.3/pyjs8call/
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)     2124 2024-05-31 19:34:15.000000 pyjs8call-0.2.3/pyjs8call/__init__.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)     6717 2024-05-31 19:34:15.000000 pyjs8call-0.2.3/pyjs8call/__main__.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    12079 2024-05-31 19:34:15.000000 pyjs8call-0.2.3/pyjs8call/appmonitor.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    10516 2024-05-31 19:34:15.000000 pyjs8call-0.2.3/pyjs8call/callbacks.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    71371 2024-05-31 19:34:15.000000 pyjs8call-0.2.3/pyjs8call/client.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    18063 2024-05-31 19:34:15.000000 pyjs8call-0.2.3/pyjs8call/confighandler.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)     8111 2024-05-31 19:34:15.000000 pyjs8call-0.2.3/pyjs8call/hbnetwork.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    16498 2024-05-31 19:34:15.000000 pyjs8call-0.2.3/pyjs8call/inboxmonitor.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    38244 2024-05-31 19:34:15.000000 pyjs8call-0.2.3/pyjs8call/js8call.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    32483 2024-05-31 19:34:15.000000 pyjs8call-0.2.3/pyjs8call/message.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    13303 2024-05-31 19:34:15.000000 pyjs8call-0.2.3/pyjs8call/notifications.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    17012 2024-05-31 19:34:15.000000 pyjs8call-0.2.3/pyjs8call/offsetmonitor.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)     7660 2024-01-26 15:44:42.000000 pyjs8call-0.2.3/pyjs8call/outgoingmonitor.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    23576 2024-05-31 19:34:15.000000 pyjs8call-0.2.3/pyjs8call/propagation.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    15723 2024-05-31 19:34:15.000000 pyjs8call-0.2.3/pyjs8call/schedulemonitor.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    47994 2024-05-31 19:34:15.000000 pyjs8call-0.2.3/pyjs8call/settings.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    10275 2024-05-31 19:34:15.000000 pyjs8call-0.2.3/pyjs8call/spotmonitor.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    21246 2024-05-31 19:34:15.000000 pyjs8call-0.2.3/pyjs8call/timemonitor.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    10682 2024-01-26 15:44:42.000000 pyjs8call-0.2.3/pyjs8call/windowmonitor.py
+drwxr-xr-x   0 otisbyron  (1000) otisbyron  (1000)        0 2024-05-31 19:57:31.475439 pyjs8call-0.2.3/pyjs8call.egg-info/
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    19946 2024-05-31 19:57:31.000000 pyjs8call-0.2.3/pyjs8call.egg-info/PKG-INFO
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)      726 2024-05-31 19:57:31.000000 pyjs8call-0.2.3/pyjs8call.egg-info/SOURCES.txt
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)        1 2024-05-31 19:57:31.000000 pyjs8call-0.2.3/pyjs8call.egg-info/dependency_links.txt
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)       12 2024-05-31 19:57:31.000000 pyjs8call-0.2.3/pyjs8call.egg-info/requires.txt
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)       10 2024-05-31 19:57:31.000000 pyjs8call-0.2.3/pyjs8call.egg-info/top_level.txt
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)       38 2024-05-31 19:57:31.475439 pyjs8call-0.2.3/setup.cfg
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)      823 2024-05-31 19:34:15.000000 pyjs8call-0.2.3/setup.py
+drwxr-xr-x   0 otisbyron  (1000) otisbyron  (1000)        0 2024-05-31 19:57:31.475439 pyjs8call-0.2.3/tests/
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)     3971 2023-06-25 19:49:03.000000 pyjs8call-0.2.3/tests/test_cross_platform.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)     1672 2023-02-25 18:49:44.000000 pyjs8call-0.2.3/tests/test_helpers.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)     1222 2023-06-25 19:49:03.000000 pyjs8call-0.2.3/tests/test_start.py
```

### Comparing `pyjs8call-0.2.2/LICENSE` & `pyjs8call-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjs8call-0.2.2/PKG-INFO` & `pyjs8call-0.2.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pyjs8call
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python package for interfacing with the JS8Call API
 Home-page: https://github.com/simplyequipped/pyjs8call
 Author: Simply Equipped LLC
 Author-email: howard@simplyequipped.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: psutil>=5.3
 
 [![pypi version](https://img.shields.io/pypi/v/pyjs8call?color=blue&label=pypi%20version)](https://pypi.org/project/pyjs8call) &nbsp;&nbsp;&nbsp;
 [![pypi downloads](https://img.shields.io/pypi/dw/pyjs8call?color=blue&label=pypi%20downloads)](https://pypi.org/project/pyjs8call) &nbsp;&nbsp;&nbsp;
 [![github license](https://img.shields.io/github/license/simplyequipped/pyjs8call?color=blue)](https://github.com/simplyequipped/pyjs8call/blob/main/LICENSE)
 
 A Python package for interfacing with the JS8Call API.
 
@@ -60,56 +61,57 @@
 
 ### Installation
 
 1. Install applications
     
     a. Install JS8Call
     
-    See the [JS8Call downloads](http://files.js8call.com/latest.html) page for OS-specific packages as well as source files. If you are compiling from source for Linux be sure to read the INSTALL file at the top level of the JS8Call repo.
-    
-    On Raspberry Pi OS:
+    On some platforms, such as Raspberry Pi OS, JS8Call can be installed with the package manager:
     ```
-    wget http://files.js8call.com/2.2.0/js8call_2.2.0_armhf.deb
-    sudo dpkg -i js8call_2.2.0_armhf.deb
+    sudo apt install js8call
     ```
 
+    Otherwise, see the [JS8Call downloads](http://files.JS8Call.com/latest.html) page for OS-specific packages as well as source files. If you are compiling from source for Linux be sure to read the INSTALL file at the top level of the JS8Call repo.
+
     **NOTE:** When installing JS8Call on Windows be sure to select the option to add JS8Call to the PATH variable during the installation process. This will allow *pyjs8call* to locate the JS8Call executable.
 
-    **NOTE:** When installing JS8Call on MacOS be sure to read the readme file included in the dmg image for information on the fix for the JS8Call shared memory error. The following directory must also be added to the PATH variable to allow *pyjs8call* to locate the JS8Call executable: /Applications/js8call.app/Contents/MacOS
+    **NOTE:** When installing JS8Call on MacOS be sure to read the readme file included in the dmg image for information on the fix for the JS8Call shared memory error. The following directory must also be added to the PATH variable to allow *pyjs8call* to locate the JS8Call executable: `/Applications/js8call.app/Contents/MacOS`
     
-    **NOTE:** When using a QRPLabs QDX tranceiver on Linux consider masking the ModemManager service to prevent CAT control dropouts. See [this post from QRPLabs](https://groups.io/g/QRPLabs/topic/87048220#74634) for more information.
-    
-    &nbsp;
+    **NOTE:** When using a QRPLabs QDX tranceiver on Linux, consider masking the ModemManager service using the below commands to prevent CAT control dropouts (aka rig control errors). See [this post from QRPLabs](https://groups.io/g/QRPLabs/topic/87048220#74634) for more information.
+    ```
+    sudo systemctl stop ModemManager.service
+    sudo systemctl mask ModemManager.service
+    ```
 
     b. Install xvfb if running headless (not supported on Windows or MacOS)
     
     On Debian systems:
     ```
     sudo apt install xvfb
     ```
 
-2. Install pyjs8call using pip3 (or pip, if python3 is the default on your system)
+2. Install pyjs8call using pip (or pip3, if python3 is not the default on your system)
     
     ```
-    pip3 install pyjs8call
+    pip install pyjs8call
     ```
 
     This will also install *psutil* for cross platform process management.
 
-3. Launch JS8Call to configure audio and CAT interface settings as needed. Launching the application and exiting normally will also initilize the configuration file, which is required by *pyjs8call*.
+3. Launch JS8Call to configure audio and CAT interface settings as needed. Launching the application and exiting normally will also initialize the configuration file, which is required by *pyjs8call*.
 
 &nbsp;
 
 ### Modules
 
 Some setup (i.e. setting callback functions) is required to use certain module features. Most modules are initialized automatically by pyjs8call.client.
 
 **Client** (pyjs8call.client)
 
-The main JS8Call API interface. Includes many functions for reading and writting settings as well as sending various types of messages.
+The main JS8Call API interface. Includes functions for sending various types of messages.
 
 **JS8Call** (pyjs8call.js8call)
 
 Manages TCP socket communication with the JS8Call application.
 
 **Application Monitor** (pyjs8call.appmonitor)
 
@@ -117,53 +119,105 @@
 
 **Configuration Handler** (pyjs8call.confighandler)
 
 Reads from and writes to the JS8Call.ini config file to change virtually any setting, including creating and activating configuration profiles. **Specific knowledge of configuration file options is required. Configuring options incorrectly may cause the JS8Call application to not run.**
 
 **Spot Monitor** (pyjs8call.spotmonitor)
 
-Monitors recent station spots. Spot data can be queried for various uses, and spot callbacks can be set for all heard stations and/or for specific stations.
+Monitors recent station spots. Spot data can be queried for various uses, and spot callbacks can be set for all heard stations and/or for specific stations and groups.
 
 **Window Monitor** (pyjs8call.windowmonitor)
 
 Monitors the next rx/tx window transition. JS8Call API messages associated with incoming and outgoing messages are used to determine the start or end of a window, and the modem speed setting is used to determine the duration of the window. Notification of a window transition is handled via callback function.
 
 **Offset Monitor** (pyjs8call.offsetmonitor)
 
-Manages JS8Call offset frequency based on activity in the pass band. The offset frequency is automatically moved to an unsed portion of the pass band if a recently heard signal overlaps with the current offset. Signal bandwidth is calculated based on the modem speed of each heard signal. Only decoded signal data is available from the JS8Call API so other QRM cannot be handled.
+Manages JS8Call offset frequency based on activity in the pass band. The offset frequency is automatically moved to an unused portion of the pass band if a recently heard signal overlaps with the current offset. Signal bandwidth is calculated based on the modem speed of each heard signal. Only decoded signal data is available from the JS8Call API so other QRM cannot be handled.
 
 **Outgoing Monitor** (pyjs8call.outgoingmonitor)
 
 Monitors JS8Call outgoing message text. Notification of a message status change is handled via callback function.
 
 **Heartbeat Networking** (pyjs8call.hbnetwork)
 
-Sends a heartbeat message in the heartbeat sub-band on a time interval.
+Sends a heartbeat message in the heartbeat sub-band on a time interval. This module is useful for enabling heatbeat networking programmatically and without using the JS8Call interface (i.e. running headless).
 
 **Time Monitor** (pyjs8call.timemonitor)
 
 Monitors a group, station, or all activity for time drift data and synchronizes local time drift. Enable automatic synchronization to the specified source on a time interval. Synchronizes to the @TIME group by default.
 
 Time master functionality is also implemented which sends outgoing messages on a time interval that other stations can use to synchronize their time drift. Targets the @TIME group by default.
 
 **Inbox Monitor** (pyjs8call.inboxmonitor)
 
 Monitors the local inbox. Notification of new messages is handled via callback function.
 
+Automatic periodic syncing of remote messages from a specified source (@ALLCALL by default) is also supported. Be aware of your local laws regarding unattended stations when using this feature.
+
+*NOTE: enabling syncing of remote messages will cause the local station to transmit immediately*
+
 **Schedule Monitor** (pyjs8call.schedulemonitor)
 
-Monitors configured schedule entries and applies the necessary setting changes at the scheduled time. Settings that can be changed on a schedule include frequency, modem speed, and configuration profile.
+Monitors configured schedule entries and applies the necessary setting changes at the scheduled time. Settings that can be changed on a schedule include frequency, modem speed, and configuration profile. The JS8Call application can also be restarted on a schedule.
 
 **Propagation** (pyjs8call.propagation)
-Parses stored spots into datasets of individual or median SNR values for grid squares or callsigns. This information can be used to infer general propagation conditions between the local station and a specific station, or the local station and a specific grid square.
+
+Parses stored spot data into datasets of individual or median SNR values for grid squares or callsigns. This information can be used to infer general propagation conditions between the local station and a specific station, or the local station and a specific grid square.
 
 **Notifications** (pyjs8call.notifications)
-Send an email message (including email-to-text) via an existing SMTP server when a message directed to the local station is received.
 
-&nbsp;  
+Send an email message (including email-to-text) via a specified SMTP server when a message directed to the local station is received, or when a specific station or group is spotted.
+
+&nbsp;
+
+### Command Line Interface (CLI)
+
+A command line interface is available for the *pyjs8call* module as of version 0.2.3. CLI usage:
+
+```
+USAGE: python -m pyjs8call [OPTIONS]
+
+OPTIONS:
+--rns
+    Utilize IO buffers to support the RNS PipeInterface, set configuration profile
+    to 'RNS', allow free text, and add group @RNS (*)
+--freq
+    Set radio frequency in Hz
+--grid
+    Set station grid square
+--speed
+    Set speed of JS8Call modem, defaults to 'fast'
+--profile
+    Set JS8Call configuration profile (**)
+--callsign
+    Set station callsign
+--settings
+    File path to pyjs8call settings file (NOT JS8CALL CONFIG FILE),
+    see pyjs8call.settings.Settings.load
+    for more information
+--headless
+    Run JS8Call headless using xvfb (only available on Linux platforms)
+--heartbeat
+    Enable pyjs8call heartbeat networking
+
+
+(*) RNS PipeInterface must be configured and enabled in the Reticulum config file,
+    see below example:
+
+    [[Pipe Interface]]
+    type = PipeInterface
+    interface_enabled = True
+    command = python -m pyjs8call --rns --settings ~/.config/pyjs8call_rns.ini
+    respawn_delay = 5
+
+(**) If the specified profile does not exist, it is created by copying 'Default'
+```
+See [RNS PipeInterface](https://markqvist.github.io/Reticulum/manual/interfaces.html#pipe-interface) for more information on configuring a RNS PipeInterface.
+
+&nbsp;
 
 ### Examples
 
 Basic usage:
 ```
 import pyjs8call
 
@@ -204,15 +258,15 @@
 # (or miles, depending on JS8Call settings)
 js8call.spots.filter(distance = 1000)
 
 # get a list of spot messages in the last 15 minutes
 max_age = 15 * 60 # convert minutes to seconds
 js8call.spots.filter(age = max_age)
 
-# get a list of the 10 most recent spot messages from regional stations in the last hour on the 40m band
+# get a list of the 10 most recent spot messages from regional stations on the 40m band
 js8call.spots.filter(distance = 500, band = '40m', count = 10)
 ```
 
 Run multiple JS8Call instances:
 ```
 import pyjs8call
 
@@ -225,14 +279,15 @@
 #js8call_ft857.start(args=['--rig-name', 'FT857'])
 
 # specify a different network port for the secondary instance
 js8call_qdx = pyjs8call.Client(port=2444)
 # specify the rig name as a command line argument
 js8call_qdx.start(args=['--rig-name', 'QDX'])
 ```
+**Note:** radio interface and audio devices should be configured manually in each JS8Call instance
 
 Using the spot monitor:
 ```
 import pyjs8call
 
 # callback function for all new spots
 def new_spots(spots):
@@ -277,16 +332,24 @@
         print('New inbox message from ' + msg['origin'])
 
 js8call = pyjs8call.Client()
 # set inbox monitor callback
 js8call.callback.inbox = new_inbox_msg
 js8call.start()
 
-# enable local inbox monitoring and periodic remote inbox message query
+# enable local inbox monitoring
 js8call.inbox.enable()
+
+# enable local inbox monitoring and periodic remote inbox message query
+# to @ALLCALL every 60 minutes
+js8call.inbox.enable(query=True)
+
+# enable local inbox monitoring and periodic remote inbox message query
+# to @MYGROUP every 30 minutes
+js8call.inbox.enable(query=True, destination='@MYGROUP', interval=30)
 ```
 
 Using the outgoing message monitor:
 ```
 import pyjs8call
 
 # callback function for message status change
@@ -308,14 +371,16 @@
 ```
 
 Using heartbeat networking:
 ```
 import pyjs8call
 
 js8call = pyjs8call.Client()
+# set heartbeat interval via config file
+js8call.settings.set_heartbeat_interval(15)
 js8call.start()
 
 # interval based on JS8Call settings
 js8call.heartbeat.enable()
 ```
 
 Using the schedule monitor:
@@ -348,14 +413,15 @@
 Set config file settings:
 ```
 import pyjs8call
 
 js8call = pyjs8call.Client()
 
 # set config file settings before starting
+# see pyjs8call.settings for many more settings options
 js8call.settings.enable_heartbeat_acknowledgements()
 js8call.settings.set_heartbeat_interval(15)
 js8call.settings.enable_reporting()
 js8call.settings.set_speed('normal')
 
 js8call.start()
 ```
@@ -369,16 +435,16 @@
 
 # use built-in spot distance filter
 regional_stations = [spot.origin for spot in js8call.spots.filter(distance = 500)]
 for station in regional_stations:
     print('{}: {} {} at {}\N{DEGREE SIGN}'.format(station.origin, station.distance, station.distance_units, station.bearing))
 
 # access message attributes directly
-# this requires the message to contain grid square data
-last_heartbeat = js8call.spots.filter(destination='@HB')[-1]
+# this requires the message to contain grid square data (ex. heartbeat message)
+last_heartbeat = js8call.spots.filter(destination='@HB', count=1)[-1]
 distance = last_heartbeat.distance
 bearing = last_heartbeat.bearing
 
 # manually calculate distance and bearing from local station
 distance, distance_units, bearing = js8call.grid_distance('FM16')
 
 # manually calculate distance and bearing between grid squares
@@ -450,14 +516,23 @@
 # set SMTP server credentials
 js8call.notifications.set_smtp_credentials('email.address@gmail.com', 'app_password')
 # set destination email address to a Verzion mobile number
 js8call.notifications.set_email_destination('2018675309@vtext.com')
 # enable automatic notifications for incoming directed messages
 js8call.notifications.enable()
 
+# set stations to watch
+js8call.spots.add_station_watch('KT7RUN')
+# enable station spot notifications
+js8call.notifications.enable_station_spots()
+
+# set groups to watch
+js8call.spots.add_group_watch('@TTP')
+# enable station spot notifications
+js8call.notifications.enable_group_spots()
 ```
 
 &nbsp;
 
 ### Acknowledgements
 
 Inspired by [js8net](https://github.com/jfrancis42/js8net) by N0GQ<br>
```

### Comparing `pyjs8call-0.2.2/README.md` & `pyjs8call-0.2.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -44,56 +44,57 @@
 
 ### Installation
 
 1. Install applications
     
     a. Install JS8Call
     
-    See the [JS8Call downloads](http://files.js8call.com/latest.html) page for OS-specific packages as well as source files. If you are compiling from source for Linux be sure to read the INSTALL file at the top level of the JS8Call repo.
-    
-    On Raspberry Pi OS:
+    On some platforms, such as Raspberry Pi OS, JS8Call can be installed with the package manager:
     ```
-    wget http://files.js8call.com/2.2.0/js8call_2.2.0_armhf.deb
-    sudo dpkg -i js8call_2.2.0_armhf.deb
+    sudo apt install js8call
     ```
 
+    Otherwise, see the [JS8Call downloads](http://files.JS8Call.com/latest.html) page for OS-specific packages as well as source files. If you are compiling from source for Linux be sure to read the INSTALL file at the top level of the JS8Call repo.
+
     **NOTE:** When installing JS8Call on Windows be sure to select the option to add JS8Call to the PATH variable during the installation process. This will allow *pyjs8call* to locate the JS8Call executable.
 
-    **NOTE:** When installing JS8Call on MacOS be sure to read the readme file included in the dmg image for information on the fix for the JS8Call shared memory error. The following directory must also be added to the PATH variable to allow *pyjs8call* to locate the JS8Call executable: /Applications/js8call.app/Contents/MacOS
+    **NOTE:** When installing JS8Call on MacOS be sure to read the readme file included in the dmg image for information on the fix for the JS8Call shared memory error. The following directory must also be added to the PATH variable to allow *pyjs8call* to locate the JS8Call executable: `/Applications/js8call.app/Contents/MacOS`
     
-    **NOTE:** When using a QRPLabs QDX tranceiver on Linux consider masking the ModemManager service to prevent CAT control dropouts. See [this post from QRPLabs](https://groups.io/g/QRPLabs/topic/87048220#74634) for more information.
-    
-    &nbsp;
+    **NOTE:** When using a QRPLabs QDX tranceiver on Linux, consider masking the ModemManager service using the below commands to prevent CAT control dropouts (aka rig control errors). See [this post from QRPLabs](https://groups.io/g/QRPLabs/topic/87048220#74634) for more information.
+    ```
+    sudo systemctl stop ModemManager.service
+    sudo systemctl mask ModemManager.service
+    ```
 
     b. Install xvfb if running headless (not supported on Windows or MacOS)
     
     On Debian systems:
     ```
     sudo apt install xvfb
     ```
 
-2. Install pyjs8call using pip3 (or pip, if python3 is the default on your system)
+2. Install pyjs8call using pip (or pip3, if python3 is not the default on your system)
     
     ```
-    pip3 install pyjs8call
+    pip install pyjs8call
     ```
 
     This will also install *psutil* for cross platform process management.
 
-3. Launch JS8Call to configure audio and CAT interface settings as needed. Launching the application and exiting normally will also initilize the configuration file, which is required by *pyjs8call*.
+3. Launch JS8Call to configure audio and CAT interface settings as needed. Launching the application and exiting normally will also initialize the configuration file, which is required by *pyjs8call*.
 
 &nbsp;
 
 ### Modules
 
 Some setup (i.e. setting callback functions) is required to use certain module features. Most modules are initialized automatically by pyjs8call.client.
 
 **Client** (pyjs8call.client)
 
-The main JS8Call API interface. Includes many functions for reading and writting settings as well as sending various types of messages.
+The main JS8Call API interface. Includes functions for sending various types of messages.
 
 **JS8Call** (pyjs8call.js8call)
 
 Manages TCP socket communication with the JS8Call application.
 
 **Application Monitor** (pyjs8call.appmonitor)
 
@@ -101,53 +102,105 @@
 
 **Configuration Handler** (pyjs8call.confighandler)
 
 Reads from and writes to the JS8Call.ini config file to change virtually any setting, including creating and activating configuration profiles. **Specific knowledge of configuration file options is required. Configuring options incorrectly may cause the JS8Call application to not run.**
 
 **Spot Monitor** (pyjs8call.spotmonitor)
 
-Monitors recent station spots. Spot data can be queried for various uses, and spot callbacks can be set for all heard stations and/or for specific stations.
+Monitors recent station spots. Spot data can be queried for various uses, and spot callbacks can be set for all heard stations and/or for specific stations and groups.
 
 **Window Monitor** (pyjs8call.windowmonitor)
 
 Monitors the next rx/tx window transition. JS8Call API messages associated with incoming and outgoing messages are used to determine the start or end of a window, and the modem speed setting is used to determine the duration of the window. Notification of a window transition is handled via callback function.
 
 **Offset Monitor** (pyjs8call.offsetmonitor)
 
-Manages JS8Call offset frequency based on activity in the pass band. The offset frequency is automatically moved to an unsed portion of the pass band if a recently heard signal overlaps with the current offset. Signal bandwidth is calculated based on the modem speed of each heard signal. Only decoded signal data is available from the JS8Call API so other QRM cannot be handled.
+Manages JS8Call offset frequency based on activity in the pass band. The offset frequency is automatically moved to an unused portion of the pass band if a recently heard signal overlaps with the current offset. Signal bandwidth is calculated based on the modem speed of each heard signal. Only decoded signal data is available from the JS8Call API so other QRM cannot be handled.
 
 **Outgoing Monitor** (pyjs8call.outgoingmonitor)
 
 Monitors JS8Call outgoing message text. Notification of a message status change is handled via callback function.
 
 **Heartbeat Networking** (pyjs8call.hbnetwork)
 
-Sends a heartbeat message in the heartbeat sub-band on a time interval.
+Sends a heartbeat message in the heartbeat sub-band on a time interval. This module is useful for enabling heatbeat networking programmatically and without using the JS8Call interface (i.e. running headless).
 
 **Time Monitor** (pyjs8call.timemonitor)
 
 Monitors a group, station, or all activity for time drift data and synchronizes local time drift. Enable automatic synchronization to the specified source on a time interval. Synchronizes to the @TIME group by default.
 
 Time master functionality is also implemented which sends outgoing messages on a time interval that other stations can use to synchronize their time drift. Targets the @TIME group by default.
 
 **Inbox Monitor** (pyjs8call.inboxmonitor)
 
 Monitors the local inbox. Notification of new messages is handled via callback function.
 
+Automatic periodic syncing of remote messages from a specified source (@ALLCALL by default) is also supported. Be aware of your local laws regarding unattended stations when using this feature.
+
+*NOTE: enabling syncing of remote messages will cause the local station to transmit immediately*
+
 **Schedule Monitor** (pyjs8call.schedulemonitor)
 
-Monitors configured schedule entries and applies the necessary setting changes at the scheduled time. Settings that can be changed on a schedule include frequency, modem speed, and configuration profile.
+Monitors configured schedule entries and applies the necessary setting changes at the scheduled time. Settings that can be changed on a schedule include frequency, modem speed, and configuration profile. The JS8Call application can also be restarted on a schedule.
 
 **Propagation** (pyjs8call.propagation)
-Parses stored spots into datasets of individual or median SNR values for grid squares or callsigns. This information can be used to infer general propagation conditions between the local station and a specific station, or the local station and a specific grid square.
+
+Parses stored spot data into datasets of individual or median SNR values for grid squares or callsigns. This information can be used to infer general propagation conditions between the local station and a specific station, or the local station and a specific grid square.
 
 **Notifications** (pyjs8call.notifications)
-Send an email message (including email-to-text) via an existing SMTP server when a message directed to the local station is received.
 
-&nbsp;  
+Send an email message (including email-to-text) via a specified SMTP server when a message directed to the local station is received, or when a specific station or group is spotted.
+
+&nbsp;
+
+### Command Line Interface (CLI)
+
+A command line interface is available for the *pyjs8call* module as of version 0.2.3. CLI usage:
+
+```
+USAGE: python -m pyjs8call [OPTIONS]
+
+OPTIONS:
+--rns
+    Utilize IO buffers to support the RNS PipeInterface, set configuration profile
+    to 'RNS', allow free text, and add group @RNS (*)
+--freq
+    Set radio frequency in Hz
+--grid
+    Set station grid square
+--speed
+    Set speed of JS8Call modem, defaults to 'fast'
+--profile
+    Set JS8Call configuration profile (**)
+--callsign
+    Set station callsign
+--settings
+    File path to pyjs8call settings file (NOT JS8CALL CONFIG FILE),
+    see pyjs8call.settings.Settings.load
+    for more information
+--headless
+    Run JS8Call headless using xvfb (only available on Linux platforms)
+--heartbeat
+    Enable pyjs8call heartbeat networking
+
+
+(*) RNS PipeInterface must be configured and enabled in the Reticulum config file,
+    see below example:
+
+    [[Pipe Interface]]
+    type = PipeInterface
+    interface_enabled = True
+    command = python -m pyjs8call --rns --settings ~/.config/pyjs8call_rns.ini
+    respawn_delay = 5
+
+(**) If the specified profile does not exist, it is created by copying 'Default'
+```
+See [RNS PipeInterface](https://markqvist.github.io/Reticulum/manual/interfaces.html#pipe-interface) for more information on configuring a RNS PipeInterface.
+
+&nbsp;
 
 ### Examples
 
 Basic usage:
 ```
 import pyjs8call
 
@@ -188,15 +241,15 @@
 # (or miles, depending on JS8Call settings)
 js8call.spots.filter(distance = 1000)
 
 # get a list of spot messages in the last 15 minutes
 max_age = 15 * 60 # convert minutes to seconds
 js8call.spots.filter(age = max_age)
 
-# get a list of the 10 most recent spot messages from regional stations in the last hour on the 40m band
+# get a list of the 10 most recent spot messages from regional stations on the 40m band
 js8call.spots.filter(distance = 500, band = '40m', count = 10)
 ```
 
 Run multiple JS8Call instances:
 ```
 import pyjs8call
 
@@ -209,14 +262,15 @@
 #js8call_ft857.start(args=['--rig-name', 'FT857'])
 
 # specify a different network port for the secondary instance
 js8call_qdx = pyjs8call.Client(port=2444)
 # specify the rig name as a command line argument
 js8call_qdx.start(args=['--rig-name', 'QDX'])
 ```
+**Note:** radio interface and audio devices should be configured manually in each JS8Call instance
 
 Using the spot monitor:
 ```
 import pyjs8call
 
 # callback function for all new spots
 def new_spots(spots):
@@ -261,16 +315,24 @@
         print('New inbox message from ' + msg['origin'])
 
 js8call = pyjs8call.Client()
 # set inbox monitor callback
 js8call.callback.inbox = new_inbox_msg
 js8call.start()
 
-# enable local inbox monitoring and periodic remote inbox message query
+# enable local inbox monitoring
 js8call.inbox.enable()
+
+# enable local inbox monitoring and periodic remote inbox message query
+# to @ALLCALL every 60 minutes
+js8call.inbox.enable(query=True)
+
+# enable local inbox monitoring and periodic remote inbox message query
+# to @MYGROUP every 30 minutes
+js8call.inbox.enable(query=True, destination='@MYGROUP', interval=30)
 ```
 
 Using the outgoing message monitor:
 ```
 import pyjs8call
 
 # callback function for message status change
@@ -292,14 +354,16 @@
 ```
 
 Using heartbeat networking:
 ```
 import pyjs8call
 
 js8call = pyjs8call.Client()
+# set heartbeat interval via config file
+js8call.settings.set_heartbeat_interval(15)
 js8call.start()
 
 # interval based on JS8Call settings
 js8call.heartbeat.enable()
 ```
 
 Using the schedule monitor:
@@ -332,14 +396,15 @@
 Set config file settings:
 ```
 import pyjs8call
 
 js8call = pyjs8call.Client()
 
 # set config file settings before starting
+# see pyjs8call.settings for many more settings options
 js8call.settings.enable_heartbeat_acknowledgements()
 js8call.settings.set_heartbeat_interval(15)
 js8call.settings.enable_reporting()
 js8call.settings.set_speed('normal')
 
 js8call.start()
 ```
@@ -353,16 +418,16 @@
 
 # use built-in spot distance filter
 regional_stations = [spot.origin for spot in js8call.spots.filter(distance = 500)]
 for station in regional_stations:
     print('{}: {} {} at {}\N{DEGREE SIGN}'.format(station.origin, station.distance, station.distance_units, station.bearing))
 
 # access message attributes directly
-# this requires the message to contain grid square data
-last_heartbeat = js8call.spots.filter(destination='@HB')[-1]
+# this requires the message to contain grid square data (ex. heartbeat message)
+last_heartbeat = js8call.spots.filter(destination='@HB', count=1)[-1]
 distance = last_heartbeat.distance
 bearing = last_heartbeat.bearing
 
 # manually calculate distance and bearing from local station
 distance, distance_units, bearing = js8call.grid_distance('FM16')
 
 # manually calculate distance and bearing between grid squares
@@ -434,14 +499,23 @@
 # set SMTP server credentials
 js8call.notifications.set_smtp_credentials('email.address@gmail.com', 'app_password')
 # set destination email address to a Verzion mobile number
 js8call.notifications.set_email_destination('2018675309@vtext.com')
 # enable automatic notifications for incoming directed messages
 js8call.notifications.enable()
 
+# set stations to watch
+js8call.spots.add_station_watch('KT7RUN')
+# enable station spot notifications
+js8call.notifications.enable_station_spots()
+
+# set groups to watch
+js8call.spots.add_group_watch('@TTP')
+# enable station spot notifications
+js8call.notifications.enable_group_spots()
 ```
 
 &nbsp;
 
 ### Acknowledgements
 
 Inspired by [js8net](https://github.com/jfrancis42/js8net) by N0GQ<br>
```

### Comparing `pyjs8call-0.2.2/pyjs8call/__init__.py` & `pyjs8call-0.2.3/pyjs8call/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,18 +19,19 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 '''
 .. include:: ../README.md
 .. include:: ../VERSION.md
+.. include:: ../ROADMAP.md
 '''
 
 __docformat__ = 'google'
-__version__ = '0.2.2'
+__version__ = '0.2.3'
 
 
 from pyjs8call.confighandler import ConfigHandler
 from pyjs8call.notifications import Notifications
 from pyjs8call.schedulemonitor import ScheduleMonitor
 from pyjs8call.spotmonitor import SpotMonitor
 from pyjs8call.appmonitor import AppMonitor
@@ -42,10 +43,10 @@
 from pyjs8call.inboxmonitor import InboxMonitor
 from pyjs8call.timemonitor import DriftMonitor
 from pyjs8call.timemonitor import TimeMaster
 from pyjs8call.outgoingmonitor import OutgoingMonitor
 from pyjs8call.hbnetwork import HeartbeatNetworking
 from pyjs8call.js8call import JS8Call
 from pyjs8call.client import Client
-from pyjs8call.client import Settings
-from pyjs8call.client import Callbacks
+from pyjs8call.settings import Settings
+from pyjs8call.callbacks import Callbacks
```

### Comparing `pyjs8call-0.2.2/pyjs8call/appmonitor.py` & `pyjs8call-0.2.3/pyjs8call/appmonitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,42 +34,39 @@
 import subprocess
 
 import psutil
 
 
 class AppMonitor:
     '''JS8Call application monitor.
-
-    If the JS8Call application is closed and *restart* is *False*, pyjs8call will exit. If *restart* is *True* pyjs8call will continue to run and JS8Call will be restarted.
-
-
-
-    Attributes:
-        headless (bool): Whether JS8Call is running headless using xvfb (see *start()*)
-        args (list): Sequence of command line arguments to be passed to JS8Call, defaults to empty list
-        restart (bool): Whether to restart the JS8Call application if it stops, defaults to False
-        terminate_js8call (bool): Whether to terminate the JS8Call application when stopping the app monitor
     '''
 
     def __init__(self, parent):
         '''Initialize JS8Call application monitor.
 
         Args:
             parent (pyjs8call.js8call): The parent js8call object
 
         Returns:
             pyjs8call.appmonitor.AppMonitor: Constructed application monitor object
         '''
         self._parent = parent
         self._xvfb_proc = None
         self._js8call_proc = None
+        self._js8_proc = None
         self.headless = False
+        '''bool: Whether JS8Call is running headless using xvfb'''
         self.args = []
+        '''list: Command line arguments passed to JS8Call, defaults to empty list'''
         self.restart = False
+        '''bool: Whether to restart the JS8Call application if it stops, defaults to False
+
+        If the JS8Call application is closed and *restart* is *False*, pyjs8call will exit. If *restart* is *True* pyjs8call will continue to run and JS8Call will be restarted.'''
         self.terminate_js8call = True
+        '''bool: Whether to terminate the JS8Call application when stopping the app monitor, defaults to True'''
 
     def start(self, headless=False, args=None):
         ''' Start JS8Call application.
 
         See the subprocess.Popen *args* parameter documentation for information on how to break command line arguments into a sequence. The *js8call* command does not need to be included, only additional arguments. For example, passing `['--rig-name', 'FT857']` as the *args* parameter results in `js8call --rig-name FT857` being called to start the JS8Call application. Note that *args* only applies if JS8Call is started by pyjs8call.
 
         Args:
@@ -146,22 +143,31 @@
         On Windows systems only SIGKILL is sent.
         '''
         if not self.is_running():
             return
 
         if not self.terminate_js8call:
             return
-        
+
         self._js8call_proc.terminate()
 
+        if self._js8_proc is not None:
+            self._js8_proc.terminate()
+
         try:
             self._js8call_proc.wait(timeout = 2)
         except psutil.TimeoutExpired:
             self._js8call_proc.kill()
 
+        if self._js8_proc is not None:
+            try:
+                self._js8_proc.wait(timeout = 2)
+            except psutil.TimeoutExpired:
+                self._js8c_proc.kill()
+
         # remove zombie process when running headless
         if self._xvfb_proc is not None:
             try:
                 self._xvfb_proc.wait(timeout = 2)
             except psutil.TimeoutExpired:
                 pass
 
@@ -236,14 +242,17 @@
 
         # wait until socket connected or timeout
         if self._socket_connected():
             # start js8call monitoring thread
             thread = threading.Thread(target=self._monitor)
             thread.daemon = True
             thread.start()
+
+            # find js8 process after js8call started and connected
+            self._find_running_js8_process()
         else:
             raise RuntimeError('JS8Call application failed to start')
 
     def _socket_connected(self, timeout=120):
         '''Wait for JS8Call socket connection after starting application.
         
         Args:
@@ -277,33 +286,49 @@
         '''Find running xvfb process and child JS8Call process.'''
         xvfb_procs = [proc for proc in psutil.process_iter(['name']) if proc.info['name'].lower() == 'xvfb-run']
 
         # check xvfb child processes for js8call process
         for proc in xvfb_procs:
             if proc.status() == psutil.STATUS_ZOMBIE:
                 continue
-                
+
+            #TODO finding js8/js8.exe could be cleaner
             for child in proc.children():
                 if child.name().lower() == 'js8call':
                     # js8call found
                     self._xvfb_proc = proc
                     self._js8call_proc = child
+                elif child.name().lower() == 'js8':
+                    # js8 found
+                    self._xvfb_proc = proc
+                    self._js8_proc = child
                     return
 
     def _find_running_js8call_process(self):
         '''Find running JS8Call process.'''
         js8call_procs = [proc for proc in psutil.process_iter(['name']) if proc.info['name'].lower() in ('js8call', 'js8call.exe')]
         
         for proc in js8call_procs:
             if proc.status() == psutil.STATUS_ZOMBIE:
                 continue
                 
             self._js8call_proc = proc
             return
 
+    def _find_running_js8_process(self):
+        '''Find running JS8 process.'''
+        js8_procs = [proc for proc in psutil.process_iter(['name']) if proc.info['name'].lower() in ('js8', 'js8.exe')]
+        
+        for proc in js8_procs:
+            if proc.status() == psutil.STATUS_ZOMBIE:
+                continue
+                
+            self._js8_proc = proc
+            return
+
     def _monitor(self):
         '''Application monitoring thread.'''
         while self._parent.online:
             if not self.is_running() and not self._parent._client.restarting:
                 if self.restart:
                     # restart the whole system and reconnect
                     self._parent._client.restart()
```

### Comparing `pyjs8call-0.2.2/pyjs8call/client.py` & `pyjs8call-0.2.3/pyjs8call/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -35,84 +35,30 @@
     js8call.send_directed_message('KT7RUN', 'Great content thx')
     ```
 '''
 
 __docformat__ = 'google'
 
 
+import os
 import time
 import shutil
 import atexit
 import threading
-from datetime import datetime, timezone
 from math import radians, sin, cos, acos, atan2, pi
 
 import pyjs8call
 from pyjs8call import Message
 
 
 class Client:
-    '''JS8Call API client.
+    '''JS8Call API client.'''
     
-    **Caution**: Custom processing of messages is an advanced feature that can break internal message handling if implemented incorrectly. Use this feature only if you understand what you are doing.
-    **Note**: Any delay in *process_incoming* and *process_outgoing* functions will cause delays in internal incoming and outgoing message processing loops. Custom processing should be kept to a minimum to avoid cumulative delays.
-    
-    Custom Incoming Message Processing:
-    
-    The *process_incoming* function is called after internal processing of an incoming message from the JS8Call application, but before adding the message to the incoming message queue.
-    
-    *process_incoming* should accept a pyjs8call.message object, and return a pyjs8call.message object. If an error occurs during processing, either:
-        - set the *msg.error* string before returning the message, which will cause the message to continue processing and be added to the incoming message queue
-        OR
-        - return None, which will cause the message to be dropped
-    
-    *process_incoming* function signatures:
-        `func(pyjs8call.Message) -> pyjs8call.Message`
-        `func(pyjs8call.Message) -> None`
-
-    Custom Outgoing Message Processing:
-    
-    The *process_outgoing* function is called just after message creation in the following functions:
-        - send_message
-        - send_directed_message
-        - send_directed_command_message
-    
-    *process_outgoing* should accept a pyjs8call.message object, and return a pyjs8call.message object. If an error occurs during processing:
-        - set the *msg.error* string, which will cause the message to be returned with a failed status (the message will not be sent)
-    
-    *process_outoing* function signature:
-        `func(pyjs8call.Message) -> pyjs8call.Message`
-
-    Attributes:
-        js8call (pyjs8call.js8call): Manages JS8Call application and TCP socket communication
-        spots (pyjs8call.spotmonitor): Monitors station activity and issues callbacks
-        window (pyjs8call.windowmonitor): Monitors the JS8Call transmit window
-        offset (pyjs8call.offsetmonitor): Manages JS8Call offset frequency
-        outgoing (pyjs8call.outgoingmonitor): Monitors JS8Call outgoing message text
-        drift_sync (pyjs8call.timemonitor): Monitors JS8Call time drift
-        time_master (pyjs8call.timemonitor): Manages time master outgoing messages
-        inbox (pyjs8call.inboxmonitor): Monitors JS8Call inbox messages
-        config (pyjs8call.confighandler): Manages JS8Call configuration file
-        heartbeat (pyjs8call.hbnetwork): Manages heartbeat outgoing messages
-        schedule (pyjs8call.schedulemonitor): Monitors and activates schedule entries
-        propagation (pyjs8call.propagation): Parse spots into propagation data
-        notifications (pyjs8call.notifications): Send email notifications via SMTP server
-        callback (pyjs8call.client.Callbacks): Callback function reference object
-        settings (pyjs8call.client.Settings): Configuration setting function reference object
-        clean_directed_text (bool): Remove JS8Call callsign structure from incoming messages, defaults to True
-        monitor_outgoing (bool): Monitor outgoing message status (see pyjs8call.outgoingmonitor), defaults to True
-        max_spot_age (int): Maximum age (in seconds) of spots to store before dropping old spots, defaults to 7 days
-        online (bool): Whether the JS8Call application and pyjs8call interface are online
-        host (str): IP address matching JS8Call *TCP Server Hostname* setting
-        port (int): Port number matching JS8Call *TCP Server Port* setting
-        process_incoming (func): Function to call for custom processing of incoming messages, defaults to None
-        process_outgoing (func): Function to call for custom processing of outgoing messages, defaults to None
-        BANDS (dict): mapping of frequency bands to minimum and maximum frequencies
-        OOB (str): out-of-band designator
-    '''
+    OOB = 'OOB'
+    '''str: Out-of-band designator'''
 
     BANDS = {
         '2190m':  (136000,       137000),
         '630m':   (472000,       479000),
         '560m':   (501000,       504000),
         '160m':   (1800000,      2000000),
         '80m':    (3500000,      4000000),
@@ -136,28 +82,30 @@
         '6cm':    (5650000000,   5925000000),
         '3cm':    (10000000000,  10500000000),
         '1.25cm': (24000000000,  24250000000),
         '6mm':    (47000000000,  47200000000),
         '4mm':    (75500000000,  81000000000),
         '2.5mm':  (119980000000, 120020000000),
         '2mm':    (142000000000, 149000000000),
-        '1mm':    (241000000000, 250000000000)
+        '1mm':    (241000000000, 250000000000),
+        OOB: (0, 0)
     }
-    
-    OOB = 'OOB'
+    '''dict: Mapping of frequency band name to minimum and maximum frequencies'''
     
     @staticmethod
     def freq_to_band(freq):
         '''Get band for specified frequency.
 
         Args:
             freq (int): Frequency in Hz
 
         Returns:
-            str: Band designator like \'40m\' if frequency is in a known band, otherwise *Client.OOB*
+            str: Band name like \'40m\'
+            
+        Returned value is Client.OOB if frequency is outside known bands.
         '''
         if freq is None:
             return Client.OOB
             
         for band, freqs in Client.BANDS.items():
             if freqs[0] <= freq <= freqs[1]:
                 return band
@@ -168,104 +116,170 @@
     def band_freq_range(band):
         '''Get frequency range for specified band.
 
         Args:
             band (str): Band designator like \'40m\'
 
         Returns:
-            tuple or str: (min_freq, max_freq) if band is known, otherwise *Client.OOB*
+            tuple: Format `(min_freq, max_freq)`
+            
+        Returned value is `(0, 0)` if band name is unknown.
         '''
         if band is None:
             return Client.OOB
             
         band = band.lower()
         
         if band in Client.BANDS:
             return Client.BANDS[band]
         
-        return Client.OOB
+        return Client.BANDS[Client.OOB]
 
-    def __init__(self, host='127.0.0.1', port=2442, config_path=None):
+    def __init__(self, settings_path=None, host='127.0.0.1', port=2442, config_path=None):
         '''Initialize JS8Call API client.
 
         Registers the Client.stop function with the atexit module.
         
-        Configures the following settings:
-        - enable autoreply at startup
-        - disable autoreply confirmation
-        - enable transmit
-
-        Initializes the following for access prior to starting:
+        Initializes the following modules for access prior to starting:
         - js8call (pyjs8call.js8call)
         - config (pyjs8call.confighandler)
-        - settings (pyjs8call.client.settings)
-        - callback (pyjs8call.client.callbacks)
+        - settings (pyjs8call.settings)
+        - callback (pyjs8call.callbacks)
         - notifications (pyjs8call.notifications)
 
         Args:
+            settings_path (str): pyjs8call settings file path, defaults to None (see pyjs8call.settings.Settings.load for more information)
             host (str): JS8Call TCP address setting, defaults to '127.0.0.1'
             port (int): JS8Call TCP port setting, defaults to 2442
             config_path (str): Non-standard JS8Call.ini configuration file path, defaults to None
 
         Returns:
-            pyjs8call.Client: Constructed client object
+            pyjs8call.client.Client: Constructed client object
 
         Raises:
             RuntimeError: JS8Call application not installed
         '''
         self.host = host
+        '''str: IP address matching JS8Call *TCP Server Hostname* setting'''
         self.port = port
+        '''int: Port number matching JS8Call *TCP Server Port* setting'''
         self.online = False
+        '''bool: True if the JS8Call application and pyjs8call interface are online, False otherwise'''
         self.restarting = False
+        '''bool: True if the JS8Call application is currently being restarted, False otherwise'''
         self.process_incoming = None
+        '''func: Function to call for custom processing of incoming messages, defaults to None
+        
+        **Caution**: Custom processing of messages is an advanced feature that can break internal message handling if implemented incorrectly. Use this feature only if you understand what you are doing.
+        
+        **Note**: Any delay in custom processing functions will cause delays in internal incoming and outgoing message processing loops. Custom processing should be kept to a minimum to avoid cumulative delays.
+        
+        If set, the Client.process_incoming function is called after internal processing of an incoming message from the JS8Call application, but before adding the message to the incoming message queue.
+        
+        Client.process_incoming should accept a pyjs8call.message.Message.Message object, and return a pyjs8call.message.Message.Message object. If an error occurs during processing, either:
+        - set the *msg.error* string before returning the message, which will cause the message to continue processing and be added to the incoming message queue
+        OR
+        - return None, which will cause the message to be dropped
+        
+        Client.process_incoming function signatures:
+        - `func(pyjs8call.message.Message.Message) -> pyjs8call.message.Message.Message`
+        - `func(pyjs8call.message.Message.Message) -> None`
+        '''
         self.process_outgoing = None
+        '''func: Function to call for custom processing of outgoing messages, defaults to None
+
+        **Caution**: Custom processing of messages is an advanced feature that can break internal message handling if implemented incorrectly. Use this feature only if you understand what you are doing.
+
+        **Note**: Any delay in custom processing functions will cause delays in internal incoming and outgoing message processing loops. Custom processing should be kept to a minimum to avoid cumulative delays.
+        
+        If set, the Client.process_outgoing function is called just after message creation in all outgoing message functions, such as Client.send_directed_message().
+        
+        Client.process_outgoing should accept a pyjs8call.message.Message.Message object, and return a pyjs8call.message.Message.Message object. If an error occurs during processing:
+        - set the *msg.error* string, which will cause the message to be returned with a failed status (the message will not be sent)
+        
+        Client.process_outgoing function signature:
+        - `func(pyjs8call.message.Message.Message) -> pyjs8call.message.Message.Message`
+        '''
         self.clean_directed_text = True
+        '''bool: Remove JS8Call callsign structure from incoming messages, defaults to True'''
+        self.autodetect_outgoing_directed_command = True
+        '''bool: Autodetect and handle commands in outgoing directed messages, defaults to True (added in version 0.2.3)'''
         self.monitor_outgoing = True
-        self.max_spot_age = 7 * 24 * 60 * 60 # 7 days 
-
+        '''bool: Monitor outgoing message status (see pyjs8call.outgoingmonitor), defaults to True'''
+        self.max_spot_age = 7 * 24 * 60 * 60 # 7 days
+        '''int: Maximum age (in seconds) of spots to store before dropping old spots, defaults to 7 days'''
+        self._previous_profile = None
+        '''str: JS8Call configuration profile name before the last profile change, defaults to None'''
+
+        self.config = None
+        '''pyjs8call.confighandler: Manages JS8Call configuration file'''
+        self.settings = None
+        '''pyjs8call.settings: Configuration and setting function container'''
+        self.callback = None
+        '''pyjs8call.callbacks: Callback function container'''
         self.js8call = None
+        '''pyjs8call.js8call: Manages JS8Call application and TCP socket communication'''
         self.spots = None
+        '''pyjs8call.spotmonitor: Monitors station activity and performs associated callbacks'''
         self.window = None
+        '''pyjs8call.windowmonitor: Monitors the JS8Call transmit window'''
         self.offset = None
+        '''pyjs8call.offsetmonitor: Manages JS8Call offset frequency'''
         self.outgoing = None
+        '''pyjs8call.outgoingmonitor: Monitors JS8Call outgoing message text'''
         self.drift_sync = None
+        '''pyjs8call.timemonitor: Monitors JS8Call time drift'''
         self.time_master = None
+        '''pyjs8call.timemonitor: Manages time master outgoing messages'''
         self.inbox = None
+        '''pyjs8call.inboxmonitor: Monitors JS8Call local and remote inbox messages'''
         self.heartbeat = None
+        '''pyjs8call.hbnetwork: Manages outgoing heartbeat network messages'''
         self.schedule = None
+        '''pyjs8call.schedulemonitor: Monitors and activates schedule entries'''
         self.propagation = None
+        '''pyjs8call.propagation: Parse spots into propagation data'''
+        self.notifications = None
+        '''pyjs8call.notifications: Send email notifications via SMTP server'''
 
         # delay between setting value and getting updated value
         self._set_get_delay = 0.1 # seconds
 
         # ensure js8call application is installed
         if shutil.which('js8call') is None:
             raise RuntimeError('JS8Call application not installed')
 
         self.config = pyjs8call.ConfigHandler(config_path = config_path)
-        self.settings = Settings(self)
-        self.callback = Callbacks()
+        self.settings = pyjs8call.Settings(self)
+        self.callback = pyjs8call.Callbacks()
         self.js8call = pyjs8call.JS8Call(self, self.host, self.port)
         self.notifications = pyjs8call.Notifications(self)
 
-        config_clean_directed_text = self.config.get('Configuration', 'pyjs8callCleanDirectedText', bool)
-        if config_clean_directed_text is not None:
-            self.clean_directed_text = config_clean_directed_text
-
-        config_monitor_outgoing = self.config.get('Configuration', 'pyjs8callMonitorOutgoing', bool)
-        if config_monitor_outgoing is not None:
-            self.monitor_outgoing = config_monitor_outgoing
-
-        config_max_spot_age = self.config.get('Configuration', 'pyjs8callMaxSpotAge', int)
-        if config_max_spot_age is not None:
-            self.max_spot_age = config_max_spot_age
+        if self.config.get('Configuration', 'pyjs8callCleanDirectedText') not in [None, 'None']:
+            config_clean_directed_text = self.config.get('Configuration', 'pyjs8callCleanDirectedText', bool)
+            if config_clean_directed_text is not None:
+                self.clean_directed_text = config_clean_directed_text
+
+        if self.config.get('Configuration', 'pyjs8callMonitorOutgoing') not in [None, 'None']:
+            config_monitor_outgoing = self.config.get('Configuration', 'pyjs8callMonitorOutgoing', bool, fallback=self.monitor_outgoing)
+            if config_monitor_outgoing is not None:
+                self.monitor_outgoing = config_monitor_outgoing
+
+        if self.config.get('Configuration', 'pyjs8callMaxSpotAge') not in [None, 'None']:
+            config_max_spot_age = self.config.get('Configuration', 'pyjs8callMaxSpotAge', int, fallback=self.max_spot_age)
+            if config_max_spot_age is not None:
+                self.max_spot_age = config_max_spot_age
 
         # stop application and client at exit
         atexit.register(self.stop)
-        
+
+        # load settings if file path specified
+        if settings_path is not None:
+            self.settings.load(settings_path)
+
     def start(self, headless=False, args=None, debugging=False, logging=False):
         '''Start and connect to the the JS8Call application.
 
         Initializes module objects:
         - Spot monitor (see pyjs8call.spotmonitor)
         - Window monitor (see pyjs8call.windowmonitor)
         - Offset monitor (see pyjs8call.offsetmonitor)
@@ -280,23 +294,21 @@
         Enables modules:
         - window
         - spots
         - offset
         - outgoing
         - schedule
 
-        Adds the @TIME group to JS8Call via the config file to enable drift monitor features.
-
         If logging is enabled the log file will be stored in the current user's *HOME* directory.
 
         if *args* contains the rig name switch (-r or --rig-name) the rig name is used to instantiate the rig specific config file before launching. Changes to the config object prior to calling *start* are saved to the rig specifc file only, and are not written to the main config file.
 
         Args:
             headless (bool): Run JS8Call headless via xvfb (Linux only)
-            args (list): Command line arguments (see appmonitor.start()), defaults to None
+            args (list): Command line arguments (see pyjs8call.appmonitor.AppMonitor.start), defaults to None
             debugging (bool): Print message data to the console, defaults to False
             logging (bool): Print message data to ~/pyjs8call.log, defaults to False
 
         Raises:
             RuntimeError: JS8Call config file section does not exist (likely because JS8Call has not been run and configured after installation)
         '''
         if args is None:
@@ -320,16 +332,14 @@
 
         try:
             # enable JS8Call TCP connection
             self.config.set('Configuration', 'TCPEnabled', 'true')
             self.config.set('Configuration', 'TCPServer', self.host)
             self.config.set('Configuration', 'TCPServerPort', str(self.port))
             self.config.set('Configuration', 'AcceptTCPRequests', 'true')
-            # support pyjs8call.timemonitor features
-            self.config.add_group('@TIME')
             self.config.write()
         except RuntimeError as e:
             raise RuntimeError('Try launching JS8Call, configuring audio and CAT interfaces as needed, '
                                'and then exiting the application normally. When the application '
                                'exits normally the first time it will initialize the config file.') from e
 
         self.js8call.start(headless = headless, args = args)
@@ -358,41 +368,57 @@
         self.propagation = pyjs8call.Propagation(self)
         
         self.window.enable()
         self.spots.enable()
         self.offset.enable()
         self.outgoing.enable()
         self.schedule.enable()
+
+        # if settings loaded, apply post start settings
+        if self.settings.loaded_settings is not None:
+            self.settings.apply_loaded_settings(post_start = True)
     
     def exit_tasks(self):
         '''Perform application exit tasks.
 
         This function is called automatically as needed.
         '''
         self.config.set('Configuration', 'pyjs8callCleanDirectedText', self.clean_directed_text)
         self.config.set('Configuration', 'pyjs8callMonitorOutgoing', self.monitor_outgoing)
         self.config.set('Configuration', 'pyjs8callMaxSpotAge', self.max_spot_age)
+
+        # restore previous config profile
+        if self._previous_profile is not None and self._previous_profile in self.settings.get_profile_list():
+            self.settings.set_profile(self._previous_profile)
+            
         self.config.write()
 
-    def stop(self):
+    def stop(self, terminate_js8call=True):
         '''Stop client, modules, and JS8Call application.
 
         Write to the configuration file, stop all threads, close the TCP socket, and kill the JS8Call application.
+
+        Args:
+            terminate_js8call (bool): Whether to terminate the JS8Call application, defaults to True
         '''
         self.online = False
         self.exit_tasks()
-        
+
+        self.js8call.app.terminate_js8call = terminate_js8call
+            
         try:
             return self.js8call.stop()
         except Exception:
             pass
 
     def restart(self):
         '''Stop and restart the JS8Call application and the associated TCP socket.
 
+        The *timer.out* file continues to grow while the JS8Call application is running, eventually consuming all available disk space and causing application errors. If the *timer.out* file exists, it is removed before restarting the application.
+
         Settings, local state, and spots are preserved.
         '''
         self.restarting = True
 
         # pause module loops to prevent errors
         modules = [
             self.outgoing,
@@ -403,30 +429,33 @@
             self.time_master,
             self.spots,
             self.schedule
         ]
 
         paused_modules = []
         
+        # avoid resuming modules paused before restart
         for module in modules:
             if module.enabled() and not module.paused():
                 module.pause()
                 paused_modules.append(module)
 
-        # write any pending config file changes, convience
+        # write config changes to file
         self.config.write()
         # reeset window monitoring
         self.window.reset()
         # save settings
         headless = self.js8call.app.headless
         args = self.js8call.app.args
         settings = self.js8call.restart_settings()
 
         # stop
-        self.stop()
+        self.online = False
+        self.js8call.stop()
+        time.sleep(1)
 
         # start
         self.js8call = pyjs8call.JS8Call(self, self.host, self.port)
         # restore settings
         self.js8call.reinitialize(settings)
         self.js8call.start(headless = headless, args = args)
         self.online = True
@@ -438,37 +467,54 @@
 
         # resume paused module loops
         for module in paused_modules:
             module.resume()
 
         self.restarting = False
 
+        if callable(self.callback.restart_complete):
+            self.callback.restart_complete()
+
     def restart_when_inactive(self, age=0):
         '''Restart the JS8Call application once there is no outgoing activity.
         
         This function is non-blocking due to the use of *threading.Thread* internally.
         
-        See *pyjs8call.js8call.activity()* for more details.
+        See pyjs8call.js8call.JS8Call.activity for more details.
         
         Args:
             age (int): Maximum age in seconds of outgoing activity to consider active, defaults to 0
         '''
         thread = threading.Thread(target=self._restart_when_inactive, args=(age,))
         thread.daemon = True
         thread.start()
         
     def _restart_when_inactive(self, age):
         '''Thread function to restart once there is no outgoing activity.'''
         self.js8call.block_until_inactive(age = age)
         self.restart()
         
+    def set_profile_on_exit(self, profile):
+        '''Set JS8Call configuration profile on exit
+
+        Args:
+            profile (str): Profile name to set on exit
+
+        Raises:
+            ValueError: Specified configuration profile does not exist
+        '''
+        if profile not in self.config.get_profile_list():
+            raise ValueError('Config profile \'' + profile + ' \' does not exist')
+
+        self._previous_profile = profile
+
     def activity(self, age=0):
         '''Whether there is outgoing activity.
 
-        This is a convenience function that calls *pyjs8call.js8call.activity()*.
+        This is a convenience function that calls pyjs8call.js8call.JS8Call.activity.
         
         Args:
             age (int): Maximum age of outgoing activity to consider active, defaults to 0 (disabled)
 
         Returns:
             bool: True if text in the tx text field, queued outgoing messages, or recent activity, False otherwise
         '''
@@ -518,39 +564,47 @@
             
         ids.append(self.settings.get_station_callsign())
         return ids
     
     def msg_is_to_me(self, msg):
         '''Determine if specified message is addressed to local station.
         
-        Utilizes *msg.is_directed_to()* and *client.identities()* internally.
+        Utilizes pyjs8call.message.Message.is_directed_to and Client.identities internally.
         
         Args:
-            msg (pyjs8call.message): Message object to evaluate
+            msg (pyjs8call.message.Message): Message object to evaluate
             
         Returns:
             bool: True if *msg* is addressed to the local station, False otherwise
         '''
         
         return msg.is_directed_to(self.identities())
     
+    def heard_freq_bands(self):
+        '''Get frequency bands with incoming messages.
+
+        Returns:
+            list: Frequency band designators like \'40m\'
+        '''
+        return self.js8call.heard_freq_bands()
+
     def clean_rx_message_text(self, msg):
         '''Clean incoming message text.
 
         Remove origin callsign, destination callsign or group (including relays), whitespace, and end-of-message characters. This leaves only the message text.
-        
-        The *pyjs8call.message.text* attribute stores the cleaned text while the *pyjs8call.message.value* attribute is unchanged.
 
-        Custom commands are also parsed out of message text. If a custom command is found, *pyjs8call.message.cmd* is set in the returned message.
+        Custom commands are also identified in the message text. If a custom command is found, *msg.cmd* is set in the returned message.
+        
+        The *msg.text* attribute stores the cleaned text while the *msg.value* attribute is unchanged.
 
         Args:
-            message (pyjs8call.message): Message object to clean
+            msg (pyjs8call.message.Message): Message object to clean
 
         Returns:
-            pyjs8call.message: Cleaned message object
+            pyjs8call.message.Message: Cleaned message object
         '''
         if msg is None:
             return msg
         # nothing to clean
         elif msg.value in (None, ''):
             return msg
         # already cleaned
@@ -588,23 +642,23 @@
         return msg
     
     def send_message(self, message):
         '''Send a raw JS8Call message.
         
         Message format: *MESSAGE*
         
-        *process_outgoing* is called just after message object creation, if set. If *msg.error* is set after custom processing, the message object is returned with a failed status and without being sent.
+        Client.process_outgoing is called just after message object creation, if set. If *msg.error* is set after custom processing, the message object is returned with a failed status and without being sent.
 
-        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if Client.monitor_outgoing is True (default).
 
         Args:
             message (str): Message text to send
 
         Returns:
-            pyjs8call.message: Constructed message object
+            pyjs8call.message.Message: Constructed message object
         '''
         # msg.type = Message.TX_SEND_MESSAGE by default
         msg = Message(value = message, origin = self.settings.get_station_callsign())
         
         # custom processing of outgoing messages
         if self.process_outgoing is not None:
             msg = self.process_outgoing(msg)
@@ -615,28 +669,65 @@
 
         if self.monitor_outgoing:
             self.outgoing.monitor(msg)
 
         self.js8call.send(msg)
         return msg
 
+    def send_directed_bytes_message(self, destination, message):
+        '''Send bytes via JS8Call message.
+        
+        Message format: *MESSAGE*
+
+        If *destination* is a list of callsigns they will be joined in the specified order and sent as a relay.
+        
+        Client.process_outgoing is called just after message object creation, if set. If *msg.error* is set after custom processing, the message object is returned with a failed status and without being sent.
+
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if Client.monitor_outgoing is True (default).
+
+        Args:
+            destination (str, list): Callsign(s) to direct the message to
+            message (bytes): Bytes to decode and send as JS8Call text
+
+        Returns:
+            pyjs8call.message.Message: Constructed message object
+        '''
+        # msg.type = Message.TX_SEND_MESSAGE by default
+        msg = Message(destination, origin = self.settings.get_station_callsign())
+        # decode message bytes to js8call supported characters
+        msg.decode(message)
+        
+        # custom processing of outgoing messages
+        if self.process_outgoing is not None:
+            msg = self.process_outgoing(msg)
+
+            if msg.error is not None:
+                msg.set('status', Message.STATUS_FAILED)
+                return msg
+
+        if self.monitor_outgoing:
+            self.outgoing.monitor(msg)
+
+        self.js8call.send(msg)
+        return msg
+
     def send_directed_command_message(self, destination, command, message=None):
         '''Send a directed JS8Call command message.
 
         Message format: *DESTINATION**COMMAND* *MESSAGE*
 
         If *destination* is a list of callsigns they will be joined in the specified order and sent as a relay.
         
-        *process_outgoing* is called just after message object creation, if set. If *msg.error* is set after custom processing, the message object is returned with a failed status and without being sent.
+        Client.process_outgoing is called just after message object creation, if set. If *msg.error* is set after custom processing, the message object is returned with a failed status and without being sent.
 
-        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if Client.monitor_outgoing is True (default).
 
         Args:
             destination (str, list): Callsign(s) to direct the message to
-            command (str): Command to include in message (see *pyjs8call.message* static commands)
+            command (str): Command to include in message (see pyjs8call.message.Message.Message static commands)
             message (str): Message text to send, defaults to None
         '''
         # msg.type = Message.TX_SEND_MESSAGE by default
         msg = Message(destination, command, message, self.settings.get_station_callsign())
         
         # custom processing of outgoing messages
         if self.process_outgoing is not None:
@@ -655,27 +746,52 @@
     def send_directed_message(self, destination, message):
         '''Send a directed JS8Call message.
         
         Message format: *DESTINATION* *MESSAGE*
 
         If *destination* is a list of callsigns they will be joined in the specified order and sent as a relay.
         
-        *process_outgoing* is called just after message object creation, if set. If *msg.error* is set after custom processing, the message object is returned with a failed status and without being sent.
+        Client.process_outgoing is called just after message object creation, if set. If *msg.error* is set after custom processing, the message object is returned with a failed status and without being sent.
 
-        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if Client.monitor_outgoing is True (default).
+
+        **Version 0.2.3:** Client.autodetect_outgoing_directed_command indicates that outgoing directed messages will be analyzed for JS8Call commands. If a command is found, a command message is constructed automatically. This simplifies outgoing message handling for applications built on top of pyjs8call.
 
         Args:
             destination (str, list): Callsign(s) to direct the message to
             message (str): Message text to send
 
         Returns:
-            pyjs8call.message: Constructed message object
+            pyjs8call.message.Message: Constructed message object
         '''
+        cmd_found = False
+        
+        # identify and handle commands in outgoing directed message
+        if self.autodetect_outgoing_directed_command:
+            # sort decending by command length to avoid matching a partial command
+            msg_cmds = sorted(pyjs8call.Message.COMMANDS, key=len, reverse=True)
+            message = message.upper()
+
+            for cmd in msg_cmds:
+                if message.startswith(cmd):
+                    cmd_found = True
+                    # preserve original message text
+                    message_text = message
+                    message = message.replace(cmd, '').strip()
+                    if len(message) == 0:
+                        message = None
+                    break
+    
         # msg.type = Message.TX_SEND_MESSAGE by default
-        msg = Message(destination, value = message, origin = self.settings.get_station_callsign())
+        if cmd_found:
+            msg = Message(destination, cmd, message, self.settings.get_station_callsign())
+            # preserve original message text
+            msg.set('text', message_text)
+        else:
+            msg = Message(destination, value = message, origin = self.settings.get_station_callsign())
         
         # custom processing of outgoing messages
         if self.process_outgoing is not None:
             msg = self.process_outgoing(msg)
 
             if msg.error is not None:
                 msg.set('status', Message.STATUS_FAILED)
@@ -686,27 +802,27 @@
 
         self.js8call.send(msg)
         return msg
 
     def send_heartbeat(self, grid=None):
         '''Send a JS8Call heartbeat message.
 
-        Note that JS8Call will only transmit API messages at the selected offset. Heartbeat messages can still be sent, but will not be in the heartbeat sub-band.
+        Note that JS8Call will only transmit API messages at the selected offset. Heartbeat messages can still be sent, but will not be in the heartbeat sub-band. See pyjs8call.hbnetwork for more information on automatically sending heartbeat messages in the heartbeat sub-band without interfacing with the JS8Call user interface.
 
         Message format: @HB HEARTBEAT *GRID*
 
         If no grid square is given the configured JS8Call grid square is used.
 
-        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if Client.monitor_outgoing is True (default).
 
         Args:
             grid (str): Grid square (truncated to 4 characters), defaults to None
 
         Returns:
-            pyjs8call.message: Constructed messsage object
+            pyjs8call.message.Message: Constructed messsage object
         '''
         if grid is None:
             grid = self.settings.get_station_grid()
 
         if grid is None:
             grid = ''
 
@@ -718,21 +834,21 @@
     def send_aprs_grid(self, grid=None):
         '''Send a JS8Call message with APRS grid square.
         
         Message format: @APRSIS GRID *GRID*
 
         If no grid square is given the configured JS8Call grid square is used.
 
-        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if Client.monitor_outgoing is True (default).
 
         Args:
             grid (str): Grid square (trucated to 4 characters), defaults to None
 
         Returns:
-            pyjs8call.message: Constructed messsage object
+            pyjs8call.message.Message: Constructed messsage object
 
         Raises:
             ValueError: Grid square not specified and JS8Call grid square not set
         '''
         if grid is None:
             grid = self.settings.get_station_grid()
         if grid in (None, ''):
@@ -743,85 +859,87 @@
         return self.send_directed_command_message('@APRSIS', Message.CMD_GRID, grid)
 
     def send_aprs_sms(self, phone, message):
         '''Send a JS8Call APRS message via a SMS gateway.
         
         Message format: @APRSIS CMD :SMSGATE&nbsp;&nbsp;&nbsp;:@1234567890 *MESSAGE*
 
-        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if Client.monitor_outgoing is True (default).
 
         Args:
             phone (str): Phone number to send SMS message to
             message (str): Message to be sent via SMS message
 
         Returns:
-            pyjs8call.message: Constructed message object
+            pyjs8call.message.Message: Constructed message object
         '''
         phone = str(phone).replace('-', '').replace('.', '').replace('(', '').replace(')', '')
         message = ':SMSGATE   :@' + phone + ' ' + message
         return self.send_directed_command_message('@APRSIS', Message.CMD_CMD, message)
     
     def send_aprs_email(self, email, message):
         '''Send a JS8Call APRS message via an e-mail gateway.
         
         Message format: @APRSIS CMD :EMAIL-2&nbsp;&nbsp;&nbsp;:EMAIL@DOMAIN.COM *MESSAGE*
 
-        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if Client.monitor_outgoing is True (default).
 
         Args:
             email (str): Email address to send message to
             message (str): Message to be sent via email
 
         Returns:
-            pyjs8call.message: Constructed message object
+            pyjs8call.message.Message: Constructed message object
         '''
         message = ':EMAIL-2   :' + email + ' ' + message
         return self.send_directed_command_message('@APRSIS', Message.CMD_CMD, message)
     
     def send_aprs_pota_spot(self, park, freq, mode, message, callsign=None):
         '''Send JS8Call APRS POTA spot message.
         
         Message format: @APRSIS CMD :POTAGW&nbsp;&nbsp;&nbsp;:*CALLSIGN* *PARK* *FREQ* *MODE* *MESSAGE*
 
         JS8Call configured callsign is used if no callsign is given.
 
-        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if Client.monitor_outgoing is True (default).
 
         Args:
             park (str): Name of park being activated
             freq (int): Frequency (in kHz) being used for park activation
             mode (str): Radio operating mode used for park activation
             message (str): Message to be sent with POTA spot
             callsign (str): Callsign of operator activating the park, defaults to None
 
         Returns:
-            pyjs8call.message: Constructed message object
+            pyjs8call.message.Message: Constructed message object
         '''
         if callsign is None:
             callsign = self.settings.get_station_callsign()
 
         message = ':POTAGW   :' + callsign + ' ' + park + ' ' + str(freq) + ' ' + mode + ' ' + message
         return self.send_directed_command_message('@APRSIS', Message.CMD_CMD, message)
     
     def get_inbox_messages(self, unread=True):
         '''Get JS8Call inbox messages.
 
         Args:
-            unread (bool): Get unread messages only if True, all messages if False
+            unread (bool): Get unread messages only if True, all messages if False, defaults to True
 
         Each inbox message is a *dict* with the following keys:
 
         | Key | Value Type |
         | -------- | -------- |
         | cmd | *str* |
         | freq | *int* | 
         | offset | *int* | 
         | snr | *int* |
         | speed | *int* |
-        | time | *str* |
+        | timestamp | *float* |
+        | utc_time_str | *str* |
+        | local_time_str | *str* |
         | origin | *str* |
         | destination | *str* |
         | path | *str* |
         | text | *str* |
         | type | *str* |
         | value | *str* |
         | status | *str* |
@@ -844,54 +962,54 @@
     def send_inbox_message(self, destination, message):
         '''Send JS8Call inbox message.
 
         Message format: *DESTINATION* MSG *MESSAGE*
 
         If *destination* is a list of callsigns they will be joined in the specified order and sent as a relay.
 
-        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if Client.monitor_outgoing is True (default).
 
         Args:
             destination (str, list): Callsign(s) to direct the message to
             message (str): Message text to send
 
         Returns:
-            pyjs8call.message: Constructed message object
+            pyjs8call.message.Message: Constructed message object
         '''
         return self.send_directed_command_message(destination, Message.CMD_MSG, message)
 
     def store_remote_inbox_message(self, remote, destination, message):
         '''Send JS8Call inbox message to be forwarded.
 
         Message format: *REMOTE* MSG TO:*DESTINATION* *MESSAGE*
 
         If *remote* is a list of callsigns they will be joined in the specified order and sent as a relay.
         
-        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if Client.monitor_outgoing is True (default).
 
         Args:
             remote (str, list): Callsign of intermediate station storing the message
             destination (str): Callsign of message recipient
             message (str): Message text to send
 
         Returns:
-            pyjs8call.message: Constructed message object
+            pyjs8call.message.Message: Constructed message object
         '''
         message = destination + ' ' + message
         return self.send_directed_command_message(remote, Message.CMD_MSG_TO, message)
 
     def store_local_inbox_message(self, destination, message):
         '''Store local JS8Call inbox message for future retrieval.
 
         Args:
             destination (str): Callsign to direct inbox message to
             message (str): Message text to send
 
         Returns:
-            pyjs8call.message: Constructed message object
+            pyjs8call.message.Message: Constructed message object
         '''
         msg = Message()
         msg.set('type', Message.INBOX_STORE_MESSAGE)
         msg.set('params', {'CALLSIGN': destination, 'TEXT': message})
         self.js8call.send(msg)
         time.sleep(self._set_get_delay)
         return self.get_inbox_messages()
@@ -899,245 +1017,344 @@
     def query_call(self, callsign, destination='@ALLCALL'):
         '''Send JS8Call callsign query.
         
         Message format: *DESTINATION* QUERY CALL *CALLSIGN*?
 
         If *destination* is a list of callsigns they will be joined in the specified order and sent as a relay.
 
-        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if Client.monitor_outgoing is True (default).
 
         Args:
             callsign (str): Callsign to query for
             destination (str, list): Callsign(s) to direct the query to, defaults to @ALLCALL
 
         Returns:
-            pyjs8call.message: Constructed message object
+            pyjs8call.message.Message: Constructed message object
         '''
         message = callsign + Message.CMD_Q
         return self.send_directed_command_message(destination, Message.CMD_QUERY_CALL, message)
 
     def query_messages(self, destination='@ALLCALL'):
         '''Send JS8Call stored message query.
         
         Message format: *DESTINATION* QUERY MSGS
 
         If *destination* is a list of callsigns they will be joined in the specified order and sent as a relay.
 
-        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if Client.monitor_outgoing is True (default).
 
         Args:
             destination (str, list): Callsign(s) to direct the query to, defaults to '@ALLCALL'
 
         Returns:
-            pyjs8call.message: Constructed message object
+            pyjs8call.message.Message: Constructed message object
         '''
         return self.send_directed_command_message(destination, Message.CMD_QUERY_MSGS)
 
     def query_message_id(self, destination, msg_id):
         '''Send JS8Call stored message ID query.
         
         Message format: *DESTINATION* QUERY MSG *ID*
 
         If *destination* is a list of callsigns they will be joined in the specified order and sent as a relay.
 
-        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if Client.monitor_outgoing is True (default).
 
         Args:
             destination (str, list): Callsign(s) to direct the query to
             msg_id (str): Message ID to query for
 
         Returns:
-            pyjs8call.message: Constructed message object
+            pyjs8call.message.Message: Constructed message object
         '''
         return self.send_directed_command_message(destination, Message.CMD_QUERY, 'MSG {}'.format(msg_id))
 
     def query_hearing(self, destination):
         '''Send JS8Call hearing query.
         
         Message format: *DESTINATION* HEARING?
 
         If *destination* is a list of callsigns they will be joined in the specified order and sent as a relay.
 
-        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if Client.monitor_outgoing is True (default).
 
         Args:
             destination (str, list): Callsign(s) to direct the query to
 
         Returns:
-            pyjs8call.message: Constructed message object
+            pyjs8call.message.Message: Constructed message object
         '''
         return self.send_directed_command_message(destination, Message.CMD_HEARING_Q)
 
     def query_snr(self, destination):
         '''Send JS8Call SNR query.
         
         Message format: *DESTINATION* SNR?
 
         If *destination* is a list of callsigns they will be joined in the specified order and sent as a relay.
 
-        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if Client.monitor_outgoing is True (default).
 
         Args:
             destination (str, list): Callsign(s) to direct the query to
 
         Returns:
-            pyjs8call.message: Constructed message object
+            pyjs8call.message.Message: Constructed message object
         '''
         return self.send_directed_command_message(destination, Message.CMD_SNR_Q)
 
     def query_grid(self, destination):
         '''Send JS8Call grid query.
         
         Message format: *DESTINATION* GRID?
 
         If *destination* is a list of callsigns they will be joined in the specified order and sent as a relay.
 
-        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if Client.monitor_outgoing is True (default).
 
         Args:
             destination (str, list): Callsign(s) to direct the query to
 
         Returns:
-            pyjs8call.message: Constructed message object
+            pyjs8call.message.Message: Constructed message object
         '''
         return self.send_directed_command_message(destination, Message.CMD_GRID_Q)
 
     def query_info(self, destination):
         '''Send JS8Call info query.
         
         Message format: *DESTINATION* INFO?
 
         If *destination* is a list of callsigns they will be joined in the specified order and sent as a relay.
 
-        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if Client.monitor_outgoing is True (default).
 
         Args:
             destination (str, list): Callsign(s) to direct the query to
 
         Returns:
-            pyjs8call.message: Constructed message object
+            pyjs8call.message.Message: Constructed message object
         '''
         return self.send_directed_command_message(destination, Message.CMD_INFO_Q)
 
     def query_status(self, destination):
         '''Send JS8Call status query.
         
         Message format: *DESTINATION* STATUS?
 
         If *destination* is a list of callsigns they will be joined in the specified order and sent as a relay.
         
-        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if Client.monitor_outgoing is True (default).
 
         Args:
             destination (str, list): Callsign(s) to direct the query to
 
         Returns:
-            pyjs8call.message: Constructed message object
+            pyjs8call.message.Message: Constructed message object
         '''
         return self.send_directed_command_message(destination, Message.CMD_STATUS_Q)
 
-    def get_call_activity(self, age=None):
+    def get_call_activity(self, age=None, hearing_age=None):
         '''Get JS8Call call activity.
 
         To get or set JS8Call callsign activity aging from the configuration file:
         `client.config.get('Configuration', 'CallsignAging', int)`
         `client.config.set('Configuration', 'CallsignAging', 120) # 120 minutes`
 
-        See *client.get_distance()* for more information on the value and format of *distance*.
-
         Each call activity item is a dictionary with the following keys:
 
         | Key | Value Type |
         | -------- | -------- |
-        | origin | str |
-        | grid | str |
-        | snr | int |
-        | time (UTC) | int |
-        | timestamp (local) | int |
-        | local_time_str | str |
-        | speed | str |
-        | hearing | list |
-        | heard_by | list |
-        | distance | tuple |
+        | origin | *str* |
+        | grid | *str* |
+        | snr | *int* |
+        | timestamp | *float* |
+        | utc_time_str | *str* |
+        | local_time_str | *str* |
+        | speed | *str* |
+        | hearing | *list* |
+        | heard_by | *list* |
+        | distance | *int* |
+        | distance_units | *str* |
+        | bearing | *int* |
 
         Args:
             age (int): Maximum activity age in minutes, defaults to JS8Call callsign activity aging
+            hearing_age (int): Maximum hearing and heard_by activity age in minutes, defaults to *age*
 
         Returns:
-            list: Call activity items, sorted decending by *time* (recent first)
-
-            If grid is not set, distance is *(None, None)*.
+            list: Call activity items, sorted decending by *timestamp* (recent first)
         '''
         if age is None:
             age = self.config.get('Configuration', 'CallsignAging', int)
 
-        age *= 60 # minutes to seconds
-
         msg = Message()
         msg.type = Message.RX_GET_CALL_ACTIVITY
         self.js8call.send(msg)
         call_activity = self.js8call.watch('call_activity')
 
-        hearing = self.hearing(age)
-        heard_by = self.heard_by(age , hearing)
+        activity_age = age * 60 # minutes to seconds
+        
+        if hearing_age is None:
+            hearing_age = age # minutes
+            
+        hearing = self.hearing(hearing_age)
+        heard_by = self.heard_by(hearing_age , hearing)
         now = time.time()
 
         for i in call_activity.copy():
             activity = call_activity.pop(0)
             activity['origin'] = activity['origin'].strip()
             activity['grid'] = activity['grid'].strip()
+            activity['distance'] = None
+            activity['distance_units'] = None
+            activity['bearing'] = None
 
             # remove aged activity
-            if age != 0 and (now - activity['timestamp']) > age:
+            if activity_age != 0 and (now - activity['timestamp']) > activity_age:
                 continue
 
-            if activity['origin'] in hearing:
-                activity['hearing'] = hearing[activity['origin']]
-            else:
-                activity['hearing'] = []
-
-            if activity['origin'] in heard_by:
-                activity['heard_by'] = heard_by[activity['origin']]
-            else:
-                activity['heard_by'] = []
+            activity['hearing'] = hearing[activity['origin']] if activity['origin'] in hearing else []
+            activity['heard_by'] = heard_by[activity['origin']] if activity['origin'] in heard_by else []
 
             if activity['grid'] not in (None, ''):
-                activity['distance'] = self.grid_distance(activity['grid'])
-            else:
-                activity['distance'] = (None, None, None)
-
-            spot = self.spots.filter(origin = activity['origin'], age = age, count = 1)
-            if len(spot) and isinstance(spot[0].get('speed'), int):
-                activity['speed'] = self.settings.submode_to_speed(spot[0].get('speed'))
-            else:
-                activity['speed'] = ''
+                try:
+                    distance, distance_units, bearing = self.grid_distance(activity['grid'])
+                    activity['distance'] = distance
+                    activity['distance_units'] = distance_units
+                    activity['bearing'] = bearing
+                except ValueError:
+                    pass
+
+            spot = self.spots.filter(origin = activity['origin'], age = activity_age, count = 1)
+            activity['speed'] = self.settings.submode_to_speed(spot[0].get('speed')) if len(spot) and isinstance(spot[0].get('speed'), int) else None
 
             call_activity.append(activity)
 
+        # sort by most recent first
+        call_activity.sort(key = lambda activity: activity['timestamp'], reverse = True)
+        return call_activity
+        
+    def get_call_activity_from_spots(self, age=None, hearing_age=None):
+        '''Get JS8Call call activity.
+
+        Similar to *Client.get_call_activity* except that stored spots are processed locally instead of using the JS8Call API. This function has better performance than *Client.get_call_activity*.
+
+        To get or set JS8Call callsign activity aging from the configuration file:
+        `client.config.get('Configuration', 'CallsignAging', int)`
+        `client.config.set('Configuration', 'CallsignAging', 120) # 120 minutes`
+
+        Each call activity item is a dictionary with the following keys:
+
+        | Key | Value Type |
+        | -------- | -------- |
+        | origin | *str* |
+        | grid | *str* |
+        | snr | *int* |
+        | timestamp | *float* |
+        | utc_time_str | *str* |
+        | local_time_str | *str* |
+        | speed | *str* |
+        | hearing | *list* |
+        | heard_by | *list* |
+        | distance | *int* |
+        | distance_units | *str* |
+        | bearing | *int* |
+
+        Args:
+            age (int): Maximum activity age in minutes, defaults to JS8Call callsign activity aging
+            hearing_age (int, None): Maximum hearing and heard_by activity age in minutes, defaults to *age*
+
+        Returns:
+            list: Call activity items, sorted decending by *timestamp* (recent first)
+        '''
+        if age is None:
+            age = self.config.get('Configuration', 'CallsignAging', int)
+        
+        spot_age = age * 60 # minutes to seconds
+        spots = self.spots.filter(age = spot_age)
+        
+        if hearing_age is None:
+            hearing_age = spot_age # seconds
+        else:
+            hearing_age = hearing_age * 60 # minutes to seconds
+        
+        call_activity = []
+        call_activity_origins = []
+        call_activity_grids = {}
+        hearing_spots = []
+
+        # improve performance by processing all spots only once,
+        # instead of multiple times by calling pre-built functions such as client.spots.filter and client.hearing (without passing spots)
+        for spot in self.spots.all():
+            # map origins to grid squares for later use
+            # keep only most recent grid square for each origin
+            if spot.origin not in (None, '') and spot.origin not in call_activity_grids and spot.grid not in (None, ''):
+                call_activity_grids[spot.origin] = (spot.grid, spot.distance, spot.distance_units, spot.bearing)
+
+            # spot age is seconds
+            if spot.age() <= hearing_age:
+                hearing_spots.append(spot)
+                
+            if spot.age() <= spot_age and spot.origin not in call_activity_origins:
+                # track origins to keep only most recent activity for each origin
+                call_activity_origins.append(spot.origin)
+
+                activity = {}
+                activity['origin'] = spot.origin
+                activity['grid'] = spot.grid
+                activity['snr'] = spot.snr
+                activity['timestamp'] = spot.timestamp
+                activity['utc_time_str'] = spot.utc_time_str
+                activity['local_time_str'] = spot.local_time_str
+                activity['distance'] = spot.distance
+                activity['distance_units'] = spot.distance_units
+                activity['bearing'] = spot.bearing
+                activity['speed'] = self.settings.submode_to_speed(spot.speed) if spot.speed is not None else None
+
+                call_activity.append(activity)
+
+        # convert seconds to minutes
+        hearing = self.hearing(hearing_age / 60, hearing_spots)
+        heard_by = self.heard_by(hearing_age / 60, hearing)
+
+        for i in range(len(call_activity)):
+            # get grid squares that were reported before *spot_age*
+            if call_activity[i]['grid'] in (None, '') and call_activity[i]['origin'] in call_activity_grids:
+                grid, distance, distance_units, bearing = call_activity_grids[call_activity[i]['origin']]
+                call_activity[i]['grid'] = grid
+                call_activity[i]['distance'] = distance
+                call_activity[i]['distance_units'] = distance_units
+                call_activity[i]['bearing'] = bearing
+
+            call_activity[i]['hearing'] = hearing[call_activity[i]['origin']] if call_activity[i]['origin'] in hearing else []
+            call_activity[i]['heard_by'] = heard_by[call_activity[i]['origin']] if call_activity[i]['origin'] in heard_by else []
+            
+        # sort by most recent first
         call_activity.sort(key = lambda activity: activity['timestamp'], reverse = True)
         return call_activity
 
     def get_band_activity(self, age=None):
         '''Get JS8Call band activity.
 
         To get or set JS8Call callsign activity aging from the configuration file:
         `client.config.get('Configuration', 'ActivityAging', int)`
         `client.config.set('Configuration', 'ActivityAging', 5) # 5 minutes`
 
         Each band activity item is a dictionary with the following keys:
 
         | Key | Value Type |
         | -------- | -------- |
-        | freq (Hz) | int |
-        | offset (Hz) | int |
-        | snr | int |
-        | time (UTC) | int |
-        | timestamp (local) | int |
-        | local_time_str | str |
-        | text | str |
+        | freq (Hz) | *int* |
+        | offset (Hz) | *int* |
+        | snr | *int* |
+        | timestamp | *float* |
+        | utc_time_str | *str* |
+        | local_time_str | *str* |
+        | text | *str* |
 
         Args:
             age (int): Maximum activity age in minutes, defaults to JS8Call band activity aging
 
         Returns:
             list: Band activity items, sorted ascending by offset
         '''
@@ -1170,16 +1387,16 @@
         band_activity.sort(key=lambda activity: activity['offset'])
         return band_activity
 
     def get_selected_call(self):
         '''Get JS8Call selected callsign.
 
         Returns:
-            str: Callsign selected on the JS8Call user interface
-            None: No callsign selected
+        - str: Callsign selected on the JS8Call user interface
+        - None: No callsign selected
         '''
         msg = Message()
         msg.type = Message.RX_GET_SELECTED_CALL
         self.js8call.send(msg)
         selected_call = self.js8call.watch('selected_call')
 
         if selected_call == '':
@@ -1269,22 +1486,19 @@
         rx_messages = []
         for msg in msgs:
             # check for first dash and opening offset parenthesis to avoid processing malformed text 
             # this string avoids finding negative SNR values in message text
             if ' - (' not in msg:
                 continue
 
-            parts = msg.split('-')
-            # handle dash/hyphen/negative in message text
-            if len(parts) > 3:
-                parts[2] = '-'.join(parts[2:])
-                parts = parts[:3]
-
+            # limit splits to avoid splitting message text
+            # 2 splits = 3 parts (timestamp, offset, text)
+            parts = msg.split('-', maxsplit=2)
+            
             data = {}
-
             data['time'] = parts[0].strip()
             data['offset'] = int(parts[1].strip(' \n()'))
             data['text'] = parts[2].strip()
             data['origin'] = None
             data['destination'] = None
 
             if ':' in data['text']:
@@ -1325,42 +1539,48 @@
             if not own and data['origin'] == callsign:
                 continue
 
             rx_messages.append(data)
 
         return rx_messages
     
-    def hearing(self, age=None):
-        '''Which stations other stations are hearing.
+    def hearing(self, age=None, spots=None):
+        '''Stations other stations are hearing.
+
+        If calling both pyjs8call.spotmonitor.SpotMonitor.filter and Client.hearing, it is more efficient to pass the result of pyjs8call.spotmonitor.SpotMonitor.filter to Client.hearing. Otherwise, Client.hearing will call pyjs8call.spotmonitor.SpotMonitor.filter again internally.
 
         Args:
             age (int): Maximum message age in minutes, defaults to JS8Call callsign activity aging
 
         Returns:
             dict: Example format `{'station': ['station', ...], ...}`
+            spots: Spots to process (ex. from pyjs8call.spotmonitor.SpotMonitor.filter), defaults to None
         '''
         if age is None:
             age = self.config.get('Configuration', 'CallsignAging', int)
 
         age *= 60 # minutes to seconds
             
         callsign = self.settings.get_station_callsign()
         hearing = {}
-        
-        for spot in self.spots.filter(age = age):
-            # only process msgs with directed commands
-            if spot.cmd is None:
-                continue
 
+        if spots is None:
+            spots = self.spots.filter(age = age)
+        
+        for spot in spots:
             # stations we are hearing
             if callsign not in hearing:
                 hearing[callsign] = [spot.origin]
             elif spot.origin not in hearing[callsign]:
                 hearing[callsign].append(spot.origin)
                 
+            # only process msgs with directed commands
+            if spot.cmd is None:
+                continue
+
             if spot.cmd == Message.CMD_HEARING and spot.hearing is not None:
                 if spot.origin not in hearing:
                     hearing[spot.origin] = spot.hearing
                 else:
                     spot_hearing = [station for station in spot.hearing if station not in hearing[spot.origin]]
                     hearing[spot.origin].extend(spot_hearing)
             
@@ -1377,17 +1597,17 @@
 
                 elif spot.destination != '@ALLCALL' and spot.destination not in hearing[spot.origin]:
                     hearing[spot.origin].append(spot.destination)
 
         return hearing
 
     def station_hearing(self, station=None, age=None):
-        '''Which stations the specified station is hearing.
+        '''Stations the specified station is hearing.
         
-        See *client.hearing()* for more information.
+        See Client.hearing for more information.
 
         Args:
             station (str): Station callsign to get hearing data for, defaults to local station callsign
             age (int): Maximum message age in minutes, defaults to JS8Call callsign activity aging
 
         Returns:
             list: Station callsigns the specified station is hearing
@@ -1399,23 +1619,23 @@
 
         if station in hearing:
             return hearing[station]
         else:
             return []
     
     def heard_by(self, age=None, hearing=None):
-        '''Which stations are hearing other station.
+        '''Stations other stations are heard by.
 
-        *client.heard_by()* is the inverse of *client.hearing()*.
+        Client.heard_by is the inverse of Client.hearing.
 
-        If calling both *client.hearing()* and *client.heard_by*, it is more efficient to pass the result of *client.hearing()* to *client.heard_by()*. Otherwise, *client.heard_by()* will call *client.hearing()* again internally.
+        If calling both Client.hearing and Client.heard_by, it is more efficient to pass the result of Client.hearing to Client.heard_by. Otherwise, Client.heard_by() will call Client.hearing again internally.
 
         Args:
             age (int): Maximum message age in minutes, defaults to JS8Call callsign activity aging
-            hearing (dict): Result of *client.hearing()*, defaults to result of *client.hearing()*
+            hearing (dict): Result of Client.hearing, defaults to result of Client.hearing
 
         Returns:
             dict: Example format `{'station': ['station', ...], ...}`
         '''
         if age is None:
             age = self.config.get('Configuration', 'CallsignAging', int)
         
@@ -1431,22 +1651,22 @@
                     heard_by[callsign] = [key]
                 elif key not in heard_by[callsign]:
                     heard_by[callsign].append(key)
 
         return heard_by
 
     def station_heard_by(self, station=None, age=None, hearing=None):
-        '''Which stations are hearing the specified station.
+        '''Stations the specified station is heard by.
 
-        See *client.heard_by()* for more information.
+        See Client.heard_by for more information.
         
         Args:
             station (str): Station callsign to get heard by data for, defaults to local station callsign
             age (int): Maximum message age in minutes, defaults to JS8Call callsign activity aging
-            hearing (dict): Result of *client.hearing()*, defaults to result of *client.hearing()*
+            hearing (dict): Result of Client.hearing, defaults to result of Client.hearing
 
         Returns:
             list: Station callsigns heard by the specified station
         '''
         heard_by = self.heard_by(age, hearing)
 
         if station is None:
@@ -1486,15 +1706,15 @@
         Args:
             grid_a (str): First grid square
             grid_b (str): Second grid square, defaults to JS8Call grid square
 
         Returns:
             tuple (int, str, int): Distance, distance units, and bearing in degrees (ex. (1194, 'mi', 312)).
             
-            Distance units match JS8Call distance units, see *client.settings.get_distance_units()*.
+            Distance units match JS8Call distance units, see pyjs8call.settings.Settings.get_distance_units.
 
         Raises:
             ValueError: *grid_b* is *None* and JS8Call grid square is not set
         '''
         earth_radius_km = 6371
         earth_radius_mi = 3958.756
 
@@ -1587,1012 +1807,7 @@
 
         except ValueError as e:
             raise ValueError('Invalid grid square format. Field and sub-square must be letters A-R '
                              '(case insensitive), and square must be numbers 0-9 (ex. EM19es).') from e
 
         return (lat, lon)
 
-
-class Settings:
-    '''Settings function container.
-    
-    This class is initilized by pyjs8call.client.Client.
-    '''
-    
-    def __init__(self, client):
-        '''Initialize settings object.
-
-        Returns:
-            pyjs8call.client.Settings: Constructed setting object
-        '''
-        self._client = client
-
-    def enable_heartbeat_networking(self):
-        '''Enable heartbeat networking via config file.
-        
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-        
-        Note that this function disables JS8Call application heartbeat networking via the config file. To enable the pyjs8call heartbeat network messaging module see pyjs8call.hbnetwork.HeartbeatNetworking.enable_networking().
-        '''
-        self._client.config.set('Common', 'SubModeHB', 'true')
-
-    def disable_heartbeat_networking(self):
-        '''Disable heartbeat networking via config file.
-        
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-        
-        Note that this function disables JS8Call application heartbeat networking via the config file. To disable the pyjs8call heartbeat network messaging module see pyjs8call.hbnetwork.HeartbeatNetworking.disable_networking().
-        '''
-        self._client.config.set('Common', 'SubModeHB', 'false')
-
-    def heartbeat_networking_enabled(self):
-        '''Whether heartbeat networking enabled in config file.
-        
-        Returns:
-            bool: True if heartbeat networking enabled, False otherwise
-        '''
-        return self._client.config.get('Common', 'SubModeHB', bool)
-
-    def get_heartbeat_interval(self):
-        '''Get heartbeat networking interval.
-        
-        Returns:
-            int: Heartbeat networking time interval in minutes
-        '''
-        return self._client.config.get('Common', 'HBInterval', int)
-        
-    def set_heartbeat_interval(self, interval):
-        '''Set the heartbeat networking interval.
-        
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-
-        Args:
-            interval (int): New heartbeat networking time interval in minutes
-        
-        Returns:
-            int: Current heartbeat networking time interval in minutes
-        '''
-        return self._client.config.set('Common', 'HBInterval', interval)
-        
-    def enable_heartbeat_acknowledgements(self):
-        '''Enable heartbeat acknowledgements via config file.
-        
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-        '''
-        self._client.config.set('Common', 'SubModeHBAck', 'true')
-
-    def disable_heartbeat_acknowledgements(self):
-        '''Disable heartbeat acknowledgements via config file.
-        
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-        '''
-        self._client.config.set('Common', 'SubModeHBAck', 'false')
-
-    def heartbeat_acknowledgements_enabled(self):
-        '''Whether heartbeat acknowledgements enabled in config file.
-        
-        Returns:
-            bool: True if heartbeat acknowledgements enabled, False otherwise
-        '''
-        return self._client.config.get('Common', 'SubModeHBAck', bool)
-        
-    def pause_heartbeat_during_qso(self):
-        '''Pause heartbeat messages during QSO via config file.
-        
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-        '''
-        self._client.config.set('Configuration', 'HeartbeatQSOPause', 'true')
-
-    def allow_heartbeat_during_qso(self):
-        '''Allow heartbeat messages during QSO via config file.
-        
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-        '''
-        self._client.config.set('Configuration', 'HeartbeatQSOPause', 'false')
-
-    def heartbeat_during_qso_paused(self):
-        '''Whether heartbeat messages paused during QSO in config file.
-        
-        Returns:
-            bool: True if heartbeat messages paused during QSO, False otherwise
-        '''
-        return self._client.config.get('Configuration', 'HeartbeatQSOPause', bool)
-
-    def enable_multi_decode(self):
-        '''Enable multi-speed decoding via config file.
-        
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-        '''
-        self._client.config.set('Common', 'SubModeHBMultiDecode', 'true')
-
-    def disable_multi_decode(self):
-        '''Disable multi-speed decoding via config file.
-        
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-        '''
-        self._client.config.set('Common', 'SubModeMultiDecode', 'false')
-
-    def multi_decode_enabled(self):
-        '''Whether multi-decode enabled in config file.
-        
-        Returns:
-            bool: True if multi-decode enabled, False otherwise
-        '''
-        return self._client.config.get('Common', 'SubModeMultiDecode', bool)
-
-    def enable_autoreply_startup(self):
-        '''Enable autoreply on start-up via config file.
-        
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-        '''
-        self._client.config.set('Configuration', 'AutoreplyOnAtStartup', 'true')
-
-    def disable_autoreply_startup(self):
-        '''Disable autoreply on start-up via config file.
-        
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-        '''
-        self._client.config.set('Configuration', 'AutoreplyOnAtStartup', 'false')
-
-    def autoreply_startup_enabled(self):
-        '''Whether autoreply enabled at start-up in config file.
-        
-        Returns:
-            bool: True if autoreply is enabled at start-up, False otherwise
-        '''
-        return self._client.config.get('Configuration', 'AutoreplyOnAtStartup', bool)
-
-    def enable_autoreply_confirmation(self):
-        '''Enable autoreply confirmation via config file.
-        
-        When running headless the autoreply confirmation dialog box will be inaccessible.
-        
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-        '''
-        self._client.config.set('Configuration', 'AutoreplyConfirmation', 'true')
-
-    def disable_autoreply_confirmation(self):
-        '''Disable autoreply confirmation via config file.
-        
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-        '''
-        self._client.config.set('Configuration', 'AutoreplyConfirmation', 'false')
-
-    def autoreply_confirmation_enabled(self):
-        '''Whether autoreply confirmation enabled in config file.
-        
-        Returns:
-            bool: True if autoreply confirmation enabled, False otherwise
-        '''
-        return self._client.config.get('Configuration', 'AutoreplyConfirmation', bool)
-
-    def enable_allcall(self):
-        '''Enable @ALLCALL participation via config file.
-        
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-        '''
-        self._client.config.set('Configuration', 'AvoidAllcall', 'false')
-
-    def disable_allcall(self):
-        '''Disable @ALLCALL participation via config file.
-        
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-        '''
-        self._client.config.set('Configuration', 'AvoidAllcall', 'true')
-
-    def allcall_enabled(self):
-        '''Whether @ALLCALL participation enabled in config file.
-        
-        Returns:
-            bool: True if @ALLCALL participation enabled, False otherwise
-        '''
-        return not self._client.config.get('Configuration', 'AvoidAllcall', bool)
-
-    def enable_reporting(self):
-        '''Enable PSKReporter reporting via config file.
-        
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-        '''
-        self._client.config.set('Configuration', 'PSKReporter', 'true')
-
-    def disable_reporting(self):
-        '''Disable PSKReporter reporting via config file.
-        
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-        '''
-        self._client.config.set('Configuration', 'PSKReporter', 'false')
-
-    def reporting_enabled(self):
-        '''Whether PSKReporter reporting enabled in config file.
-        
-        Returns:
-            bool: True if reporting enabled, False otherwise
-        '''
-        return self._client.config.get('Configuration', 'PSKReporter', bool)
-
-    def enable_transmit(self):
-        '''Enable JS8Call transmitting via config file.
-        
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-        '''
-        self._client.config.set('Configuration', 'TransmitOFF', 'false')
-
-    def disable_transmit(self):
-        '''Disable JS8Call transmitting via config file.
-        
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-        '''
-        self._client.config.set('Configuration', 'TransmitOFF', 'true')
-
-    def transmit_enabled(self):
-        '''Whether JS8Call transmitting enabled in config file.
-        
-        Returns:
-            bool: True if transmitting enabled, False otherwise
-        '''
-        return not self._client.config.get('Configuration', 'TransmitOFF', bool)
-
-    def get_profile(self):
-        '''Get active JS8call configuration profile via config file.
-
-        This is a convenience function. See pyjs8call.confighandler for other configuration related functions.
-
-        Returns:
-            str: Name of the active configuration profile
-        '''
-        return self._client.config.get_active_profile()
-
-    def get_profile_list(self):
-        '''Get list of JS8Call configuration profiles via config file.
-
-        This is a convenience function. See pyjs8call.confighandler for other configuration related functions.
-
-        Returns:
-            list: List of configuration profile names
-        '''
-        return self._client.config.get_profile_list()
-
-    def set_profile(self, profile):
-        '''Set active JS8Call configuration profile via config file.
-        
-        This is a convenience function. See pyjs8call.confighandler for other configuration related functions.
-        
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-
-        Args:
-            profile (str): Profile name
-
-        Raises:
-            ValueError: Specified profile name does not exist
-        '''
-        if profile not in self._client.config.get_profile_list():
-            raise ValueError('Config profile \'' + profile + '\' does not exist')
-
-        # set the profile as active
-        self._client.config.change_profile(profile)
-
-    def get_primary_highlight_words(self):
-        '''Get primary highlight words via config file.
-
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-        
-        Returns:
-            list: Words that should be highlighted on the JC8Call UI
-        '''
-        words = self._client.config.get('Configuration', 'PrimaryHighlightWords')
-
-        if words == '@Invalid()':
-            words = []
-        elif words is not None:
-            words = words.split(', ')
-
-        return words
-
-    def set_primary_highlight_words(self, words):
-        '''Set primary highlight words via config file.
-
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-        
-        Args:
-            words (list): Words that should be highlighted on the JC8Call UI
-        '''
-        if len(words) == 0:
-            words = '@Invalid()'
-        else:
-            words = ', '.join(words)
-
-        self._client.config.set('Configuration', 'PrimaryHighlightWords', words)
-
-    def get_secondary_highlight_words(self):
-        '''Get secondary highlight words via config file.
-
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-        
-        Returns:
-            list: Words that should be highlighted on the JC8Call UI
-        '''
-        words = self._client.config.get('Configuration', 'SecondaryHighlightWords')
-
-        if words == '@Invalid()':
-            words = []
-        elif words is not None:
-            words = words.split(', ')
-
-        return words
-
-    def set_secondary_highlight_words(self, words):
-        '''Set secondary highlight words via config file.
-
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-        
-        Args:
-            words (list): Words that should be highlighted on the JC8Call UI
-        '''
-        if len(words) == 0:
-            words = '@Invalid()'
-        else:
-            words = ', '.join(words)
-
-        self._client.config.set('Configuration', 'SecondaryHighlightWords', words)
-
-    def submode_to_speed(self, submode):
-        '''Map submode *int* to speed *str*.
-
-        | Submode | Speed |
-        | -------- | -------- |
-        | 0 | normal |
-        | 1 | fast |
-        | 2 | turbo |
-        | 4 | slow |
-        | 8 | ultra |
-
-        Args:
-            submode (int): Submode to map to text
-
-        Returns:
-            str: Speed as text
-        '''
-        # map integer to text
-        speeds = {4:'slow', 0:'normal', 1:'fast', 2:'turbo', 8:'ultra'}
-
-        if submode is not None and int(submode) in speeds:
-            return speeds[int(submode)]
-        else:
-            raise ValueError('Invalid submode \'' + str(submode) + '\'')
-
-    def get_speed(self, update=False):
-        '''Get JS8Call modem speed.
-
-        Possible modem speeds:
-        - slow
-        - normal
-        - fast
-        - turbo
-        - ultra
-
-        Args:
-            update (bool): Update speed if True or use local state if False, defaults to False
-
-        Returns:
-            str: JS8call modem speed setting
-        '''
-        speed = self._client.js8call.get_state('speed')
-
-        if update or speed is None:
-            msg = Message()
-            msg.set('type', Message.MODE_GET_SPEED)
-            self._client.js8call.send(msg)
-            speed = self._client.js8call.watch('speed')
-
-        return self.submode_to_speed(speed)
-
-    def set_speed(self, speed):
-        '''Set JS8Call modem speed via config file.
-
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-
-        Possible modem speeds:
-        - slow
-        - normal
-        - fast
-        - turbo
-        - ultra
-
-        Args:
-            speed (str): Speed to set
-
-        Returns:
-            str: JS8Call modem speed setting
-
-        '''
-        if isinstance(speed, str):
-            speeds = {'slow':4, 'normal':0, 'fast':1, 'turbo':2, 'ultra':8}
-            if speed in speeds:
-                speed = speeds[speed]
-            else:
-                raise ValueError('Invalid speed: ' + str(speed))
-
-        return self._client.config.set('Common', 'SubMode', speed)
-
-#        TODO this code sets speed via API, which doesn't work as of JS8Call v2.2
-#        msg = Message()
-#        msg.set('type', Message.MODE_SET_SPEED)
-#        msg.set('params', {'SPEED': speed})
-#        self._client.js8call.send(msg)
-#        time.sleep(self._client._set_get_delay)
-#        return self.get_speed()
-
-    def get_freq(self, update=False):
-        '''Get JS8Call dial frequency.
-
-        Args:
-            update (bool): Update if True or use local state if False, defaults to False
-
-        Returns:
-            int: Dial frequency in Hz
-        '''
-        freq = self._client.js8call.get_state('dial')
-
-        if update or freq is None:
-            msg = Message()
-            msg.type = Message.RIG_GET_FREQ
-            self._client.js8call.send(msg)
-            freq = self._client.js8call.watch('dial')
-
-        return freq
-
-    def set_freq(self, freq):
-        '''Set JS8Call dial frequency.
-
-        Args:
-            freq (int): Dial frequency in Hz
-
-        Returns:
-            int: Dial frequency in Hz
-        '''
-        msg = Message()
-        msg.set('type', Message.RIG_SET_FREQ)
-        msg.set('params', {'DIAL': freq, 'OFFSET': self._client.js8call.get_state('offset')})
-        self._client.js8call.send(msg)
-        time.sleep(self._client._set_get_delay)
-        return self.get_freq(update = True)
-
-    def get_band(self):
-        '''Get frequency band designation.
-
-        Returns:
-            str: Band designator like \'40m\' or Client.OOB (out-of-band)
-        '''
-        return Client.freq_to_band(self.get_freq())
-
-    def get_offset(self, update=False):
-        '''Get JS8Call offset frequency.
-
-        Args:
-            update (bool): Update if True or use local state if False, defaults to False
-
-        Returns:
-            int: Offset frequency in Hz
-        '''
-        offset = self._client.js8call.get_state('offset')
-        
-        if update or offset is None:
-            msg = Message()
-            msg.type = Message.RIG_GET_FREQ
-            self._client.js8call.send(msg)
-            offset = self._client.js8call.watch('offset')
-
-        return offset
-
-    def set_offset(self, offset):
-        '''Set JS8Call offset frequency.
-
-        Args:
-            offset (int): Offset frequency in Hz
-
-        Returns:
-            int: Offset frequency in Hz
-        '''
-        msg = Message()
-        msg.set('type', Message.RIG_SET_FREQ)
-        msg.set('params', {'DIAL': self._client.js8call.get_state('dial'), 'OFFSET': offset})
-        self._client.js8call.send(msg)
-        time.sleep(self._client._set_get_delay)
-        return self.get_offset(update = True)
-
-    def get_station_callsign(self, update=False):
-        '''Get JS8Call callsign.
-
-        Args:
-            update (bool): Update if True or use local state if False, defaults to False
-
-        Returns:
-            str: JS8Call configured callsign
-        '''
-        callsign = self._client.js8call.get_state('callsign')
-
-        if update or callsign is None:
-            msg = Message()
-            msg.type = Message.STATION_GET_CALLSIGN
-            self._client.js8call.send(msg)
-            callsign = self._client.js8call.watch('callsign')
-
-        return callsign
-
-    def set_station_callsign(self, callsign):
-        '''Set JS8Call callsign.
-
-        Callsign must be a maximum of 9 characters and contain at least one number.
-
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-
-        Args:
-            callsign (str): Callsign to set
-
-        Returns:
-            str: JS8Call configured callsign
-        '''
-        callsign = callsign.upper()
-
-        if len(callsign) <= 9 and any(char.isdigit() for char in callsign):
-            return self._client.config.set('Configuration', 'MyCall', callsign)
-        else:
-            raise ValueError('callsign must be <= 9 characters in length and contain at least 1 number')
-
-    def get_idle_timeout(self):
-        '''Get JS8Call idle timeout.
-
-        Returns:
-            int: Idle timeout in minutes
-        '''
-        return self._client.config.get('Configuration', 'TxIdleWatchdog', value_type=int)
-
-    def set_idle_timeout(self, timeout):
-        '''Set JS8Call idle timeout.
-
-        If the JS8Call idle timeout is between 1 and 5 minutes, JS8Call will force the idle timeout to 5 minutes on the next application start or exit.
-
-        The maximum idle timeout is 1440 minutes (24 hours).
-
-        Disable the idle timeout by setting it to 0 (zero).
-
-        It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
-
-        Args:
-            timeout (int): Idle timeout in minutes
-
-        Returns:
-            int: Current idle timeout in minutes
-
-        Raises:
-            ValueError: Idle timeout must be between 0 and 1440 minutes
-        '''
-        if timeout < 0 or timeout > 1440:
-            raise ValueError('Idle timeout must be between 0 and 1440 minutes')
-
-        self._client.config.set('Configuration', 'TxIdleWatchdog', timeout)
-        return self.get_idle_timeout()
-
-    def get_distance_units_miles(self):
-        '''Get JS8Call distance unit setting.
-        
-        Returns:
-            bool: True if distance units are set to miles, False if km
-        '''
-        return self._client.config.get('Configuration', 'Miles', bool)
-        
-    def set_distance_units_miles(self, units_miles):
-        '''Set JS8Call distance unit setting.
-        
-        Args:
-            units_miles (bool): Set units to miles if True, set to km if False
-            
-        Returns:
-            bool: True if distance units are set to miles, False if km
-        '''
-        self._client.config.set('Configuration', 'Miles', str(units_miles).lower())
-        return self.get_distance_units_miles()
-        
-    def get_distance_units(self):
-        '''Get JS8Call distance units.
-        
-        Returns:
-            str: Configured distance units: 'mi' or 'km'
-        '''
-        if self.get_distance_units_miles():
-            return 'mi'
-        else:
-            return 'km'
-        
-    def set_distance_units(self, units):
-        ''' Set JS8Call distance units.
-        
-        Args:
-            units (str): Distance units: 'mi', 'miles', 'km', or 'kilometers'
-            
-        Returns:
-            str: Configured distance units: 'miles' or 'km'
-        '''
-        if units.lower() in ['mi', 'miles']:
-            self.set_distance_units_miles(True)
-            return self.get_distance_units()
-        elif units.lower() in ['km', 'kilometers']:
-            self.set_distance_units_miles(False)
-            return self.get_distance_units()
-        else:
-            raise ValueError('Distance units must be: mi, miles, km, or kilometers')
-    
-    def get_station_grid(self, update=False):
-        '''Get JS8Call grid square.
-
-        Args:
-            update (bool): Update if True or use local state if False, defaults to False
-
-        Returns:
-            str: JS8Call configured grid square
-        '''
-        grid = self._client.js8call.get_state('grid')
-
-        if update or grid is None:
-            msg = Message()
-            msg.type = Message.STATION_GET_GRID
-            self._client.js8call.send(msg)
-            grid = self._client.js8call.watch('grid')
-
-        return grid
-
-    def set_station_grid(self, grid):
-        '''Set JS8Call grid square.
-
-        Args:
-            grid (str): Grid square
-
-        Returns:
-            str: JS8Call configured grid square
-        '''
-        grid = grid.upper()
-        msg = Message()
-        msg.type = Message.STATION_SET_GRID
-        msg.value = grid
-        self._client.js8call.send(msg)
-        time.sleep(self._client._set_get_delay)
-        return self.get_station_grid(update = True)
-
-    def get_station_info(self, update=False):
-        '''Get JS8Call station information.
-
-        Args:
-            update (bool): Update if True or use local state if False, defaults to False
-
-        Returns:
-            str: JS8Call configured station information
-        '''
-        info = self._client.js8call.get_state('info')
-
-        if update or info is None:
-            msg = Message()
-            msg.type = Message.STATION_GET_INFO
-            self._client.js8call.send(msg)
-            info = self._client.js8call.watch('info')
-
-        return info
-
-    def set_station_info(self, info):
-        '''Set JS8Call station information.
-
-        Args:
-            info (str): Station information
-
-        Returns:
-            str: JS8Call configured station information
-        '''
-        msg = Message()
-        msg.type = Message.STATION_SET_INFO
-        msg.value = info
-        self._client.js8call.send(msg)
-        time.sleep(self._client._set_get_delay)
-        return self.get_station_info(update = True)
-
-    def append_pyjs8call_to_station_info(self):
-        '''Append pyjs8call info to station info
-
-        A string like ', PYJS8CALL V0.0.0' is appended to the current station info.
-        Example: 'QRPLABS QDX, 40M DIPOLE 33FT, PYJS8CALL V0.2.2'
-
-        If a string like ', PYJS8CALL' or ',PYJS8CALL' is found in the current station info, that substring (and everything after it) is dropped before appending the new pyjs8call info.
-
-        Returns:
-            str: JS8Call configured station information
-        '''
-        info = self.get_station_info().upper()
-        
-        if ', PYJS8CALL' in info:
-            info = info.split(', PYJS8CALL')[0]
-        elif ',PYJS8CALL' in info:
-            info = info.split(',PYJS8CALL')[0]
-            
-        info = '{}, PYJS8CALL {}'.format(info, pyjs8call.__version__)
-        return self.set_station_info(info)
-
-    def get_bandwidth(self, speed=None):
-        '''Get JS8Call signal bandwidth based on modem speed.
-
-        Uses JS8Call configured speed if no speed is given.
-
-        | Speed | Bandwidth |
-        | -------- | -------- |
-        | slow | 25 Hz |
-        | normal | 50 Hz |
-        | fast | 80 Hz |
-        | turbo | 160 Hz |
-        | ultra | 250 Hz |
-
-        Args:
-            speed (str): Speed setting, defaults to None
-
-        Returns:
-            int: Bandwidth of JS8Call signal
-        '''
-        if speed is None:
-            speed = self.get_speed()
-        elif isinstance(speed, int):
-            speed = self.submode_to_speed(speed)
-
-        bandwidths = {'slow':25, 'normal':50, 'fast':80, 'turbo':160, 'ultra':250}
-
-        if speed in bandwidths:
-            return bandwidths[speed]
-        else:
-            raise ValueError('Invalid speed \'' + speed + '\'')
-
-    def get_window_duration(self, speed=None):
-        '''Get JS8Call rx/tx window duration based on modem speed.
-
-        Uses JS8Call configured speed if no speed is given.
-
-        | Speed | Duration |
-        | -------- | -------- |
-        | slow | 30 seconds |
-        | normal | 15 seconds |
-        | fast | 10 seconds |
-        | turbo | 6 seconds |
-        | ultra | 4 seconds |
-
-        Args:
-            speed (str): Speed setting, defaults to None
-
-        Returns:
-            int: Duration of JS8Call rx/tx window in seconds
-        '''
-        if speed is None:
-            speed = self.get_speed()
-        elif isinstance(speed, int):
-            speed = self.submode_to_speed(speed)
-
-        duration = {'slow': 30, 'normal': 15, 'fast': 10, 'turbo': 6, 'ultra':4}
-        return duration[speed]
-
-
-
-class Callbacks:
-    '''Callback functions container.
-    
-    This class is initilized by pyjs8call.client.Client.
-
-    Attributes:
-        incoming (dict): Incoming message callback function lists organized by message type
-        outgoing (func): Outgoing message status change callback function, defaults to None
-        spots (list): New spots callback funtions, defaults to empty list
-        station_spot (list): Watched station spot callback functions, defaults to empty list
-        group_spot (list): Watched group spot callback functions, defaults to empty list
-        window (func): rx/tx window transition callback function, defaults to None
-        inbox (func): New inbox message callback function, defaults to None
-        schedule (func): Schedule entry activation callback function, defaults to None
-
-    *incoming* structure: *{type: [callback, ...], ...}*
-    - *type* is an incoming  message type (see pyjs8call.message for information on message types)
-    - *callback* signature: *func(msg)* where *msg* is a pyjs8call.message object
-
-    *outgoing* callback signature: *func(msg)* where *msg* is a pyjs8call.message object
-    - Called by pyjs8call.txmonitor
-
-    *spots* structure: *[callback, ...]*
-    - callback signature: *func( list(msg, ...) )* where *msg* is a pyjs8call.message object
-    - Called by pyjs8call.spotmonitor
-
-    *station_spot* structure: *[callback, ...]*
-    - callback signature: *func(msg)* where *msg* is a pyjs8call.message object
-    - Called by pyjs8call.spotmonitor
-
-    *group_spot* structure: *[callback, ...]*
-    - callback signature: *func(msg)* where *msg* is a pyjs8call.message object
-    - Called by pyjs8call.spotmonitor
-
-    *window* callback signature: *func()*
-    - Called by pyjs8call.windowmonitor
-
-    *inbox* callback signature: *func(msgs)* where *msgs* is a list of *dict* message items
-    - See *client.get_inbox_messages()* for message item *dict* key details
-    - Called by pyjs8call.inboxmonitor
-
-    *schedule* callback signature: *func(sch)* where *sch* is a pyjs8call.schedule.Schedule object
-    - See *pyjs8call.schedule.Schedule* for object property details
-    - Called by pyjs8call.schedulemonitor
-    '''
-
-    def __init__(self):
-        '''Initialize callback object.
-
-        Returns:
-            pyjs8call.client.Callbacks: Constructed callback object
-        '''
-        self.outgoing = None
-        self.spots = []
-        self.station_spot = []
-        self.group_spot = []
-        self.window = None
-        self.inbox = None
-        self.schedule = None
-        self.incoming = {
-            Message.RX_DIRECTED: [],
-        }
-        self.commands = {}
-
-    def register_incoming(self, callback, message_type=Message.RX_DIRECTED):
-        '''Register incoming message callback function.
-
-        Incoming message callback functions are associated with specific message types. The directed message type is assumed unless otherwise specified. See pyjs8call.message for more information on message types.
-
-        Note that pyjs8call internal modules may register callback functions for specific message type handling. Keep this in mind if minipulating registered callback functions directly.
-
-        Args:
-            callback (func): Callback function object
-            message_type (str): Associated message type, defaults to RX_DIRECTED
-
-        *callback* function signature: *func(msg)* where *msg* is a pyjs8call.message object
-
-        Raises:
-            TypeError: An invaid message type is specified
-        '''
-        if message_type not in Message.RX_TYPES:
-            raise TypeError('Invalid message type \'' + str(message_type) + '\', see pyjs8call.Message.RX_TYPES')
-
-        if message_type not in self.incoming:
-            self.incoming[message_type] = []
-
-        self.incoming[message_type].append(callback)
-
-    def remove_incoming(self, callback, message_type=None):
-        '''Remove incoming message callback function.
-    
-        If *message_type* is None *callback* is removed from all message types.
-
-        Args:
-            callback (func): Function to remove
-            message_type (str): Message type to remove function from, defaults to None
-        '''
-        for msg_type, callbacks in self.incoming.items():
-            if message_type in (None, msg_type) and callback in callbacks:
-                self.incoming[msg_type].remove(callback)
-
-    def incoming_type(self, message_type=Message.RX_DIRECTED):
-        '''Get incoming message callback functions.
-        
-        See pyjs8call.message for more information on message types.
-        
-        Args:
-            message_type (str): Message type, defaults to RX_DIRECTED
-        
-        Returns:
-            list: Callback functions associated with the specified message type
-        '''
-        if message_type in self.incoming:
-            return self.incoming[message_type]
-        else:
-            return []
-
-    def register_command(self, cmd, callback):
-        '''Register command callback function.
-
-        Note: All JS8Call commands must have a leading space. Custom command strings also require a leading space for consistent internal handling.
-
-        Note: Custom commands are only processed for directed messages.
-
-        Args:
-            cmd (str): Command string (with leading space)
-            callback (func): Callback function object
-
-        *callback* function signature: *func(msg)* where *msg* is a pyjs8call.message object
-
-        Raises:
-            ValueError: Specified command string is an exsiting JS8Call command
-            ValueError: Specified command string does not have a leading space
-        '''
-        if cmd in Message.COMMANDS:
-            raise ValueError('\'' + cmd + '\' is an existing JS8Call command')
-
-        if cmd[0] != ' ':
-            raise ValueError('All JS8Call commands must have a leading space')
-
-        if cmd not in self.commands:
-            self.commands[cmd] = []
-
-        self.commands[cmd].append(callback)
-        
-    def remove_command(self, cmd):
-        '''Remove command and callback functions.
-
-        Args:
-            cmd (str): Command to remove
-        '''
-        if cmd in self.commands:
-            del self.commands[cmd]
-
-    def remove_command_callback(self, callback):
-        '''Remove command callback function.
-
-        Args:
-            callback (func): Function to remove
-        '''
-        for cmd, callbacks in self.commands.items():
-            if callback in callbacks:
-                self.commands[cmd].remove(callback)
-
-    def register_spots(self, callback):
-        '''Register spots callback.
-
-        Args:
-            callback (func): Callback function object
-            
-        *callback* function signature: *func(msg)* where *msg* is a pyjs8call.message object
-        '''
-        if callback not in self.spots:
-            self.spots.append(callback)
-
-    def remove_spots(self, callback):
-        '''Remove spots callback.
-
-        Args:
-            callback (func): Callback function object
-        '''
-        if callback in self.spots:
-            del self.spots[callback]
-
-    def register_station_spot(self, callback):
-        '''Register station spot callback.
-
-        Args:
-            callback (func): Callback function object
-            
-        *callback* function signature: *func(msg)* where *msg* is a pyjs8call.message object
-        '''
-        if callback not in self.station_spot:
-            self.station_spot.append(callback)
-
-    def remove_station_spot(self, callback):
-        '''Remove station spot callback.
-
-        Args:
-            callback (func): Callback function object
-        '''
-        if callback in self.station_spot:
-            del self.station_spot[callback]
-
-    def register_group_spot(self, callback):
-        '''Register group spot callback.
-
-        Args:
-            callback (func): Callback function object
-            
-        *callback* function signature: *func(msg)* where *msg* is a pyjs8call.message object
-        '''
-        if callback not in self.group_spot:
-            self.group_spot.append(callback)
-
-    def remove_group_spot(self, callback):
-        '''Remove group spot callback.
-
-        Args:
-            callback (func): Callback function object
-        '''
-        if callback in self.group_spot:
-            del self.group_spot[callback]
```

### Comparing `pyjs8call-0.2.2/pyjs8call/confighandler.py` & `pyjs8call-0.2.3/pyjs8call/confighandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,38 +50,40 @@
 import configparser
 
 # Note: Callsign (Configuration > MyCall) required to contain at least one number and have a max length of 9 characters
 
 class ConfigHandler:
     '''JS8Call.ini configuration file handler.
 
-    Default configuration file path is QT5 *QStandardPaths::ConfigLocation* file path.
+    Default configuration file base path is QT5 *QStandardPaths::ConfigLocation*:
 
     | Platform | Configuration File Path |
     | -------- | -------- |
     | Windows | C:\\Users\\$USERNAME\\AppData\\Local\\JS8Call\\JS8Call.ini |
-    | Mac OS | $HOME/Library/Preferences/JS8Call.ini |
-    | Unix | $HOME/.config/JS8Call.ini |
-
-    Attributes:
-        path (str): File path to the JS8Call config file
-        config (configparser.ConfigParser): Config parser object containing config file data
+    | Mac OS | ~/Library/Preferences/JS8Call.ini |
+    | Unix | ~/.config/JS8Call.ini |
     '''
 
     def __init__(self, config_path=None):
         '''Initialize JS8Call config handler.
 
         Args:
             config_path (str): Alternate config file path, defaults to None
 
         Raises:
             FileNotFoundError: Config file not found at specified path
         '''
         self.file = 'JS8Call.ini'
+        '''str: JS8Call default configuration file name'''
+        self.path = None
+        '''str: JS8Call configuration file path'''
+        self.config = None
+        '''JS8Call configuration container (see python3 configparser for more information)'''
         self.rig = None
+        '''str: Rig name passed to JS8Call at application launch, defaults to None'''
 
         if config_path is not None:
             self.path, self.file = os.path.split(config_path)
         elif psutil.WINDOWS:
             self.path = os.path.expandvars('C:\\Users\\$USERNAME\\AppData\\Local\\JS8Call')
         elif psutil.MACOS:
             self.path = os.path.join(os.path.expanduser('~'), 'Library/Preferences')
@@ -356,15 +358,15 @@
         self.set('MultiSettings', 'CurrentName', new_profile)
 
     def create_new_profile(self, new_profile, copy_profile='Default'):
         '''Create new JS8Call configuration profile.
 
         Args:
             new_profile (str): Name of new profile to create
-            copy_profile (str): Name of an existing profile to copy when creating the new profile
+            copy_profile (str): Name of an existing profile to copy when creating the new profile, defaults to 'Default'
 
         Raises:
             Exception: Specified profile to be copied does not exist
         '''
         if copy_profile not in self.get_profile_list():
             raise Exception('Profile ' + copy_profile + ' cannot be copied because it does not exist')
 
@@ -428,20 +430,19 @@
             group (str): Name of the callsign group to create
         '''
         # strip spaces, ensure a single @ symbol
         group = '@' + group.strip(' @')
 
         if group not in self.get_groups():
             groups = self.config.get('Configuration', 'MyGroups')
-
-            if len(groups.strip()) > 0:
-                groups += ', '
-
+            groups = [g.strip() for g in groups.split(',')]
             # add second @ symbol to match config file formatting
-            groups += '@' + group
+            groups.append('@' + group)
+            groups = ','.join(groups)
+
             self.config.set('Configuration', 'MyGroups', groups)
 
     def remove_group(self, group):
         '''Remove an existing JS8Call callsign group.
 
         Args:
             group (str): Name of the callsign group to remove
```

### Comparing `pyjs8call-0.2.2/pyjs8call/hbnetwork.py` & `pyjs8call-0.2.3/pyjs8call/hbnetwork.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,17 @@
         return self._paused
 
     def enable(self):
         '''Enable heartbeat networking.'''
         if self._enabled:
             return
 
+        # enable js8call heartbeat networking
+        # heartbeat acknowledgements only function if heartbeat networking is enabled
+        self._client.settings.enable_heartbeat_networking()
         self._enabled = True
 
         self._offset = OffsetMonitor(self._client, hb = True)
         self._offset.min_offset = 500
         self._offset.max_offset = 1000
         self._offset.bandwidth_safety_factor = 1.1
         self._offset.activity_cycles = 4
@@ -94,15 +97,17 @@
         thread = threading.Thread(target=self._monitor)
         thread.daemon = True
         thread.start()
 
     def disable(self):
         '''Disable heartbeat networking.'''
         self._enabled = False
-        self._offset.disable()
+        
+        if self._offset is not None:
+            self._offset.disable()
 
     def pause(self):
         '''Pause heartbeat networking.'''
         self._paused = True
 
     def resume(self):
         '''Resume heartbeat networking.'''
```

### Comparing `pyjs8call-0.2.2/pyjs8call/inboxmonitor.py` & `pyjs8call-0.2.3/pyjs8call/inboxmonitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,37 +20,37 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 '''Monitor local and remote inbox messages.
 
 **CAUTION: Enabling inbox monitoring will cause your radio to transmit almost immediately. Consider cabling and antenna connections prior to enabling inbox monitoring.**
 
-Autoreply on at startup must be enabled, and autoreply confirmation must be disabled, in order to allow periodic message queries or automatic responses to *MSG* commands.
+Autoreply (aka autoreply on at startup) must be enabled, and autoreply confirmation must be disabled, in order to allow periodic message queries or automatic responses to *MSG* commands.
 
 Set `client.callback.inbox` to receive new inbox messages as they arrive. See pyjs8call.client.Callbacks for *inbox* callback function details.
 '''
 
 __docformat__ = 'google'
 
 
 import os
 import time
 import json
 import sqlite3
 import threading
+from datetime import datetime, timezone
 
 from pyjs8call import Message
 
 class InboxMonitor:
     '''Monitor local and remote inbox messages.
     
     Note that inbox functions in this class access the JS8Call sqlite3 inbox database directly.
     
     The JS8Call sqlite3 inbox database has the following schema:
-    
     ```
     CREATE TABLE inbox_v1 (
         id INTEGER PRIMARY KEY AUTOINCREMENT,
         blob TEXT
     );
     ```
     '''
@@ -127,15 +127,17 @@
         | Key | Value Type |
         | -------- | -------- |
         | cmd | *str* |
         | freq | *int* | 
         | offset | *int* | 
         | snr | *int* |
         | speed | *int* |
-        | time | *str* |
+        | timestamp | *float* |
+        | utc_time_str | *str* |
+        | local_time_str | *str* |
         | origin | *str* |
         | destination | *str* |
         | path | *str* |
         | text | *str* |
         | type | *str* |
         | value | *str* |
         | status | *str* |
@@ -156,22 +158,26 @@
         conn.close()
 
         if msg is None:
             return None
 
         msg_id, blob = msg
         blob = json.loads(blob)
+        dt_utc = datetime.strptime(blob['params']['UTC'], '%Y-%m-%d %H:%M:%S').replace(tzinfo = timezone.utc)
+
         msg = {
             'id': int(msg_id),
             'cmd' : blob['params']['CMD'],
             'freq' : blob['params']['DIAL'],
             'offset' : blob['params']['OFFSET'],
             'snr' : blob['params']['SNR'],
             'speed' : blob['params']['SUBMODE'],
-            'time' : blob['params']['UTC'],
+            'timestamp' : dt_utc.timestamp(),
+            'utc_time_str' : '{} UTC'.format(dt_utc.strftime('%X')),
+            'local_time_str' : '{}L'.format(dt_utc.astimezone().strftime('%X')),
             'origin' : blob['params']['FROM'],
             'destination' : blob['params']['TO'],
             'path' : blob['params']['PATH'],
             'text' : blob['params']['TEXT'].strip(),
             'value' : blob['value'],
             'status' : blob['type'].lower(),
             'unread': bool(blob['type'].lower() == 'unread'),
@@ -188,15 +194,17 @@
         | Key | Value Type |
         | -------- | -------- |
         | cmd | *str* |
         | freq | *int* | 
         | offset | *int* | 
         | snr | *int* |
         | speed | *int* |
-        | time | *str* |
+        | timestamp | *float* |
+        | utc_time_str | *str* |
+        | local_time_str | *str* |
         | origin | *str* |
         | destination | *str* |
         | path | *str* |
         | text | *str* |
         | type | *str* |
         | value | *str* |
         | status | *str* |
@@ -214,22 +222,26 @@
 
         if len(inbox) == 0:
             return []
 
         msgs = []
         for msg_id, blob in inbox:
             blob = json.loads(blob)
+            dt_utc = datetime.strptime(blob['params']['UTC'], '%Y-%m-%d %H:%M:%S').replace(tzinfo = timezone.utc)
+
             msgs.append({
                 'id': int(msg_id),
                 'cmd' : blob['params']['CMD'],
                 'freq' : blob['params']['DIAL'],
                 'offset' : blob['params']['OFFSET'],
                 'snr' : blob['params']['SNR'],
                 'speed' : blob['params']['SUBMODE'],
-                'time' : blob['params']['UTC'],
+                'timestamp' : dt_utc.timestamp(),
+                'utc_time_str' : '{} UTC'.format(dt_utc.strftime('%X')),
+                'local_time_str' : '{}L'.format(dt_utc.astimezone().strftime('%X')),
                 'origin' : blob['params']['FROM'],
                 'destination' : blob['params']['TO'],
                 'path' : blob['params']['PATH'],
                 'text' : blob['params']['TEXT'].strip(),
                 'value' : blob['value'],
                 'status' : blob['type'].lower(),
                 'unread': bool(blob['type'].lower() == 'unread'),
```

### Comparing `pyjs8call-0.2.2/pyjs8call/js8call.py` & `pyjs8call-0.2.3/pyjs8call/js8call.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,16 +27,18 @@
 
 __docformat__ = 'google'
 
 
 import os
 import time
 import json
+import psutil
 import socket
 import threading
+from datetime import datetime
 
 import pyjs8call
 from pyjs8call import Message
 
 
 class JS8Call:
     '''Low-level JS8Call TCP socket and local state management.
@@ -45,41 +47,35 @@
 
     Initializes pyjs8call.appmonitor as well as rx, tx, logging, application ping, and local state monitoring threads.
 
     Note: *last_band_change* is set to the current time when *pyjs8call* is started.
     
     Attributes:
         app (pyjs8call.appmonitor): Application monitor object
-        connected (bool): Whether the JS8Call TCP socket is connected
-        last_incoming (float): Timestamp of last incoming user message, defaults to 0 (zero)
-        last_outgoing (float): Timestamp of last outgoing user message, defaults to 0 (zero)
-        last_band_change (float): Timestamp of last frequency band change
     '''
 
     def __init__(self, client, host='127.0.0.1', port=2442):
         '''Initialize JS8Call TCP socket and local state.
 
         Args:
             client (pyjs8call.client): Parent client object
             host (str): JS8Call TCP address setting, defaults to '127.0.0.1'
             port (int): JS8Call TCP port setting, defaults to 2442
-
-        Returns:
-            pyjs8call.js8call: Constructed js8call object
         '''
         self._client = client
         self._host = host
         self._port = port
         self._rx_queue = []
         self._rx_queue_lock = threading.Lock()
         self._tx_queue = []
         self._tx_queue_lock = threading.Lock()
         self._socket = None
         self._socket_ping_delay = 60 # seconds
         self.connected = False
+        '''bool: Whether the JS8Call TCP socket is connected'''
 
         self._debug = False
         self._debug_all = False
         self._log = False
         self._log_all = False
         self._log_path = os.path.join(os.path.expanduser('~'), 'pyjs8call.log')
         self._log_queue = ''
@@ -97,16 +93,19 @@
         self._spots = []
         self._recent_spots = []
         self._spots_lock = threading.Lock()
 
         self._last_incoming_by_band = dict()
         self._last_outgoing_by_band = dict()
         self.last_incoming = 0
+        '''float: Timestamp of last incoming user message, defaults to 0 (zero)'''
         self.last_outgoing = 0
+        '''float: Timestamp of last outgoing user message, defaults to 0 (zero)'''
         self.last_band_change = time.time()
+        '''float: Timestamp of last frequency band change'''
         self._last_incoming_api_msg = 0
         
         self._watching = None
         self._watch_timeout = 3 # seconds
 
         # update frequency:
         #   positive value: update every X seconds
@@ -223,31 +222,61 @@
                 'last_update': 0,
                 'last_update_request': 0,
                 'msg_type': Message.RX_GET_SELECTED_CALL
             }
         }
         
         self.app = pyjs8call.AppMonitor(self)
+        '''pyjs8call.appmonitor: Application monitor object'''
 
-    def start(self, headless=False, args = None):
+    def start(self, headless=False, args=None):
         '''Start the JS8Call application.
 
-        This function is blocking until the JS8Call application responds to a network command which ensures that the application is operational before continuing. This handles slower computers such as Raspberry Pi.
+        This function is blocking until the JS8Call application responds to a network command, which ensures that the application is operational before continuing. This supports slower computers such as Raspberry Pi 3 where starting the application may take several seconds.
+
+        The *timer.out* file continues to grow while the application is running, eventually consuming all available disk space and causing application errors. If the *timer.out* file exists, it is removed before starting the application. The *timer.out* file can be removed during extended operation by calling *client.restart()*, which calls this function. The *timer.out* base path is QT5 *QStandardPaths::DataLocation*:
+    
+        | Platform | timer.out File Path |
+        | -------- | -------- |
+        | Windows | C:\\Users\\$USERNAME\\AppData\\Local\\JS8Call\\timer.out |
+        | Mac OS | ~/Library/Application Support/timer.out |
+        | Unix | ~/.local/share/JS8Call/timer.out |
 
-        Used internally by client.start().
+        This function is called internally by client.start().
 
         Args:
             headless (bool): Run JS8Call headless using xvfb (Linux only), defaults to False
             args (list): Command line arguments (see appmonitor.start), defaults to empty list
 
         Raises:
             RuntimeError: JS8Call application failed to start
         '''
         if args is None:
             args = []
+
+        # remove timer.out file when starting, if exists
+        # timer.out file grows continuously until it fills entire disk space and causes an application error
+        # restarting via client.restart() will remove the time.out file
+        # paths based on QT5 writable path QStandardPaths::DataLocation
+        if psutil.WINDOWS:
+            timer_out_path = os.path.expandvars('C:\\Users\\$USERNAME\\AppData\\Local\\JS8Call\\timer.out')
+        elif psutil.MACOS:
+            timer_out_path = os.path.join(os.path.expanduser('~'), 'Library/Application Support/JS8Call/timer.out')
+        else:
+            timer_out_path = os.path.join(os.path.expanduser('~'), '.local/share/JS8Call/timer.out')
+            
+        if os.path.exists(timer_out_path):
+            # allow processes to release file handle on restart
+            timeout = time.time() + 10 # 10 seconds
+            while time.time() < timeout:
+                try:
+                    os.remove(timer_out_path)
+                    break
+                except PermissionError:
+                    time.sleep(0.5)
         
         self.online = True
         self.app.start(headless=headless, args = args)
 
         tx_thread = threading.Thread(target=self._tx)
         tx_thread.daemon = True
         tx_thread.start()
@@ -352,15 +381,15 @@
         
         if log_all:
             self._log_all = True
 
     def process_freq_change(self, previous_freq, current_freq=None):
         '''Manage last incoming/outgoing timestamps on band change.
 
-        This function is called internally when the local frequency state is updated. If a band change has occured, last incoming and outgoing timestamps for the previous band are stored, and last incoming and outgoing timestamps for the current band of loaded (if available).
+        This function is called internally when the local frequency state is updated. If a band change has occured, last incoming and outgoing timestamps for the previous band are stored, and last incoming and outgoing timestamps for the current band are loaded (if available).
 
         Note: Changing from one out-of-band frequency to another out-of-band frequency is not considered a band change.
 
         Args:
             previous_freq (int): Previous frequency in Hz
             current_freq (int): Current frequency in Hz, defaults to current frequency
         '''
@@ -388,14 +417,22 @@
             self.last_incoming = 0
 
         if current_band in self._last_outgoing_by_band:
             self.last_outgoing = self._last_outgoing_by_band[current_band]
         else:
             self.last_outgoing = 0
 
+    def heard_freq_bands(self):
+        '''Get frequency bands with incoming messages.
+
+        Returns:
+            list: Frequency band designators like \'40m\'
+        '''
+        return list(self._last_incoming_by_band.keys())
+
     def activity(self, age=0):
         '''Whether there is outgoing activity.
         
         Args:
             age (int): Maximum age in seconds of outgoing activity to consider active, defaults to 0
 
         Returns:
@@ -595,15 +632,15 @@
 
         Args:
             spots (list): list of spot message objects
             append (bool): append to spot list if True, replace spots if False, defaults to True
         '''
         with self._spots_lock:
             if append:
-                self._spots.append(spots)
+                self._spots.extend(spots)
             else:
                 self._spots = spots
 
     def set_spots_str(self, spots, append=True):
         '''Set spotted message objects from json string.
 
          Used with *get_spots_str* to load previously saved spot messages.
@@ -642,15 +679,16 @@
     def _log_msg(self, msg):
         '''Add message to log queue.'''
         if msg.type in Message.TX_TYPES:
             msg_type = 'TX'
         elif msg.type in Message.RX_TYPES:
             msg_type = 'RX'
 
-        msg_time = time.strftime('%x %X', time.localtime(msg.timestamp))
+        dt_msg = datetime.utcfromtimestamp(msg.timestamp)
+        msg_time = dt_msg.astimezone().strftime('%x %X')
 
         with self._log_queue_lock:
             self._log_queue += msg_time + '  ' + msg_type + '  ' + msg.dump() + '\n'
 
     def _log_monitor(self):
         '''Log queue monitor thread.'''
         while self.online:
```

### Comparing `pyjs8call-0.2.2/pyjs8call/message.py` & `pyjs8call-0.2.3/pyjs8call/message.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,31 +27,41 @@
 
 __docformat__ = 'google'
 
 
 import json
 import time
 import math
+import base64
 import secrets
 from datetime import datetime, timezone
 
 
+BASE64_ALPHABET = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/'
+'''Base64 characters for mapping to JS8Call supported characters'''
+JS8CALL_BASE64_ALPHABET = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ,.-"?!)(~:_&$%#@*><[]{}|;^0123456789+/'
+'''JS8Call supported characters for mapping to Base64 characters'''
+BASE64_TO_JS8CALL_TRANSLATION_TABLE = str.maketrans(BASE64_ALPHABET, JS8CALL_BASE64_ALPHABET)
+'''Translation table from JS8Call supported characters to Base64 characters'''
+JS8CALL_TO_BASE64_TRANSLATION_TABLE = str.maketrans(JS8CALL_BASE64_ALPHABET, BASE64_ALPHABET)
+'''Translation table from Base64 characters to JS8Call supported characters'''
+
 class Message:
     '''Message object for incoming and outgoing messages.
 
     Most attributes with a default value of None are included so messages can be handled internally without worrying about the nuances of JS8Call API message attributes, which vary greatly.
 
     Attributes:
         id (str): Random url-safe text string, 16 bytes in length
         type (str): Message type (see static types), defaults to TX_SEND_MESSAGE
         destination (str): Destination callsign
         value (str): Message contents
-        time (float): UTC timestamp (see *datetime.now(timezone.utc).timestamp*)
-        timestamp (float): Local timestamp (see *time.time*)
-        local_time_str (str): Local time string (see *time.strftime('%X', time.localtime())*)
+        timestamp (float): Epoch timestamp (always referenced to UTC)
+        utc_time_str (float): UTC time string (ex. '21:42 UTC')
+        local_time_str (str): Local time string (ex. '21:42L')
         tdrift (float): Time drift specified by JS8call, defaults to None
         params (dict): Message parameters used by certain JS8Call API messages
         attributes (list): Attributes for internal use (see *Message.set*)
         status (str): Message status (see static statuses), defaults to STATUS_CREATED
         raw (str): Raw message string passed to *Message.parse*, defaults to None
         packed (bytes): Byte string returned from *pack()*, defaults to None
         freq (str): Dial frequency plus offset frequency in Hz, defaults to None
@@ -59,15 +69,15 @@
         offset (str): Passband offset frequency in Hz, defaults to None
         call (str): Callsign, used by certain JS8Call API messages, defaults to None
         grid (str): Grid square, default to None
         path (list): Parsed relay path, defaults to None
         snr (str): Signal-to-noise ratio, defaults to None
         from (str): Origin callsign, defaults to None
         origin (str): Origin callsign, defaults to None
-        utc (str): UTC timestamp, defaults to None
+        utc (str): UTC date/time string, defaults to None
         cmd (str): JS8Call command (see static commands), defaults to None
         text (str): Used by certain JS8Call API messages, defaults to None
         speed (str): JS8Call modem speed of received signal
         extra (str): Used by certain JS8Call API messages, defaults to None
         hearing (list): Response to HEARING? query, defaults to None
         messages (list): Inbox messages, defaults to None
         band_activity (list): JS8Call band activity items, defaults to None
@@ -87,16 +97,16 @@
     RX_GET_BAND_ACTIVITY    = 'RX.GET_BAND_ACTIVITY'
     RX_GET_SELECTED_CALL    = 'RX.GET_CALL_SELECTED'
     TX_SEND_MESSAGE         = 'TX.SEND_MESSAGE'
     TX_GET_TEXT             = 'TX.GET_TEXT'
     TX_SET_TEXT             = 'TX.SET_TEXT'
     MODE_GET_SPEED          = 'MODE.GET_SPEED'
     MODE_SET_SPEED          = 'MODE.SET_SPEED'
-    STATION_GET_INFO        = 'STATION.SET_INFO'
-    STATION_SET_INFO        = 'STATION.GET_INFO'
+    STATION_GET_INFO        = 'STATION.GET_INFO'
+    STATION_SET_INFO        = 'STATION.SET_INFO'
     STATION_GET_GRID        = 'STATION.GET_GRID'
     STATION_SET_GRID        = 'STATION.SET_GRID'
     STATION_GET_CALLSIGN    = 'STATION.GET_CALLSIGN'
     INBOX_GET_MESSAGES      = 'INBOX.GET_MESSAGES'
     INBOX_STORE_MESSAGE     = 'INBOX.STORE_MESSAGE'
     RIG_GET_FREQ            = 'RIG.GET_FREQ'
     RIG_SET_FREQ            = 'RIG.SET_FREQ'
@@ -289,18 +299,21 @@
         Returns:
             pyjs8call.message: Constructed message object
         '''
         self.attributes = []
         '''List of attributes set using Message.set()'''
         self.raw = None
         '''Raw incoming message string, defaults to None, not used for outgoing messages'''
+        self.is_packed = False
+        '''Whether message has been packed, defaults to False, not used for incoming messages'''
         self.packed = None
         '''Packed outgoing message string, defaults to None, not used for incoming messages'''
         self.packed_dict = None
         '''Packed outgoing message dictionary, defaults to None, not used for incoming messages'''
+        self._bytes = None
 
         # initialize common msg fields
         common = [
             'freq',
             'dial',
             'offset',
             'tdrift',
@@ -324,23 +337,25 @@
             'profile',
             'error'
         ]
 
         for attribute in common:
             self.set(attribute, None)
         
+        dt_utc = datetime.now(timezone.utc)
+
         self.set('id', secrets.token_urlsafe(16))
         self.set('type', Message.TX_SEND_MESSAGE)
         self.set('destination', destination)
         self.set('cmd', cmd)
         self.set('value', value)
         self.set('origin', origin)
-        self.set('time', datetime.now(timezone.utc).timestamp())
-        self.set('timestamp', time.time())
-        self.set('local_time_str', '{}L'.format(time.strftime('%X', time.localtime(self.get('timestamp')))))
+        self.set('timestamp', dt_utc.timestamp())
+        self.set('utc_time_str', '{} UTC'.format(dt_utc.strftime('%X')))
+        self.set('local_time_str', '{}L'.format(dt_utc.astimezone().strftime('%X')))
         self.set('params', {})
         self.set('status', Message.STATUS_CREATED)
 
     def set(self, attribute, value):
         '''Set message attribute value.
 
         Uses *setattr* internally to add attributes to the message object. Added attributes are tracked in the *attributes* attribute. Attributes are converted to lowercase for consistency.
@@ -385,15 +400,14 @@
         elif attribute == 'destination' and isinstance(value, list):
             # handle relay
             self.destination = [dest.upper() for dest in value]
             
         elif attribute == 'destination' and isinstance(value, str):
             self.destination = value.upper()
 
-
     def get(self, attribute):
         '''Get message attribute value.
 
         Uses *getattr* internally.
 
         Args:
             attribute (str): Name of attribute to get
@@ -459,47 +473,56 @@
                 data[attribute] = value
 
         return data
 
     def pack(self, exclude=None):
         '''Pack message for transmission over TCP socket.
 
+        If message is already packed, packed value is returned without repacking.
+
         The following attributes are excluded by default:
         - id
         - destination
         - origin
         - cmd
         - from
-        - time
         - timestamp
+        - utc_time_str
+        - local_time_str
         - text
         - status
         - profile
         - error
 
         Args:
             exclude (list): Attribute names to exclude, defaults to None
             
         Returns:
             UTF-8 encoded byte string. A dictionary representation of the message attributes is converted to a string using *json.dumps* before encoding.
         '''
+        if self.is_packed:
+            return self.packed
+            
         if exclude is None:
             exclude = [] 
 
-        exclude.extend(['id', 'destination', 'cmd', 'time', 'timestamp', 'from', 'origin', 'text', 'status', 'profile', 'error'])
+        exclude.extend(['id', 'destination', 'cmd', 'timestamp', 'utc_time_str', 'local_time_str', 'from', 'origin', 'text', 'status', 'profile', 'error'])
 
         self.packed_dict = self.dict(exclude = exclude)
         # convert dict to json string
         packed = json.dumps(self.packed_dict) + '\r\n'
         self.packed = packed.encode('utf-8')
-
+        self.is_packed = True
+        
         return self.packed
 
     def parse(self, msg_str):
         '''Load message string into message object.
+        
+        Supports usage like `Message().parse(raw_incoming_string)`
 
         *Message.parse* should be called inside a try/except block to handle parsing errors.
 
         Args:
             msg_str (str): Received message string to parse
 
         Returns:
@@ -520,30 +543,31 @@
 
             # maintain spaces before commands
             if isinstance(value, str) and param != 'CMD':
                 value = value.strip()
 
             self.set(param, value)
         
-        
         # type handling
         
         if self.type == Message.INBOX_MESSAGES:
             self.messages = []
             
             for message in msg['params']['MESSAGES']:
+                dt_utc = datetime.strptime(message['params']['UTC'], '%Y-%m-%d %H:%M:%S').replace(tzinfo=timezone.utc)
+
                 self.messages.append({
                     'cmd' : message['params']['CMD'],
                     'freq' : message['params']['DIAL'],
                     'offset' : message['params']['OFFSET'],
                     'snr' : message['params']['SNR'],
                     'speed' : message['params']['SUBMODE'],
-                    'time' : message['params']['UTC'] / 1000, # milliseconds to seconds
-                    'timestamp' : time.mktime(time.localtime(value['UTC'] / 1000)), # milliseconds to seconds
-                    'local_time_str' : '{}L'.format(time.strftime('%X', time.localtime(value['UTC'] / 1000))), # milliseconds to seconds
+                    'timestamp' : dt_utc.timestamp(),
+                    'utc_time_str': '{} UTC'.format(dt_utc.strftime('%X')),
+                    'local_time_str' : '{}L'.format(dt_utc.astimezone().strftime('%X')),
                     'origin' : message['params']['FROM'],
                     'destination' : message['params']['TO'],
                     'path' : message['params']['PATH'],
                     'text' : message['params']['TEXT'].strip(),
                     'value' : message['value'],
                     'status' : message['type'].lower(),
                     'unread': bool(message['type'].lower() == 'unread'),
@@ -552,57 +576,59 @@
 
         elif self.type == Message.RX_CALL_ACTIVITY:
             self.call_activity = []
             for key, value in msg['params'].items():
                 if key == '_ID' or value is None:
                     continue
 
+                dt_utc = datetime.utcfromtimestamp(value['UTC'] / 1000) # milliseconds to seconds
+
                 self.call_activity.append({
                     'origin' : key,
                     'grid' : value['GRID'].strip(),
                     'snr' : value['SNR'],
-                    'time' : value['UTC'] / 1000, # milliseconds to seconds
-                    'timestamp' : time.mktime(time.localtime(value['UTC'] / 1000)), # milliseconds to seconds
-                    'local_time_str' : '{}L'.format(time.strftime('%X', time.localtime(value['UTC'] / 1000))) # milliseconds to seconds
+                    'timestamp' : dt_utc.timestamp(),
+                    'utc_time_str' : '{} UTC'.format(dt_utc.strftime('%X')),
+                    'local_time_str' : '{}L'.format(dt_utc.astimezone().strftime('%X'))
                 })
 
         elif self.type == Message.RX_BAND_ACTIVITY:
             self.band_activity = []
             for key, value in msg['params'].items():
                 try:
                     # skip if key is not a freq offset (int)
                     int(key)
 
+                    dt_utc = datetime.utcfromtimestamp(value['UTC'] / 1000) # milliseconds to seconds
+
                     self.band_activity.append({
                         'freq' : value['DIAL'],
                         'offset' : value['OFFSET'],
                         'snr' : value['SNR'],
-                        'time' : value['UTC'] / 1000, # milliseconds to seconds
-                        'timestamp' : time.mktime(time.localtime(value['UTC'] / 1000)), # milliseconds to seconds
-                        'local_time_str' : '{}L'.format(time.strftime('%X', time.localtime(value['UTC'] / 1000))), # milliseconds to seconds
+                        'timestamp' : dt_utc.timestamp(),
+                        'utc_time_str' : '{} UTC'.format(dt_utc.strftime('%X')),
+                        'local_time_str' : '{}L'.format(dt_utc.astimezone().strftime('%X')),
                         'text' : value['TEXT']
                     })
                 except ValueError:
                     continue
 
-                
         # command handling
 
         if self.cmd == Message.CMD_GRID and self.text is not None and Message.ERR not in self.text:
             grid = self.text.split()
             
             if len(grid) >= 4:
                 self.set('grid', grid[3])
                 
         elif self.cmd == Message.CMD_HEARING and self.text is not None and Message.ERR not in self.text:
             # 0 = origin, 1 = destination, 2 = command, -1 = EOM
             hearing = self.text.split()[3:-1]
             self.set('hearing', hearing)
 
-
         # relay path handling
 
         if self.path is not None and Message.CMD_RELAY in self.path and Message.ERR not in self.path:
             self.path = self.path.strip(Message.CMD_RELAY).split(Message.CMD_RELAY)
 
         # allow usage like: msg = Message().parse(rx_str)
         return self
@@ -676,14 +702,87 @@
         Returns:
             pyjs8call.Message: self, for use like `msg = Message().load(str)`
         '''
         for attribute, value in json.loads(msg_str.strip()).items():
             self.set(attribute, value)
 
         return self
+
+    def encode(self):
+        '''Encode incoming JS8Call compatible message value to bytes.
+
+        Due to the limited character set of JS8Call, a unique process is used to re-encode JS8Call compatible text back to bytes. The text to be re-encoded is derived by *Message.decode()*.
+        
+        Custom encoding process: `JS8Call compatible text -> translate to Base64 alphabet -> encode to byte string -> decode Base64 to bytes`
+
+        The *text* attribute is processed to support cleaning of incoming directed message text. If *text* is not set, and *value* is set, *value* is processed instead.
+        
+        Returns:
+            bytes: Message text converted to bytes
+        '''
+        global JS8CALL_TO_BASE64_TRANSLATION_TABLE
+
+        if self.get('text') is not None and len(self.get('text')) > 0:
+            # use msg.text if set
+            msg_value = self.text
+        elif self.get('value') is not None and len(self.get('value')) > 0:
+            # use msg.value if set
+            msg_value = self.value
+        else:
+            # set and return empty bytes string
+            self._bytes = b''
+            return self._bytes
+
+        try:
+            # translate js8call alphabet to base46 alphabet
+            base64_text = msg_value.translate(JS8CALL_TO_BASE64_TRANSLATION_TABLE)
+            # encode to bytes
+            base64_bytes = base64_text.encode()
+            # decode base64 to bytes
+            self._bytes = base64.b64decode(base64_bytes)
+        except Exception as e:
+            self._bytes = b''
+            
+        return self._bytes
+    
+    def decode(self, bytes_str):
+        '''Decode outgoing bytes to JS8Call compatible message value.
+
+        Due to the limited character set of JS8Call, a unique process is used to decode bytes into JS8Call compatible text. The decoded text can be re-encoded using *Message.encode()*.
+        
+        Custom decoding process: `bytes -> encode bytes to Base64 -> decode to string -> translate to JS8Call alphabet -> JS8Call compatible text`
+
+        Supports usage like `Message().decode(byte_string)`.
+
+        Args:
+            bytes_str (bytes): Byte string to decode into JS8Call compatible text
+
+        Returns:
+            pyjs8call.Message: Message object with *value* attribute set to decoded text string
+
+        Raises:
+            TypeError: *bytes_str* is not type bytes
+        '''
+        global BASE64_TO_JS8CALL_TRANSLATION_TABLE
+
+        if not isinstance(bytes_str, bytes):
+            raise TypeError('Only type \'bytes\' can be decoded')
+        
+        try:
+            # convert bytes to base64
+            base64_bytes = base64.b64encode(bytes_str)
+            # decode from bytes
+            base64_text = base64_bytes.decode()
+            # translate base64 alphabet to js8call alphabet
+            msg_value = base64_text.translate(BASE64_TO_JS8CALL_TRANSLATION_TABLE)
+            self.set('value', msg_value)
+        except Exception as e:
+            self.set('value', '')
+            
+        return self
         
     def __eq__(self, msg):
         '''Whether another message is considered equal to self.
 
         There are multiple cases where spots are considered equal:
         - When both incoming messages have the same timestamps (literally the same message)
         - When both incoming messages have the same origin, offset frequency, and snr (same station event reported by differnt JS8Call API messages at slightly different times)
```

### Comparing `pyjs8call-0.2.2/pyjs8call/notifications.py` & `pyjs8call-0.2.3/pyjs8call/notifications.py`

 * *Files 14% similar despite different names*

```diff
@@ -59,26 +59,15 @@
 import smtplib
 import socket
 
 import pyjs8call
 
 
 class Notifications:
-    '''Send email notifiations via SMTP server.
-    
-    Attributes:
-        incoming_enabled (bool): Process incoming directed messages if True, ignore otherwise, defaults to True
-        spots_enabled (bool): Process spots if True, ignore otherwise, defaults to False
-        station_spots_enabled (bool): Process watched station spot if True, ignore otherwise, defaults to False
-        group_spots_enabled (bool): Process watched group spot if True, ignore otherwise, defaults to False
-        notify_on_incoming_if_callsign_selected (bool): Process incoming messages while a callsign is selected on the UI if True, ignore otherwise, defaults to False
-        commands (list): Commands matching incoming *Message.cmd* to notify for, defaults to MSG and freetext
-
-    See pyjs8call.Message for more information on message commands.
-    '''
+    '''Send email notifiations via SMTP server.'''
     def __init__(self, client):
         '''Initialize notifications.
 
         Returns:
             pyjs8call.Notifications: Constructed notifications object
         '''
         self._client = client
@@ -87,20 +76,25 @@
         self._smtp_port = 465
         self._smtp_email = None
         self.__smtp_password = None
         self._email_destination = None
         self._email_subject = None
 
         self.incoming_enabled = True
+        '''bool: Notify on incoming directed messages if True, ignore otherwise, defaults to True'''
         self.spots_enabled = False
+        '''bool: Notify on all spots if True, ignore otherwise, defaults to False'''
         self.station_spots_enabled = False
+        '''bool: Notify on watched station spot (see *pyjs8call.spotmonitor.add_station_watch*) if True, ignore otherwise, defaults to False'''
         self.group_spots_enabled = False
+        '''bool: Notify on watched group spot (see *pyjs8call.spotmonitor.add_group_watch*) if True, ignore otherwise, defaults to False'''
         self.notify_on_incoming_if_callsign_selected = False
-
+        '''bool: Process incoming messages while a callsign is selected on the JC8Call UI if True, ignore otherwise, defaults to False'''
         self.commands = [pyjs8call.Message.CMD_MSG, pyjs8call.Message.CMD_FREETEXT]
+        '''list: *pyjs8call.Message* commands to notify for, defaults to MSG and free text (single space, includes directed messages)'''
 
     def enabled(self):
         '''Get enabled status.
 
         Returns:
             bool: True if enabled, False if disabled
         '''
@@ -124,14 +118,46 @@
         '''Disable automatic email notifiations.'''
         self._enabled = False
         self._client.callback.remove_incoming(self.process_incoming)
         self._client.callback.remove_spots(self.process_spots)
         self._client.callback.remove_station_spot(self.process_station_spots)
         self._client.callback.remove_group_spot(self.process_group_spots)
 
+    def enable_incoming(self):
+        '''Enable incoming directed message handling.'''
+        self.incoming_enabled = True
+
+    def disable_incoming(self):
+        '''Disable incoming directed message handling.'''
+        self.incoming_enabled = False
+
+    def enable_spots(self):
+        '''Enable spot handling.'''
+        self.spots_enabled = True
+
+    def disable_spots(self):
+        '''Disable spot handling.'''
+        self.spots_enabled = False
+
+    def enable_station_spots(self):
+        '''Enable station spot handling.'''
+        self.station_spots_enabled = True
+
+    def disable_station_spots(self):
+        '''Disable station spot handling.'''
+        self.station_spots_enabled = False
+
+    def enable_group_spots(self):
+        '''Enable group spot handling.'''
+        self.group_spots_enabled = True
+
+    def disable_group_spots(self):
+        '''Disable group spot handling.'''
+        self.group_spots_enabled = False
+
     def process_incoming(self, msg):
         '''Process incoming directed messages.
 
         This function is used internally.
         '''
         if not self.incoming_enabled:
             return
@@ -185,14 +211,34 @@
         Args:
             email (str): SMTP server username (email address)
             password (str): SMTP server password
         '''
         self._smtp_email = email
         self.__smtp_password = password
 
+    def set_smtp_email_address(self, email):
+        '''Set SMTP server account email address.
+
+        Note: Credentials are not written to disk and must be set each time *pyjs8call* is started. Credentials are stored in plain text internally in a variable. This variable is destroyed when the program is closed.
+
+        Args:
+            email (str): SMTP server username (email address)
+        '''
+        self._smtp_email = email
+
+    def set_smtp_password(self, password):
+        '''Set SMTP server account password.
+
+        Note: Credentials are not written to disk and must be set each time *pyjs8call* is started. Credentials are stored in plain text internally in a variable. This variable is destroyed when the program is closed.
+
+        Args:
+            password (str): SMTP server password
+        '''
+        self.__smtp_password = password
+
     def set_smtp_server(self, server, port = None):
         '''Set SMTP server domain.
 
         Args:
             server (str): SMTP server domain (ex. smtp.gmail.com)
             port (int): SMTP server port, defaults to 465 (SSL)
         '''
@@ -205,14 +251,22 @@
         '''Set destination email address.
 
         Args:
             email (str): Destination (aka "to") email address
         '''
         self._email_destination = email
 
+    def set_smtp_server_port(self, port):
+        '''Set SMTP server port.
+
+        Args:
+            port (int): SMTP server port
+        '''
+        self._smtp_port = int(port)
+
     def set_email_subject(self, subject):
         '''Set email subject.
 
         Args:
             subject (str): Email subject text
         '''
         self._email_subject = subject
```

### Comparing `pyjs8call-0.2.2/pyjs8call/offsetmonitor.py` & `pyjs8call-0.2.3/pyjs8call/offsetmonitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,38 +34,35 @@
 import random
 import time
 
 from pyjs8call import Message
 
 
 class OffsetMonitor:
-    '''Monitor offset frequency based on activity in the pass band.
-
-    Attributes:
-        min_offset (int): Minimum offset for adjustment and recent activity monitoring, defaults to 1000
-        max_offset (int): Maximum offset for adjustment and recent activity monitoring, defaults to 2500
-        bandwidth_safety_factor (float): Safety factor to apply around outgoing signal bandwith, defaults to 1.25
-        activity_cycles (int, float): rx/tx cycles to consider recent activity, defaults to 2.5
-    '''
+    '''Monitor offset frequency based on activity in the pass band.'''
 
     def __init__(self, client, hb=False):
         '''Initialize offset monitor.
 
         Args:
             client (pyjs8call.client): Parent client object
             hb (bool): Whether offset monitor is for heartbeat monitoring, defaults to False
 
         Returns:
             pyjs8call.offsetmonitor: Constructed offset monitor object
         '''
         self._client = client
         self.min_offset = 1000
+        '''int: Minimum offset for adjustment and recent activity monitoring, defaults to 1000'''
         self.max_offset = 2500
+        '''int: Maximum offset for adjustment and recent activity monitoring, defaults to 2500'''
         self.activity_cycles = 2.5
+        '''int, float: rx/tx cycles to consider recent activity, defaults to 2.5'''
         self.bandwidth_safety_factor = 1.25
+        '''float: Safety factor to apply around outgoing signal bandwith, defaults to 1.25'''
         self._bandwidth = self._client.settings.get_bandwidth()
         self._offset = self._client.settings.get_offset()
         self._enabled = False
         self._paused = False
         self._hb = hb
 
         self._recent_signals = []
```

### Comparing `pyjs8call-0.2.2/pyjs8call/outgoingmonitor.py` & `pyjs8call-0.2.3/pyjs8call/outgoingmonitor.py`

 * *Files identical despite different names*

### Comparing `pyjs8call-0.2.2/pyjs8call/schedulemonitor.py` & `pyjs8call-0.2.3/pyjs8call/schedulemonitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 Set *client.callback.schedule* to receive schedule change activity.
 
 Examples:
     ```
     js8call.schedule.add('18:30') # use current freq, speed, and profile
     js8call.schedule.add('8:00', 7078000, 'normal', 'Field Ops')
     js8call.schedule.remove('18:30')
+    js8call.schedule.add('2:00', restart=True) # restart application daily at 2am
     ```
 '''
 
 __docformat__ = 'google'
 
 
 import time
@@ -48,15 +49,15 @@
 
 
 class ScheduleEntry:
     '''Schedule entry container object.
 
     Do not use this object to create a schedule entry directly. See ScheduleMonitor.add().
 
-    This object is passed to the *client.callback.schedule* callback function when a schedule entry is activated.
+    This object is passed to the *callbacks.Callbacks.schedule* callback function when a schedule entry is activated.
     
     String (str) format:
         {time}L | {state: <8} | {freq_mhz: <11} | {speed: <6} | {profile}
         
         Examples:
             '18:30L | inactive | 7.078 MHz   | normal | Default'
             '10:00L | active   | 14.078 MHz  | fast   | FT857'
@@ -65,76 +66,88 @@
         <ScheduleEntry {time}L : {freq_mhz} : {speed} : {profile}>
         
         Examples:
             '<ScheduleEntry 18:30L : 7.078 MHz : normal : Default>'
             '<ScheduleEntry 10:00L : 14.078 MHz : fast : FT857>'
     '''
 
-    def __init__(self, start, freq, speed, profile):
+    def __init__(self, start, freq, speed, profile, restart):
         '''Initialize schedule entry.
 
         Args:
             start (str): Start time as *datetime.time* object
             freq (int): Dial frequency in Hz
             speed (str): Modem speed ('slow', 'normal', 'fast', 'turbo')
             profile (str): Configuration profile name
+            restart (bool): Whether to forece application restart
 
         Returns:
             pyjs8call.schedulemonitor.ScheduleEntry: Constructed schedule entry
         '''
         self.profile = profile
+        '''str: JS8Call configuration profile to set when activated'''
         self.start = start
+        '''datetime.time: Local start time'''
         self.freq = freq
+        '''int: Frequency in Hz to set when activated'''
         self.speed = speed
+        '''str: JS8Call modem speed to set when activated'''
+        self.restart = restart
+        '''bool: Whether to force a restart of JS8Call when activated'''
         self.active = False
+        '''bool: Whether this schedule entry is currently activated'''
         self.run = False
+        '''bool: Whether this schedule entry has been run today'''
     
     def dict(self):
         '''Get dictionary representation of shedule entry.
         
         Returns:
             Dictionary of schedule entry object with the following keys:
             - start (datetime.time)
-            - time (str): local time in 24-hour format, ex. '18:30'
+            - time (str): Local time in 24-hour format, ex. '18:30'
             - freq (int): Frequency in Hz, ex. 7078000
-            - freq_mhz (str): frequency in MHz with 3 decimal places, ex. '7.078 MHz'
+            - freq_mhz (str): Frequency in MHz with 3 decimal places, ex. '7.078 MHz'
             - speed (str): Modem speed, ('slow', 'normal', 'fast', or 'turbo')
-            - profile (str): configuration profile name, ex. 'Default'
+            - restart (bool): Whether application is forced to restart
+            - profile (str): Configuration profile name, ex. 'Default'
             - active (bool): True if entry is the active schedule, False otherwise
             - state (str): 'active' if self.active is True, 'inactive' otherwise
             - run (bool): True if entry has been run today, False otherwise
         '''
         return {
             'start': self.start,
             'time': self.start.strftime('%H:%M'),
             'freq': self.freq,
             'freq_mhz': '{:.3f} MHz'.format(self.freq / 1000000),
             'speed': self.speed,
+            'restart': self.restart,
             'profile': self.profile,
             'active': self.active,
             'state': 'active' if self.active else 'inactive',
             'run': self.run
         }
 
     def __eq__(self, schedule):
         '''Equality test.'''
         return bool(
             self.profile == schedule.profile and
             self.start == schedule.start and
             self.freq == schedule.freq and
-            self.speed == schedule.speed
+            self.speed == schedule.speed and
+            self.restart == schedule.restart
         )
     
     def __repr__(self):
         '''Get schedule entry object representation.'''
-        return '<ScheduleEntry {0[time]}L : {0[freq_mhz]} : {0[speed]} : {0[profile]}>'.format(self.dict())
+        return '<ScheduleEntry {0[time]}L : {0[freq_mhz]} : {0[speed]} : {0[profile]} : {0[restart]}>'.format(self.dict())
             
     def __str__(self):
         '''Get schedule entry string.'''
-        return '{0[time]}L | {0[state]: <8} | {0[freq_mhz]: <11} | {0[speed]: <6} | {0[profile]}'.format(self.dict())
+        return '{0[time]}L | {0[state]: <8} | {0[freq_mhz]: <11} | {0[speed]: <6} | {0[restart] <5} | {0[profile]}'.format(self.dict())
 
 
 class ScheduleMonitor:
     '''Monitor and activate schedule entries.'''
 
     def __init__(self, client):
         '''Initialize schedule monitor.
@@ -150,15 +163,16 @@
         self._schedule = []
         self._schedule_lock = threading.Lock()
         self._enabled = False
         self._paused = False
 
         config_schedules = self._client.config.get('Configuration', 'pyjs8callSchedule')
 
-        if config_schedules is not None:
+        if config_schedules is not None and config_schedules != 'None':
+            config_schedules = config_schedules.replace('""', '"')
             config_schedules = json.loads(config_schedules)
 
             for schedule in config_schedules:
                 self.add(*schedule)
 
     def enabled(self):
         '''Get enabled status.
@@ -188,15 +202,15 @@
 
         # prevent unnessary restarts on first schedule change
         if self._active_schedule is None:
             profile = self._client.settings.get_profile()
             freq = self._client.settings.get_freq()
             speed = self._client.settings.get_speed()
 
-            self._active_schedule = ScheduleEntry(None, freq, speed, profile)
+            self._active_schedule = ScheduleEntry(None, freq, speed, profile, False)
 
         # prevent running past schedule entries when re-enabled
         with self._schedule_lock:
             self._schedule.sort(key=lambda sch: sch.start)
             now = datetime.datetime.now().time()
             
             for i in range(len(self._schedule)):
@@ -217,60 +231,68 @@
         '''Pause schedule monitoring.'''
         self._paused = True
 
     def resume(self):
         '''Resume schedule monitoring.'''
         self._paused = False
 
-    def add(self, start_time, freq=None, speed=None, profile=None):
+    def add(self, start_time, freq=None, speed=None, profile=None, restart=False):
         '''Add new schedule entry.
 
         Args:
             start_time (str): Local start time in 24-hour format (ex. '18:30')
             freq (int): Dial frequency in Hz, defaults to current frequency
             speed (str): Modem speed ('slow', 'normal', 'fast', 'turbo'), defaults to current speed
             profile (str): Configuration profile name, defaults to the current profile
+            restart (bool): Whether to force an application restart, defaults to False
+
+        Returns:
+            ScheduleEntry: New schedule entry object
         '''
         start_time = datetime.datetime.strptime(start_time, '%H:%M').time()
         now = datetime.datetime.now().time()
 
         if freq is None:
             freq = self._client.settings.get_freq()
 
         if speed is None:
             speed = self._client.settings.get_speed()
 
         if profile is None:
             profile = self._client.settings.get_profile()
 
-        new_schedule = ScheduleEntry(start_time, int(freq), speed, profile)
+        new_schedule = ScheduleEntry(start_time, int(freq), speed, profile, restart)
 
         # avoid running past schedule entry immediately after creation
         if new_schedule.start < now:
             new_schedule.run = True
 
         if new_schedule in self._schedule:
-            return
+            return new_schedule
 
         with self._schedule_lock:
             self._schedule.append(new_schedule)
 
         self._save_to_config()
+        return new_schedule
 
-    def remove(self, start_time=None, profile=None):
+    def remove(self, start_time=None, profile=None, schedule=None):
         '''Remove existing schedule entry.
 
-        If *start_time* is not given, all schedule entries with profile name *profile* are removed.
-
-        if *profile* is not given, all schedule entries with start time *start_time* are removed.
+        If *start_time* is not given, all schedule entries with profile name *profile* are removed. If *profile* is not given, all schedule entries with start time *start_time* are removed. If *schedule* is set to a *schedulemonitor.ScheduleEntry* object, *start_time* and *profile* are set via *schedule*.
 
         Args:
             start_time (str): Local start time in 24-hour format (ex. '18:30'), defaults to None
             profile (str): Configuration profile name, defaults to None
+            schedule (ScheduleEntry): Schedule entry object to source *start_time* and *profile* from, defaults to None
         '''
+        if schedule is not None and isinstance(schedule, ScheduleEntry):
+            start_time = schedule.start.strftime('%H:%M')
+            profile = schedule.profile
+        
         if start_time is not None:
             start_time = datetime.datetime.strptime(start_time, '%H:%M').time()
 
         with self._schedule_lock:
             for schedule in self._schedule.copy():
                 if (
                     (start_time is None and profile == schedule.profile) or
@@ -283,28 +305,28 @@
 
     def get_schedule(self):
         '''Get all schedule entries.
 
         Schedule entries are sorted by start time.
 
         Returns:
-            list: list of Schedule objects (see pyjs8call.schedulemonitor.Schedule)
+            list: list of Schedule objects (see schedulemonitor.Schedule)
         '''
         with self._schedule_lock:
             schedule = self._schedule.copy()
             
         schedule.sort(key=lambda sch: sch.start)
         return schedule
 
     def _save_to_config(self):
         '''Save schedule to configuration file.'''
         with self._schedule_lock:
-            schedule = [ [sch.start.strftime('%H:%M'), sch.freq, sch.speed, sch.profile] for sch in self._schedule]
+            schedule = [ [sch.start.strftime('%H:%M'), sch.freq, sch.speed, sch.profile, sch.restart] for sch in self._schedule]
             
-        schedule = json.dumps(schedule)
+        schedule = json.dumps(schedule).replace('"', '""')
         self._client.config.set('Configuration', 'pyjs8callSchedule', schedule)
 
     def _restart_required(self, schedule_a, schedule_b):
         '''Whether schedule changes require restart.'''
         if schedule_a is None or schedule_b is None:
             return True
         elif schedule_a.profile == schedule_b.profile and schedule_a.speed == schedule_b.speed:
@@ -353,15 +375,15 @@
                         schedule.run = False
 
                     # skip invalid profiles
                     if schedule.profile not in profile_list:
                         continue
 
                     if not schedule.run and not schedule.active and schedule.start < now:
-                        if self._restart_required(schedule, self._active_schedule):
+                        if schedule.restart or self._restart_required(schedule, self._active_schedule):
                             # window duration based on current speed setting
                             window = self._client.settings.get_window_duration()
                             
                             # change config file settings
                             self._client.settings.set_profile(schedule.profile)
                             self._client.settings.set_speed(schedule.speed)
                             # restart when inactive
```

### Comparing `pyjs8call-0.2.2/pyjs8call/spotmonitor.py` & `pyjs8call-0.2.3/pyjs8call/spotmonitor.py`

 * *Files 7% similar despite different names*

```diff
@@ -112,24 +112,24 @@
         Args:
             origin (str): Message origin callsign to match, defaults to None
             destination (str): Message destination callsign or group designator to match, defaults to None
             grid (str): Message grid square to match, defaults to None
             distance (int): Maximum message grid square distance, defaults to 0 (zero)
             age (int): Maximum message age in seconds, defaults to 0 (zero)
             count (int): Number of most recent spot messages to return, defaults to 0 (zero)
-            profile (str): Configuration profile at the time spot was sent or received, defaults to None
+            profile (str): Configuration profile at the time spot was received, defaults to None
             dial_freq (int): Dial frequency in Hz to match, defaults to None
             band (str): Frequency band (ex. \'40m\') to match, defaults to None
 
         Returns:
             list: Spot messages matching specified filter criteria
         '''
         spots = []
         
-        for spot in self._client.js8call.get_spots():
+        for spot in self.all():
             if (
                 (age == 0 or spot.age() <= age) and
                 (grid is None or grid.upper() == spot.grid) and
                 (distance == 0 or (spot.distance is not None and spot.distance <= distance)) and
                 (origin is None or origin.upper() == spot.origin) and 
                 (destination is None or destination.upper() == spot.destination) and
                 (profile is None or profile == spot.profile) and
@@ -140,14 +140,29 @@
 
         if 0 < count < len(spots):
             count *= -1
             spots = spots[count:]
 
         return spots
 
+    def get_origin_grid(self, origin):
+        '''Get grid square for specified origin callsign.
+
+        Args:
+            origin (str): Origin callsign to match
+
+        Returns:
+            str, None: Most recent grid square spotted for *origin*, or None if not found
+        '''
+        for spot in self.all():
+            if spot.origin == origin.upper() and spot.grid not in (None, ''):
+                return spot.grid
+
+        return None
+
     def last_heard(self, count=1):
         '''Get last heard spot messages.
 
         Args:
             count (int): Number of spot messages to return
 
         Returns:
@@ -202,22 +217,45 @@
         '''Get watched stations.
 
         Returns:
             list: Watched station callsigns
         '''
         return self._station_watch_list
 
+    def set_watched_stations(self, stations):
+        '''Set watched stations.
+
+        Args:
+            stations (list): List of station callsigns to watch for
+        '''
+        if isinstance(stations, str):
+            stations = [station.strip() for station in stations.split(',')]
+
+        self._station_watch_list = stations
+
     def get_watched_groups(self):
         '''Get watched groups.
 
         Returns:
             list: Watched group designators
         '''
         return self._group_watch_list
 
+    def set_watched_groups(self, groups):
+        '''Set watched groups.
+
+        Args:
+            groups (list): List of group designators to watch for
+        '''
+        if isinstance(groups, str):
+            groups = [group.strip() for group in groups.split(',')]
+
+        self._groups_watch_list = groups
+
+
     def _callback(self, spots):
         '''New spots callback function handling.
 
         Calls each callback function in *pyjs8call.client.callback.spots*, *pyjs8call.client.callback.station_spot*, and *pyjs8call.client.callback.group_spot* using *threading.Thread*.
 
         Args:
             spots (list): Spotted message objects
```

### Comparing `pyjs8call-0.2.2/pyjs8call/timemonitor.py` & `pyjs8call-0.2.3/pyjs8call/timemonitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 
 from pyjs8call import Message
 
 
 class DriftMonitor:
     '''Monitor time drift.
 
+    Add the @TIME group to the stations configuration to participate in the time group.
+
     Note that the JS8Call API does not support changing the time drift. The application will be restarted to apply new time drift settings via the configuration file.
 
     Note that only JS8Call rx/tx window timing relative to other stations is effected. Clock time is not effected.
         
     There are 3 sources of time drift information:
     - recently heard stations in a group (ex. @TIME)
     - a single station
```

### Comparing `pyjs8call-0.2.2/pyjs8call/windowmonitor.py` & `pyjs8call-0.2.3/pyjs8call/windowmonitor.py`

 * *Files identical despite different names*

### Comparing `pyjs8call-0.2.2/pyjs8call.egg-info/PKG-INFO` & `pyjs8call-0.2.3/pyjs8call.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pyjs8call
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python package for interfacing with the JS8Call API
 Home-page: https://github.com/simplyequipped/pyjs8call
 Author: Simply Equipped LLC
 Author-email: howard@simplyequipped.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: psutil>=5.3
 
 [![pypi version](https://img.shields.io/pypi/v/pyjs8call?color=blue&label=pypi%20version)](https://pypi.org/project/pyjs8call) &nbsp;&nbsp;&nbsp;
 [![pypi downloads](https://img.shields.io/pypi/dw/pyjs8call?color=blue&label=pypi%20downloads)](https://pypi.org/project/pyjs8call) &nbsp;&nbsp;&nbsp;
 [![github license](https://img.shields.io/github/license/simplyequipped/pyjs8call?color=blue)](https://github.com/simplyequipped/pyjs8call/blob/main/LICENSE)
 
 A Python package for interfacing with the JS8Call API.
 
@@ -60,56 +61,57 @@
 
 ### Installation
 
 1. Install applications
     
     a. Install JS8Call
     
-    See the [JS8Call downloads](http://files.js8call.com/latest.html) page for OS-specific packages as well as source files. If you are compiling from source for Linux be sure to read the INSTALL file at the top level of the JS8Call repo.
-    
-    On Raspberry Pi OS:
+    On some platforms, such as Raspberry Pi OS, JS8Call can be installed with the package manager:
     ```
-    wget http://files.js8call.com/2.2.0/js8call_2.2.0_armhf.deb
-    sudo dpkg -i js8call_2.2.0_armhf.deb
+    sudo apt install js8call
     ```
 
+    Otherwise, see the [JS8Call downloads](http://files.JS8Call.com/latest.html) page for OS-specific packages as well as source files. If you are compiling from source for Linux be sure to read the INSTALL file at the top level of the JS8Call repo.
+
     **NOTE:** When installing JS8Call on Windows be sure to select the option to add JS8Call to the PATH variable during the installation process. This will allow *pyjs8call* to locate the JS8Call executable.
 
-    **NOTE:** When installing JS8Call on MacOS be sure to read the readme file included in the dmg image for information on the fix for the JS8Call shared memory error. The following directory must also be added to the PATH variable to allow *pyjs8call* to locate the JS8Call executable: /Applications/js8call.app/Contents/MacOS
+    **NOTE:** When installing JS8Call on MacOS be sure to read the readme file included in the dmg image for information on the fix for the JS8Call shared memory error. The following directory must also be added to the PATH variable to allow *pyjs8call* to locate the JS8Call executable: `/Applications/js8call.app/Contents/MacOS`
     
-    **NOTE:** When using a QRPLabs QDX tranceiver on Linux consider masking the ModemManager service to prevent CAT control dropouts. See [this post from QRPLabs](https://groups.io/g/QRPLabs/topic/87048220#74634) for more information.
-    
-    &nbsp;
+    **NOTE:** When using a QRPLabs QDX tranceiver on Linux, consider masking the ModemManager service using the below commands to prevent CAT control dropouts (aka rig control errors). See [this post from QRPLabs](https://groups.io/g/QRPLabs/topic/87048220#74634) for more information.
+    ```
+    sudo systemctl stop ModemManager.service
+    sudo systemctl mask ModemManager.service
+    ```
 
     b. Install xvfb if running headless (not supported on Windows or MacOS)
     
     On Debian systems:
     ```
     sudo apt install xvfb
     ```
 
-2. Install pyjs8call using pip3 (or pip, if python3 is the default on your system)
+2. Install pyjs8call using pip (or pip3, if python3 is not the default on your system)
     
     ```
-    pip3 install pyjs8call
+    pip install pyjs8call
     ```
 
     This will also install *psutil* for cross platform process management.
 
-3. Launch JS8Call to configure audio and CAT interface settings as needed. Launching the application and exiting normally will also initilize the configuration file, which is required by *pyjs8call*.
+3. Launch JS8Call to configure audio and CAT interface settings as needed. Launching the application and exiting normally will also initialize the configuration file, which is required by *pyjs8call*.
 
 &nbsp;
 
 ### Modules
 
 Some setup (i.e. setting callback functions) is required to use certain module features. Most modules are initialized automatically by pyjs8call.client.
 
 **Client** (pyjs8call.client)
 
-The main JS8Call API interface. Includes many functions for reading and writting settings as well as sending various types of messages.
+The main JS8Call API interface. Includes functions for sending various types of messages.
 
 **JS8Call** (pyjs8call.js8call)
 
 Manages TCP socket communication with the JS8Call application.
 
 **Application Monitor** (pyjs8call.appmonitor)
 
@@ -117,53 +119,105 @@
 
 **Configuration Handler** (pyjs8call.confighandler)
 
 Reads from and writes to the JS8Call.ini config file to change virtually any setting, including creating and activating configuration profiles. **Specific knowledge of configuration file options is required. Configuring options incorrectly may cause the JS8Call application to not run.**
 
 **Spot Monitor** (pyjs8call.spotmonitor)
 
-Monitors recent station spots. Spot data can be queried for various uses, and spot callbacks can be set for all heard stations and/or for specific stations.
+Monitors recent station spots. Spot data can be queried for various uses, and spot callbacks can be set for all heard stations and/or for specific stations and groups.
 
 **Window Monitor** (pyjs8call.windowmonitor)
 
 Monitors the next rx/tx window transition. JS8Call API messages associated with incoming and outgoing messages are used to determine the start or end of a window, and the modem speed setting is used to determine the duration of the window. Notification of a window transition is handled via callback function.
 
 **Offset Monitor** (pyjs8call.offsetmonitor)
 
-Manages JS8Call offset frequency based on activity in the pass band. The offset frequency is automatically moved to an unsed portion of the pass band if a recently heard signal overlaps with the current offset. Signal bandwidth is calculated based on the modem speed of each heard signal. Only decoded signal data is available from the JS8Call API so other QRM cannot be handled.
+Manages JS8Call offset frequency based on activity in the pass band. The offset frequency is automatically moved to an unused portion of the pass band if a recently heard signal overlaps with the current offset. Signal bandwidth is calculated based on the modem speed of each heard signal. Only decoded signal data is available from the JS8Call API so other QRM cannot be handled.
 
 **Outgoing Monitor** (pyjs8call.outgoingmonitor)
 
 Monitors JS8Call outgoing message text. Notification of a message status change is handled via callback function.
 
 **Heartbeat Networking** (pyjs8call.hbnetwork)
 
-Sends a heartbeat message in the heartbeat sub-band on a time interval.
+Sends a heartbeat message in the heartbeat sub-band on a time interval. This module is useful for enabling heatbeat networking programmatically and without using the JS8Call interface (i.e. running headless).
 
 **Time Monitor** (pyjs8call.timemonitor)
 
 Monitors a group, station, or all activity for time drift data and synchronizes local time drift. Enable automatic synchronization to the specified source on a time interval. Synchronizes to the @TIME group by default.
 
 Time master functionality is also implemented which sends outgoing messages on a time interval that other stations can use to synchronize their time drift. Targets the @TIME group by default.
 
 **Inbox Monitor** (pyjs8call.inboxmonitor)
 
 Monitors the local inbox. Notification of new messages is handled via callback function.
 
+Automatic periodic syncing of remote messages from a specified source (@ALLCALL by default) is also supported. Be aware of your local laws regarding unattended stations when using this feature.
+
+*NOTE: enabling syncing of remote messages will cause the local station to transmit immediately*
+
 **Schedule Monitor** (pyjs8call.schedulemonitor)
 
-Monitors configured schedule entries and applies the necessary setting changes at the scheduled time. Settings that can be changed on a schedule include frequency, modem speed, and configuration profile.
+Monitors configured schedule entries and applies the necessary setting changes at the scheduled time. Settings that can be changed on a schedule include frequency, modem speed, and configuration profile. The JS8Call application can also be restarted on a schedule.
 
 **Propagation** (pyjs8call.propagation)
-Parses stored spots into datasets of individual or median SNR values for grid squares or callsigns. This information can be used to infer general propagation conditions between the local station and a specific station, or the local station and a specific grid square.
+
+Parses stored spot data into datasets of individual or median SNR values for grid squares or callsigns. This information can be used to infer general propagation conditions between the local station and a specific station, or the local station and a specific grid square.
 
 **Notifications** (pyjs8call.notifications)
-Send an email message (including email-to-text) via an existing SMTP server when a message directed to the local station is received.
 
-&nbsp;  
+Send an email message (including email-to-text) via a specified SMTP server when a message directed to the local station is received, or when a specific station or group is spotted.
+
+&nbsp;
+
+### Command Line Interface (CLI)
+
+A command line interface is available for the *pyjs8call* module as of version 0.2.3. CLI usage:
+
+```
+USAGE: python -m pyjs8call [OPTIONS]
+
+OPTIONS:
+--rns
+    Utilize IO buffers to support the RNS PipeInterface, set configuration profile
+    to 'RNS', allow free text, and add group @RNS (*)
+--freq
+    Set radio frequency in Hz
+--grid
+    Set station grid square
+--speed
+    Set speed of JS8Call modem, defaults to 'fast'
+--profile
+    Set JS8Call configuration profile (**)
+--callsign
+    Set station callsign
+--settings
+    File path to pyjs8call settings file (NOT JS8CALL CONFIG FILE),
+    see pyjs8call.settings.Settings.load
+    for more information
+--headless
+    Run JS8Call headless using xvfb (only available on Linux platforms)
+--heartbeat
+    Enable pyjs8call heartbeat networking
+
+
+(*) RNS PipeInterface must be configured and enabled in the Reticulum config file,
+    see below example:
+
+    [[Pipe Interface]]
+    type = PipeInterface
+    interface_enabled = True
+    command = python -m pyjs8call --rns --settings ~/.config/pyjs8call_rns.ini
+    respawn_delay = 5
+
+(**) If the specified profile does not exist, it is created by copying 'Default'
+```
+See [RNS PipeInterface](https://markqvist.github.io/Reticulum/manual/interfaces.html#pipe-interface) for more information on configuring a RNS PipeInterface.
+
+&nbsp;
 
 ### Examples
 
 Basic usage:
 ```
 import pyjs8call
 
@@ -204,15 +258,15 @@
 # (or miles, depending on JS8Call settings)
 js8call.spots.filter(distance = 1000)
 
 # get a list of spot messages in the last 15 minutes
 max_age = 15 * 60 # convert minutes to seconds
 js8call.spots.filter(age = max_age)
 
-# get a list of the 10 most recent spot messages from regional stations in the last hour on the 40m band
+# get a list of the 10 most recent spot messages from regional stations on the 40m band
 js8call.spots.filter(distance = 500, band = '40m', count = 10)
 ```
 
 Run multiple JS8Call instances:
 ```
 import pyjs8call
 
@@ -225,14 +279,15 @@
 #js8call_ft857.start(args=['--rig-name', 'FT857'])
 
 # specify a different network port for the secondary instance
 js8call_qdx = pyjs8call.Client(port=2444)
 # specify the rig name as a command line argument
 js8call_qdx.start(args=['--rig-name', 'QDX'])
 ```
+**Note:** radio interface and audio devices should be configured manually in each JS8Call instance
 
 Using the spot monitor:
 ```
 import pyjs8call
 
 # callback function for all new spots
 def new_spots(spots):
@@ -277,16 +332,24 @@
         print('New inbox message from ' + msg['origin'])
 
 js8call = pyjs8call.Client()
 # set inbox monitor callback
 js8call.callback.inbox = new_inbox_msg
 js8call.start()
 
-# enable local inbox monitoring and periodic remote inbox message query
+# enable local inbox monitoring
 js8call.inbox.enable()
+
+# enable local inbox monitoring and periodic remote inbox message query
+# to @ALLCALL every 60 minutes
+js8call.inbox.enable(query=True)
+
+# enable local inbox monitoring and periodic remote inbox message query
+# to @MYGROUP every 30 minutes
+js8call.inbox.enable(query=True, destination='@MYGROUP', interval=30)
 ```
 
 Using the outgoing message monitor:
 ```
 import pyjs8call
 
 # callback function for message status change
@@ -308,14 +371,16 @@
 ```
 
 Using heartbeat networking:
 ```
 import pyjs8call
 
 js8call = pyjs8call.Client()
+# set heartbeat interval via config file
+js8call.settings.set_heartbeat_interval(15)
 js8call.start()
 
 # interval based on JS8Call settings
 js8call.heartbeat.enable()
 ```
 
 Using the schedule monitor:
@@ -348,14 +413,15 @@
 Set config file settings:
 ```
 import pyjs8call
 
 js8call = pyjs8call.Client()
 
 # set config file settings before starting
+# see pyjs8call.settings for many more settings options
 js8call.settings.enable_heartbeat_acknowledgements()
 js8call.settings.set_heartbeat_interval(15)
 js8call.settings.enable_reporting()
 js8call.settings.set_speed('normal')
 
 js8call.start()
 ```
@@ -369,16 +435,16 @@
 
 # use built-in spot distance filter
 regional_stations = [spot.origin for spot in js8call.spots.filter(distance = 500)]
 for station in regional_stations:
     print('{}: {} {} at {}\N{DEGREE SIGN}'.format(station.origin, station.distance, station.distance_units, station.bearing))
 
 # access message attributes directly
-# this requires the message to contain grid square data
-last_heartbeat = js8call.spots.filter(destination='@HB')[-1]
+# this requires the message to contain grid square data (ex. heartbeat message)
+last_heartbeat = js8call.spots.filter(destination='@HB', count=1)[-1]
 distance = last_heartbeat.distance
 bearing = last_heartbeat.bearing
 
 # manually calculate distance and bearing from local station
 distance, distance_units, bearing = js8call.grid_distance('FM16')
 
 # manually calculate distance and bearing between grid squares
@@ -450,14 +516,23 @@
 # set SMTP server credentials
 js8call.notifications.set_smtp_credentials('email.address@gmail.com', 'app_password')
 # set destination email address to a Verzion mobile number
 js8call.notifications.set_email_destination('2018675309@vtext.com')
 # enable automatic notifications for incoming directed messages
 js8call.notifications.enable()
 
+# set stations to watch
+js8call.spots.add_station_watch('KT7RUN')
+# enable station spot notifications
+js8call.notifications.enable_station_spots()
+
+# set groups to watch
+js8call.spots.add_group_watch('@TTP')
+# enable station spot notifications
+js8call.notifications.enable_group_spots()
 ```
 
 &nbsp;
 
 ### Acknowledgements
 
 Inspired by [js8net](https://github.com/jfrancis42/js8net) by N0GQ<br>
```

### Comparing `pyjs8call-0.2.2/pyjs8call.egg-info/SOURCES.txt` & `pyjs8call-0.2.3/pyjs8call.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 LICENSE
 README.md
 setup.py
 pyjs8call/__init__.py
+pyjs8call/__main__.py
 pyjs8call/appmonitor.py
+pyjs8call/callbacks.py
 pyjs8call/client.py
 pyjs8call/confighandler.py
 pyjs8call/hbnetwork.py
 pyjs8call/inboxmonitor.py
 pyjs8call/js8call.py
 pyjs8call/message.py
 pyjs8call/notifications.py
 pyjs8call/offsetmonitor.py
 pyjs8call/outgoingmonitor.py
 pyjs8call/propagation.py
 pyjs8call/schedulemonitor.py
+pyjs8call/settings.py
 pyjs8call/spotmonitor.py
 pyjs8call/timemonitor.py
 pyjs8call/windowmonitor.py
 pyjs8call.egg-info/PKG-INFO
 pyjs8call.egg-info/SOURCES.txt
 pyjs8call.egg-info/dependency_links.txt
 pyjs8call.egg-info/requires.txt
```

### Comparing `pyjs8call-0.2.2/setup.py` & `pyjs8call-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyjs8call',
-    version='0.2.2',
+    version='0.2.3',
     author='Simply Equipped LLC',
     author_email='howard@simplyequipped.com',
     description='Python package for interfacing with the JS8Call API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/simplyequipped/pyjs8call',
     packages=setuptools.find_packages(),
```

### Comparing `pyjs8call-0.2.2/tests/test_cross_platform.py` & `pyjs8call-0.2.3/tests/test_cross_platform.py`

 * *Files identical despite different names*

### Comparing `pyjs8call-0.2.2/tests/test_helpers.py` & `pyjs8call-0.2.3/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pyjs8call-0.2.2/tests/test_start.py` & `pyjs8call-0.2.3/tests/test_start.py`

 * *Files identical despite different names*

