# Comparing `tmp/DynamicRoutingTask-0.1.94.tar.gz` & `tmp/DynamicRoutingTask-0.1.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DynamicRoutingTask-0.1.94.tar", last modified: Fri Mar 29 23:53:41 2024, max compression
+gzip compressed data, was "DynamicRoutingTask-0.1.95.tar", last modified: Tue Apr  9 01:02:14 2024, max compression
```

## Comparing `DynamicRoutingTask-0.1.94.tar` & `DynamicRoutingTask-0.1.95.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 23:53:41.613720 DynamicRoutingTask-0.1.94/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 23:53:41.613720 DynamicRoutingTask-0.1.94/Analysis/
--rw-r--r--   0 runner    (1001) docker     (127)    34708 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/Analysis/DynamicRoutingAnalysisUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    64403 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/Analysis/RLmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    13100 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/Analysis/RLmodelHPC.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/Analysis/RLmodelSlurm.py
--rw-r--r--   0 runner    (1001) docker     (127)    34502 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/Analysis/RLmodel_old.py
--rw-r--r--   0 runner    (1001) docker     (127)    18931 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/Analysis/behaviorClustering.py
--rw-r--r--   0 runner    (1001) docker     (127)   124608 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/Analysis/dr_analysis_sam.py
--rw-r--r--   0 runner    (1001) docker     (127)   109301 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/Analysis/dr_behav_figs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18638 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/Analysis/dr_ephys_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    21061 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/Analysis/glm_hmm_sam.py
--rw-r--r--   0 runner    (1001) docker     (127)    32899 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/Analysis/ncb_meeting_01272023.py
--rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/Analysis/npc_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    87697 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/Analysis/presentation_June2023.py
--rw-r--r--   0 runner    (1001) docker     (127)    13758 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/Analysis/regressionModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    69812 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/Analysis/sac_may2023.py
--rw-r--r--   0 runner    (1001) docker     (127)    17010 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/Analysis/sessionSummaryFigs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/Analysis/sound_ephys_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/Analysis/sound_sync_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/Analysis/variableBlockDur.py
--rw-r--r--   0 runner    (1001) docker     (127)    56355 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/DynamicRouting1.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/DynamicRouting1_postSessionAnalysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 23:53:41.613720 DynamicRoutingTask-0.1.94/DynamicRoutingTask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-29 23:53:41.000000 DynamicRoutingTask-0.1.94/DynamicRoutingTask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-03-29 23:53:41.000000 DynamicRoutingTask-0.1.94/DynamicRoutingTask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 23:53:41.000000 DynamicRoutingTask-0.1.94/DynamicRoutingTask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-29 23:53:41.000000 DynamicRoutingTask-0.1.94/DynamicRoutingTask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-29 23:53:41.000000 DynamicRoutingTask-0.1.94/DynamicRoutingTask.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 23:53:41.613720 DynamicRoutingTask-0.1.94/OptoGui/
--rw-r--r--   0 runner    (1001) docker     (127)    34068 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/OptoGui/OptoGui.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/OptoTagging.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-29 23:53:41.613720 DynamicRoutingTask-0.1.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/RFMapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 23:53:41.613720 DynamicRoutingTask-0.1.94/SamStimGui/
--rw-r--r--   0 runner    (1001) docker     (127)    15618 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/SamStimGui/SamStimGui.py
--rw-r--r--   0 runner    (1001) docker     (127)    61122 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/TaskControl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/TaskUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/camstimControl.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-29 23:53:39.000000 DynamicRoutingTask-0.1.94/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     5846 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/runTask.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 23:53:41.613720 DynamicRoutingTask-0.1.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-03-29 23:53:17.000000 DynamicRoutingTask-0.1.94/startTask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:02:14.814663 DynamicRoutingTask-0.1.95/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:02:14.814663 DynamicRoutingTask-0.1.95/Analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)    34540 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/DynamicRoutingAnalysisUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64516 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/RLmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/RLmodelHPC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/RLmodelSlurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34502 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/RLmodel_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18931 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/behaviorClustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)   124608 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/dr_analysis_sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)   110108 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/dr_behav_figs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18638 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/dr_ephys_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21061 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/glm_hmm_sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32899 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/ncb_meeting_01272023.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/npc_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87697 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/presentation_June2023.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13758 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/regressionModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69812 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/sac_may2023.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17010 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/sessionSummaryFigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/sound_ephys_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/sound_sync_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/Analysis/variableBlockDur.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56355 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/DynamicRouting1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/DynamicRouting1_postSessionAnalysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:02:14.814663 DynamicRoutingTask-0.1.95/DynamicRoutingTask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-09 01:02:14.000000 DynamicRoutingTask-0.1.95/DynamicRoutingTask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-09 01:02:14.000000 DynamicRoutingTask-0.1.95/DynamicRoutingTask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 01:02:14.000000 DynamicRoutingTask-0.1.95/DynamicRoutingTask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-09 01:02:14.000000 DynamicRoutingTask-0.1.95/DynamicRoutingTask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-09 01:02:14.000000 DynamicRoutingTask-0.1.95/DynamicRoutingTask.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:02:14.814663 DynamicRoutingTask-0.1.95/OptoGui/
+-rw-r--r--   0 runner    (1001) docker     (127)    34068 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/OptoGui/OptoGui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/OptoTagging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-09 01:02:14.814663 DynamicRoutingTask-0.1.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/RFMapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:02:14.814663 DynamicRoutingTask-0.1.95/SamStimGui/
+-rw-r--r--   0 runner    (1001) docker     (127)    15618 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/SamStimGui/SamStimGui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62349 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/TaskControl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/TaskUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/camstimControl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-09 01:02:11.000000 DynamicRoutingTask-0.1.95/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     5846 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/runTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 01:02:14.814663 DynamicRoutingTask-0.1.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-09 01:01:27.000000 DynamicRoutingTask-0.1.95/startTask.py
```

### Comparing `DynamicRoutingTask-0.1.94/Analysis/DynamicRoutingAnalysisUtils.py` & `DynamicRoutingTask-0.1.95/Analysis/DynamicRoutingAnalysisUtils.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,16 +281,14 @@
             if ((stage in (1,2) and all(h[0] >= hitThresh for h in hits) and all(d[0] >= dprimeThresh for d in dprimeSame)) or
                 (stage==5 and np.all(np.sum((np.array(dprimeSame) >= dprimeThresh) & (np.array(dprimeOther) >= dprimeThresh),axis=1) > 3))):
                 sessionsToPass = np.where(sessions==sessionInd)[0][0] + 1
                 break
     if np.isnan(sessionsToPass):
         if stage in (1,2) and mouseId in (614910,684071,682893):
             sessionsToPass = len(sessions)
