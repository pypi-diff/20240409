# Comparing `tmp/RepMan-1.0.1.tar.gz` & `tmp/RepMan-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RepMan-1.0.1.tar", last modified: Sat Apr  6 21:50:28 2024, max compression
+gzip compressed data, was "RepMan-1.0.2.tar", last modified: Tue Apr  9 18:17:00 2024, max compression
```

## Comparing `RepMan-1.0.1.tar` & `RepMan-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-06 21:50:28.282084 RepMan-1.0.1/
--rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-06 11:46:27.000000 RepMan-1.0.1/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     2420 2024-04-06 21:50:28.281592 RepMan-1.0.1/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      222 2024-04-06 16:08:22.000000 RepMan-1.0.1/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1110 2024-04-06 17:17:50.000000 RepMan-1.0.1/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-06 21:50:28.282174 RepMan-1.0.1/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-06 21:50:28.272094 RepMan-1.0.1/src/
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-06 21:50:28.280990 RepMan-1.0.1/src/RepMan.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     2420 2024-04-06 21:50:28.000000 RepMan-1.0.1/src/RepMan.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      367 2024-04-06 21:50:28.000000 RepMan-1.0.1/src/RepMan.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-06 21:50:28.000000 RepMan-1.0.1/src/RepMan.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       46 2024-04-06 21:50:28.000000 RepMan-1.0.1/src/RepMan.egg-info/entry_points.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       60 2024-04-06 21:50:28.000000 RepMan-1.0.1/src/RepMan.egg-info/requires.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        7 2024-04-06 21:50:28.000000 RepMan-1.0.1/src/RepMan.egg-info/top_level.txt
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-06 21:50:28.280212 RepMan-1.0.1/src/repman/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-06 11:46:27.000000 RepMan-1.0.1/src/repman/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)    17700 2024-04-06 21:49:48.000000 RepMan-1.0.1/src/repman/_repmanclass.py
--rw-r--r--   0 d33pster   (501) staff       (20)     1280 2024-04-06 21:32:52.000000 RepMan-1.0.1/src/repman/_repmanfunctions.py
--rw-r--r--   0 d33pster   (501) staff       (20)    10058 2024-04-06 21:15:53.000000 RepMan-1.0.1/src/repman/_repmanhelps.py
--rw-r--r--   0 d33pster   (501) staff       (20)    12833 2024-04-06 21:35:49.000000 RepMan-1.0.1/src/repman/repman.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-09 18:17:00.318386 RepMan-1.0.2/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-06 11:46:27.000000 RepMan-1.0.2/LICENSE
+-rw-r--r--   0 d33pster   (501) staff       (20)     5327 2024-04-09 18:17:00.317995 RepMan-1.0.2/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)     3129 2024-04-09 18:10:40.000000 RepMan-1.0.2/README.md
+-rw-r--r--   0 d33pster   (501) staff       (20)     1110 2024-04-09 15:55:56.000000 RepMan-1.0.2/pyproject.toml
+-rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-09 18:17:00.318446 RepMan-1.0.2/setup.cfg
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-09 18:17:00.309274 RepMan-1.0.2/src/
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-09 18:17:00.317448 RepMan-1.0.2/src/RepMan.egg-info/
+-rw-r--r--   0 d33pster   (501) staff       (20)     5327 2024-04-09 18:17:00.000000 RepMan-1.0.2/src/RepMan.egg-info/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)      367 2024-04-09 18:17:00.000000 RepMan-1.0.2/src/RepMan.egg-info/SOURCES.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-09 18:17:00.000000 RepMan-1.0.2/src/RepMan.egg-info/dependency_links.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       46 2024-04-09 18:17:00.000000 RepMan-1.0.2/src/RepMan.egg-info/entry_points.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       60 2024-04-09 18:17:00.000000 RepMan-1.0.2/src/RepMan.egg-info/requires.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        7 2024-04-09 18:17:00.000000 RepMan-1.0.2/src/RepMan.egg-info/top_level.txt
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-09 18:17:00.316793 RepMan-1.0.2/src/repman/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-06 11:46:27.000000 RepMan-1.0.2/src/repman/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)    25047 2024-04-09 17:21:56.000000 RepMan-1.0.2/src/repman/_repmanclass.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     1417 2024-04-09 17:24:32.000000 RepMan-1.0.2/src/repman/_repmanfunctions.py
+-rw-r--r--   0 d33pster   (501) staff       (20)    11066 2024-04-09 17:29:32.000000 RepMan-1.0.2/src/repman/_repmanhelps.py
+-rw-r--r--   0 d33pster   (501) staff       (20)    15517 2024-04-09 17:24:50.000000 RepMan-1.0.2/src/repman/repman.py
```

### Comparing `RepMan-1.0.1/LICENSE` & `RepMan-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `RepMan-1.0.1/pyproject.toml` & `RepMan-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "RepMan"
-version = "1.0.1"
+version = "1.0.2"
 description = "RepMan: Repository Manager (alias: Project Manager)"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development",
     "License :: OSI Approved :: MIT License",
```

### Comparing `RepMan-1.0.1/src/repman/_repmanclass.py` & `RepMan-1.0.2/src/repman/_repmanclass.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,14 +29,16 @@
             self.path = projectpath
         # working path -> where it is called.
         self.workingpath = pwd()
         # get current os
         self.operatingsystem = platform.system()
         # projectlist
         self.projects: list[dict] = []
+        # default branch
+        self.default_branch: str = ''
     
     ################### SET PATH FROM OUTSIDE ###############################
     def setvariables(self):
         try:
             self.path = environ['REPMAN_PROJECT_PATH']
         except KeyError:
             raise RuntimeError('bad call of setvariables function before running init.')
@@ -53,68 +55,197 @@
                 data = {
                     'project':c.split(':')[0],
                     'path':c.split(':')[1]
                 }
                 self.projects.append(data)
         except FileNotFoundError:
             pass
+        # -> get default branch
+        try:
+            with open(join(self.dotfolder, '.branch'), 'r') as b:
+                content = b.readlines()
+            for c in content:
+                c = c.replace('\n','')
+                if c.split(':')[0] == 'default':
+                    self.default_branch = c.split(':')[1]
+        except FileNotFoundError:
+            pass
     
