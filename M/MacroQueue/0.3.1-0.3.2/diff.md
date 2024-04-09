# Comparing `tmp/MacroQueue-0.3.1.tar.gz` & `tmp/MacroQueue-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MacroQueue-0.3.1.tar", last modified: Mon Apr  8 14:51:29 2024, max compression
+gzip compressed data, was "MacroQueue-0.3.2.tar", last modified: Tue Apr  9 14:57:34 2024, max compression
```

## Comparing `MacroQueue-0.3.1.tar` & `MacroQueue-0.3.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 14:51:29.896589 MacroQueue-0.3.1/
--rw-rw-rw-   0        0        0     1088 2024-03-19 20:51:50.000000 MacroQueue-0.3.1/LICENSE.md
-drwxrwxrwx   0        0        0        0 2024-04-08 14:51:29.836594 MacroQueue-0.3.1/MacroQueue/
-drwxrwxrwx   0        0        0        0 2024-04-08 14:51:29.866175 MacroQueue-0.3.1/MacroQueue/Bitmaps/
--rw-rw-rw-   0        0        0    65674 2022-02-15 20:38:04.000000 MacroQueue-0.3.1/MacroQueue/Bitmaps/DownArrow.bmp
--rw-rw-rw-   0        0        0   786570 2022-02-15 20:38:07.000000 MacroQueue-0.3.1/MacroQueue/Bitmaps/Remove.bmp
--rw-rw-rw-   0        0        0    65674 2022-02-15 20:38:12.000000 MacroQueue-0.3.1/MacroQueue/Bitmaps/UpArrow.bmp
--rw-rw-rw-   0        0        0    69978 2024-04-08 14:29:58.000000 MacroQueue-0.3.1/MacroQueue/Dialogs.py
-drwxrwxrwx   0        0        0        0 2024-04-08 14:51:29.876979 MacroQueue-0.3.1/MacroQueue/Functions/
--rw-rw-rw-   0        0        0    11702 2024-04-04 18:23:56.000000 MacroQueue-0.3.1/MacroQueue/Functions/BField.py
--rw-rw-rw-   0        0        0    14949 2024-04-04 18:21:46.000000 MacroQueue-0.3.1/MacroQueue/Functions/CreaTec.py
--rw-rw-rw-   0        0        0     1094 2024-04-08 14:39:54.000000 MacroQueue-0.3.1/MacroQueue/Functions/General.py
--rw-rw-rw-   0        0        0     7641 2024-04-04 18:16:32.000000 MacroQueue-0.3.1/MacroQueue/Functions/RF.py
--rw-rw-rw-   0        0        0    23101 2023-04-19 20:00:33.000000 MacroQueue-0.3.1/MacroQueue/Functions/RHK.py
--rw-rw-rw-   0        0        0     6042 2024-03-20 15:39:38.000000 MacroQueue-0.3.1/MacroQueue/Functions/SXM.py
--rw-rw-rw-   0        0        0    16085 2024-03-19 20:14:36.000000 MacroQueue-0.3.1/MacroQueue/Functions/SXMRemote.py
--rw-rw-rw-   0        0        0      460 2024-04-08 14:35:52.000000 MacroQueue-0.3.1/MacroQueue/Functions/Testing.py
--rw-rw-rw-   0        0        0    21014 2024-04-08 14:29:40.000000 MacroQueue-0.3.1/MacroQueue/GUIDesign.py
--rw-rw-rw-   0        0        0    57939 2024-04-08 14:49:36.000000 MacroQueue-0.3.1/MacroQueue/MacroQueue.py
--rw-rw-rw-   0        0        0   181242 2022-03-08 20:23:43.000000 MacroQueue-0.3.1/MacroQueue/MacroQueueIcon.ico
-drwxrwxrwx   0        0        0        0 2024-04-08 14:51:29.886565 MacroQueue-0.3.1/MacroQueue/Macros/
--rw-rw-rw-   0        0        0    20611 2024-04-08 12:41:13.000000 MacroQueue-0.3.1/MacroQueue/Macros/CreaTecMacro.json
--rw-rw-rw-   0        0        0       59 2024-04-08 14:20:52.000000 MacroQueue-0.3.1/MacroQueue/Macros/RHKMacro.json
--rw-rw-rw-   0        0        0      738 2024-04-08 14:36:30.000000 MacroQueue-0.3.1/MacroQueue/Macros/TestingMacro.json
--rw-rw-rw-   0        0        0      565 2024-04-02 17:43:33.000000 MacroQueue-0.3.1/MacroQueue/MakeExe.sh
--rw-rw-rw-   0        0        0      529 2024-04-08 14:48:46.000000 MacroQueue-0.3.1/MacroQueue/__init__.py
--rw-rw-rw-   0        0        0      178 2024-03-19 19:42:01.000000 MacroQueue-0.3.1/MacroQueue/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 14:51:29.896589 MacroQueue-0.3.1/MacroQueue.egg-info/
--rw-rw-rw-   0        0        0     4000 2024-04-08 14:51:29.000000 MacroQueue-0.3.1/MacroQueue.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      887 2024-04-08 14:51:29.000000 MacroQueue-0.3.1/MacroQueue.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 14:51:29.000000 MacroQueue-0.3.1/MacroQueue.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-04-08 14:51:29.000000 MacroQueue-0.3.1/MacroQueue.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-08 14:51:29.000000 MacroQueue-0.3.1/MacroQueue.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4000 2024-04-08 14:51:29.896589 MacroQueue-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     3109 2024-04-03 16:00:45.000000 MacroQueue-0.3.1/README.md
--rw-rw-rw-   0        0        0       86 2024-04-08 14:51:29.896589 MacroQueue-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     2259 2024-04-08 14:49:58.000000 MacroQueue-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 14:51:29.896589 MacroQueue-0.3.1/test/
--rw-rw-rw-   0        0        0      571 2024-04-04 18:40:22.000000 MacroQueue-0.3.1/test/test_MainFrame.py
--rw-rw-rw-   0        0        0      920 2024-04-05 13:00:39.000000 MacroQueue-0.3.1/test/test_STMthread.py
--rw-rw-rw-   0        0        0      730 2024-03-19 18:07:48.000000 MacroQueue-0.3.1/test/test_readdata.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:57:34.318325 MacroQueue-0.3.2/
+-rw-rw-rw-   0        0        0     1088 2024-03-19 20:51:50.000000 MacroQueue-0.3.2/LICENSE.md
+drwxrwxrwx   0        0        0        0 2024-04-09 14:57:34.056877 MacroQueue-0.3.2/MacroQueue/
+drwxrwxrwx   0        0        0        0 2024-04-09 14:57:34.136427 MacroQueue-0.3.2/MacroQueue/Bitmaps/
+-rw-rw-rw-   0        0        0    65674 2022-02-15 20:38:04.000000 MacroQueue-0.3.2/MacroQueue/Bitmaps/DownArrow.bmp
+-rw-rw-rw-   0        0        0   786570 2022-02-15 20:38:07.000000 MacroQueue-0.3.2/MacroQueue/Bitmaps/Remove.bmp
+-rw-rw-rw-   0        0        0    65674 2022-02-15 20:38:12.000000 MacroQueue-0.3.2/MacroQueue/Bitmaps/UpArrow.bmp
+-rw-rw-rw-   0        0        0    69988 2024-04-08 17:15:22.000000 MacroQueue-0.3.2/MacroQueue/Dialogs.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:57:34.236959 MacroQueue-0.3.2/MacroQueue/Functions/
+-rw-rw-rw-   0        0        0    11798 2024-04-08 16:46:49.000000 MacroQueue-0.3.2/MacroQueue/Functions/BField.py
+-rw-rw-rw-   0        0        0    14949 2024-04-04 18:21:46.000000 MacroQueue-0.3.2/MacroQueue/Functions/CreaTec.py
+-rw-rw-rw-   0        0        0     1115 2024-04-09 14:43:05.000000 MacroQueue-0.3.2/MacroQueue/Functions/General.py
+-rw-rw-rw-   0        0        0     7641 2024-04-04 18:16:32.000000 MacroQueue-0.3.2/MacroQueue/Functions/RF.py
+-rw-rw-rw-   0        0        0    23101 2023-04-19 20:00:33.000000 MacroQueue-0.3.2/MacroQueue/Functions/RHK.py
+-rw-rw-rw-   0        0        0     6042 2024-03-20 15:39:38.000000 MacroQueue-0.3.2/MacroQueue/Functions/SXM.py
+-rw-rw-rw-   0        0        0    16085 2024-03-19 20:14:36.000000 MacroQueue-0.3.2/MacroQueue/Functions/SXMRemote.py
+-rw-rw-rw-   0        0        0      460 2024-04-08 14:35:52.000000 MacroQueue-0.3.2/MacroQueue/Functions/Testing.py
+-rw-rw-rw-   0        0        0    21392 2024-04-08 17:08:17.000000 MacroQueue-0.3.2/MacroQueue/GUIDesign.py
+-rw-rw-rw-   0        0        0    58564 2024-04-09 14:47:18.000000 MacroQueue-0.3.2/MacroQueue/MacroQueue.py
+-rw-rw-rw-   0        0        0   181242 2022-03-08 20:23:43.000000 MacroQueue-0.3.2/MacroQueue/MacroQueueIcon.ico
+drwxrwxrwx   0        0        0        0 2024-04-09 14:57:34.267368 MacroQueue-0.3.2/MacroQueue/Macros/
+-rw-rw-rw-   0        0        0    53277 2024-04-08 16:48:27.000000 MacroQueue-0.3.2/MacroQueue/Macros/CreaTecMacro.json
+-rw-rw-rw-   0        0        0     9140 2024-04-08 14:54:21.000000 MacroQueue-0.3.2/MacroQueue/Macros/RHKMacro.json
+-rw-rw-rw-   0        0        0     2524 2024-04-08 16:57:56.000000 MacroQueue-0.3.2/MacroQueue/Macros/TestingMacro.json
+-rw-rw-rw-   0        0        0      565 2024-04-02 17:43:33.000000 MacroQueue-0.3.2/MacroQueue/MakeExe.sh
+-rw-rw-rw-   0        0        0      529 2024-04-08 14:48:46.000000 MacroQueue-0.3.2/MacroQueue/__init__.py
+-rw-rw-rw-   0        0        0      178 2024-03-19 19:42:01.000000 MacroQueue-0.3.2/MacroQueue/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:57:34.315307 MacroQueue-0.3.2/MacroQueue.egg-info/
+-rw-rw-rw-   0        0        0     4000 2024-04-09 14:57:33.000000 MacroQueue-0.3.2/MacroQueue.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      887 2024-04-09 14:57:33.000000 MacroQueue-0.3.2/MacroQueue.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 14:57:33.000000 MacroQueue-0.3.2/MacroQueue.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-09 14:57:33.000000 MacroQueue-0.3.2/MacroQueue.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-09 14:57:33.000000 MacroQueue-0.3.2/MacroQueue.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4000 2024-04-09 14:57:34.318325 MacroQueue-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3109 2024-04-03 16:00:45.000000 MacroQueue-0.3.2/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-09 14:57:34.318325 MacroQueue-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     2259 2024-04-09 14:47:28.000000 MacroQueue-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:57:34.307924 MacroQueue-0.3.2/test/
+-rw-rw-rw-   0        0        0      571 2024-04-04 18:40:22.000000 MacroQueue-0.3.2/test/test_MainFrame.py
+-rw-rw-rw-   0        0        0      920 2024-04-05 13:00:39.000000 MacroQueue-0.3.2/test/test_STMthread.py
+-rw-rw-rw-   0        0        0      730 2024-03-19 18:07:48.000000 MacroQueue-0.3.2/test/test_readdata.py
```

### Comparing `MacroQueue-0.3.1/LICENSE.md` & `MacroQueue-0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.3.1/MacroQueue/Bitmaps/DownArrow.bmp` & `MacroQueue-0.3.2/MacroQueue/Bitmaps/DownArrow.bmp`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.3.1/MacroQueue/Bitmaps/Remove.bmp` & `MacroQueue-0.3.2/MacroQueue/Bitmaps/Remove.bmp`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.3.1/MacroQueue/Bitmaps/UpArrow.bmp` & `MacroQueue-0.3.2/MacroQueue/Bitmaps/UpArrow.bmp`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.3.1/MacroQueue/Dialogs.py` & `MacroQueue-0.3.2/MacroQueue/Dialogs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1198,17 +1198,18 @@
         for MenuItem in self.Parent.SystemMenuItems:
             MenuItem.Check(False)
         if softwareIndex is not None:
             self.Parent.SystemMenuItems[softwareIndex].Check(True)
             software = self.Parent.Systems[softwareIndex]
             self.Parent.Software = software
             self.Parent.MacroPath = self.Parent.MacroPaths[software]
+            SettingsDict = {"Software":software,'PauseAfterCancel':self.Parent.m_PauseAfterCancel.IsChecked(),'LaunchWithConnect':self.Parent.m_LaunchWithConnect.IsChecked()}
             if self.FunctionsToLoad is None:
-                SettingsDict = {"Software":software,'Functions':['General'],'PauseAfterCancel':self.Parent.m_PauseAfterCancel.IsChecked()}
+                SettingsDict['Functions'] = ['General']
             else:
-                SettingsDict = {"Software":software,'Functions':self.FunctionsToLoad,'PauseAfterCancel':self.Parent.m_PauseAfterCancel.IsChecked()}
+                SettingsDict['Functions'] = self.FunctionsToLoad
                 
             pd.Series(SettingsDict).to_csv(self.SavedSettingsFile,header=False)
             self.Parent.MakeFunctionButtons()
             self.Parent.IncomingQueue.put(["SoftwareChange",[software,self.FunctionsToLoad]])
             
         self.Destroy()
```