-        elif stage==5 and  mouseId in (677352,688770):
-            sessionsToPass = np.where(['timeouts' in task for task in  df['task version'][sessions]])[0][-1] + 1
     return sessionsToPass
 
 
 def getSessionData(mouseId,startTime):
     if not isinstance(startTime,str):
         startTime = startTime.strftime('%Y%m%d_%H%M%S')
     fileName = 'DynamicRouting1_' + str(mouseId) + '_' + startTime + '.hdf5'
```

### Comparing `DynamicRoutingTask-0.1.94/Analysis/RLmodel.py` & `DynamicRoutingTask-0.1.95/Analysis/RLmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,24 +98,24 @@
 clusterColors = 'krgb'
 if fitClusters:
     trainingPhaseNames = ('clusters',)
     trainingPhaseColors = 'k'
 else:
     trainingPhaseNames = ('initial training','after learning')#,'nogo','noAR','rewardOnly','no reward')
     trainingPhaseColors = 'mgrbck'
-modelTypeNames = ('basicRL','contextRLmultiState','contextRLmultiStateRPE','contextRLweightStates','contextRLweightStatesRPE')
-modelTypeColors = 'krmbc'
+modelTypeNames = ('basicRL','basicRLvectorRPE','contextRLmultiState','contextRLmultiStateRPE','contextRLweightStates','contextRLweightStatesRPE')
+modelTypeColors = 'kgrmbc'
 
 paramNames = {}
 paramBounds = {}
 fixedParamNames = {}
 fixedParamValues = {}
 nModelParams = {}
 for modelType in modelTypeNames:
-    if modelType == 'basicRL':
+    if modelType in ('basicRL','basicRLvectorRPE'):
         paramNames[modelType] = ('betaAction','biasAction','biasAttention','visConf','audConf','alphaReward','alphaStim')
         paramBounds[modelType] = ([0,40],[-1,1],[-1,1],[0.5,1],[0.5,1],[0,1],[0,1])
         if fitClusters:
             fixedParamNames[modelType] = ('Full model','alphaStim')
             fixedParamValues[modelType] = (None,0)
             nModelParams[modelType] = (7,5)
         else:
@@ -293,15 +293,15 @@
                         dprime.append(calcDprime(hitRate,falseAlarmRate,hitTrials,falseAlarmTrials))
                 performanceData[trainingPhase][modelType][fixedParam]['respFirst'].append(np.mean(respFirst))
                 performanceData[trainingPhase][modelType][fixedParam]['respLast'].append(np.mean(respLast))
                 performanceData[trainingPhase][modelType][fixedParam]['dprime'].append(np.mean(dprime))
 
 
 # plot performance data
-for modelType in ('basicRL',):
+for modelType in ('basicRL','basicRLvectorRPE'):
     fig = plt.figure(figsize=(10,4))
     ax = fig.add_subplot(1,1,1)
     xlbls = ('mice',) + fixedParamNames[modelType]
     for trainingPhase,clr in zip(trainingPhases,trainingPhaseColors):
         for x,lbl in enumerate(xlbls):
             d = performanceData[trainingPhase][modelType][lbl]['dprime']
             m = np.mean(d)
@@ -347,15 +347,15 @@
 ax.set_xlim([-0.25,len(xlbls)+0.25])
 # ax.set_ylim([0,0.7])
 ax.set_ylabel('cross-modal d\'')
 ax.set_title('after learning')
 ax.legend(loc='lower left')
 plt.tight_layout()
     
-for modelType in ('basicRL',):
+for modelType in ('basicRL','basicRLvectorRPE'):
     fig = plt.figure(figsize=(10,4))
     ax = fig.add_subplot(1,1,1)
     xlbls = ('mice',) + fixedParamNames[modelType]
     ax.plot([-1,len(xlbls)+1],[0,0],'k--')
     for trainingPhase,clr in zip(trainingPhases,trainingPhaseColors):
         for x,lbl in enumerate(xlbls):
             respFirst = performanceData[trainingPhase][modelType][lbl]['respFirst']
@@ -435,15 +435,15 @@
 ax.set_xticklabels(['Naive model\n(constant response probability)'] + modelTypes)
 ax.set_xlim([-0.25,len(xlbls)+0.25])
 ax.set_ylim([0,0.7])
 ax.set_ylabel('Negative log-likelihood')
 ax.legend(loc='lower right')
 plt.tight_layout()
 
-for modelType in ('basicRL',):
+for modelType in ('basicRL','basicRLvectorRPE'):
     fig = plt.figure(figsize=(10,4))
     ax = fig.add_subplot(1,1,1)
     xticks = np.arange(len(fixedParamNames[modelType]))
     xlim = [-0.25,xticks[-1]+0.25]
     ax.plot(xlim,[0,0],'--',color='0.5')
     for trainingPhase,clr in zip(trainingPhases,trainingPhaseColors):
         d = modelData[trainingPhase]