+    ############################ set remote ##############################
+    def setremote(self, project:str, remote:str):
+        # get project path.
+        path = None
+        for d in self.projects:
+            if d['project'].lower() == project.lower():
+                path = d['path']
+        
+        if path==None:
+            print(colored('RepMan', 'red')+f": No project named {project}.")
+            exit(1)
+        
+        # change dir
+        chdir(path)
+        
+        # identify remote
+        link = False
+        if match(r'^https://github.com/\w+/\w+', remote):
+            link = True
+        elif match(r'^\w+/\w+', remote):
+            link = False
+        
+        
+        with open(join(self.dotfolder, '.log'), 'w') as logfile:
+            if link:
+                subprocess.Popen(['git','remote', 'add', 'origin', f'{remote}'], stderr=logfile, stdout=logfile).wait()
+            else:
+                subprocess.Popen(['git','remote', 'add', 'origin', f'https://github.com/{remote}.git'], stderr=logfile, stdout=logfile).wait()
+        
+        with open(join(self.dotfolder, '.log'), 'r') as l:
+            logfile = l.readlines()
+        
+        if len(logfile)!=0:
+            print('RepMan:', colored('Remote is already set.', 'red'), end='')
+            if link:
+                subprocess.Popen(['git', 'remote', 'set-url', 'origin', f'{remote}']).wait()
+            else:
+                subprocess.Popen(['git', 'remote', 'set-url', 'origin', f'https://github.com/{remote}.git']).wait()
+            print(colored('Overwritten.', 'blue'))
+        else:
+            if link:
+                print('RepMan:', colored('Remote', 'blue'), 'is set ->', colored(f'{remote}', 'blue'))
+            else:
+                print('RepMan:', colored('Remote', 'blue'), 'is set ->', colored(f'https://github.com/{remote}.git', 'blue'))
+        
     ####################### ADD LOCAL FUNCTION ######################### NEEDS FIXING ##################
     def addlocal(self, paths:list[str]):
         # ask for default branch if not set
         if there(join(self.dotfolder, '.branch')):
             with open(join(self.dotfolder, '.branch'), 'r') as bfile:
                 content = bfile.readlines()
             
             for c in content:
                 c = c.replace('\n','')
                 if c.split(':')[0] == 'default':
-                    branch = c.split(':')[1]
+                    branch = c.split(':')[1].replace('\n','').strip()
         else:
-            branch = input('RepMan -> Enter '+colored('default branch', 'blue')+colored('(one-time)'+'dark_grey') + ': ')
+            branch = input('RepMan -> Enter '+colored('default branch', 'blue')+colored('(one-time)','dark_grey') + ': ').strip()
+            if branch=='\n' or branch=='':
+                print('RepMan:', colored('Defaulting to main.', 'light_blue'))
+                branch = 'main'
+            
             with open(join(self.dotfolder, '.branch'), 'w') as bfile:
                 bfile.write('default:'+branch+"\n")
         
         # copy the files
         for path in paths:
             path = abspath(path)
             # -> check if already inside the directory
             if dirname(path) == self.path:
+                # check existence of the folder.
+                if not there(path):
+                    print(colored('RepMan', 'red'), f': No such file or directory. <- {path}')
+                    exit(1)
                 # add entry in the .projects file
                 with open(join(self.dotfolder, '.projects'), 'a') as projfile:
                     projfile.write(basename(path)+':'+path+'\n')
                 print('RepMan:', colored(f'Added {basename(path)} -> {path}', 'green'))
+                newpath = path
             else:
                 ## copy
                 try:
                     newpath = copytree(path, join(self.path, basename(path)))
                 except FileNotFoundError:
-                    print(colored('RepMan', 'red'), f': No such file in this directory. <- {path}')
+                    print(colored('RepMan', 'red'), f': No such file or directory. <- {path}')
                     exit(1)
+                
+                ## add it in the projfile.
+                with open(join(self.dotfolder, '.projects'), 'a') as projfile:
+                    projfile.write(basename(newpath)+":"+newpath+"\n")
+                
                 print('RepMan:', colored(f'Added {basename(path)} -> {newpath}', 'green'))
-        
-        # 
+            
+            #change dir to newdir
+            chdir(newpath)
+            # check for git folder
+            if there(join(newpath, '.git')):
+                print('RepMan:', colored(f'{basename(newpath)} is already a git repository.', 'green'))
+            else:
+                print('RepMan:', colored(f'{basename(newpath)} is not a git repository.', 'red'))
+                subprocess.Popen(['git', 'init'], stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL).wait()
+                print('RepMan:', colored(f'{basename(newpath)} has been initialized as a git repository.', 'blue'))
+            
+            
+            # set branch to default branch
+            subprocess.Popen(['git', 'branch', '-M', f'{branch}'], stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL).wait()
+            print('RepMan:', colored(f'Branch is set to \'{branch}\' by default.', 'yellow'), 'To change this, change default branch. For more info run \'-h\'.')
+            
+            # check the files that were to be added.
+            files = getoutputof('git diff --name-only').readlines()
+            files2 = getoutputof('git ls-files --others --exclude-standard').readlines()
+            msgs = []
+            for file in files:
+                file = file.replace('\n','')
+                commitmsg = input('RepMan -> Enter commit msg for ' + colored(f'{join(basename(path), file)}', 'blue') + ': ')
+                msgs.append(commitmsg)
+            
+            for file in files2:
+                file = file.replace('\n','')
+                commitmsg = input('RepMan -> Enter commit msg for ' + colored(f'{join(basename(path), file)}', 'blue') + colored('(new)', 'dark_grey') + ': ')
+                msgs.append(commitmsg)
+            
+            files.extend(files2)
+            
+            # commit the changes
+            for i in range(len(files)):
+                subprocess.Popen(['git', 'add', f"{files[i].replace('\n','')}"], stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL).wait()
+                subprocess.Popen(['git', 'commit', '-m', f'{msgs[i]}'], stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL).wait()
+                print('RepMan:', colored(f"Added {join(basename(path), files[i].replace('\n',''))}", 'green'))
+            
+            remote = input('RepMan -> Enter ' + colored('remote', 'blue') + f' for {basename(newpath)}' + colored('one-time', 'dark_grey') + ': ').strip()
+            # exit if remote not provided.
+            if remote=='' or remote==' ' or remote=='\n':
+                print('RepMan:', colored('Skipping remote. Add later using \'repman -sr <reponame> <remote>\'. For more help, run \'repman -sr -h\''))
+                exit(0)
+            else:
+                # else remote is given.
+                # -> check for the pattern "github.com/..."
+                if match(r'^https://github.com/\w+/\w+', remote):
+                    # add origin
+                    subprocess.Popen(['git','remote','add','origin',f'{remote}'], stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL).wait()
+                    print('RepMan:', colored('Added Remote', 'dark_grey'), '->', colored(f'{remote}', 'blue'))
+                elif match(r'^\w+/\w+', remote):
+                    # <username>/<repo>
+                    # add origin
+                    subprocess.Popen(['git','remote','add','origin',f'https://github.com/{remote}.git'], stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL).wait()
+                    print('RepMan:', colored('Added Remote', 'dark_grey'), '->', colored(f'https://github.com/{remote}.git', 'blue'))
+                
+                # git push
+                print('RepMan:', colored('Pushing', 'yellow'), end='\r')
+                subprocess.Popen(['git', 'push', '-u', 'origin', f'{branch}'], stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL).wait()
+                print('                                                      ', end='\r')
+                print('RepMan:', colored('Pushed.', 'green'))
+                exit(0)
     
     ###################### UPDATE FUNCTION #######################################
     def update(self, projectname:str):
         try:
             code = requests.get('https://google.com/').status_code
             if code == 200:
-                # get data from saved file
-                with open(join(self.dotfolder, '.projects'), 'r') as p:
-                    content = p.readlines()
                 
                 # get filepath of the project
-                for c in content:
-                    c = c.replace('\n','')
-                    if c.split(':')[0] == projectname:
-                       path = c.split(':')[1]
+                for d in self.projects:
+                    if d['project'].lower() == projectname.lower():
+                        path = d['path']
                 
                 # change to the path
-                chdir(path)
+                try:
+                    chdir(path)
+                except UnboundLocalError:
+                    print(colored('RepMan', 'red'), f": no project named {projectname}.")
+                    exit(1)
                 # get files that are changed.
                 files = getoutputof('git diff --name-only').readlines()
                 files2 = getoutputof('git ls-files --others --exclude-standard').readlines()
                 msgs = []
                 for file in files:
                     file = file.replace('\n','')
                     commitmsg = input('RepMan -> Enter commit msg for ' + colored(f'{join(basename(path), file)}', 'blue') + ': ')
@@ -128,37 +259,46 @@
                 files.extend(files2)
                 
                 for i in range(len(files)):
                     subprocess.Popen(['git', 'add', f"{files[i].replace('\n','')}"], stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL).wait()
                     subprocess.Popen(['git', 'commit', '-m', f'{msgs[i]}'], stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL).wait()
                     print('RepMan:', colored(f"Added {join(basename(path), files[i].replace('\n',''))}", 'green'))
                 
+                # get current branch
+                branch = getoutputof('git rev-parse --abbrev-ref HEAD').read().replace('\n','')
+                print('RepMan: Resolved current branch ->', colored(f'{branch}', 'blue'))
+                
                 print('RepMan:', colored('Pushing', 'yellow'), end='\r')
-                subprocess.Popen(['git', 'push'], stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL).wait()
+                subprocess.Popen(['git', 'push', '-u', 'origin', f'{branch}'], stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL).wait()
                 print('                                                      ', end='\r')
                 print('RepMan:', colored('Pushed', 'green'))
         except ConnectionError:
             print(colored('RepMan','red'), ': Please connect to the internet to use this feature.')
             exit(1)
 
     ############## OPEN FUNCTION INSIDE REPMAN CLASS #############################
     def open(self, projects:list[str]):
-        with open(join(self.dotfolder, '.projects'), 'r') as t:
-            projfile = t.readlines()
+        count = 0
         for project in projects:
-            for proj in projfile:
-                proj = proj.replace('\n','')
-                if project == proj.split(':')[0]:
+            for d in self.projects:
+                if d['project'].lower() == project.lower():
+                    path = d['path']
+                    count += 1
                     # check the project for templates and stuff -> add later
                     # open the project.
-                    chdir(proj.split(':')[1])
+                    chdir(path)
                     subprocess.Popen(['code', '.'], stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL).wait()
                     # print it out
-                    print('RepMan:', colored(f'Opened {project}', 'green'), 'from', colored(f"{proj.split(':')[1]}", 'blue'))
+                    print('RepMan:', colored(f'Opened {project}', 'green'), 'from', colored(f"{path}", 'blue'))
                     chdir(self.workingpath)
+        
+            if count == 0:
+                print(colored('RepMan', 'red')+f": No project name \'{project}\' under my care.")
+            
+            count = 0
     
     ############## LISTER FUNCTION INSIDE REPMAN CLASS #############################
     def lister(self, path:bool=False):
         if len(self.projects)>0:
             lister = pd.DataFrame(self.projects)
             if not path:
                 lister = pd.DataFrame(lister['project'].to_list(), columns=['project'])
@@ -188,15 +328,15 @@
     
     ############## ADD FUNCTION INSIDE REPMAN CLASS #############################
     def add(self, url:str):
         # set project path
         self.path = environ['REPMAN_PROJECT_PATH']
         chdir(self.path)
         # check format -> must be github link or <username>/<repo>
-        if match(r'^https://github.com/\w+/\w+$', url):
+        if match(r'^https://github.com/\w+/\w+', url):
             if match(r'^https://github.com/\w+/\w+.git$', url):
                 # remove extension and save
                 urlbasename = Path(url).stem
             else:
                 urlbasename = basename(url)
 
             # -> try cloning
@@ -211,15 +351,15 @@
         
         # -> check log for output
         with open(join(self.dotfolder, '.log'), 'r') as log:
             logfile = log.readlines()
         # -> check output
         index = len(logfile)-1
         # -> if error
-        if match(r'^fatal:\s+\w+$', logfile[index]):
+        if match(r'^fatal:\s+\w+', logfile[index]):
             print('RepMan:', colored(f'Cannot add \'{urlbasename}\'. Check for Spelling Errors.', 'red'))
             exit(1)
         
         # if no error
         # -> save project data to .projects
         with open(join(self.dotfolder, '.projects'), 'a') as projfile:
             projfile.write(f"{urlbasename}:{join(self.path, urlbasename)}\n")
@@ -373,8 +513,9 @@
             print('RepMan:', colored('Installing vscode', 'yellow'), end='\r')
             subprocess.Popen(['sudo', 'dpkg', '-i', './code-arm64.deb'], stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL).wait()
             print('RepMan:', colored(f"vscode installed -> v{getoutputof('code -v').readline().replace('\n','')}", 'green'))
     elif os == 'Darwin':
         if getoutputof('arch').read().replace('\n','')=='arm64':
             print('RepMan:', colored('Using Brew to install vscode.', 'yellow'), end='\r')
             subprocess.Popen(['brew', 'install', '--cask', 'visual-studio-code'], stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL).wait()