### Comparing `MacroQueue-0.3.1/MacroQueue/Functions/BField.py` & `MacroQueue-0.3.2/MacroQueue/Functions/BField.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,17 @@
 
 
 
 
 ChannelDict = {'Y':0,'X':1,'Z':2}
 DirDict = {'p':0,'n':1}
 ZZero = None
-def Set_B_Field_Keep_Away(B=1,LogPath='D:\\LabData\\BFieldLoop.csv'):
+
+# {"Name":"B","Units":"T","Min":-1,"Max":1,"Tooltip":"The magnetic field strength in T"}
+def Set_B_Field_Keep_Tip_Away(B=1,LogPath='D:\\LabData\\BFieldLoop.csv'):
     try:
         STM = MacroQueueSelf.Functions[MacroQueueSelf.Software].STM
     except:
         STM = None
     global BField, BFieldPowerControl, Ramping, ZZero
     if BField is None:
         BField = 0
```

### Comparing `MacroQueue-0.3.1/MacroQueue/Functions/CreaTec.py` & `MacroQueue-0.3.2/MacroQueue/Functions/CreaTec.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.3.1/MacroQueue/Functions/General.py` & `MacroQueue-0.3.2/MacroQueue/Functions/General.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from time import sleep
 
-Systems =['RHK','CreaTec','SXM',"Testing"]
+Systems =['RHK','CreaTec','SXM']
+IgnoreFiles =["SXMRemote.py"]
 
 
 Cancel = False
 MacroQueueSelf = None