@@ -488,15 +488,15 @@
 ax.set_xticklabels([fixedParamNames[modelType][0]]+[name+'='+str(val) for name,val in zip(fixedParamNames[modelType][1:],fixedParamValues[modelType][1:])])
 ax.set_xlim(xlim)
 ax.set_ylabel(r'$\Delta$ NLL')
 ax.set_title('after learning')
 ax.legend(loc='upper left')
 plt.tight_layout()
 
-for modelType in modelTypes[:1]:
+for modelType in modelTypes[:2]:
     fig = plt.figure(figsize=(5,10))
     for i,(fixedParam,fixedVal) in enumerate(zip(fixedParamNames[modelType],fixedParamValues[modelType])):
         ax = fig.add_subplot(len(fixedParamNames[modelType]),1,i+1)
         ax.plot([0,0],[0,1],'--',color='0.5')
         for trainingPhase,clr in zip(trainingPhases,trainingPhaseColors):
             d = modelData[trainingPhase]
             if len(d) > 0:
@@ -548,15 +548,15 @@
     ax.set_title((fixedParam if fixedParam == 'Full model' else fixedParam+'='+str(fixedVal)))
     if i==0:
         ax.legend(loc='upper left',bbox_to_anchor=(1,1))
 plt.tight_layout()
                 
                 
 # plot param values
-for modelType in ('basicRL',):
+for modelType in ('basicRL','basicRLvectorRPE'):
     fig = plt.figure(figsize=(11,11))
     gs = matplotlib.gridspec.GridSpec(len(fixedParamNames[modelType]),len(paramNames[modelType]))
     for i,(fixedParam,fixedVal) in enumerate(zip(fixedParamNames[modelType],fixedParamValues[modelType])):
         for j,(param,xlim) in enumerate(zip(paramNames[modelType],paramBounds[modelType])):
             ax = fig.add_subplot(gs[i,j])
             for trainingPhase,clr in zip(trainingPhases,trainingPhaseColors):
                 d = modelData[trainingPhase]
@@ -623,21 +623,21 @@
             ax.set_title((fixedParam+'(after learning)' if fixedParam == 'Full model' else fixedParam+'='+str(fixedVal)))
         if i==0 and j==len(paramNames[modelType])-1:
             ax.legend(bbox_to_anchor=(1,1))
 plt.tight_layout()
 
 
 # compare model and mice
-for modelType in modelTypes[1:]:
+for modelType in modelTypes[:2]:
     var = 'prediction'
     stimNames = ('vis1','vis2','sound1','sound2')
     preTrials = 5
     postTrials = 15
     x = np.arange(-preTrials,postTrials+1)
-    for trainingPhase in trainingPhases[1:]:
+    for trainingPhase in trainingPhases:
         fig = plt.figure(figsize=(12,10))
         nRows = int(np.ceil((len(fixedParamNames[modelType])+1)/2))
         gs = matplotlib.gridspec.GridSpec(nRows,4)
         for i,(fixedParam,fixedVal) in enumerate(zip(('mice',) + fixedParamNames[modelType],(None,)+fixedParamValues[modelType])):
             if fixedParam == 'mice':
                 d = sessionData[trainingPhase]
             else:
@@ -646,15 +646,15 @@
                 continue
             for j,(rewardStim,blockLabel) in enumerate(zip(('vis1','sound1'),('visual rewarded blocks','sound rewarded blocks'))):
                 if i>=nRows:
                     row = i-nRows
                     col = j+2
                 else:
                     row,col = i,j
-                if modelType != 'basicRL' and col>1:
+                if 'basicRL' not in modelType and col>1:
                     row += 1
                 ax = fig.add_subplot(gs[row,col])
                 for stim,clr,ls in zip(stimNames,'ggmm',('-','--','-','--')):
                     y = []
                     for mouse in d:
                         y.append([])
                         for session in d[mouse]:
```

### Comparing `DynamicRoutingTask-0.1.94/Analysis/RLmodelHPC.py` & `DynamicRoutingTask-0.1.95/Analysis/RLmodelHPC.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 
 def calcLogisticProb(q,beta,bias):
     return 1 / (1 + np.exp(-beta * (q - 0.5 + bias)))
 
 
 def runModel(obj,betaAction,biasAction,biasAttention,visConfidence,audConfidence,alphaReward,alphaStim,
-             alphaContext,decayContext,alphaHabit,weightAttention=False,useRPE=False,useHistory=True,nReps=1):
+             alphaContext,decayContext,alphaHabit,weightAttention=False,useRPE=False,scalarRPE=True,useHistory=True,nReps=1):
 
     stimNames = ('vis1','vis2','sound1','sound2')
     stimConfidence = [visConfidence,audConfidence]
     modality = 0
 
     pContext = 0.5 + np.zeros((nReps,obj.nTrials,2))
 
@@ -121,15 +121,21 @@
                 qContext[i,trial+1] = qContext[i,trial]
                 qStim[i,trial+1] = qStim[i,trial]
                 wHabit[i,trial+1] = wHabit[i,trial]
                 wReward[i,trial+1] = wReward[i,trial]
                 
                 if action[i,trial] or obj.autoRewarded[trial]:
                     outcome = 1 if stim == obj.rewardedStim[trial] or obj.autoRewarded[trial] else 0
-                    predictionError = outcome - expectedValue[i,trial]
+                    if scalarRPE:
+                        predictionError = outcome - expectedValue[i,trial]
+                    else:
+                        if weightAttention or alphaContext == 0:
+                            predictionError = outcome - qStim[i,trial]
+                        else:
+                            predictionError = outcome - qContext[i,trial]
                     
                     if stim != 'catch':
                         if alphaContext > 0:
                             if useRPE:
                                 contextError = predictionError
                             else:
                                 if outcome:
@@ -199,29 +205,30 @@
     alphaHabitBounds = (0,1)
 
     bounds = (betaActionBounds,biasActionBounds,biasAttentionBounds,visConfidenceBounds,audConfidenceBounds,
               alphaRewardBounds,alphaStimBounds,alphaContextBounds,decayContextBounds,alphaHabitBounds)
 
     fixedValues = [None,0,0,1,1,0,0,0,0,0]
 
-    modelTypeParamNames = ('weightAttention','useRPE')
+    modelTypeParamNames = ('weightAttention','useRPE','scalarRPE')
     modelTypeNames,modelTypes = zip(
-                                    ('basicRL', (0,0)),
-                                    ('contextRLmultiState',(0,0)),
-                                    ('contextRLmultiStateRPE',(0,1)),
-                                    ('contextRLweightStates',(1,0)),
-                                    ('contextRLweightStatesRPE',(1,1)),
+                                    #('basicRL', (0,0,1)),
+                                    ('basicRLvectorRPE', (0,0,0)),
+                                    #('contextRLmultiState',(0,0,1)),
+                                    #('contextRLmultiStateRPE',(0,1,1)),
+                                    #('contextRLweightStates',(1,0,1)),
+                                    #('contextRLweightStatesRPE',(1,1,1)),
                                    )
 
     clustIds = np.arange(4)+1 if trainingPhase == 'clusters' else (None,)
 
     optParams = {'eps': 1e-4, 'maxfun': int(1e4),'maxiter': int(1e3),'locally_biased': True,'vol_tol': 1e-16,'len_tol': 1e-6}
 
     for modelTypeName,modelType in zip(modelTypeNames,modelTypes):
-        if modelTypeName == 'basicRL':
+        if 'basicRL' in modelTypeName:
             if trainingPhase == 'clusters':
                 fixedParamIndices = ([7,8,9],[6,7,8,9])
             else:
                 fixedParamIndices = [[7,8,9]] + [[7,8,9] + [i] for i in range(1,7)]
         else:
             if trainingPhase == 'clusters':
                 fixedParamIndices = (9,[6,9])
```

### Comparing `DynamicRoutingTask-0.1.94/Analysis/RLmodelSlurm.py` & `DynamicRoutingTask-0.1.95/Analysis/RLmodelSlurm.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
               time='24:00:00',
               mem_per_cpu='1gb')
 
 summarySheets = pd.read_excel('/allen/programs/mindscope/workgroups/dynamicrouting/Sam/BehaviorSummary.xlsx',sheet_name=None)
 summaryDf = pd.concat((summarySheets['not NSB'],summarySheets['NSB']))
 drSheets,nsbSheets = [pd.read_excel(os.path.join('/allen/programs/mindscope/workgroups/dynamicrouting/DynamicRoutingTask',fileName),sheet_name=None) for fileName in ('DynamicRoutingTraining.xlsx','DynamicRoutingTrainingNSB.xlsx')]
 trainingPhases = ('initial training','after learning','nogo','noAR','rewardOnly','no reward','clusters')
-for trainingPhase in trainingPhases[-1:]:
+for trainingPhase in trainingPhases[:2]:
     if trainingPhase in ('initial training','after learning','clusters'):
         hasIndirectRegimen = np.array(summaryDf['stage 3 alt'] | summaryDf['stage 3 distract'] | summaryDf['stage 4'] | summaryDf['stage var'])
         ind = ~hasIndirectRegimen & summaryDf['stage 5 pass'] & summaryDf['moving grating'] & summaryDf['AM noise'] & ~summaryDf['cannula'] & ~summaryDf['stage 5 repeats']
         mice = np.array(summaryDf[ind]['mouse id'])
         if trainingPhase == 'clusters':
             nSessions = []
             for mouseId in mice:
```

### Comparing `DynamicRoutingTask-0.1.94/Analysis/RLmodel_old.py` & `DynamicRoutingTask-0.1.95/Analysis/RLmodel_old.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.94/Analysis/behaviorClustering.py` & `DynamicRoutingTask-0.1.95/Analysis/behaviorClustering.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.94/Analysis/dr_analysis_sam.py` & `DynamicRoutingTask-0.1.95/Analysis/dr_analysis_sam.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.94/Analysis/dr_behav_figs.py` & `DynamicRoutingTask-0.1.95/Analysis/dr_behav_figs.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 
 summarySheets = pd.read_excel(os.path.join(baseDir,'Sam','BehaviorSummary.xlsx'),sheet_name=None)
 summaryDf = pd.concat((summarySheets['not NSB'],summarySheets['NSB']))
 
 drSheets = pd.read_excel(os.path.join(baseDir,'DynamicRoutingTask','DynamicRoutingTraining.xlsx'),sheet_name=None)
 nsbSheets = pd.read_excel(os.path.join(baseDir,'DynamicRoutingTask','DynamicRoutingTrainingNSB.xlsx'),sheet_name=None)
 