-            print('RepMan:', colored(f"vscode installed -> v{getoutputof('code -v').readline().replace('\n','')}", 'green'))
+            print('RepMan:', colored(f"vscode installed -> v{getoutputof('code -v').readline().replace('\n','')}", 'green'))
+
```

### Comparing `RepMan-1.0.1/src/repman/_repmanfunctions.py` & `RepMan-1.0.2/src/repman/_repmanfunctions.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,8 +41,12 @@
     # function to update a repo
     def update(self, projectname:str):
         self.repman.setvariables()
         self.repman.update(projectname)
     
     def addlocal(self, paths: list[str]):
         self.repman.setvariables()
-        self.repman.addlocal(paths)
+        self.repman.addlocal(paths)
+    
+    def setremote(self, project:str, remote:str):
+        self.repman.setvariables()
+        self.repman.setremote(project, remote)
```

### Comparing `RepMan-1.0.1/src/repman/_repmanhelps.py` & `RepMan-1.0.2/src/repman/_repmanhelps.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,16 @@
         print('  |  -i or --init          : initialize settings, configurations and exit.')
         print('  |  -a or --add           : add a git repository under RepMan\'s care.')
         print('  |  -o or --open          : open a project/repository.')
         print('  |  -l or --list          : list all the projects under RepMan\'s care. and exit.')
         print('  |  -lp or --list-w-path  : list all the projects under RepMan\'s care with their paths and exit.')
         print('  |  -ae or --add-existing : Add an already cloned repository under RepMan\'s care.')
         print('  |  -al or --add-local    : Add a local git repository under RepMan\'s care.')
-        print('  |  -u or --update        : update a repository.',colored('[requires internet]\n', 'red'))
+        print('  |  -u or --update        : update a repository.',colored('[requires internet]', 'red'))
+        print('  |  -sr or --set-remote   : set remote for a project.\n')
         print(colored('NOTE', 'blue'), ': For further help, run', colored('\'repman <argument> -h\'', 'red'), 'or', colored('\'repman <argument> --help\'.', 'red'))
         print('\nEND')
         exit(0)
     
      # function to print specialized help on '-v' or '--version'
     def version_h(self, arg:str):
         print(colored('RepMan', 'blue'), ': Repository Manager (alias: Project Manager)')
@@ -54,15 +55,15 @@
         print('  |                                              |')
         print('  | It will automatically detect and try to Ini- |')
         print('  | tialize RepMan and all its Configurations.   |')
         print('  |                                              |')
         print('  | This Argument may ask input from the user a- |')
         print('  | bout few Configurations.                     |')
         print('  |                                              |')
-        print('  |', colored('Format', 'red'), ': \'repman -i\' or \'repman --init\'      |')
+        print('  |', colored('Format', 'red')+': \'repman -i\' or \'repman --init\'       |')
         print('  |                                              |')
         print('  | Note: you can also specify the init path af- |')
         print('  | ter the -i or --init arg.                    |')
         print('  |                                              |')
         print('\nEND')
         exit(0)
     
@@ -71,15 +72,15 @@
         print(colored('RepMan', 'blue'), ': Repository Manager (alias: Project Manager)')
         print(colored(f'v{self.version}\n', 'red'))
         print('help', colored('EXTENDED', 'blue'), f': help for \'{arg}\'\n')
         print('  | This argument is used to add git repositori- |')
         print('  | es under RepMan\'s care. This basically means |')
         print('  | RepMan will manage that repository for you.  |')
         print('  |                                              |')
-        print('  |', colored('Format', 'red'), ': \'repman -a <link>\'                  |')
+        print('  |', colored('Format', 'red')+': \'repman -a <link>\'                   |')
         print('  |                 or                           |')
         print('  |          \'repman -a <username>/<repo>\'       |')
         print('  |                                              |')
         print('\nEND')
         exit(0)
     
     # function to print specialized help on '-o' or '--open'
@@ -95,54 +96,54 @@
         print('  | ct.                                          |')
         print('  |                                              |')
         print('  | Since this is a python project itself, RepMan|')
         print('  | will add the necessary files in the .gitign- |')
         print('  | ore file. such as \'dist\' if the destination  |')
         print('  | is found to be a python project.             |')
         print('  |                                              |')
-        print('  |',colored('Format', 'red'), ': \'repman -o <project-name>\'          |')
+        print('  |',colored('Format', 'red')+': \'repman -o <project-name>\'           |')
         print('  |                                              |')
         print('\nEND')
         exit(0)
     
     # function to print specialized help on '-l' or '--list'
     def list_h(self, arg:str):
         print(colored('RepMan', 'blue'), ': Repository Manager (alias: Project Manager)')
         print(colored(f'v{self.version}\n', 'red'))
         print('help', colored('EXTENDED', 'blue'), f': help for \'{arg}\'\n')
         print('  | This argument is used to list all the proje- |')
         print('  | cts under RepMan\'s care.                     |')
         print('  |                                              |')
-        print('  |', colored('Format', 'red'), ': \'repman -l\' or \'repman --list\'      |')
+        print('  |', colored('Format', 'red')+': \'repman -l\' or \'repman --list\'       |')
         print('  |                                              |')
         print('\nEND')
         exit(0)
     
     # function to print specialized help on '-lp' or '--list-w-path'
     def listwpath_h(self, arg:str):
         print(colored('RepMan', 'blue'), ': Repository Manager (alias: Project Manager)')
         print(colored(f'v{self.version}\n', 'red'))
         print('help', colored('EXTENDED', 'blue'), f': help for \'{arg}\'\n')
         print('  | This argument is used to list all the proje- |')
         print('  | cts  and their paths under RepMan\'s care.    |')
         print('  |                                              |')
-        print('  |', colored(' Format', 'red'), ': \'repman -lp\'                       |')
+        print('  |', colored(' Format', 'red')+': \'repman -lp\'                        |')
         print('  |                                              |')
         print('\nEND')
         exit(0)
     
     # function to print specialized help on '-ae' or '--add-existing'
     def addexisting_h(self ,arg: str):
         print(colored('RepMan', 'blue'), ': Repository Manager (alias: Project Manager)')
         print(colored(f'v{self.version}\n', 'red'))
         print('help', colored('EXTENDED', 'blue'), f': help for \'{arg}\'\n')
         print('  | This argument is used to add pre-cloned dir- |')
         print('  | ectory under RepMan\'s care.                  |')
         print('  |                                              |')