```

### Comparing `MacroQueue-0.3.1/MacroQueue/Functions/RF.py` & `MacroQueue-0.3.2/MacroQueue/Functions/RF.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.3.1/MacroQueue/Functions/RHK.py` & `MacroQueue-0.3.2/MacroQueue/Functions/RHK.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.3.1/MacroQueue/Functions/SXM.py` & `MacroQueue-0.3.2/MacroQueue/Functions/SXM.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.3.1/MacroQueue/Functions/SXMRemote.py` & `MacroQueue-0.3.2/MacroQueue/Functions/SXMRemote.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.3.1/MacroQueue/GUIDesign.py` & `MacroQueue-0.3.2/MacroQueue/GUIDesign.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 		self.m_menubar1.Append( self.m_FileMenu, u"File" )
 
 		self.m_OptionsMenu = wx.Menu()
 		self.m_PauseAfterCancel = wx.MenuItem( self.m_OptionsMenu, wx.ID_ANY, u"Pause After Cancel", wx.EmptyString, wx.ITEM_CHECK )
 		self.m_OptionsMenu.Append( self.m_PauseAfterCancel )
 		self.m_PauseAfterCancel.Check( True )
 
+		self.m_LaunchWithConnect = wx.MenuItem( self.m_OptionsMenu, wx.ID_ANY, u"Launch with Connect in Queue", wx.EmptyString, wx.ITEM_CHECK )
+		self.m_OptionsMenu.Append( self.m_LaunchWithConnect )
+		self.m_LaunchWithConnect.Check( True )
+
 		self.m_menuItem17 = wx.MenuItem( self.m_OptionsMenu, wx.ID_ANY, u"Reload Functions"+ u"\t" + u"CTRL+R", wx.EmptyString, wx.ITEM_NORMAL )
 		self.m_OptionsMenu.Append( self.m_menuItem17 )
 
 		self.m_menubar1.Append( self.m_OptionsMenu, u"Options" )
 
 		self.m_MacroMenu = wx.Menu()
 		self.m_MakeMacroMenuItem = wx.MenuItem( self.m_MacroMenu, wx.ID_ANY, u"Make New Macro"+ u"\t" + u"CRTL+M", wx.EmptyString, wx.ITEM_NORMAL )