+miceToIgnore = summaryDf['wheel fixed'] & summaryDf['cannula']
+
 hasIndirectRegimen = np.array(summaryDf['stage 3 alt'] | summaryDf['stage 3 distract'] | summaryDf['stage 4'] | summaryDf['stage var'])
 
 hitThresh = 100
 dprimeThresh = 1.5
 
 deltaLickProbLabels = ('5 rewarded/auto-rewarded targets',
                        '1 rewarded target',
@@ -159,89 +161,103 @@
     ax.set_xlim(xlim)
     ax.set_ylim([0,1.01])
     ax.set_xlabel('Sessions to pass',fontsize=14)
     ax.set_ylabel('Cumalative fraction',fontsize=14)
     plt.legend(loc='lower right')
     plt.tight_layout()
     
+    
+## drop out summary
+stage1Mice = summaryDf['moving grating'] & summaryDf['timeouts'] & ~miceToIgnore 
+print(np.sum(stage1Mice & summaryDf['stage 1 pass']),'of',np.sum(stage1Mice),'passed')
+summaryDf[stage1Mice & ~summaryDf['stage 1 pass']]['reason for early termination']
+
+stage2Mice = stage1Mice & summaryDf['stage 1 pass'] & summaryDf['AM noise']
+print(np.sum(stage2Mice & summaryDf['stage 2 pass']),'of',np.sum(stage2Mice),'passed')
+summaryDf[stage2Mice & ~summaryDf['stage 2 pass']]['reason for early termination']
+
+stage5Mice = ~summaryDf['nsb'] & ~summaryDf['alive'] & stage2Mice & summaryDf['stage 2 pass'] & ~(summaryDf['reason for early termination']=='ephys before stage 5') & ~hasIndirectRegimen & ~summaryDf['stage 5 repeats']
+print(np.sum(stage5Mice & summaryDf['stage 5 pass']),'of',np.sum(stage5Mice),'passed')
+summaryDf[stage5Mice & ~summaryDf['stage 5 pass']]['reason for early termination']
+    
 
 ## stage 1, stationary gratings with or without timeouts
-ind = summaryDf['stage 1 pass'] & summaryDf['stat grating'] & ~summaryDf['wheel fixed'] & ~summaryDf['cannula']
+ind = summaryDf['stage 1 pass'] & summaryDf['stat grating'] & ~miceToIgnore
 mice = {'stationary, timeouts': np.array(summaryDf[ind & summaryDf['timeouts']]['mouse id']),
         'stationary, no timeouts': np.array(summaryDf[ind & ~summaryDf['timeouts']]['mouse id'])}
 plotLearning(mice,stage=1,xlim=(0.5,20.5))
 
 # stage 1, stationary vs moving gratings, both with timeouts
-ind = summaryDf['stage 1 pass'] & summaryDf['timeouts'] & ~summaryDf['wheel fixed'] & ~summaryDf['cannula']
+ind = summaryDf['stage 1 pass'] & summaryDf['timeouts'] & ~miceToIgnore
 mice = {'moving':  np.array(summaryDf[ind & summaryDf['moving grating']]['mouse id']),
         'stationary': np.array(summaryDf[ind & summaryDf['stat grating']]['mouse id'])}
 plotLearning(mice,stage=1,xlim=(0.5,20.5))
 
 # stage 1, moving gratings with or without reward clicks
-ind = summaryDf['stage 1 pass'] & summaryDf['moving grating'] & summaryDf['timeouts'] & ~summaryDf['cannula']
+ind = summaryDf['stage 1 pass'] & summaryDf['moving grating'] & summaryDf['timeouts'] & ~miceToIgnore
 mice = {'moving, reward click': np.array(summaryDf[ind & summaryDf['reward click']]['mouse id']),
         'moving, no reward click':  np.array(summaryDf[ind & ~summaryDf['reward click']]['mouse id'])}
 plotLearning(mice,stage=1,xlim=(0.5,20.5))
 
 # stage 1, moving gratings with early or late autorewards
-ind = summaryDf['stage 1 pass'] & summaryDf['moving grating'] & summaryDf['timeouts'] & ~summaryDf['cannula']
+ind = summaryDf['stage 1 pass'] & summaryDf['moving grating'] & summaryDf['timeouts'] & ~miceToIgnore
 mice = {'moving, early AR': np.array(summaryDf[ind & ~summaryDf['late autoreward (stage 1)']]['mouse id']),
         'moving, late AR':  np.array(summaryDf[ind & summaryDf['late autoreward (stage 1)']]['mouse id'])}
 plotLearning(mice,stage=1,xlim=(0.5,20.5))
                 
 
 # stage 2, tones, timeouts with noise vs no timeouts
-ind = summaryDf['stage 2 pass'] & summaryDf['tone'] & ~summaryDf['wheel fixed'] & ~summaryDf['cannula']
+ind = summaryDf['stage 2 pass'] & summaryDf['tone'] & ~summaryDf['wheel fixed'] & ~miceToIgnore
 mice = {'tones, timeouts': np.array(summaryDf[ind & summaryDf['timeouts']]['mouse id']),
         'tones, no timeouts':  np.array(summaryDf[ind  & ~summaryDf['timeouts']]['mouse id'])}
 plotLearning(mice,stage=2)
 
 # stage 2, tones with noise timeouts vs AMN with noiseless timeouts
-ind = summaryDf['stage 2 pass'] & summaryDf['timeouts'] & ~summaryDf['wheel fixed'] & ~summaryDf['cannula']
+ind = summaryDf['stage 2 pass'] & summaryDf['timeouts'] & ~summaryDf['wheel fixed'] & ~miceToIgnore
 mice = {'tones': np.array(summaryDf[ind & summaryDf['tone']]['mouse id']),
         'AM noise':  np.array(summaryDf[ind & summaryDf['AM noise']]['mouse id'])}
 plotLearning(mice,stage=2)
 
 # stage 2, AMN
-ind = summaryDf['stage 2 pass'] & summaryDf['AM noise'] & summaryDf['timeouts'] & ~summaryDf['cannula']
+ind = summaryDf['stage 2 pass'] & summaryDf['AM noise'] & summaryDf['timeouts'] & ~miceToIgnore
 mice = {'AM noise': np.array(summaryDf[ind]['mouse id'])}
 plotLearning(mice,stage=2)
 
 # stage 2, AMN with or without reward clicks
-ind = summaryDf['stage 2 pass'] & summaryDf['AM noise'] & summaryDf['timeouts'] & ~summaryDf['cannula']
+ind = summaryDf['stage 2 pass'] & summaryDf['AM noise'] & summaryDf['timeouts'] & ~miceToIgnore
 mice = {'AM noise, reward click': np.array(summaryDf[ind & summaryDf['reward click']]['mouse id']),
         'AM noise, no reward click':  np.array(summaryDf[ind & ~summaryDf['reward click']]['mouse id'])}
 plotLearning(mice,stage=2)
 
 # stage 2, AMN with early or late autorewwards
-ind = summaryDf['stage 2 pass'] & summaryDf['AM noise'] & summaryDf['timeouts'] & ~summaryDf['cannula']
+ind = summaryDf['stage 2 pass'] & summaryDf['AM noise'] & summaryDf['timeouts'] & ~miceToIgnore
 mice = {'AM noise, early AR': np.array(summaryDf[ind & ~summaryDf['late autoreward (stage 2)']]['mouse id']),
         'AM noise, late AR':  np.array(summaryDf[ind & summaryDf['late autoreward (stage 2)']]['mouse id'])}
 plotLearning(mice,stage=2)
 
 
 # stage 5, repeats vs no repeats
-ind = ~hasIndirectRegimen & summaryDf['stage 5 pass'] & ~summaryDf['cannula']
+ind = ~hasIndirectRegimen & summaryDf['stage 5 pass'] & ~miceToIgnore
 mice = {'no repeats': np.array(summaryDf[ind & ~summaryDf['stage 5 repeats']]['mouse id']),
         'repeats': np.array(summaryDf[ind & summaryDf['stage 5 repeats']]['mouse id'])}
 plotStage5Learning(mice)
 
 # stage 5, moving, AMN, no repeats
-ind = ~hasIndirectRegimen & summaryDf['stage 5 pass'] & summaryDf['moving grating'] & summaryDf['AM noise'] & ~summaryDf['cannula'] & ~summaryDf['stage 5 repeats']
+ind = ~hasIndirectRegimen & summaryDf['stage 5 pass'] & summaryDf['moving grating'] & summaryDf['AM noise'] & ~summaryDf['stage 5 repeats'] & ~miceToIgnore
 mice = {'moving, AMN': np.array(summaryDf[ind]['mouse id'])}
 plotStage5Learning(mice)
 
 # stage 5, with or without reward clicks
-ind = ~hasIndirectRegimen & summaryDf['stage 5 pass'] & summaryDf['moving grating'] & summaryDf['AM noise'] & ~summaryDf['cannula'] & ~summaryDf['stage 5 repeats']
+ind = ~hasIndirectRegimen & summaryDf['stage 5 pass'] & summaryDf['moving grating'] & summaryDf['AM noise'] & ~summaryDf['stage 5 repeats'] & ~miceToIgnore
 mice = {'reward click': np.array(summaryDf[ind & summaryDf['reward click']]['mouse id']),
         'no reward click':  np.array(summaryDf[ind & ~summaryDf['reward click']]['mouse id'])}
 plotStage5Learning(mice)
 
 # stage 5, early or late autorewards
-ind = ~hasIndirectRegimen & summaryDf['stage 5 pass'] & summaryDf['moving grating'] & summaryDf['AM noise'] & ~summaryDf['cannula'] & ~summaryDf['stage 5 repeats']
+ind = ~hasIndirectRegimen & summaryDf['stage 5 pass'] & summaryDf['moving grating'] & summaryDf['AM noise'] & ~summaryDf['stage 5 repeats'] & ~miceToIgnore
 mice = {'early AR': np.array(summaryDf[ind & ~summaryDf['late autoreward (stage 5)']]['mouse id']),
         'late AR':  np.array(summaryDf[ind & summaryDf['late autoreward (stage 5)']]['mouse id'])}
 plotStage5Learning(mice)
 
 
 ## moving to stationary grating switch
 preSessions = 1
@@ -282,15 +298,15 @@
 ax.set_ylim([0,4.1])
 ax.set_xlabel('Session',fontsize=14)
 ax.set_ylabel('d\'',fontsize=14)
 plt.tight_layout()
 
 
 ## within modality d' after stage 2
-ind = ~hasIndirectRegimen & summaryDf['stage 5 pass'] & summaryDf['moving grating'] & summaryDf['AM noise'] & ~summaryDf['cannula'] & ~summaryDf['stage 5 repeats']
+ind = ~hasIndirectRegimen & summaryDf['stage 5 pass'] & summaryDf['moving grating'] & summaryDf['AM noise'] & ~summaryDf['stage 5 repeats'] & ~miceToIgnore
 mice = np.array(summaryDf[ind]['mouse id'])
 
 dprime = {'vis': [], 'aud': []}
 for mid in mice:
     df = drSheets[str(mid)] if str(mid) in drSheets else nsbSheets[str(mid)]
     sessions = np.array(['stage 5' in task for task in df['task version']]) & ~np.array(df['ignore'].astype(bool))
     firstExperimentSession = getFirstExperimentSession(df)
@@ -336,15 +352,15 @@
 ax.set_xlabel('Session',fontsize=14)
 ax.set_ylabel('d\' (same modality)',fontsize=14)
 plt.legend(loc='lower right')
 plt.tight_layout()
 
  
 ## stage 5 training
-ind = ~hasIndirectRegimen & summaryDf['stage 5 pass'] & summaryDf['moving grating'] & summaryDf['AM noise'] & ~summaryDf['cannula'] & ~summaryDf['stage 5 repeats']
+ind = ~hasIndirectRegimen & summaryDf['stage 5 pass'] & summaryDf['moving grating'] & summaryDf['AM noise'] & ~summaryDf['stage 5 repeats'] & ~miceToIgnore
 mice = np.array(summaryDf[ind]['mouse id'])
 hasLateAutorewards = np.array(summaryDf[ind]['late autoreward (stage 5)'])
 
 dprime = {comp: {mod: [] for mod in ('all','vis','sound')} for comp in ('same','other')}
 sessionsToPass = []
 sessionData = []
 for mid in mice:
```

### Comparing `DynamicRoutingTask-0.1.94/Analysis/dr_ephys_analysis.py` & `DynamicRoutingTask-0.1.95/Analysis/dr_ephys_analysis.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.94/Analysis/glm_hmm_sam.py` & `DynamicRoutingTask-0.1.95/Analysis/glm_hmm_sam.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.94/Analysis/ncb_meeting_01272023.py` & `DynamicRoutingTask-0.1.95/Analysis/ncb_meeting_01272023.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.94/Analysis/npc_analysis.py` & `DynamicRoutingTask-0.1.95/Analysis/npc_analysis.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.94/Analysis/presentation_June2023.py` & `DynamicRoutingTask-0.1.95/Analysis/presentation_June2023.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.94/Analysis/regressionModel.py` & `DynamicRoutingTask-0.1.95/Analysis/regressionModel.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.94/Analysis/sac_may2023.py` & `DynamicRoutingTask-0.1.95/Analysis/sac_may2023.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.94/Analysis/sessionSummaryFigs.py` & `DynamicRoutingTask-0.1.95/Analysis/sessionSummaryFigs.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.94/Analysis/sound_ephys_analysis.py` & `DynamicRoutingTask-0.1.95/Analysis/sound_ephys_analysis.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.94/Analysis/sound_sync_test.py` & `DynamicRoutingTask-0.1.95/Analysis/sound_sync_test.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.94/Analysis/variableBlockDur.py` & `DynamicRoutingTask-0.1.95/Analysis/variableBlockDur.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.94/DynamicRouting1.py` & `DynamicRoutingTask-0.1.95/DynamicRouting1.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.94/DynamicRouting1_postSessionAnalysis.py` & `DynamicRoutingTask-0.1.95/DynamicRouting1_postSessionAnalysis.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.94/DynamicRoutingTask.egg-info/SOURCES.txt` & `DynamicRoutingTask-0.1.95/DynamicRoutingTask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.94/OptoGui/OptoGui.py` & `DynamicRoutingTask-0.1.95/OptoGui/OptoGui.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.94/OptoTagging.py` & `DynamicRoutingTask-0.1.95/OptoTagging.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 class OptoTagging(TaskControl):
     
     def __init__(self,params):
         TaskControl.__init__(self,params)
         
-        self.monBackgroundColor = -1
+        self.monBackgroundColor = -0.95
         self.maxFrames = params['maxFrames'] if 'maxFrames' in params and params['maxFrames'] is not None else None
         self.maxTrials = params['maxTrials'] if 'maxTrials' in params and params['maxTrials'] is not None else None
         
         self.trialsPerType = 25
         self.optoPower = [5] # mW
         self.optoDur = [0.01,0.2] # seconds
         self.optoOnRamp = 0.001 # seconds
```

### Comparing `DynamicRoutingTask-0.1.94/RFMapping.py` & `DynamicRoutingTask-0.1.95/RFMapping.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.94/SamStimGui/SamStimGui.py` & `DynamicRoutingTask-0.1.95/SamStimGui/SamStimGui.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.94/TaskControl.py` & `DynamicRoutingTask-0.1.95/TaskControl.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         self.saveFrameIntervals = True
         self.monBackgroundColor = 0 # gray; can adjust this for luminance measurement
         self.minWheelAngleChange = 0 # radians per frame
         self.maxWheelAngleChange = 0.5 # radians per frame
         self.spacebarRewardsEnabled = False
         self.soundSampleRate = 48000 # Hz
         self.soundHanningDur = 0.005 # seconds
+        self.soundFilter = None
         self.optoSampleRate = 2000 # Hz
         
         # rig specific settings
         self.frameRate = 60
         self.screen = 0 # monitor to present stimuli on
         self.monWidth = 52.0 # cm
         self.monDistance = 15.3 # cm
@@ -59,14 +60,15 @@
         self.digitalSolenoidTrigger = True
         self.solenoidOpenTime = 0.03
         self.rewardSoundDeviceOpenTime = 0.01
         self.microphoneCh = None
         self.syncNidaqDevice = None
         self.frameSignalLine = None
         self.acquisitionSignalLine = None
+        self.rewardSyncLine = None
         self.soundMode = 'sound card' # 'sound card', or 'daq'
         self.soundNidaqDevice = None
         self.soundChannel = None
         self.optoNidaqDevice = None
         self.galvoChannels = None
         self.optoChannels = None
         
@@ -107,14 +109,15 @@
                     self.behavNidaqDevice = 'Dev0'
                     self.rewardLine = (0,7)
                     self.rewardSoundLine = (2,0)
                     self.lickLine = (0,0)
                     self.syncNidaqDevice = 'Dev1'
                     self.frameSignalLine = (1,4)
                     self.acquisitionSignalLine = (1,7)
+                    self.rewardSyncLine = (2,1)
                     if self.rigName == 'NP1':
                         self.rotaryEncoderSerialPort = 'COM6'
                         self.networkNidaqDevices = ['zcDAQ9185-217ECE0']
                         self.optoNidaqDevice = 'zcDAQ9185-217ECE0Mod1'
                         self.galvoChannels = (0,1)
                         self.optoChannels = {'laser_488': (2,3), 'laser_633': (4,5)}
                     elif self.rigName == 'NP2':
@@ -249,14 +252,19 @@
                     self.rotaryEncoderSerialPort = 'COM3'
                     self.behavNidaqDevice = 'Dev1'
                     self.rewardLine = (0,1)
                     self.lickLine = (0,0)
                     self.soundMode = 'daq'
                     self.soundNidaqDevice = 'Dev1'
                     self.soundChannel = (0,np.nan)
+                    soundFilterPath = r"C:\Users\teenspirit\Desktop\Tilda's behavior\01252024_npx_spkrleft_31-80k_fs200k.mat"
+                    import scipy.io
+                    d = scipy.io.loadmat(soundFilterPath)
+                    self.soundSampleRate = d['Fs'][0]
+                    self.soundFilter = d['FILT'][0]
                 else:
                     raise ValueError(self.rigName + ' is not a recognized rig name')
                 
             
     def prepareSession(self,window=True):
         self._win = None
         self._nidaqTasks = []
@@ -514,14 +522,20 @@
             self._nidaqTasks.append(self._frameSignalOutput)
 
             self._acquisitionSignalOutput = nidaqmx.Task()
             self._acquisitionSignalOutput.do_channels.add_do_chan(self.syncNidaqDevice+'/port'+str(self.acquisitionSignalLine[0])+'/line'+str(self.acquisitionSignalLine[1]),
                                                                   line_grouping=nidaqmx.constants.LineGrouping.CHAN_PER_LINE)
             self._acquisitionSignalOutput.write(False)
             self._nidaqTasks.append(self._acquisitionSignalOutput)
+
+            self._rewardSyncOutput = nidaqmx.Task()
+            self._rewardSyncOutput.do_channels.add_do_chan(self.syncNidaqDevice+'/port'+str(self.rewardSyncLine[0])+'/line'+str(self.rewardSyncLine[1]),
+                                                           line_grouping=nidaqmx.constants.LineGrouping.CHAN_PER_LINE)
+            self._rewardSyncOutput.write(False)
+            self._nidaqTasks.append(self._rewardSyncOutput)
     
     
     def stopNidaqDevice(self):
         if hasattr(self,'_optoOutput'):
             self.optoOff(devices=self.optoChannels.keys())
         for task in self._nidaqTasks:
             # task.stop()
@@ -648,28 +662,32 @@
         self._solenoid = None
         
         
     def triggerReward(self,openTime):
         if self.digitalSolenoidTrigger:
             t = Timer(openTime,self.endReward)
             self._rewardOutput.write(True)
+            if self.syncNidaqDevice is not None:
+                self._rewardSyncOutput.write(True)
             t.start()
         else:
             sampleRate = self._rewardOutput.timing.samp_clk_rate
             nSamples = int(openTime * sampleRate) + 1
             s = np.zeros(nSamples)
             s[:-1] = 5
             self._rewardOutput.stop()
             self._rewardOutput.timing.samp_quant_samp_per_chan = nSamples
             self._rewardOutput.write(s,auto_start=True)
     
     
     def endReward(self):
         if self.digitalSolenoidTrigger:
             self._rewardOutput.write(False)
+            if self.syncNidaqDevice is not None:
+                self._rewardSyncOutput.write(False)
             
             
     def triggerRewardSound(self):
         t = Timer(self.rewardSoundDeviceOpenTime,self.endRewardSound)
         self._rewardSoundOutput.write(True)
         t.start()
     
@@ -695,14 +713,17 @@
             self._soundOutput.ao_channels.add_ao_voltage_chan(self.soundNidaqDevice+'/ao'+soundCh,min_val=-10,max_val=10)
             self._soundOutput.write(output)
             self._soundOutput.timing.cfg_samp_clk_timing(self.soundSampleRate)
             self._nidaqTasks.append(self._soundOutput)
                 
     
     def loadSound(self,soundArray):
+        if self.soundFilter is not None:
+            soundArray = np.convolve(soundArray, self.soundFilter, 'same')
+        
         if self.soundMode == 'sound card':
             self._audioStream.fill_buffer(soundArray)
         elif self.soundMode == 'daq':
             if np.isnan(self.soundChannel[1]):
                 output = soundArray * 10
             else:
                 output = np.zeros((2,soundArray.size))
@@ -1272,20 +1293,20 @@
             galvoX,galvoY = TaskUtils.getGalvoWaveforms(task.optoSampleRate,x,y,dwell,nSamples)
         task.loadOptoWaveform([params['optoDev']],optoWaveforms,galvoX,galvoY)
         task.startOpto()
         time.sleep(dur + 0.5)
         task.stopNidaqDevice()
     elif params['taskVersion'] == 'spontaneous':
         task = Spontaneous(params)
-        task.monBackgroundColor = -1
+        task.monBackgroundColor = -0.95
         task.maxFrames = params['maxFrames'] if 'maxFrames' in params and params['maxFrames'] is not None else 10 * 3600
         task.start(params['subjectName'])
     elif params['taskVersion'] == 'spontaneous rewards':
         task = SpontaneousRewards(params,numRewards=6,rewardInterval=90*60)
-        task.monBackgroundColor = -1
+        task.monBackgroundColor = -0.95
         if 'rewardSound' in params:
             task.rewardSound = params['rewardSound']
         task.maxFrames = params['maxFrames'] if 'maxFrames' in params and params['maxFrames'] is not None else 10 * 3600
         task.start(params['subjectName'])
     else:
         task = TaskControl(params)
         task.saveParams = False
```

### Comparing `DynamicRoutingTask-0.1.94/TaskUtils.py` & `DynamicRoutingTask-0.1.95/TaskUtils.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.94/camstimControl.py` & `DynamicRoutingTask-0.1.95/camstimControl.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.94/pyproject.toml` & `DynamicRoutingTask-0.1.95/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "DynamicRoutingTask"
-version = "0.1.94"
+version = "0.1.95"
 dependencies = [
     "h5py",
     "numpy",
     "pandas",
     "scipy",
     "matplotlib",
 ]
```

### Comparing `DynamicRoutingTask-0.1.94/runTask.py` & `DynamicRoutingTask-0.1.95/runTask.py`

 * *Files identical despite different names*

### Comparing `DynamicRoutingTask-0.1.94/startTask.py` & `DynamicRoutingTask-0.1.95/startTask.py`

 * *Files identical despite different names*

