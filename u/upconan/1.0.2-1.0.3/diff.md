# Comparing `tmp/upconan-1.0.2.tar.gz` & `tmp/upconan-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upconan-1.0.2.tar", last modified: Fri May 19 13:20:55 2023, max compression
+gzip compressed data, was "upconan-1.0.3.tar", last modified: Mon May 22 05:13:23 2023, max compression
```

## Comparing `upconan-1.0.2.tar` & `upconan-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 13:20:54.999582 upconan-1.0.2/
--rw-rw-rw-   0        0        0     1062 2023-05-19 13:12:37.000000 upconan-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      452 2023-05-19 13:20:54.999582 upconan-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-05-19 13:13:20.000000 upconan-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-19 13:20:54.999582 upconan-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      813 2023-05-19 13:20:40.000000 upconan-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 13:20:54.987583 upconan-1.0.2/src/
--rw-rw-rw-   0        0        0        0 2023-04-18 02:21:11.000000 upconan-1.0.2/src/__init__.py
--rw-rw-rw-   0        0        0     4604 2023-05-19 13:08:26.000000 upconan-1.0.2/src/upconan.py
-drwxrwxrwx   0        0        0        0 2023-05-19 13:20:54.998583 upconan-1.0.2/upconan.egg-info/
--rw-rw-rw-   0        0        0      452 2023-05-19 13:20:54.000000 upconan-1.0.2/upconan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-05-19 13:20:54.000000 upconan-1.0.2/upconan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 13:20:54.000000 upconan-1.0.2/upconan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-19 13:20:54.000000 upconan-1.0.2/upconan.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-19 13:20:54.000000 upconan-1.0.2/upconan.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       20 2023-05-19 13:20:54.000000 upconan-1.0.2/upconan.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-19 13:20:54.000000 upconan-1.0.2/upconan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 05:13:23.168184 upconan-1.0.3/
+-rw-rw-rw-   0        0        0     1062 2023-05-19 13:12:37.000000 upconan-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      452 2023-05-22 05:13:23.168184 upconan-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-05-19 13:13:20.000000 upconan-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-22 05:13:23.168184 upconan-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      813 2023-05-22 05:12:10.000000 upconan-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 05:13:23.163165 upconan-1.0.3/src/
+-rw-rw-rw-   0        0        0        0 2023-04-18 02:21:11.000000 upconan-1.0.3/src/__init__.py
+-rw-rw-rw-   0        0        0     4913 2023-05-22 05:12:24.000000 upconan-1.0.3/src/upconan.py
+drwxrwxrwx   0        0        0        0 2023-05-22 05:13:23.168184 upconan-1.0.3/upconan.egg-info/
+-rw-rw-rw-   0        0        0      452 2023-05-22 05:13:23.000000 upconan-1.0.3/upconan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-05-22 05:13:23.000000 upconan-1.0.3/upconan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 05:13:23.000000 upconan-1.0.3/upconan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-22 05:13:23.000000 upconan-1.0.3/upconan.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-22 05:13:05.000000 upconan-1.0.3/upconan.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       20 2023-05-22 05:13:23.000000 upconan-1.0.3/upconan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-22 05:13:23.000000 upconan-1.0.3/upconan.egg-info/top_level.txt
```

### Comparing `upconan-1.0.2/LICENSE` & `upconan-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `upconan-1.0.2/setup.py` & `upconan-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
     name='upconan',
-    version="1.0.2",
+    version="1.0.3",
     description="一个更新conanfile的便捷工具",
     long_description="""从剪贴板复制conan包信息，更新当前路径下的conanfile.py或conanfile.txt文件中对应的conan包版本""",
     keywords='python conan',
     author='leytou',
     author_email='hi_litao@163.com',
     url='https://github.com/leytou/upconan',
     license='MIT',
```

### Comparing `upconan-1.0.2/src/upconan.py` & `upconan-1.0.3/src/upconan.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,24 @@
 import pyperclip
 from git.cmd import Git
 from git import Repo, GitCommandError,InvalidGitRepositoryError
 
 
 pattern = re.compile(r'(?P<name>[a-zA-Z0-9_]+)\/(?P<version>\d+(\.\d+){2,3})(\@(?P<owner>\w+))?(\/(?P<channel>[a-zA-Z0-9_]+))?')
 
-
+def GetNewlineType(filename):
+    with open(filename, 'r', newline='', encoding='utf-8') as f:
+        line = f.readline()
+        if '\r\n' in line:
+            return '\r\n'
+        elif '\n' in line:
+            return '\n'
+        elif '\r' in line:
+            print(3)
+        return ''
 
 def _GitCmd(cmd):
     git = Git(os.getcwd())
     return git.execute(cmd)
 
 def Diff(path):
     cmd = ["git", "-c", "color.ui=always", "diff", path]
@@ -84,15 +93,14 @@
             if target_package_info:
                 lines[idx] = UpdatePackageInfoLine(line,curent_package_info, target_package_info)
                 is_changed=True
        
 
     return lines
 
-    
 
 test_target_text='''asio/1.25.0
 hello/2.3.4@world/stable
 good/1.0.1@boy/snapshot
 
 1.修复一些已知问题
 2.优化性能
@@ -128,15 +136,15 @@
     if not conanfile :
         print(f"未找到文件:{file_list}") 
 
 
 
 
 
-def main():
+def Main():
     EnvCheck()
 
     target_package_infos = []
     while True:
         target_text = GetTargetText()
         target_package_infos = ParsePackageInfoText(target_text)
         if target_package_infos:
@@ -152,23 +160,26 @@
 
     with open(conanfile, "r") as inf:
         input_lines = inf.readlines()
         updated_lines = UpdatePackageInfoLines(input_lines,  target_package_infos)
 
         if is_changed:
             #写回原文件，替换文本
-            with open(conanfile, 'w', newline='\n') as outf:
+            with open(conanfile, 'w', newline=GetNewlineType(conanfile)) as outf:
                 outf.writelines(updated_lines)
 
-                # 检测是否是git项目，若是则打印修改项
-                if IsGitRepoRecursively(os.getcwd()):
-                    diff = Diff(conanfile)
-                    print(f'修改项:\n{diff}')
+            # 检测是否是git项目，若是则打印修改项
+            if IsGitRepoRecursively(os.getcwd()):
+                diff = Diff(conanfile)
+                print(f'修改项:\n{diff}')
         else:
             print("无修改")
 
    
 
 
+
+
 if __name__ == "__main__":
-    main()
+    EnvCheck()
+    Main()
```