@@ -57,15 +61,15 @@
 
 		self.m_menubar1.Append( self.m_Connectmenu, u"Connect" )
 
 		self.m_SystemMenu = wx.Menu()
 		self.m_menubar1.Append( self.m_SystemMenu, u"System" )
 
 		self.m_NotSTMMenu = wx.Menu()
-		self.m_menubar1.Append( self.m_NotSTMMenu, u"Included Functions" )
+		self.m_menubar1.Append( self.m_NotSTMMenu, u"Auxiliary Functions" )
 
 		self.m_menu5 = wx.Menu()
 		self.m_menuItem10 = wx.MenuItem( self.m_menu5, wx.ID_ANY, u"Basic Usage", wx.EmptyString, wx.ITEM_NORMAL )
 		self.m_menu5.Append( self.m_menuItem10 )
 
 		self.m_menuItem102 = wx.MenuItem( self.m_menu5, wx.ID_ANY, u"Expand Numerical Parameters", wx.EmptyString, wx.ITEM_NORMAL )
 		self.m_menu5.Append( self.m_menuItem102 )
@@ -139,14 +143,15 @@
 		self.Centre( wx.BOTH )
 
 		# Connect Events
 		self.Bind( wx.EVT_CLOSE, self.OnClose )
 		self.Bind( wx.EVT_IDLE, self.IdleLoop )
 		self.Bind( wx.EVT_SIZE, self.OnSize )
 		self.Bind( wx.EVT_MENU, self.OpenSourceFolder, id = self.m_SourceMenuItem.GetId() )