-        print('  |', colored('Format', 'red'), ': \'repman -ae <path>\'                 |')
+        print('  |', colored('Format', 'red')+': \'repman -ae <path>\'                  |')
         print('  |                                              |')
         print('\nEND')
         exit(0)
     
     # function to print specialized help on '-al' or '--add-local'
     def addlocal_h(self, arg:str):
         print(colored('RepMan', 'blue'), ': Repository Manager (alias: Project Manager)')
@@ -151,27 +152,43 @@
         print('  | This argument is for adding local git repos- |')
         print('  | itory under RepMan\'s care.                   |')
         print('  |                                              |')
         print('  | You might be prompted to set the default     |')
         print('  | branch and remote repository link(if not yet |')
         print('  | created, then create one.)                   |')
         print('  |                                              |')
-        print('  |', colored('Format', 'red'), ': \'repman -al <path>\'                 |')
+        print('  |', colored('Format', 'red')+': \'repman -al <path>\'                  |')
         print('  |                                              |')
         print('\nEND')
         exit(0)
     
         # function to print specialized help on '-u' or '--update'
     def update_h(self, arg:str):
         print(colored('RepMan', 'blue'), ': Repository Manager (alias: Project Manager)')
         print(colored(f'v{self.version}\n', 'red'))
         print('help', colored('EXTENDED', 'blue'), f': help for \'{arg}\'\n')
         print('  | This argument is used to update a project    |')
         print('  | with github remote repository.               |')
         print('  |                                              |')
         print('  | Each file\'s commit msg will be asked.        |')
         print('  |                                              |')
-        print('  |', colored('Format', 'red'), ': \'repman -u <project-name>\'          |')
+        print('  |', colored('Format', 'red')+': \'repman -u <project-name>\'           |')
         print('  |                                              |')
         print(colored('\nNote', 'red'), ': Requires Internet Connectivity.')
         print('\nEND')
+        exit(0)
+    
+    def setremote_h(self, arg:str):
+        print(colored('RepMan', 'blue'), ': Repository Manager (alias: Project Manager)')
+        print(colored(f'v{self.version}\n', 'red'))
+        print('help', colored('EXTENDED', 'blue'), f': help for \'{arg}\'\n')
+        print('  | This argument is used to set the remote or-  |')
+        print('  | igin of a project. If remote is already set, |')
+        print('  | It will be overwritten.                      |')
+        print('  |                                              |')
+        print('  |', colored('Format', 'red')+': \'repman -sr <project> <remote>\'      |')
+        print('  |                                              |')
+        print('  | <remote> can be either in the form of a link |')
+        print('  | or <username>/<repo>                         |')
+        print('  |                                              |')
+        print('\nEND')
         exit(0)
```

### Comparing `RepMan-1.0.1/src/repman/repman.py` & `RepMan-1.0.2/src/repman/repman.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,318 +4,351 @@
 # Linux -> aarch64
 # MacOs -> AppleSilicon(arm64)
 
 __version__ = '1.0.1'
 
 from repman._repmanfunctions import funcdefs
 from repman._repmanhelps import helptext
+from termcolor import colored
 from optioner import options
 from sys import argv
-from termcolor import colored
+from re import match
+
 
 # list value removing function
 def rem(original:list[str], remove:list[str]) -> list[str]:
     removed:list[str] = []
     for x in original:
         if x not in remove:
             removed.append(x)
     
     return removed
 
 # main function
 def main():
-    # helptext
-    help = helptext(__version__)
-    # functions
-    funk = funcdefs(__version__)
-    # create arguments
-    shortargs = ['h', 'v', 'a', 'i', 'o', 'l', 'lp', 'ae', 'al', 'u']
-    longargs = ['help', 'version', 'add', 'init', 'open', 'list', 'list-w-path', 'add-existing', 'add-local', 'update']
-    
-    # All args
-    original = shortargs.copy()
-    original.extend(longargs)
-    
-    # mutually exclusive args
-    mutex = [
-        ['v', 'version'],rem(original, ['v', 'version', 'h', 'help']),
-        ['a', 'add'],rem(original, ['a', 'add', 'h', 'help']),
-        ['o','open'],rem(original, ['o','open', 'h', 'help']),
-        ['i', 'init'],rem(original, ['i', 'init', 'h', 'help']),
-        ['l', 'list'],rem(original, ['l', 'list', 'h', 'help']),
-        ['lp', 'list-w-path'],rem(original, ['lp', 'list-w-path', 'h', 'help']),
-        ['ae', 'add-existing'],rem(original, ['ae', 'add-existing', 'h', 'help']),
-        ['al', 'add-local'], rem(original, ['al', 'add-local', 'h', 'help']),
-        ['u', 'update'], rem(original, ['u', 'update', 'h', 'help'])
-    ]
-    
-    optctrl = options(shortargs, longargs, argv[1:], ifthisthennotthat=mutex)
-    
-    args, check, error, falseargs = optctrl._argparse()
-    
-    if not check:
-        print(colored('RepMan Err', 'red'), f': {error}')
-        exit(1)
-    else:
-        if len(args)==0:
-            if len(falseargs)>0:
-                print(colored('RepMan Err', 'red'), ': you got the wrong guy bruh.')
-                exit(1)
-            print(colored('RepMan Err', 'red'), ': Please tell me what to do.')
+    try:
+        # helptext
+        help = helptext(__version__)
+        # functions
+        funk = funcdefs(__version__)
+        # create arguments
+        shortargs = ['h', 'v', 'a', 'i', 'o', 'l', 'lp', 'ae', 'al', 'u', 'sr']
+        longargs = ['help', 'version', 'add', 'init', 'open', 'list', 'list-w-path', 'add-existing', 'add-local', 'update', 'set-remote']
+        
+        # All args
+        original = shortargs.copy()
+        original.extend(longargs)
+        
+        # mutually exclusive args
+        mutex = [
+            ['v', 'version'],rem(original, ['v', 'version', 'h', 'help']),
+            ['a', 'add'],rem(original, ['a', 'add', 'h', 'help']),
+            ['o','open'],rem(original, ['o','open', 'h', 'help']),
+            ['i', 'init'],rem(original, ['i', 'init', 'h', 'help']),
+            ['l', 'list'],rem(original, ['l', 'list', 'h', 'help']),
+            ['lp', 'list-w-path'],rem(original, ['lp', 'list-w-path', 'h', 'help']),
+            ['ae', 'add-existing'],rem(original, ['ae', 'add-existing', 'h', 'help']),
+            ['al', 'add-local'], rem(original, ['al', 'add-local', 'h', 'help']),
+            ['u', 'update'], rem(original, ['u', 'update', 'h', 'help']),
+            ['sr', 'set-remote'], rem(original, ['sr', 'set-remote', 'h', 'help'])
+        ]
+        
+        optctrl = options(shortargs, longargs, argv[1:], ifthisthennotthat=mutex)
+        
+        args, check, error, falseargs = optctrl._argparse()
+        
+        if not check:
+            print(colored('RepMan Err', 'red'), f': {error}')
             exit(1)
         else:
-            # help
-            if '-h' in args:
-                # check for other args if there, and show help accordingly
-                otherarg = ''
-                if len(args)==2:
-                    # if length of all args = 2, i.e some other arg is there
-                    # find -h's index, the other one must be the arg, the user is asking help for.
-                    index = args.index('-h')
-                    if index==0:
-                        otherarg = args[1]
+            if len(args)==0:
+                if len(falseargs)>0:
+                    print(colored('RepMan Err', 'red'), ': you got the wrong guy bruh.')
+                    exit(1)
+                print(colored('RepMan Err', 'red'), ': Please tell me what to do.')
+                exit(1)
+            else:
+                # help
+                if '-h' in args:
+                    # check for other args if there, and show help accordingly
+                    otherarg = ''
+                    if len(args)==2:
+                        # if length of all args = 2, i.e some other arg is there
+                        # find -h's index, the other one must be the arg, the user is asking help for.
+                        index = args.index('-h')
+                        if index==0:
+                            otherarg = args[1]
+                        else:
+                            otherarg = args[0]
+                        
+                        if otherarg=='-h' or otherarg=='--help':
+                            help.base()
+                        elif otherarg=='-v' or otherarg=='--version':
+                            help.version_h(otherarg)
+                        elif otherarg=='-i' or otherarg=='--init':
+                            help.init_h(otherarg)
+                        elif otherarg=='-a' or otherarg=='--add':
+                            help.add_h(otherarg)
+                        elif otherarg=='-o' or otherarg=='--open':
+                            help.open_h(otherarg)
+                        elif otherarg == '-l' or otherarg == '--list':
+                            help.list_h(otherarg)
+                        elif otherarg == '-lp' or otherarg == '--list-w-path':
+                            help.listwpath_h(otherarg)
+                        elif otherarg == '-ae' or otherarg == '--add-existing':
+                            help.addexisting_h(otherarg)
+                        elif otherarg == '-al' or otherarg == '--add-local':
+                            help.addlocal_h(otherarg)
+                        elif otherarg == '-u' or otherarg == '--update':
+                            help.update_h(otherarg)
+                        elif otherarg == '-sr' or otherarg == '--set-remote':
+                            help.setremote_h(otherarg)
+                        else:
+                            print(colored('RepMan Err', 'red'), f': argument \'{otherarg}\' is not recognised.')
+                    elif len(args)<2:
+                        help.base()
+                    elif len(args)>2:
+                        print(colored('RepMan Err', 'red'), ': Please use one argument at a time to show help on that argument.')
+                        print(colored('Format', 'blue'), ': \'repman <argument> -h\' or \'repman <argument> --help\'.')
+                        exit(1)
                     else:
-                        otherarg = args[0]
-                    
-                    if otherarg=='-h' or otherarg=='--help':
+                        print(colored('RepMan Err', 'red'), ': Could not resolve arguments.')
+                        print(colored('RepMan Hint', 'blue'), ': Run \'repman -h\' or \'repman --help\'.')
+                        exit(1)
+                elif '--help' in args:
+                    # check for other args if there, and show help accordingly
+                    otherarg = ''
+                    if len(args)==2:
+                        # if length of all args = 2, i.e some other arg is there
+                        # find -h's index, the other one must be the arg, the user is asking help for.
+                        index = args.index('--help')
+                        if index==0:
+                            otherarg = args[1]
+                        else:
+                            otherarg = args[0]
+                        
+                        if otherarg=='-h' or otherarg=='--help':
+                            help.base()
+                        elif otherarg=='-v' or otherarg=='--version':
+                            help.version_h(otherarg)
+                        elif otherarg=='-i' or otherarg=='--init':
+                            help.init_h(otherarg)
+                        elif otherarg=='-a' or otherarg=='--add':
+                            help.add_h(otherarg)
+                        elif otherarg=='-o' or otherarg=='--open':
+                            help.open_h(otherarg)
+                        elif otherarg == '-l' or otherarg == '--list':
+                            help.list_h(otherarg)
+                        elif otherarg == '-lp' or otherarg == '--list-w-path':
+                            help.listwpath_h(otherarg)
+                        elif otherarg == '-ae' or otherarg == '--add-existing':
+                            help.addexisting_h(otherarg)
+                        elif otherarg == '-al' or otherarg == '--add-local':
+                            help.addlocal_h(otherarg)
+                        elif otherarg == '-u' or otherarg == '--update':
+                            help.update_h(otherarg)
+                        elif otherarg == '-sr' or otherarg == '--set-remote':
+                            help.setremote_h(otherarg)
+                        else:
+                            print(colored('RepMan Err', 'red'), f': argument \'{otherarg}\' is not recognised.')
+                    elif len(args)<2:
                         help.base()
-                    elif otherarg=='-v' or otherarg=='--version':
-                        help.version_h(otherarg)
-                    elif otherarg=='-i' or otherarg=='--init':
-                        help.init_h(otherarg)
-                    elif otherarg=='-a' or otherarg=='--add':
-                        help.add_h(otherarg)
-                    elif otherarg=='-o' or otherarg=='--open':
-                        help.open_h(otherarg)
-                    elif otherarg == '-l' or otherarg == '--list':
-                        help.list_h(otherarg)
-                    elif otherarg == '-lp' or otherarg == '--list-w-path':
-                        help.listwpath_h(otherarg)
-                    elif otherarg == '-ae' or otherarg == '--add-existing':
-                        help.addexisting_h(otherarg)
-                    elif otherarg == '-al' or otherarg == '--add-local':
-                        help.addlocal_h(otherarg)
-                    elif otherarg == '-u' or otherarg == '--update':
-                        help.update_h(otherarg)
+                    elif len(args)>2:
+                        print(colored('RepMan Err', 'red'), ': Please use one argument at a time to show help on that argument.')
+                        print(colored('Format', 'blue'), ': \'repman <argument> -h\' or \'repman <argument> --help\'.')
+                        exit(1)
                     else:
