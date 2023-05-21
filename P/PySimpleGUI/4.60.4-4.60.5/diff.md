# Comparing `tmp/PySimpleGUI-4.60.4.tar.gz` & `tmp/PySimpleGUI-4.60.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySimpleGUI-4.60.4.tar", last modified: Mon Oct 10 23:12:28 2022, max compression
+gzip compressed data, was "dist\PySimpleGUI-4.60.5.tar", last modified: Sun May 21 23:31:07 2023, max compression
```

## Comparing `PySimpleGUI-4.60.4.tar` & `PySimpleGUI-4.60.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2022-10-10 23:12:28.000000 PySimpleGUI-4.60.4/
--rw-rw-rw-   0        0        0    63997 2022-10-10 23:12:28.000000 PySimpleGUI-4.60.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-10-10 23:12:28.000000 PySimpleGUI-4.60.4/PySimpleGUI/
--rw-rw-rw-   0        0        0  1777503 2022-10-10 23:11:49.000000 PySimpleGUI-4.60.4/PySimpleGUI/PySimpleGUI.py
--rw-rw-rw-   0        0        0       88 2021-10-16 15:47:23.000000 PySimpleGUI-4.60.4/PySimpleGUI/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-10 23:12:28.000000 PySimpleGUI-4.60.4/PySimpleGUI.egg-info/
--rw-rw-rw-   0        0        0        1 2022-10-10 23:12:28.000000 PySimpleGUI-4.60.4/PySimpleGUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      355 2022-10-10 23:12:28.000000 PySimpleGUI-4.60.4/PySimpleGUI.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0    63997 2022-10-10 23:12:28.000000 PySimpleGUI-4.60.4/PySimpleGUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2022-10-10 23:12:28.000000 PySimpleGUI-4.60.4/PySimpleGUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       12 2022-10-10 23:12:28.000000 PySimpleGUI-4.60.4/PySimpleGUI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-10 23:12:28.000000 PySimpleGUI-4.60.4/setup.cfg
--rw-rw-rw-   0        0        0     2281 2022-10-10 23:12:06.000000 PySimpleGUI-4.60.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 23:31:07.000000 PySimpleGUI-4.60.5/
+-rw-rw-rw-   0        0        0    64049 2023-05-21 23:31:07.000000 PySimpleGUI-4.60.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-21 23:31:07.000000 PySimpleGUI-4.60.5/PySimpleGUI/
+-rw-rw-rw-   0        0        0  1788343 2023-05-21 16:08:27.000000 PySimpleGUI-4.60.5/PySimpleGUI/PySimpleGUI.py
+-rw-rw-rw-   0        0        0       88 2021-10-16 15:47:23.000000 PySimpleGUI-4.60.5/PySimpleGUI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 23:31:07.000000 PySimpleGUI-4.60.5/PySimpleGUI.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-21 23:31:07.000000 PySimpleGUI-4.60.5/PySimpleGUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      355 2023-05-21 23:31:07.000000 PySimpleGUI-4.60.5/PySimpleGUI.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0    64049 2023-05-21 23:31:07.000000 PySimpleGUI-4.60.5/PySimpleGUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-05-21 23:31:07.000000 PySimpleGUI-4.60.5/PySimpleGUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       12 2023-05-21 23:31:07.000000 PySimpleGUI-4.60.5/PySimpleGUI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 23:31:07.000000 PySimpleGUI-4.60.5/setup.cfg
+-rw-rw-rw-   0        0        0     2332 2023-05-21 15:58:04.000000 PySimpleGUI-4.60.5/setup.py
```

### Comparing `PySimpleGUI-4.60.4/PKG-INFO` & `PySimpleGUI-4.60.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySimpleGUI
-Version: 4.60.4
+Version: 4.60.5
 Summary: Python GUIs for Humans. Launched in 2018. It's 2022 & PySimpleGUI is an ACTIVE & supported project. Super-simple to create custom GUI's. 325+ Demo programs & Cookbook for rapid start. Extensive documentation. Main docs at www.PySimpleGUI.org. Fun & your success are the focus. Examples using Machine Learning (GUI, OpenCV Integration), Rainmeter Style Desktop Widgets, Matplotlib + Pyplot, PIL support, add GUI to command line scripts, PDF & Image Viewers. Great for beginners & advanced GUI programmers.
 Home-page: https://github.com/PySimpleGUI/PySimpleGUI
 Author: PySimpleGUI
 Author-email: PySimpleGUI@PySimpleGUI.org
 License: UNKNOWN
 Description: 
         <p align="center">
@@ -14,16 +14,16 @@
         
         <table>
           <tr>
             <td>
               <img src="https://www.dropbox.com/s/6wzf3ebmj97v4zs/PySimpleGUI-GitHub-Udemy-Course.png?raw=1" width=200 alt="PySimpleGUI Udemy Course">
             </td>
             <td>
-              <h5>apply coupon for discount:<br>4FD91A459D56B1029FF8</h6>
-              <a href="https://www.udemy.com/course/pysimplegui/?couponCode=4FD91A459D56B1029FF8">click here to visit course page</a>
+              <h5>apply coupon for discount:<br>9AF99B123C49D51EB547</h6>
+              <a href="https://www.udemy.com/course/pysimplegui/?couponCode=9AF99B123C49D51EB547">click here to visit course page</a>
             </td>
           </tr>
         </table>
         
         Transforms the tkinter, Qt, WxPython, and Remi (browser-based) GUI frameworks into a simpler interface.  The window definition is simplified by using Python core data types understood by beginners (lists and dictionaries). Further simplification happens by changing event handling from a callback-based model to a message passing one.  
         
         Your code is not _required_ to have an object oriented architecture which makes the package usable by a larger audience. While the architecture is simple to understand, it does not *necessarily* limit you to only simple problems.  
@@ -895,11 +895,12 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_ye4rarhr_/tmps1e2v_mm_TarContainer/0/1", line 22, column 16: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_ye4rarhr_/tmps1e2v_mm_TarContainer/0/1", line 22, column 16: Levels of opening and closing headings don't match*

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: PySimpleGUI Version: 4.60.4 Summary: Python GUIs
+Metadata-Version: 2.1 Name: PySimpleGUI Version: 4.60.5 Summary: Python GUIs
 for Humans. Launched in 2018. It's 2022 & PySimpleGUI is an ACTIVE & supported
 project. Super-simple to create custom GUI's. 325+ Demo programs & Cookbook for
 rapid start. Extensive documentation. Main docs at www.PySimpleGUI.org. Fun &
 your success are the focus. Examples using Machine Learning (GUI, OpenCV
 Integration), Rainmeter Style Desktop Widgets, Matplotlib + Pyplot, PIL
 support, add GUI to command line scripts, PDF & Image Viewers. Great for
 beginners & advanced GUI programmers. Home-page: https://github.com/
 PySimpleGUI/PySimpleGUI Author: PySimpleGUI Author-email:
 PySimpleGUI@PySimpleGUI.org License: UNKNOWN Description:
                            [Python GUIs for Humans]
                       ***** Python GUIs for Humans *****
                            ** apply coupon for discount:
-[PySimpleGUI Udemy Course] 4FD91A459D56B1029FF8 **
+[PySimpleGUI Udemy Course] 9AF99B123C49D51EB547 **
                            click_here_to_visit_course_page
 Transforms the tkinter, Qt, WxPython, and Remi (browser-based) GUI frameworks
 into a simpler interface. The window definition is simplified by using Python
 core data types understood by beginners (lists and dictionaries). Further
 simplification happens by changing event handling from a callback-based model
 to a message passing one. Your code is not _required_ to have an object
 oriented architecture which makes the package usable by a larger audience.
@@ -752,11 +752,11 @@
 WxPython Remi wrapper simple easy beginner novice student graphics progressbar
 progressmeter Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4 Classifier: Programming
 Language :: Python :: 3.5 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: License :: OSI Approved :: GNU Lesser
-General Public License v3 or later (LGPLv3+) Classifier: Topic :: Multimedia ::
-Graphics Classifier: Operating System :: OS Independent Description-Content-
-Type: text/markdown
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or
+later (LGPLv3+) Classifier: Topic :: Multimedia :: Graphics Classifier:
+Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `PySimpleGUI-4.60.4/PySimpleGUI/PySimpleGUI.py` & `PySimpleGUI-4.60.5/PySimpleGUI/PySimpleGUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 #!/usr/bin/python3
 
-version = __version__ = "4.60.4 Released 10-Oct-2022"
+version = __version__ = "4.60.5 Released 21-May-2023"
 
 _change_log = """
     Changelog since 4.60.0 released to PyPI on 8-May-2022.  These are "Dot" releases....
 
     4.60.1
         A "dot-release" / patch for crash that occurs if the horizontal_scroll parm is set in Listbox element
             Was created when the ttk scrollbars were added
     4.60.2
         A "dot-release" for Mac 12.3+ "Invisible window" problem. Adds option in Mac control panel to set Alpha to 0.99 as default
     4.60.3
         Another shot at the 12.3+ Mac OS problem.  Had bug in the version check code
     4.60.4
         Dot release to quickly fix the Trinket detection which stopped working recently
+    4.60.5
+        Fix for the Mac.  If running MacOS Ventura 13.2.1 then windows with no titlebar had problems with Input elements. Added support for the Upgrade Service.
+        Change to the 0.99 Alpha patch.  ONLY apply to tkinter version 8.6.12. This will automatically turn it off for 8.6.13+, even if previously enabled
+        Updated GitHub Issue post GUI.  Changed hostname in SDK help window to use PySimpleGUI.org rather than readthedocs.
     """
 
 __version__ = version.split()[0]  # For PEP 396 and PEP 345
 
 # The shortened version of version
 try:
     ver = version.split(' ')[0]
@@ -33,15 +37,15 @@
 # 8eeee8 8    8 8eeeee 8  8  8  8 8   8 8     8    8e     8e  8 8e
 # 88     8eeee8     88 8e 8e 8  8 8eee8 8e    8eee 88  ee 88  8 88
 # 88       88   e   88 88 88 8  8 88    88    88   88   8 88  8 88
 # 88       88   8eee88 88 88 8  8 88    88eee 88ee 88eee8 88ee8 88
 
 
 """
-    Copyright 2018, 2019, 2020, 2021, 2022 PySimpleGUI(tm)
+    Copyright 2018, 2019, 2020, 2021, 2022, 2023 PySimpleGUI(tm)
 
     Before getting into the details, let's talk about the high level goals of the PySimpleGUI project.
 
     From the inception these have been the project principals upon which it is all built
     1. Fun - it's a serious goal of the project. If we're not having FUN while making stuff, then something's not right
     2. Successful - you need to be successful or it's all for naught
     3. You are the important party - It's your success that determines the success of PySimpleGUI
@@ -16839,15 +16843,18 @@
 
     window.TKroot = root
 
     window._create_thread_queue()
 
     # for the Raspberry Pi. Need to set the attributes here, prior to the building of the window
     # so going ahead and doing it for all platforms, in addition to doing it after the window is packed
-    _no_titlebar_setup(window)
+    # 2023-April - this call seems to be causing problems on MacOS 13.2.1 Ventura.  Input elements become non-responsive
+    # if this call is made here and at the end of building the window
+    if not running_mac():
+        _no_titlebar_setup(window)
 
     if not window.Resizable:
         root.resizable(False, False)
 
     if window.DisableMinimize:
         root.attributes("-toolwindow", 1)
 
@@ -22318,14 +22325,18 @@
 
     if not running_mac():
         return False
 
     if not ENABLE_MAC_ALPHA_99_PATCH:
         return False
 
+    # ONLY enable this patch for tkinter version 8.6.12
+    if framework_version != '8.6.12':
+        return False
+
     # At this point, we're running a Mac and the alpha patch is enabled
     # Final check is to see if Mac OS version is 12.3 or later
     try:
         platform_mac_ver = platform.mac_ver()[0]
         mac_ver = platform_mac_ver.split('.') if '.' in platform_mac_ver  else (platform_mac_ver, 0)
         if (int(mac_ver[0]) >= 12 and int(mac_ver[1]) >= 3) or int(mac_ver[0]) >= 13 :
             print("Mac OS Version is {} and patch enabled so applying the patch".format(platform_mac_ver))
@@ -23173,14 +23184,211 @@
 PYTHON_COLORED_HEARTS_BASE64 = b'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'
 
 RED_X_BASE64 = b'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'
 
 GREEN_CHECK_BASE64 = b'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'
 
 
+
+'''
+M""MMMMM""M                                           dP          
+M  MMMMM  M                                           88          
+M  MMMMM  M 88d888b. .d8888b. 88d888b. .d8888b. .d888b88 .d8888b. 
+M  MMMMM  M 88'  `88 88'  `88 88'  `88 88'  `88 88'  `88 88ooood8 
+M  `MMM'  M 88.  .88 88.  .88 88       88.  .88 88.  .88 88.  ... 
+Mb       dM 88Y888P' `8888P88 dP       `88888P8 `88888P8 `88888P' 
+MMMMMMMMMMM 88            .88                                     
+            dP        d8888P                                      
+MP""""""`MM                            oo                   
+M  mmmmm..M                                                 
+M.      `YM .d8888b. 88d888b. dP   .dP dP .d8888b. .d8888b. 
+MMMMMMM.  M 88ooood8 88'  `88 88   d8' 88 88'  `"" 88ooood8 
+M. .MMM'  M 88.  ... 88       88 .88'  88 88.  ... 88.  ... 
+Mb.     .dM `88888P' dP       8888P'   dP `88888P' `88888P' 
+MMMMMMMMMMM
+'''
+
+__upgrade_server_ip = 'upgradeapi.PySimpleGUI.com'
+__upgrade_server_port = '5353'
+
+
+def __send_dict(ip, port, dict_to_send):
+    """
+    Send a dictionary to the upgrade server and get back a dictionary in response
+    :param ip:           ip address of the upgrade server
+    :type ip:            str
+    :param port:         port number
+    :type port:          int | str
+    :param dict_to_send: dictionary of items to send
+    :type dict_to_send:  dict
+    :return:             dictionary that is the reply
+    :rtype:              dict
+    """
+
+    # print(f'sending dictionary to ip {ip} port {port}')
+    try:
+        # Create a socket object
+        s = socket.socket()
+
+        s.settimeout(5.0)       # set a 5 second timeout
+
+        # connect to the server on local computer
+        s.connect((ip , int(port)))
+        # send a python dictionary
+        s.send(json.dumps(dict_to_send).encode())
+
+        # receive data from the server
+        reply_data = s.recv(1024).decode()
+        # close the connection
+        s.close()
+    except Exception as e:
+        # print(f'Error sending to server:', e)
+        # print(f'payload:\n', dict_to_send)
+        reply_data = e
+    try:
+        data_dict = json.loads(reply_data)
+    except Exception as e:
+        # print(f'UPGRADE THREAD - Error decoding reply {reply_data} as a dictionary. Error = {e}')
+        data_dict = {}
+    return data_dict
+
+def __show_previous_upgrade_information():
+    """
+    Shows information about upgrades if upgrade information is waiting to be shown
+
+    :return:
+    """
+
+    # if nothing to show, then just return
+    if pysimplegui_user_settings.get('-upgrade info seen-', True) and not pysimplegui_user_settings.get('-upgrade info available-', False):
+        return
+    if pysimplegui_user_settings.get('-upgrade show only critical-', False) and pysimplegui_user_settings.get('-severity level-', '') != 'Critical':
+        return
+
+    message1 = pysimplegui_user_settings.get('-upgrade message 1-', '')
+    message2 = pysimplegui_user_settings.get('-upgrade message 2-', '')
+    recommended_version = pysimplegui_user_settings.get('-upgrade recommendation-', '')
+    severity_level = pysimplegui_user_settings.get('-severity level-', '')
+
+    if severity_level != 'Critical':
+        return
+
+    layout = [[Image(EMOJI_BASE64_HAPPY_THUMBS_UP), T('An upgrade is available & recommended', font='_ 14')],
+              [T('It is recommended you upgrade to version {}'.format(recommended_version))],
+              [T(message1, enable_events=True, k='-MESSAGE 1-')],
+              [T(message2, enable_events=True, k='-MESSAGE 2-')],
+              [CB('Do not show this message again in the future', default=True, k='-SKIP IN FUTURE-')],
+              [B('Close'), T('This window auto-closes in'), T('30', k='-CLOSE TXT-', text_color='white', background_color='red'), T('seconds')]]
+
+    window = Window('PySimpleGUI Intelligent Upgrade', layout, finalize=True)
+    if 'http' in message1:
+        window['-MESSAGE 1-'].set_cursor('hand1')
+    if 'http' in message2:
+        window['-MESSAGE 2-'].set_cursor('hand1')
+
+    seconds_left=30
+    while True:
+        event, values = window.read(timeout=1000)
+        if event in ('Close', WIN_CLOSED) or seconds_left < 1:
+            break
+        if values['-SKIP IN FUTURE-']:
+            if not running_trinket():
+                pysimplegui_user_settings['-upgrade info available-'] = False
+                pysimplegui_user_settings['-upgrade info seen-'] = True
+        if event == '-MESSAGE 1-' and 'http' in message1 and webbrowser_available:
+            webbrowser.open_new_tab(message1)
+        elif event == '-MESSAGE 2-' and 'http' in message2 and webbrowser_available:
+            webbrowser.open_new_tab(message2)
+        window['-CLOSE TXT-'].update(seconds_left)
+        seconds_left -= 1
+
+    window.close()
+
+
+def __get_linux_distribution():
+    line_tuple = ('Linux Distro', 'Unknown', 'No lines Found in //etc//os-release')
+    try:
+        with open('/etc/os-release') as f:
+            data = f.read()
+        lines = data.split('\n')
+        for line in lines:
+            if line.startswith('PRETTY_NAME'):
+                line_split = line.split('=')[1].strip('"')
+                line_tuple = tuple(line_split.split(' '))
+                return line_tuple
+    except:
+        line_tuple = ('Linux Distro', 'Exception','Error reading//processing //etc//os-release')
+
+    return line_tuple
+
+
+def __perform_upgrade_check_thread():
+    # print(f'Upgrade thread...seen = {pysimplegui_user_settings.get("-upgrade info seen-", False)}')
+    try:
+        if running_trinket():
+            os_name = 'Trinket'
+            os_ver = __get_linux_distribution()
+        elif running_replit():
+            os_name = 'REPL.IT'
+            os_ver = __get_linux_distribution()
+        elif running_windows():
+            os_name = 'Windows'
+            os_ver = platform.win32_ver()
+        elif running_linux():
+            os_name = 'Linux'
+            os_ver = __get_linux_distribution()
+        elif running_mac():
+            os_name = 'Mac'
+            os_ver = platform.mac_ver()
+        else:
+            os_name = 'Other'
+            os_ver = ''
+
+        psg_ver = version
+        framework_ver = framework_version
+        python_ver = sys.version
+
+        upgrade_dict = {
+            'OSName' : str(os_name),
+            'OSVersion' : str(os_ver),
+            'PythonVersion' : str(python_ver),
+            'PSGVersion' : str(psg_ver),
+            'FrameworkName' : 'tkinter',
+            'FrameworkVersion' : str(framework_ver),
+        }
+        reply_data = __send_dict(__upgrade_server_ip, __upgrade_server_port, upgrade_dict)
+
+        recommended_version = reply_data.get('SuggestedVersion', '')
+        message1 = reply_data.get('Message1', '')
+        message2 = reply_data.get('Message2', '')
+        severity_level = reply_data.get('SeverityLevel', '')
+        # If any part of the reply has changed from the last reply, overwrite the data and set flags so user will be informed
+        if (message1 or message2) and not running_trinket():
+            if pysimplegui_user_settings.get('-upgrade message 1-', '') != message1 or \
+               pysimplegui_user_settings.get('-upgrade message 2-', '') != message2 or \
+               pysimplegui_user_settings.get('-upgrade recommendation-', '') != recommended_version or \
+               pysimplegui_user_settings.get('-severity level-', '') != severity_level:
+                # Save the data to the settings file
+                pysimplegui_user_settings['-upgrade info seen-'] = False
+                pysimplegui_user_settings['-upgrade info available-'] = True
+                pysimplegui_user_settings['-upgrade message 1-'] = message1
+                pysimplegui_user_settings['-upgrade message 2-'] = message2
+                pysimplegui_user_settings['-upgrade recommendation-'] = recommended_version
+                pysimplegui_user_settings['-severity level-'] = severity_level
+    except Exception as e:
+        reply_data = {}
+        # print('Upgrade server error', e)
+    # print(f'Upgrade Reply = {reply_data}')
+
+def __perform_upgrade_check():
+    # For now, do not show data returned. Still testing and do not want to "SPAM" users with any popups
+    __show_previous_upgrade_information()
+    threading.Thread(target=lambda: __perform_upgrade_check_thread(), daemon=True).start()
+
+
 # =========================================================================#
 # MP""""""`MM                                                                dP                  dP
 # M  mmmmm..M                                                                88                  88
 # M.      `YM .d8888b. 88d888b. .d8888b. .d8888b. .d8888b. 88d888b. .d8888b. 88d888b. .d8888b. d8888P
 # MMMMMMM.  M 88'  `"" 88'  `88 88ooood8 88ooood8 88ooood8 88'  `88 Y8ooooo. 88'  `88 88'  `88   88
 # M. .MMM'  M 88.  ... 88       88.  ... 88.  ... 88.  ... 88    88       88 88    88 88.  .88   88
 # Mb.     .dM `88888P' dP       `88888P' `88888P' `88888P' dP    dP `88888P' dP    dP `88888P'   dP
@@ -23266,15 +23474,15 @@
 # M  M       88       88 88.  .88 88.  ...
 # M  M `88888P' `88888P' `88888P' `88888P'
 # MMMM
 
 
 def _github_issue_post_make_markdown(issue_type, operating_system, os_ver, psg_port, psg_ver, gui_ver, python_ver,
                                      python_exp, prog_exp, used_gui, gui_notes,
-                                     cb_docs, cb_demos, cb_demo_port, cb_readme_other, cb_command_line, cb_issues, cb_github,
+                                     cb_docs, cb_demos, cb_demo_port, cb_readme_other, cb_command_line, cb_issues, cb_latest_pypi, cb_github,
                                      detailed_desc, code, project_details, where_found):
     body = \
 """
 ## Type of Issue (Enhancement, Error, Bug, Question)
 
 {}
 
@@ -23324,19 +23532,20 @@
 ---------------------
 
 ## Troubleshooting
 
 These items may solve your problem. Please check those you've done by changing - [ ] to - [X]
 
 - [{}] Searched main docs for your problem  www.PySimpleGUI.org
-- [{}] Looked for Demo Programs that are similar to your goal Demos.PySimpleGUI.org
+- [{}] Looked for Demo Programs that are similar to your goal. It is recommend you use the Demo Browser! Demos.PySimpleGUI.org
 - [{}] If not tkinter - looked for Demo Programs for specific port
 - [{}] For non tkinter - Looked at readme for your specific port if not PySimpleGUI (Qt, WX, Remi)
 - [{}] Run your program outside of your debugger (from a command line)
 - [{}] Searched through Issues (open and closed) to see if already reported Issues.PySimpleGUI.org
+- [{}] Upgraded to the latest official release of PySimpleGUI on PyPI
 - [{}] Tried using the PySimpleGUI.py file on GitHub. Your problem may have already been fixed but not released
 
 ## Detailed Description
 
 {}
 
 #### Code To Duplicate
@@ -23349,15 +23558,15 @@
 ```
 
 #### Screenshot, Sketch, or Drawing
 
 
 
 """.format(python_exp, prog_exp, used_gui, gui_notes,
-                cb_docs, cb_demos, cb_demo_port, cb_readme_other, cb_command_line, cb_issues, cb_github,
+                cb_docs, cb_demos, cb_demo_port, cb_readme_other, cb_command_line, cb_issues, cb_latest_pypi, cb_github,
                 detailed_desc, code if len(code) > 10 else '# Paste your code here')
 
 
     if project_details or where_found:
         body2 +=  '------------------------'
 
     if project_details:
@@ -23533,19 +23742,20 @@
                       [In(size=(4, 1), k='-EXP PROG-'), T('Years Programming')],
                       [In(size=(4, 1), k='-EXP PYTHON-'), T('Years Writing Python')],
                       [CB('Previously programmed a GUI', k='-CB PRIOR GUI-')],
                       [T('Share more if you want....')],
                       [In(size=(25, 1), k='-EXP NOTES-', expand_x=True)]]
 
     checklist = (('Searched main docs for your problem', 'www.PySimpleGUI.org'),
-                 ('Looked for Demo Programs that are similar to your goal ', 'http://Demos.PySimpleGUI.org'),
+                 ('Looked for Demo Programs that are similar to your goal.\nIt is recommend you use the Demo Browser!', 'https://Demos.PySimpleGUI.org'),
                  ('If not tkinter - looked for Demo Programs for specific port', ''),
                  ('For non tkinter - Looked at readme for your specific port if not PySimpleGUI (Qt, WX, Remi)', ''),
                  ('Run your program outside of your debugger (from a command line)', ''),
-                 ('Searched through Issues (open and closed) to see if already reported', 'http://Issues.PySimpleGUI.org'),
+                 ('Searched through Issues (open and closed) to see if already reported', 'https://Issues.PySimpleGUI.org'),
+                 ('Upgraded to the latest official release of PySimpleGUI on PyPI', 'https://Upgrading.PySimpleGUI.org'),
                  ('Tried using the PySimpleGUI.py file on GitHub. Your problem may have already been fixed but not released.', ''))
 
     checklist_col1 = Col([[CB(c, k=('-CB-', i)), T(t, k='-T{}-'.format(i), enable_events=True)] for i, (c, t) in enumerate(checklist[:4])], k='-C FRAME CBs1-')
     checklist_col2 = Col([[CB(c, k=('-CB-', i + 4)), T(t, k='-T{}-'.format(i + 4), enable_events=True)] for i, (c, t) in enumerate(checklist[4:])], pad=(0, 0),
                          k='-C FRAME CBs2-')
     checklist_tabgropup = TabGroup(
         [[Tab('Checklist 1 *', [[checklist_col1]], expand_x=True, expand_y=True), Tab('Checklist 2  *', [[checklist_col2]]), Tab('Experience', col_experience, k='-Tab Exp-', pad=(0, 0))]], expand_x=True, expand_y=True)
@@ -23600,14 +23810,23 @@
     # for i in range(len(checklist)):
     [window['-T{}-'.format(i)].set_cursor('hand1') for i in range(len(checklist))]
     # window['-TABGROUP-'].expand(True, True, True)
     # window['-ML CODE-'].expand(True, True, True)
     # window['-ML DETAILS-'].expand(True, True, True)
     # window['-ML MARKDOWN-'].expand(True, True, True)
     # window['-PANE-'].expand(True, True, True)
+
+    if running_mac():
+        window['-OS MAC VER-'].update(platform.mac_ver())
+    elif running_windows():
+        window['-OS WIN VER-'].update(platform.win32_ver())
+    elif running_linux():
+        window['-OS LINUX VER-'].update(platform.libc_ver())
+
+
     window.bring_to_front()
     while True:  # Event Loop
         event, values = window.read()
         # print(event, values)
         if event in (WINDOW_CLOSE_ATTEMPTED_EVENT, 'Quit'):
             if popup_yes_no('Do you really want to exit?',
                             'If you have not clicked Post Issue button and then clicked "Submit New Issue" button '
@@ -23661,15 +23880,15 @@
                 continue
             checkboxes = ['X' if values[('-CB-', i)] else ' ' for i in range(len(checklist))]
 
             if not _github_issue_post_validate(values, checklist, issue_types):
                 continue
 
             cb_dict = {'cb_docs': checkboxes[0], 'cb_demos': checkboxes[1], 'cb_demo_port': checkboxes[2], 'cb_readme_other': checkboxes[3],
-                       'cb_command_line': checkboxes[4], 'cb_issues': checkboxes[5], 'cb_github': checkboxes[6], 'detailed_desc': values['-ML DETAILS-'],
+                       'cb_command_line': checkboxes[4], 'cb_issues': checkboxes[5], 'cb_latest_pypi': checkboxes[6], 'cb_github': checkboxes[7], 'detailed_desc': values['-ML DETAILS-'],
                        'code': values['-ML CODE-'],
                        'project_details': values['-ML PROJECT DETAILS-'].rstrip(),
                        'where_found': values['-ML FOUND PSG-']}
 
             markdown = _github_issue_post_make_markdown(issue_type, operating_system, os_ver, 'tkinter', values['-VER PSG-'], values['-VER TK-'],
                                                         values['-VER PYTHON-'],
                                                         values['-EXP PYTHON-'],values['-EXP PROG-'], 'Yes' if values['-CB PRIOR GUI-'] else 'No',
@@ -24236,45 +24455,45 @@
 
 def main_sdk_help():
     """
     Display a window that will display the docstrings for each PySimpleGUI Element and the Window object
 
     """
     online_help_links = {
-        'Button': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#button-element',
-        'ButtonMenu': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#buttonmenu-element',
-        'Canvas': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#canvas-element',
-        'Checkbox': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#checkbox-element',
-        'Column': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#column-element',
-        'Combo': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#combo-element',
-        'Frame': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#frame-element',
-        'Graph': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#graph-element',
-        'HorizontalSeparator': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#horizontalseparator-element',
-        'Image': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#image-element',
-        'Input': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#input-element',
-        'Listbox': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#listbox-element',
-        'Menu': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#menu-element',
-        'MenubarCustom': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#menubarcustom-element',
-        'Multiline': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#multiline-element',
-        'OptionMenu': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#optionmenu-element',
-        'Output': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#output-element',
-        'Pane': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#pane-element',
-        'ProgressBar': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#progressbar-element',
-        'Radio': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#radio-element',
-        'Slider': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#slider-element',
-        'Spin': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#spin-element',
-        'StatusBar': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#statusbar-element',
-        'Tab': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#tab-element',
-        'TabGroup': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#tabgroup-element',
-        'Table': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#table-element',
-        'Text': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#text-element',
-        'Titlebar': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#titlebar-element',
-        'Tree': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#tree-element',
-        'VerticalSeparator': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#verticalseparator-element',
-        'Window': r'https://pysimplegui.readthedocs.io/en/latest/call%20reference/#window',
+        'Button': r'https://PySimpleGUI.org/en/latest/call%20reference/#button-element',
+        'ButtonMenu': r'https://PySimpleGUI.org/en/latest/call%20reference/#buttonmenu-element',
+        'Canvas': r'https://PySimpleGUI.org/en/latest/call%20reference/#canvas-element',
+        'Checkbox': r'https://PySimpleGUI.org/en/latest/call%20reference/#checkbox-element',
+        'Column': r'https://PySimpleGUI.org/en/latest/call%20reference/#column-element',
+        'Combo': r'https://PySimpleGUI.org/en/latest/call%20reference/#combo-element',
+        'Frame': r'https://PySimpleGUI.org/en/latest/call%20reference/#frame-element',
+        'Graph': r'https://PySimpleGUI.org/en/latest/call%20reference/#graph-element',
+        'HorizontalSeparator': r'https://PySimpleGUI.org/en/latest/call%20reference/#horizontalseparator-element',
+        'Image': r'https://PySimpleGUI.org/en/latest/call%20reference/#image-element',
+        'Input': r'https://PySimpleGUI.org/en/latest/call%20reference/#input-element',
+        'Listbox': r'https://PySimpleGUI.org/en/latest/call%20reference/#listbox-element',
+        'Menu': r'https://PySimpleGUI.org/en/latest/call%20reference/#menu-element',
+        'MenubarCustom': r'https://PySimpleGUI.org/en/latest/call%20reference/#menubarcustom-element',
+        'Multiline': r'https://PySimpleGUI.org/en/latest/call%20reference/#multiline-element',
+        'OptionMenu': r'https://PySimpleGUI.org/en/latest/call%20reference/#optionmenu-element',
+        'Output': r'https://PySimpleGUI.org/en/latest/call%20reference/#output-element',
+        'Pane': r'https://PySimpleGUI.org/en/latest/call%20reference/#pane-element',
+        'ProgressBar': r'https://PySimpleGUI.org/en/latest/call%20reference/#progressbar-element',
+        'Radio': r'https://PySimpleGUI.org/en/latest/call%20reference/#radio-element',
+        'Slider': r'https://PySimpleGUI.org/en/latest/call%20reference/#slider-element',
+        'Spin': r'https://PySimpleGUI.org/en/latest/call%20reference/#spin-element',
+        'StatusBar': r'https://PySimpleGUI.org/en/latest/call%20reference/#statusbar-element',
+        'Tab': r'https://PySimpleGUI.org/en/latest/call%20reference/#tab-element',
+        'TabGroup': r'https://PySimpleGUI.org/en/latest/call%20reference/#tabgroup-element',
+        'Table': r'https://PySimpleGUI.org/en/latest/call%20reference/#table-element',
+        'Text': r'https://PySimpleGUI.org/en/latest/call%20reference/#text-element',
+        'Titlebar': r'https://PySimpleGUI.org/en/latest/call%20reference/#titlebar-element',
+        'Tree': r'https://PySimpleGUI.org/en/latest/call%20reference/#tree-element',
+        'VerticalSeparator': r'https://PySimpleGUI.org/en/latest/call%20reference/#verticalseparator-element',
+        'Window': r'https://PySimpleGUI.org/en/latest/call%20reference/#window',
     }
 
     NOT_AN_ELEMENT = 'Not An Element'
     element_classes = Element.__subclasses__()
     element_names = {element.__name__: element for element in element_classes}
     element_names['Window'] = Window
     element_classes.append(Window)
@@ -24553,52 +24772,61 @@
         [B('Get File'), B('Get Folder'), B('Get Date'), B('Get Text')]]
 
     GRAPH_SIZE=(500, 200)
     graph_elem = Graph(GRAPH_SIZE, (0, 0), GRAPH_SIZE, key='+GRAPH+')
 
     frame6 = [[VPush()],[graph_elem]]
 
-    global_settings_tab_layout = [[T('Settings Filename:'), T(pysimplegui_user_settings.full_filename, s=(50,2))],
-                                  [T('Settings Dictionary:'), MLine(pysimplegui_user_settings, size=(50,8))],
-                                  ]
-
     themes_tab_layout = [[T('You can see a preview of the themes, the color swatches, or switch themes for this window')],
                          [T('If you want to change the default theme for PySimpleGUI, use the Global Settings')],
                          [B('Themes'), B('Theme Swatches'), B('Switch Themes')]]
 
+
+    upgrade_recommendation_tab_layout = [[T('Latest Recommendation and Announcements For You', font='_ 14')],
+                                         [T('Severity Level of Update:'), T(pysimplegui_user_settings.get('-severity level-',''))],
+                                         [T('Recommended Version To Upgrade To:'), T(pysimplegui_user_settings.get('-upgrade recommendation-',''))],
+                                         [T(pysimplegui_user_settings.get('-upgrade message 1-',''))],
+                                         [T(pysimplegui_user_settings.get('-upgrade message 2-',''))],
+                                         [Checkbox('Show Only Critical Messages', default=pysimplegui_user_settings.get('-upgrade show only critical-', False), key='-UPGRADE SHOW ONLY CRITICAL-', enable_events=True)],
+                                         [Button('Show Notification Again'),
+],
+                                         ]
+    tab_upgrade = Tab('Upgrade\n',upgrade_recommendation_tab_layout,  expand_x=True)
+
+
     tab1 = Tab('Graph\n', frame6, tooltip='Graph is in here', title_color='red')
     tab2 = Tab('CB, Radio\nList, Combo',
                [[Frame('Multiple Choice Group', frame2, title_color='#FFFFFF', tooltip='Checkboxes, radio buttons, etc', vertical_alignment='t',),
                  Frame('Binary Choice Group', frame3, title_color='#FFFFFF', tooltip='Binary Choice', vertical_alignment='t', ), ]])
     # tab3 = Tab('Table and Tree', [[Frame('Structured Data Group', frame5, title_color='red', element_justification='l')]], tooltip='tab 3', title_color='red', )
     tab3 = Tab('Table &\nTree', [[Column(frame5, element_justification='l', vertical_alignment='t')]], tooltip='tab 3', title_color='red', k='-TAB TABLE-')
     tab4 = Tab('Sliders\n', [[Frame('Variable Choice Group', frame4, title_color='blue')]], tooltip='tab 4', title_color='red', k='-TAB VAR-')
     tab5 = Tab('Input\nMultiline', [[Frame('TextInput', frame1, title_color='blue')]], tooltip='tab 5', title_color='red', k='-TAB TEXT-')
     tab6 = Tab('Course or\nSponsor', frame7, k='-TAB SPONSOR-')
     tab7 = Tab('Popups\n', pop_test_tab_layout, k='-TAB POPUP-')
     tab8 = Tab('Themes\n', themes_tab_layout, k='-TAB THEMES-')
-    tab9 = Tab('Global\nSettings', global_settings_tab_layout, k='-TAB GlOBAL SETTINGS-')
 
     def VerLine(version, description, justification='r', size=(40, 1)):
-        return [T(version, justification=justification, font='Any 12', text_color='yellow', size=size, pad=(0,0)), vtop(T(description, font='Any 12', pad=(0,0)))]
+        return [T(version, justification=justification, font='Any 12', text_color='yellow', size=size, pad=(0,0)), T(description, font='Any 12', pad=(0,0))]
 
     layout_top = Column([
         [Image(EMOJI_BASE64_HAPPY_BIG_SMILE, enable_events=True, key='-LOGO-', tooltip='This is PySimpleGUI logo'),
          Image(data=DEFAULT_BASE64_LOADING_GIF, enable_events=True, key='-IMAGE-'),
-         Text('PySimpleGUI Test Harness\nYou are running PySimpleGUI.py file vs importing', font='ANY 14',
+         Text('PySimpleGUI Test Harness', font='ANY 14',
               tooltip='My tooltip', key='-TEXT1-')],
         VerLine(ver, 'PySimpleGUI Version') + [Image(HEART_3D_BASE64, subsample=4)],
-        VerLine('{}/{}'.format(tkversion, tclversion), 'TK/TCL Versions'),
+        # VerLine('{}/{}'.format(tkversion, tclversion), 'TK/TCL Versions'),
         VerLine(tclversion_detailed, 'detailed tkinter version'),
-        VerLine(os.path.dirname(os.path.abspath(__file__)), 'PySimpleGUI Location', size=(40, 2)),
+        VerLine(os.path.dirname(os.path.abspath(__file__)), 'PySimpleGUI Location', size=(40, None)),
+        VerLine(sys.executable, 'Python Executable'),
         VerLine(sys.version, 'Python Version', size=(40,2)) +[Image(PYTHON_COLORED_HEARTS_BASE64, subsample=3, k='-PYTHON HEARTS-', enable_events=True)]], pad=0)
 
     layout_bottom = [
         [B(SYMBOL_DOWN, pad=(0, 0), k='-HIDE TABS-'),
-         pin(Col([[TabGroup([[tab1, tab2, tab3, tab6, tab4, tab5, tab7, tab8, tab9]], key='-TAB_GROUP-')]], k='-TAB GROUP COL-'))],
+         pin(Col([[TabGroup([[tab1, tab2, tab3, tab6, tab4, tab5, tab7, tab8, tab_upgrade]], key='-TAB_GROUP-')]], k='-TAB GROUP COL-'))],
         [B('Button', highlight_colors=('yellow', 'red'),pad=(1, 0)),
          B('ttk Button', use_ttk_buttons=True, tooltip='This is a TTK Button',pad=(1, 0)),
          B('See-through Mode', tooltip='Make the background transparent',pad=(1, 0)),
          B('Upgrade PySimpleGUI from GitHub', button_color='white on red', key='-INSTALL-',pad=(1, 0)),
          B('Global Settings', tooltip='Settings across all PySimpleGUI programs',pad=(1, 0)),
          B('Exit', tooltip='Exit button',pad=(1, 0))],
         # [B(image_data=ICON_BUY_ME_A_COFFEE,pad=(1, 0), key='-COFFEE-'),
@@ -24693,37 +24921,37 @@
         elif event == 'Launch Debugger':
             show_debugger_window()
         elif event == 'About...':
             popup('About this program...', 'You are looking at the test harness for the PySimpleGUI program', version, keep_on_top=True, image=DEFAULT_BASE64_ICON)
         elif event.startswith('See'):
             window._see_through = not window._see_through
             window.set_transparent_color(theme_background_color() if window._see_through else '')
-        elif event == '-INSTALL-':
+        elif event == '-INSTALL-' or event == '-UPGRADE FROM GITHUB-':
             _upgrade_gui()
         elif event == 'Popup':
             popup('This is your basic popup', keep_on_top=True)
         elif event == 'Get File':
             popup_scrolled('Returned:', popup_get_file('Get File', keep_on_top=True))
         elif event == 'Get Folder':
             popup_scrolled('Returned:', popup_get_folder('Get Folder', keep_on_top=True))
         elif event == 'Get Date':
             popup_scrolled('Returned:', popup_get_date(keep_on_top=True))
         elif event == 'Get Text':
             popup_scrolled('Returned:', popup_get_text('Enter some text', keep_on_top=True))
         elif event.startswith('-UDEMY-'):
-                webbrowser.open_new_tab(r'https://udemy.com/PySimpleGUI')
+            webbrowser.open_new_tab(r'https://www.udemy.com/course/pysimplegui/?couponCode=9AF99B123C49D51EB547')
         elif event.startswith('-SPONSOR-'):
             if webbrowser_available:
                 webbrowser.open_new_tab(r'https://www.paypal.me/pythongui')
         elif event == '-COFFEE-':
             if webbrowser_available:
                 # webbrowser.open_new_tab(r'https://udemy.com/PySimpleGUI')
                 webbrowser.open_new_tab(r'https://www.buymeacoffee.com/PySimpleGUI')
         elif event in  ('-EMOJI-HEARTS-', '-HEART-', '-PYTHON HEARTS-'):
-            popup_scrolled("Oh look!  It's a Udemy discount coupon!", '4FD91A459D56B1029FF8',
+            popup_scrolled("Oh look!  It's a Udemy discount coupon!", '9AF99B123C49D51EB547',
                            'A personal message from Mike -- thank you so very much for supporting PySimpleGUI!', title='Udemy Coupon', image=EMOJI_BASE64_MIKE, keep_on_top=True)
 
         elif event == 'Themes':
             search_string = popup_get_text('Enter a search term or leave blank for all themes', 'Show Available Themes', keep_on_top=True)
             if search_string is not None:
                 theme_previewer(search_string=search_string)
         elif event == 'Theme Swatches':
@@ -24763,14 +24991,23 @@
                 popup_auto_close('Will autoclose in 3 seconds', auto_close_duration=3, keep_on_top=True)
         elif event == 'Versions for GitHub':
             main_get_debug_data()
         elif event == 'Open GitHub Issue':
             window.minimize()
             main_open_github_issue()
             window.normal()
+        elif event == 'Show Notification Again':
+            if not running_trinket():
+                pysimplegui_user_settings.set('-upgrade info seen-', False)
+                __show_previous_upgrade_information()
+        elif event == '-UPGRADE SHOW ONLY CRITICAL-':
+            if not running_trinket():
+                pysimplegui_user_settings.set('-upgrade show only critical-', values['-UPGRADE SHOW ONLY CRITICAL-'])
+
+
         i += 1
         # _refresh_debugger()
     print('event = ', event)
     window.close()
     set_options(force_modal_windows=forced_modal)
 
 # ------------------------ PEP8-ify The SDK ------------------------#
@@ -24852,23 +25089,27 @@
     except Exception as e:
         print('Error using the taskbar icon patch', e)
 
 
 _read_mac_global_settings()
 
 if _mac_should_set_alpha_to_99():
-    print('Applyting Mac OS 12.3+ Alpha Channel fix.  Your default Alpha Channel is now 0.99')
+    # Applyting Mac OS 12.3+ Alpha Channel fix.  Sets the default Alpha Channel to 0.99
     set_options(alpha_channel=0.99)
 # if running_mac():
 #     print('Your Mac patches are:')
 #     print('Modal windows disabled:', ENABLE_MAC_MODAL_DISABLE_PATCH)
 #     print('No titlebar patch:', ENABLE_MAC_NOTITLEBAR_PATCH)
 #     print('No grab anywhere allowed with titlebar:', ENABLE_MAC_DISABLE_GRAB_ANYWHERE_WITH_TITLEBAR)
 #     print('Currently the no titlebar patch ' + ('WILL' if _mac_should_apply_notitlebar_patch() else 'WILL NOT') + ' be applied')
 
+
+__perform_upgrade_check()
+
+
 # -------------------------------- ENTRY POINT IF RUN STANDALONE -------------------------------- #
 if __name__ == '__main__':
     # To execute the upgrade from command line, type:
     # python -m PySimpleGUI.PySimpleGUI upgrade
     if len(sys.argv) > 1 and sys.argv[1] == 'upgrade':
         _upgrade_gui()
         exit(0)
```

### Comparing `PySimpleGUI-4.60.4/PySimpleGUI.egg-info/PKG-INFO` & `PySimpleGUI-4.60.5/PySimpleGUI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySimpleGUI
-Version: 4.60.4
+Version: 4.60.5
 Summary: Python GUIs for Humans. Launched in 2018. It's 2022 & PySimpleGUI is an ACTIVE & supported project. Super-simple to create custom GUI's. 325+ Demo programs & Cookbook for rapid start. Extensive documentation. Main docs at www.PySimpleGUI.org. Fun & your success are the focus. Examples using Machine Learning (GUI, OpenCV Integration), Rainmeter Style Desktop Widgets, Matplotlib + Pyplot, PIL support, add GUI to command line scripts, PDF & Image Viewers. Great for beginners & advanced GUI programmers.
 Home-page: https://github.com/PySimpleGUI/PySimpleGUI
 Author: PySimpleGUI
 Author-email: PySimpleGUI@PySimpleGUI.org
 License: UNKNOWN
 Description: 
         <p align="center">
@@ -14,16 +14,16 @@
         
         <table>
           <tr>
             <td>
               <img src="https://www.dropbox.com/s/6wzf3ebmj97v4zs/PySimpleGUI-GitHub-Udemy-Course.png?raw=1" width=200 alt="PySimpleGUI Udemy Course">
             </td>
             <td>
-              <h5>apply coupon for discount:<br>4FD91A459D56B1029FF8</h6>
-              <a href="https://www.udemy.com/course/pysimplegui/?couponCode=4FD91A459D56B1029FF8">click here to visit course page</a>
+              <h5>apply coupon for discount:<br>9AF99B123C49D51EB547</h6>
+              <a href="https://www.udemy.com/course/pysimplegui/?couponCode=9AF99B123C49D51EB547">click here to visit course page</a>
             </td>
           </tr>
         </table>
         
         Transforms the tkinter, Qt, WxPython, and Remi (browser-based) GUI frameworks into a simpler interface.  The window definition is simplified by using Python core data types understood by beginners (lists and dictionaries). Further simplification happens by changing event handling from a callback-based model to a message passing one.  
         
         Your code is not _required_ to have an object oriented architecture which makes the package usable by a larger audience. While the architecture is simple to understand, it does not *necessarily* limit you to only simple problems.  
@@ -895,11 +895,12 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_ye4rarhr_/tmps1e2v_mm_TarContainer/0/8", line 22, column 16: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_ye4rarhr_/tmps1e2v_mm_TarContainer/0/8", line 22, column 16: Levels of opening and closing headings don't match*

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: PySimpleGUI Version: 4.60.4 Summary: Python GUIs
+Metadata-Version: 2.1 Name: PySimpleGUI Version: 4.60.5 Summary: Python GUIs
 for Humans. Launched in 2018. It's 2022 & PySimpleGUI is an ACTIVE & supported
 project. Super-simple to create custom GUI's. 325+ Demo programs & Cookbook for
 rapid start. Extensive documentation. Main docs at www.PySimpleGUI.org. Fun &
 your success are the focus. Examples using Machine Learning (GUI, OpenCV
 Integration), Rainmeter Style Desktop Widgets, Matplotlib + Pyplot, PIL
 support, add GUI to command line scripts, PDF & Image Viewers. Great for
 beginners & advanced GUI programmers. Home-page: https://github.com/
 PySimpleGUI/PySimpleGUI Author: PySimpleGUI Author-email:
 PySimpleGUI@PySimpleGUI.org License: UNKNOWN Description:
                            [Python GUIs for Humans]
                       ***** Python GUIs for Humans *****
                            ** apply coupon for discount:
-[PySimpleGUI Udemy Course] 4FD91A459D56B1029FF8 **
+[PySimpleGUI Udemy Course] 9AF99B123C49D51EB547 **
                            click_here_to_visit_course_page
 Transforms the tkinter, Qt, WxPython, and Remi (browser-based) GUI frameworks
 into a simpler interface. The window definition is simplified by using Python
 core data types understood by beginners (lists and dictionaries). Further
 simplification happens by changing event handling from a callback-based model
 to a message passing one. Your code is not _required_ to have an object
 oriented architecture which makes the package usable by a larger audience.
@@ -752,11 +752,11 @@
 WxPython Remi wrapper simple easy beginner novice student graphics progressbar
 progressmeter Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4 Classifier: Programming
 Language :: Python :: 3.5 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: License :: OSI Approved :: GNU Lesser
-General Public License v3 or later (LGPLv3+) Classifier: Topic :: Multimedia ::
-Graphics Classifier: Operating System :: OS Independent Description-Content-
-Type: text/markdown
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or
+later (LGPLv3+) Classifier: Topic :: Multimedia :: Graphics Classifier:
+Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `PySimpleGUI-4.60.4/setup.py` & `PySimpleGUI-4.60.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
             return f.read()
     except IOError:
         return ''
 
 
 setuptools.setup(
     name="PySimpleGUI",
-    version="4.60.4",
+    version="4.60.5",
     author="PySimpleGUI",
     author_email="PySimpleGUI@PySimpleGUI.org",
     description="Python GUIs for Humans. Launched in 2018. It's 2022 & PySimpleGUI is an ACTIVE & supported project. Super-simple to create custom GUI's. 325+ Demo programs & Cookbook for rapid start. Extensive documentation. Main docs at www.PySimpleGUI.org. Fun & your success are the focus. Examples using Machine Learning (GUI, OpenCV Integration), Rainmeter Style Desktop Widgets, Matplotlib + Pyplot, PIL support, add GUI to command line scripts, PDF & Image Viewers. Great for beginners & advanced GUI programmers.",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords="GUI UI tkinter Qt WxPython Remi wrapper simple easy beginner novice student graphics progressbar progressmeter",
     url="https://github.com/PySimpleGUI/PySimpleGUI",
@@ -25,14 +25,15 @@
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
         "Topic :: Multimedia :: Graphics",
         "Operating System :: OS Independent"
     ),
     entry_points={
         'gui_scripts': [
             'psgissue=PySimpleGUI.PySimpleGUI:main_open_github_issue',
```