+		self.Bind( wx.EVT_MENU, self.OnLaunchConnect, id = self.m_LaunchWithConnect.GetId() )
 		self.Bind( wx.EVT_MENU, self.ReloadFunctions, id = self.m_menuItem17.GetId() )
 		self.Bind( wx.EVT_MENU, self.StartMakeNewMacro, id = self.m_MakeMacroMenuItem.GetId() )
 		self.Bind( wx.EVT_MENU, self.OpenMacroFile, id = self.m_OpenMacroMenuItem.GetId() )
 		self.Bind( wx.EVT_MENU, self.AddConnectToQueue, id = self.m_menuItem7.GetId() )
 		self.Bind( wx.EVT_MENU, self.AddDisconnectToQueue, id = self.m_menuItem8.GetId() )
 		self.Bind( wx.EVT_MENU, self.BasicUseageHelp, id = self.m_menuItem10.GetId() )
 		self.Bind( wx.EVT_MENU, self.ExpandNumericalParameters, id = self.m_menuItem102.GetId() )
@@ -171,14 +176,17 @@
 
 	def OnSize( self, event ):
 		event.Skip()
 
 	def OpenSourceFolder( self, event ):
 		event.Skip()
 
+	def OnLaunchConnect( self, event ):
+		event.Skip()
+
 	def ReloadFunctions( self, event ):
 		event.Skip()
 
 	def StartMakeNewMacro( self, event ):
 		event.Skip()
 
 	def OpenMacroFile( self, event ):