-                        print(colored('RepMan Err', 'red'), f': argument \'{otherarg}\' is not recognised.')
-                elif len(args)<2:
-                    help.base()
-                elif len(args)>2:
-                    print(colored('RepMan Err', 'red'), ': Please use one argument at a time to show help on that argument.')
-                    print(colored('Format', 'blue'), ': \'repman <argument> -h\' or \'repman <argument> --help\'.')
-                    exit(1)
+                        print(colored('RepMan Err', 'red'), ': Could not resolve arguments.')
+                        print(colored('RepMan Hint', 'blue'), ': Run \'repman -h\' or \'repman --help\'.')
+                        exit(1)
                 else:
-                    print(colored('RepMan Err', 'red'), ': Could not resolve arguments.')
-                    print(colored('RepMan Hint', 'blue'), ': Run \'repman -h\' or \'repman --help\'.')
-                    exit(1)
-            elif '--help' in args:
-                # check for other args if there, and show help accordingly
-                otherarg = ''
-                if len(args)==2:
-                    # if length of all args = 2, i.e some other arg is there
-                    # find -h's index, the other one must be the arg, the user is asking help for.
-                    index = args.index('--help')
-                    if index==0:
-                        otherarg = args[1]
+                    pass
+                
+                # version
+                if '-v' in args or '--version' in args:
+                    help.version()
+                
+                # init
+                if '-i' in args:
+                    index = argv.index('-i')
+                    try:
+                        value = argv[index+1]
+                    except IndexError:
+                        value = None
+                    
+                    if value==None:
+                        funk.init()
                     else:
-                        otherarg = args[0]
+                        funk.init(value)
+                elif '--init' in args:
+                    index = argv.index('--init')
+                    try:
+                        value = argv[index+1]
+                    except IndexError:
+                        value = None
                     
-                    if otherarg=='-h' or otherarg=='--help':
-                        help.base()
-                    elif otherarg=='-v' or otherarg=='--version':
-                        help.version_h(otherarg)
-                    elif otherarg=='-i' or otherarg=='--init':
-                        help.init_h(otherarg)
-                    elif otherarg=='-a' or otherarg=='--add':
-                        help.add_h(otherarg)
-                    elif otherarg=='-o' or otherarg=='--open':
-                        help.open_h(otherarg)
-                    elif otherarg == '-l' or otherarg == '--list':
-                        help.list_h(otherarg)
-                    elif otherarg == '-lp' or otherarg == '--list-w-path':
-                        help.listwpath_h(otherarg)
-                    elif otherarg == '-ae' or otherarg == '--add-existing':
-                        help.addexisting_h(otherarg)
-                    elif otherarg == '-al' or otherarg == '--add-local':
-                        help.addlocal_h(otherarg)
-                    elif otherarg == '-u' or otherarg == '--update':
-                        help.update_h(otherarg)
+                    if value==None:
+                        funk.init()
                     else:
-                        print(colored('RepMan Err', 'red'), f': argument \'{otherarg}\' is not recognised.')
-                elif len(args)<2:
-                    help.base()
-                elif len(args)>2:
-                    print(colored('RepMan Err', 'red'), ': Please use one argument at a time to show help on that argument.')
-                    print(colored('Format', 'blue'), ': \'repman <argument> -h\' or \'repman <argument> --help\'.')
-                    exit(1)
-                else:
-                    print(colored('RepMan Err', 'red'), ': Could not resolve arguments.')
-                    print(colored('RepMan Hint', 'blue'), ': Run \'repman -h\' or \'repman --help\'.')
-                    exit(1)
-            else:
-                pass
-            
-            # version
-            if '-v' in args or '--version' in args:
-                help.version()
-            
-            # init
-            if '-i' in args:
-                index = argv.index('-i')
-                try:
-                    value = argv[index+1]
-                except IndexError:
-                    value = None
-                
-                if value==None:
-                    funk.init()
-                else:
-                    funk.init(value)
-            elif '--init' in args:
-                index = argv.index('--init')
-                try:
-                    value = argv[index+1]
-                except IndexError:
-                    value = None
-                
-                if value==None:
-                    funk.init()
-                else:
-                    funk.init(value)
-            
-            # add
-            if '-a' in args:
-                index = argv.index('-a')
-                try:
-                    value = argv[index+1]
-                except IndexError:
-                    value = None
-                
-                if value==None:
-                    print(colored('RepMan', 'red'), ': \'-a\' needs a value.')
-                    exit(1)
-                else:
-                    funk.add(value)
-            elif '--add' in args:
-                index = argv.index('--add')
-                
-                try:
-                    value = argv[index+1]
-                except IndexError:
-                    value = None
+                        funk.init(value)
                 
-                if value==None:
-                    print(colored('RepMan', 'red'), ': \'--add\' needs a value.')
-                    exit(1)
-                else:
-                    funk.add(value)
-            
-            # add existing
-            if '-ae' in args:
-                index = argv.index('-ae')
-                
-                value:list[str] = []
-                try:
-                    for i in range(index+1, len(argv)):
-                        value.append(argv[i])
-                except IndexError:
-                    print(colored('RepMan', 'red'), ': \'-ae\' needs atleast one value.')
-                    exit(1)
-                
-                funk.addexisting(value)
-                
-            elif '--add-existing' in args:
-                index = argv.index('--add-existing')
-                
-                value:list[str] = []
-                try:
-                    for i in range(index+1, len(argv)):
-                        value.append(argv[i])
-                except IndexError:
-                    print(colored('RepMan', 'red'), ': \'--add-existing\' needs atleast one value.')
-                    exit(1)
-                
-                funk.addexisting(value)
-            
-            # list
-            if '-l' in args or '--list' in args:
-                funk.lister(False)
-            
-            # list with path
-            if '-lp' in args or '--list-w-path' in args:
-                funk.lister(True)
-            
-            # open
-            if '-o' in args:
-                index = argv.index('-o')
-                
-                value:list[str] = []
-                try:
-                    for i in range(index+1, len(argv)):
-                        value.append(argv[i])
-                except IndexError:
-                    print(colored('RepMan', 'red'), ': \'-o\' needs atleast one value.')
-                    exit(1)
+                # add
+                if '-a' in args:
+                    index = argv.index('-a')
+                    try:
+                        value = argv[index+1]
+                    except IndexError:
+                        value = None
+                    
+                    if value==None:
+                        print(colored('RepMan', 'red'), ': \'-a\' needs a value.')
+                        exit(1)
+                    else:
+                        funk.add(value)
+                elif '--add' in args:
+                    index = argv.index('--add')
+                    
+                    try:
+                        value = argv[index+1]
+                    except IndexError:
+                        value = None
+                    
+                    if value==None:
+                        print(colored('RepMan', 'red'), ': \'--add\' needs a value.')
+                        exit(1)
+                    else:
+                        funk.add(value)
                 