```

### Comparing `MacroQueue-0.3.1/MacroQueue/MacroQueue.py` & `MacroQueue-0.3.2/MacroQueue/MacroQueue.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,27 +49,34 @@
 
 # BUG:
 # Canceled during move to image start of a dIdV scan and it stopped responding.
 
 # TODO:
 # Show number of items in queue in status bar
 
-VersionNumber = "v0.3.1"
+VersionNumber = "v0.3.2"
 # VersionNumber also in conf.py & setup.py
 Date = "4/2024"
 
 
 class MacroQueue(MyFrame):
     try:
         import General
         Systems = General.Systems
     except:
         Systems =['RHK','CreaTec','SXM',"Testing"]
+    try:
+        import General
+        IgnoreFiles = General.IgnoreFiles
+    except:
+        IgnoreFiles =["SXMRemote.py"]
+
     NotAuxFiles = [f"{system}.py" for system in Systems]
-    NotAuxFiles.append("SXMRemote.py")
+    for Ignorefile in IgnoreFiles:
+        NotAuxFiles.append(Ignorefile)
     MacroPaths = {system:f"Macros//{system}Macro.json" for system in Systems}
 
 # Scanning, fine motion, course motion, dI/dV scans, point spectra, tip form, 
     TheQueue = []
     AddToQueue = []
     FunctionsLoaded = []
     Paused = True
@@ -128,14 +135,16 @@
         if os.path.exists(self.SavedSettingsFile) and not self.test:
             SettingsSeries = pd.read_csv(self.SavedSettingsFile,names=['key','value'])
             self.SettingsDict = SettingsSeries.set_index('key').T.iloc[0].to_dict()
             if "Functions" in self.SettingsDict.keys():
                 self.FunctionsLoaded = [string.replace(" ", "").replace("'", "") for string in (self.SettingsDict["Functions"][1:-1].split(','))]
             if "PauseAfterCancel" in self.SettingsDict.keys():
                 self.m_PauseAfterCancel.Check(self.SettingsDict['PauseAfterCancel'] != 'False')
+            if "LaunchWithConnect" in self.SettingsDict.keys():
+                self.m_LaunchWithConnect.Check(self.SettingsDict['LaunchWithConnect'] != 'False')
             self.Software = self.SettingsDict["Software"]
             ThisChooseSoftwareDialog = MyChooseSoftwareDialog(self,self.FunctionsLoaded)
             ThisChooseSoftwareDialog.SetSoftware(self.Systems.index(self.Software))
             
             for item in self.m_NotSTMMenu.GetMenuItems():
                 if item.GetItemLabel() in self.FunctionsLoaded:
                     item.Check()
@@ -171,15 +180,16 @@
         self.m_QueueWindow.SetSizer(self.m_FunctionNameSizer)
         dt = MyPanelDropTarget(self.m_QueueWindow,self)
         self.m_QueueWindow.SetDropTarget(dt)
         def OnQueueSize(event):
             # self.m_QueueWindow.Layout()
             self.m_QueueWindow.FitInside()
         self.m_QueueWindow.Bind( wx.EVT_SIZE, OnQueueSize )
-        self.AddConnectToQueue()
+        if self.m_LaunchWithConnect.IsChecked():
+            self.AddConnectToQueue()
         self.Show()
 
     def CheckQueue(self,event):
         # This funtion runs on a timer.  Twice a second.
         try:
             # A try loop to ignore any queue.Empty exceptions 
             Message = self.OutgoingQueue.get(False)
@@ -781,17 +791,21 @@
     def AddDisconnectToQueue(self, event=None):
         OnClose = [['OnClose',{},True],['Pause',{},True]]
         ThisStartMacroDialog = MyStartMacroDialog(self,"Disconnect",OnClose)
         ThisStartMacroDialog.AddToQueue()
         self.AddConnectToQueue()
         return
     def OnSoftware(self,i,event):
-        ThisChooseSoftwareDialog = MyChooseSoftwareDialog(self)
+        ThisChooseSoftwareDialog = MyChooseSoftwareDialog(self,self.FunctionsLoaded)
         ThisChooseSoftwareDialog.SetSoftware(i)
 
+    def OnLaunchConnect(self,event):
+        ThisChooseSoftwareDialog = MyChooseSoftwareDialog(self,self.FunctionsLoaded)
+        ThisChooseSoftwareDialog.SetSoftware(self.Systems.index(self.Software))
+        pass
     def PauseAfterCancel(self,event):
         ThisChooseSoftwareDialog = MyChooseSoftwareDialog(self,self.FunctionsLoaded)
         ThisChooseSoftwareDialog.SetSoftware(self.Systems.index(self.Software))
         pass
     def ReloadFunctions(self,event):
         self.LoadFunctions(Reloading=True)
         self.IncomingQueue.put(["SoftwareChange",[self.Software,self.FunctionsLoaded]])
```

### Comparing `MacroQueue-0.3.1/MacroQueue/MacroQueueIcon.ico` & `MacroQueue-0.3.2/MacroQueue/MacroQueueIcon.ico`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.3.1/MacroQueue/MakeExe.sh` & `MacroQueue-0.3.2/MacroQueue/MakeExe.sh`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.3.1/MacroQueue/__init__.py` & `MacroQueue-0.3.2/MacroQueue/__init__.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.3.1/MacroQueue.egg-info/PKG-INFO` & `MacroQueue-0.3.2/MacroQueue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: MacroQueue
-Version: 0.3.1
+Version: 0.3.2
 Summary: Automating Scanning Probe Microscopy
 Home-page: https://github.com/guptagroupstm/STMMacroQueue
-Download-URL: https://github.com/guptagroupstm/STMMacroQueue/archive/refs/tags/v0.3.1.tar.gz
+Download-URL: https://github.com/guptagroupstm/STMMacroQueue/archive/refs/tags/v0.3.2.tar.gz
 Author: Brad Goff
 Author-email: guptagroupstm@gmail.com
 License: MIT
 Keywords: Automation,Scanning Probe Microscopy,Macro,Queue
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `MacroQueue-0.3.1/MacroQueue.egg-info/SOURCES.txt` & `MacroQueue-0.3.2/MacroQueue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.3.1/PKG-INFO` & `MacroQueue-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: MacroQueue
-Version: 0.3.1
+Version: 0.3.2
 Summary: Automating Scanning Probe Microscopy
 Home-page: https://github.com/guptagroupstm/STMMacroQueue
-Download-URL: https://github.com/guptagroupstm/STMMacroQueue/archive/refs/tags/v0.3.1.tar.gz
+Download-URL: https://github.com/guptagroupstm/STMMacroQueue/archive/refs/tags/v0.3.2.tar.gz
 Author: Brad Goff
 Author-email: guptagroupstm@gmail.com
 License: MIT
 Keywords: Automation,Scanning Probe Microscopy,Macro,Queue
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `MacroQueue-0.3.1/README.md` & `MacroQueue-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.3.1/setup.py` & `MacroQueue-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 # read the contents of your README file
   from pathlib import Path
   this_directory = Path(__file__).parent
   long_description = (this_directory / "README.md").read_text()
 setup(
   name = 'MacroQueue',         # How you named your package folder (MyLib)
   packages = ['MacroQueue'],   # Chose the same as "name"
-  version = '0.3.1',      # Start with a small number and increase it with every change you make
+  version = '0.3.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Automating Scanning Probe Microscopy',   # Give a short description about your library
   author = 'Brad Goff',                   # Type in your name
   author_email = 'guptagroupstm@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/guptagroupstm/STMMacroQueue',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/guptagroupstm/STMMacroQueue/archive/refs/tags/v0.3.1.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/guptagroupstm/STMMacroQueue/archive/refs/tags/v0.3.2.tar.gz',    # I explain this later on
   keywords = ['Automation', 'Scanning Probe Microscopy', 'Macro',"Queue"],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'pandas',
           'wxPython',
           'pyvisa',
           'PyWin32',
           'pyinstaller'
```

### Comparing `MacroQueue-0.3.1/test/test_MainFrame.py` & `MacroQueue-0.3.2/test/test_MainFrame.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.3.1/test/test_STMthread.py` & `MacroQueue-0.3.2/test/test_STMthread.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.3.1/test/test_readdata.py` & `MacroQueue-0.3.2/test/test_readdata.py`

 * *Files identical despite different names*