-                funk.openthis(value)
-            elif '--open' in args:
-                index = argv.index('--open')
-                
-                value:list[str] = []
-                try:
-                    for i in range(index+1, len(argv)):
-                        value.append(argv[i])
-                except IndexError:
-                    print(colored('RepMan', 'red'), ': \'--open\' needs atleast one value.')
-                    exit(1)
+                # add existing
+                if '-ae' in args:
+                    index = argv.index('-ae')
+                    
+                    value:list[str] = []
+                    try:
+                        for i in range(index+1, len(argv)):
+                            value.append(argv[i])
+                    except IndexError:
+                        print(colored('RepMan', 'red'), ': \'-ae\' needs atleast one value.')
+                        exit(1)
+                    
+                    funk.addexisting(value)
+                    
+                elif '--add-existing' in args:
+                    index = argv.index('--add-existing')
+                    
+                    value:list[str] = []
+                    try:
+                        for i in range(index+1, len(argv)):
+                            value.append(argv[i])
+                    except IndexError:
+                        print(colored('RepMan', 'red'), ': \'--add-existing\' needs atleast one value.')
+                        exit(1)
+                    
+                    funk.addexisting(value)
                 
-                funk.openthis(value)
-            
-            # update
-            if '-u' in args:
-                index = argv.index('-u')
-                try:
-                    value = argv[index+1]
-                    funk.update(value)
-                except IndexError:
-                    print(colored('RepMan', 'red'), ': \'-u\' needs a value.')
-                    exit(1)
-            elif '--update' in args:
-                index = argv.index('--update')
-                try:
-                    value = argv[index+1]
-                    funk.update(value)
-                except IndexError:
-                    print(colored('RepMan', 'red'), ': \'--update\' needs a value.')
-                    exit(1)
-            
-            # add local
-            if '-al' in args:
-                index = argv.index('-al')
-                value:list[str] = []
-                try:
-                    for i in range(index+1, len(argv)):
-                        value.append(argv[i])
-                except IndexError:
-                    print(colored('RepMan', 'red'), ': \'-al\' needs atleast one value.')
-                    exit(1)
+                # list
+                if '-l' in args or '--list' in args:
+                    funk.lister(False)
+                
+                # list with path
+                if '-lp' in args or '--list-w-path' in args:
+                    funk.lister(True)
+                
+                # open
+                if '-o' in args:
+                    index = argv.index('-o')
+                    
+                    value:list[str] = []
+                    try:
+                        for i in range(index+1, len(argv)):
+                            value.append(argv[i])
+                    except IndexError:
+                        print(colored('RepMan', 'red'), ': \'-o\' needs atleast one value.')
+                        exit(1)
+                    
+                    funk.openthis(value)
+                elif '--open' in args:
+                    index = argv.index('--open')
+                    
+                    value:list[str] = []
+                    try:
+                        for i in range(index+1, len(argv)):
+                            value.append(argv[i])
+                    except IndexError:
+                        print(colored('RepMan', 'red'), ': \'--open\' needs atleast one value.')
+                        exit(1)
+                    
+                    funk.openthis(value)
                 
+                # update
+                if '-u' in args:
+                    index = argv.index('-u')
+                    try:
+                        value = argv[index+1]
+                        funk.update(value)
+                    except IndexError:
+                        print(colored('RepMan', 'red'), ': \'-u\' needs a value.')
+                        exit(1)
+                elif '--update' in args:
+                    index = argv.index('--update')
+                    try:
+                        value = argv[index+1]
+                        funk.update(value)
+                    except IndexError:
+                        print(colored('RepMan', 'red'), ': \'--update\' needs a value.')
+                        exit(1)
+                
+                # add local
+                if '-al' in args:
+                    index = argv.index('-al')
+                    value:list[str] = []
+                    try:
+                        for i in range(index+1, len(argv)):
+                            value.append(argv[i])
+                    except IndexError:
+                        print(colored('RepMan', 'red'), ': \'-al\' needs atleast one value.')
+                        exit(1)
+                elif '--add-local' in args:
+                    index = argv.index('--add-local')
+                    value:list[str] = []
+                    try:
+                        for i in range(index+1, len(argv)):
+                            value.append(argv[i])
+                    except IndexError:
+                        print(colored('RepMan', 'red'), ': \'--add-local\' needs atleast one value.')
+                        exit(1)
+                    
                 funk.addlocal(value)
-            elif '--add-local' in args:
-                index = argv.index('--add-local')
-                value:list[str] = []
-                try:
-                    for i in range(index+1, len(argv)):
-                        value.append(argv[i])
-                except IndexError:
-                    print(colored('RepMan', 'red'), ': \'--add-local\' needs atleast one value.')
-                    exit(1)
                 
-                funk.addlocal(value)
+                # set remote
+                if '-sr' in args:
+                    index = argv.index('-sr')
+                    value:list[str] = []
+                    try:
+                        for i in range(index+1, len(argv)):
+                            value.append(argv[i])
+                    except IndexError:
+                        print(colored('RepMan', 'red')+': \'-sr\' needs two values. <project> and <remote>')
+                        exit(1)
+                    
+                    project:str = ''
+                    remote:str = ''
+                    if len(value)==2:
+                        for v in value:
+                            if match(r'^https://github.com/\w+/\w+', v) or match(r'^\w+/\w+', v):
+                                remote = v
+                            else:
+                                project = v
+                        funk.setremote(project, remote)
+                    else:
+                        print(colored('RepMan', 'red')+': \'-sr\' accepts only two values')
+                        exit(1)
+                    
+    except KeyboardInterrupt:
+        print('\n'+colored('RepMan', 'red')+": Decide Karen!")
                 
 
 if __name__=='__main__':
     try:
         main()
     except KeyboardInterrupt:
         print('\nRepMan: Keyboard Interrupt')
```

