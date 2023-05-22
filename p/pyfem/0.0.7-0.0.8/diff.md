# Comparing `tmp/pyfem-0.0.7.tar.gz` & `tmp/pyfem-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfem-0.0.7.tar", last modified: Sun May 21 14:43:31 2023, max compression
+gzip compressed data, was "pyfem-0.0.8.tar", last modified: Mon May 22 04:05:01 2023, max compression
```

## Comparing `pyfem-0.0.7.tar` & `pyfem-0.0.8.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:31.562430 pyfem-0.0.7/
--rw-rw-rw-   0        0        0    11524 2023-05-03 09:58:16.000000 pyfem-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      793 2023-05-21 14:43:31.561438 pyfem-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-19 11:01:17.000000 pyfem-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-21 14:43:31.562430 pyfem-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      941 2023-05-21 14:39:32.000000 pyfem-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:31.466622 pyfem-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:31.479603 pyfem-0.0.7/src/pyfem/
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.7/src/pyfem/__init__.py
--rw-rw-rw-   0        0        0      927 2023-05-21 14:38:58.000000 pyfem-0.0.7/src/pyfem/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:31.491554 pyfem-0.0.7/src/pyfem/assembly/
--rw-rw-rw-   0        0        0     8732 2023-05-20 17:12:32.000000 pyfem-0.0.7/src/pyfem/assembly/Assembly.py
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.7/src/pyfem/assembly/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:31.498903 pyfem-0.0.7/src/pyfem/bc/
--rw-rw-rw-   0        0        0      781 2023-05-19 11:01:17.000000 pyfem-0.0.7/src/pyfem/bc/BaseBC.py
--rw-rw-rw-   0        0        0     2262 2023-05-19 14:23:03.000000 pyfem-0.0.7/src/pyfem/bc/DirichletBC.py
--rw-rw-rw-   0        0        0        0 2023-05-19 11:01:17.000000 pyfem-0.0.7/src/pyfem/bc/__init__.py
--rw-rw-rw-   0        0        0      876 2023-05-19 11:01:17.000000 pyfem-0.0.7/src/pyfem/bc/get_bc_data.py
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:31.510827 pyfem-0.0.7/src/pyfem/elements/
--rw-rw-rw-   0        0        0     4293 2023-05-20 15:49:28.000000 pyfem-0.0.7/src/pyfem/elements/BaseElement.py
--rw-rw-rw-   0        0        0     1793 2023-05-18 15:11:46.000000 pyfem-0.0.7/src/pyfem/elements/IsoElementDiagram.py
--rw-rw-rw-   0        0        0    19983 2023-05-19 11:01:17.000000 pyfem-0.0.7/src/pyfem/elements/IsoElementShape.py
--rw-rw-rw-   0        0        0     4367 2023-05-20 16:49:40.000000 pyfem-0.0.7/src/pyfem/elements/SolidPlaneSmallStrain.py
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.7/src/pyfem/elements/__init__.py
--rw-rw-rw-   0        0        0     1894 2023-05-18 11:01:59.000000 pyfem-0.0.7/src/pyfem/elements/get_element_data.py
--rw-rw-rw-   0        0        0     1793 2023-05-17 14:10:35.000000 pyfem-0.0.7/src/pyfem/elements/get_iso_element_type.py
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:31.512315 pyfem-0.0.7/src/pyfem/fem/
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.7/src/pyfem/fem/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:31.531134 pyfem-0.0.7/src/pyfem/io/
--rw-rw-rw-   0        0        0      679 2023-05-19 11:01:17.000000 pyfem-0.0.7/src/pyfem/io/BC.py
--rw-rw-rw-   0        0        0      577 2023-05-18 14:20:30.000000 pyfem-0.0.7/src/pyfem/io/Dof.py
--rw-rw-rw-   0        0        0     2299 2023-05-18 15:11:46.000000 pyfem-0.0.7/src/pyfem/io/Material.py
--rw-rw-rw-   0        0        0      520 2023-05-18 14:20:30.000000 pyfem-0.0.7/src/pyfem/io/Mesh.py
--rw-rw-rw-   0        0        0      575 2023-05-20 17:12:32.000000 pyfem-0.0.7/src/pyfem/io/Output.py
--rw-rw-rw-   0        0        0    10304 2023-05-21 14:35:56.000000 pyfem-0.0.7/src/pyfem/io/Properties.py
--rw-rw-rw-   0        0        0      815 2023-05-18 14:20:30.000000 pyfem-0.0.7/src/pyfem/io/Section.py
--rw-rw-rw-   0        0        0      466 2023-05-18 14:20:30.000000 pyfem-0.0.7/src/pyfem/io/Solver.py
--rw-rw-rw-   0        0        0        0 2023-04-19 14:26:23.000000 pyfem-0.0.7/src/pyfem/io/__init__.py
--rw-rw-rw-   0        0        0     1704 2023-05-21 14:40:55.000000 pyfem-0.0.7/src/pyfem/io/arguments.py
--rw-rw-rw-   0        0        0     3657 2023-05-21 14:31:44.000000 pyfem-0.0.7/src/pyfem/io/write_vtk.py
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:31.538161 pyfem-0.0.7/src/pyfem/materials/
--rw-rw-rw-   0        0        0      840 2023-05-18 15:34:49.000000 pyfem-0.0.7/src/pyfem/materials/BaseMaterial.py
--rw-rw-rw-   0        0        0     6168 2023-05-18 11:01:59.000000 pyfem-0.0.7/src/pyfem/materials/ElasticIsotropic.py
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.7/src/pyfem/materials/__init__.py
--rw-rw-rw-   0        0        0     1129 2023-05-18 15:11:46.000000 pyfem-0.0.7/src/pyfem/materials/get_material_data.py
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:31.543121 pyfem-0.0.7/src/pyfem/mesh/
--rw-rw-rw-   0        0        0     3282 2023-05-21 14:35:56.000000 pyfem-0.0.7/src/pyfem/mesh/ElementSet.py
--rw-rw-rw-   0        0        0     3478 2023-05-21 14:35:56.000000 pyfem-0.0.7/src/pyfem/mesh/NodeSet.py
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.7/src/pyfem/mesh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:31.549570 pyfem-0.0.7/src/pyfem/solvers/
--rw-rw-rw-   0        0        0      887 2023-05-20 17:07:22.000000 pyfem-0.0.7/src/pyfem/solvers/BaseSolver.py
--rw-rw-rw-   0        0        0      973 2023-05-20 17:12:32.000000 pyfem-0.0.7/src/pyfem/solvers/LinearSolver.py
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.7/src/pyfem/solvers/__init__.py
--rw-rw-rw-   0        0        0      920 2023-05-20 14:12:09.000000 pyfem-0.0.7/src/pyfem/solvers/get_solver_data.py
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:31.559980 pyfem-0.0.7/src/pyfem/utils/
--rw-rw-rw-   0        0        0     2313 2023-05-18 11:01:59.000000 pyfem-0.0.7/src/pyfem/utils/IntKeyDict.py
--rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.7/src/pyfem/utils/__init__.py
--rw-rw-rw-   0        0        0      707 2023-05-18 14:59:47.000000 pyfem-0.0.7/src/pyfem/utils/colors.py
--rw-rw-rw-   0        0        0     1516 2023-05-06 15:26:11.000000 pyfem-0.0.7/src/pyfem/utils/logger.py
--rw-rw-rw-   0        0        0     1738 2023-05-19 11:01:17.000000 pyfem-0.0.7/src/pyfem/utils/visualization.py
--rw-rw-rw-   0        0        0      982 2023-05-18 15:11:46.000000 pyfem-0.0.7/src/pyfem/utils/wrappers.py
-drwxrwxrwx   0        0        0        0 2023-05-21 14:43:31.488082 pyfem-0.0.7/src/pyfem.egg-info/
--rw-rw-rw-   0        0        0      793 2023-05-21 14:43:31.000000 pyfem-0.0.7/src/pyfem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1493 2023-05-21 14:43:31.000000 pyfem-0.0.7/src/pyfem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 14:43:31.000000 pyfem-0.0.7/src/pyfem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-21 14:43:31.000000 pyfem-0.0.7/src/pyfem.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-05-21 14:43:31.000000 pyfem-0.0.7/src/pyfem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 04:05:01.969822 pyfem-0.0.8/
+-rw-rw-rw-   0        0        0    11525 2023-05-04 02:49:52.000000 pyfem-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      793 2023-05-22 04:05:01.968822 pyfem-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-19 03:01:04.000000 pyfem-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-22 04:05:01.969822 pyfem-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      941 2023-05-22 04:03:18.000000 pyfem-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 04:05:01.904823 pyfem-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-05-22 04:05:01.915823 pyfem-0.0.8/src/pyfem/
+-rw-rw-rw-   0        0        0      857 2023-05-22 03:57:50.000000 pyfem-0.0.8/src/pyfem/Job.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.8/src/pyfem/__init__.py
+-rw-rw-rw-   0        0        0      277 2023-05-22 03:59:51.000000 pyfem-0.0.8/src/pyfem/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 04:05:01.922823 pyfem-0.0.8/src/pyfem/assembly/
+-rw-rw-rw-   0        0        0     8732 2023-05-22 02:53:25.000000 pyfem-0.0.8/src/pyfem/assembly/Assembly.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.8/src/pyfem/assembly/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 04:05:01.926823 pyfem-0.0.8/src/pyfem/bc/
+-rw-rw-rw-   0        0        0      781 2023-05-19 07:42:39.000000 pyfem-0.0.8/src/pyfem/bc/BaseBC.py
+-rw-rw-rw-   0        0        0     2262 2023-05-22 02:53:25.000000 pyfem-0.0.8/src/pyfem/bc/DirichletBC.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.8/src/pyfem/bc/__init__.py
+-rw-rw-rw-   0        0        0      876 2023-05-19 09:14:01.000000 pyfem-0.0.8/src/pyfem/bc/get_bc_data.py
+drwxrwxrwx   0        0        0        0 2023-05-22 04:05:01.934822 pyfem-0.0.8/src/pyfem/elements/
+-rw-rw-rw-   0        0        0     4293 2023-05-22 02:53:25.000000 pyfem-0.0.8/src/pyfem/elements/BaseElement.py
+-rw-rw-rw-   0        0        0     1793 2023-05-15 02:23:48.000000 pyfem-0.0.8/src/pyfem/elements/IsoElementDiagram.py
+-rw-rw-rw-   0        0        0    19983 2023-05-19 05:44:29.000000 pyfem-0.0.8/src/pyfem/elements/IsoElementShape.py
+-rw-rw-rw-   0        0        0     4367 2023-05-22 02:53:25.000000 pyfem-0.0.8/src/pyfem/elements/SolidPlaneSmallStrain.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.8/src/pyfem/elements/__init__.py
+-rw-rw-rw-   0        0        0     1894 2023-05-18 07:52:50.000000 pyfem-0.0.8/src/pyfem/elements/get_element_data.py
+-rw-rw-rw-   0        0        0     1793 2023-05-18 05:01:54.000000 pyfem-0.0.8/src/pyfem/elements/get_iso_element_type.py
+drwxrwxrwx   0        0        0        0 2023-05-22 04:05:01.936823 pyfem-0.0.8/src/pyfem/fem/
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.8/src/pyfem/fem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 04:05:01.948822 pyfem-0.0.8/src/pyfem/io/
+-rw-rw-rw-   0        0        0      679 2023-05-19 08:44:54.000000 pyfem-0.0.8/src/pyfem/io/BC.py
+-rw-rw-rw-   0        0        0      577 2023-05-19 02:59:20.000000 pyfem-0.0.8/src/pyfem/io/Dof.py
+-rw-rw-rw-   0        0        0     2299 2023-05-19 02:59:20.000000 pyfem-0.0.8/src/pyfem/io/Material.py
+-rw-rw-rw-   0        0        0      520 2023-05-19 02:59:20.000000 pyfem-0.0.8/src/pyfem/io/Mesh.py
+-rw-rw-rw-   0        0        0      575 2023-05-22 02:53:25.000000 pyfem-0.0.8/src/pyfem/io/Output.py
+-rw-rw-rw-   0        0        0    10250 2023-05-22 03:55:12.000000 pyfem-0.0.8/src/pyfem/io/Properties.py
+-rw-rw-rw-   0        0        0      815 2023-05-19 02:59:20.000000 pyfem-0.0.8/src/pyfem/io/Section.py
+-rw-rw-rw-   0        0        0      466 2023-05-19 02:59:20.000000 pyfem-0.0.8/src/pyfem/io/Solver.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.8/src/pyfem/io/__init__.py
+-rw-rw-rw-   0        0        0     1704 2023-05-22 04:03:27.000000 pyfem-0.0.8/src/pyfem/io/arguments.py
+-rw-rw-rw-   0        0        0     3224 2023-05-22 04:02:40.000000 pyfem-0.0.8/src/pyfem/io/write_vtk.py
+drwxrwxrwx   0        0        0        0 2023-05-22 04:05:01.953823 pyfem-0.0.8/src/pyfem/materials/
+-rw-rw-rw-   0        0        0      840 2023-05-19 02:59:20.000000 pyfem-0.0.8/src/pyfem/materials/BaseMaterial.py
+-rw-rw-rw-   0        0        0     5986 2023-05-18 08:03:05.000000 pyfem-0.0.8/src/pyfem/materials/ElasticIsotropic.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.8/src/pyfem/materials/__init__.py
+-rw-rw-rw-   0        0        0     1129 2023-05-19 02:59:20.000000 pyfem-0.0.8/src/pyfem/materials/get_material_data.py
+drwxrwxrwx   0        0        0        0 2023-05-22 04:05:01.956831 pyfem-0.0.8/src/pyfem/mesh/
+-rw-rw-rw-   0        0        0     3282 2023-05-22 02:53:25.000000 pyfem-0.0.8/src/pyfem/mesh/ElementSet.py
+-rw-rw-rw-   0        0        0     3482 2023-05-22 03:16:36.000000 pyfem-0.0.8/src/pyfem/mesh/NodeSet.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.8/src/pyfem/mesh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 04:05:01.960822 pyfem-0.0.8/src/pyfem/solvers/
+-rw-rw-rw-   0        0        0      887 2023-05-22 02:53:25.000000 pyfem-0.0.8/src/pyfem/solvers/BaseSolver.py
+-rw-rw-rw-   0        0        0      966 2023-05-22 03:16:04.000000 pyfem-0.0.8/src/pyfem/solvers/LinearSolver.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.8/src/pyfem/solvers/__init__.py
+-rw-rw-rw-   0        0        0      854 2023-05-22 03:15:35.000000 pyfem-0.0.8/src/pyfem/solvers/get_solver_data.py
+drwxrwxrwx   0        0        0        0 2023-05-22 04:05:01.967822 pyfem-0.0.8/src/pyfem/utils/
+-rw-rw-rw-   0        0        0     2313 2023-05-18 08:06:24.000000 pyfem-0.0.8/src/pyfem/utils/IntKeyDict.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.8/src/pyfem/utils/__init__.py
+-rw-rw-rw-   0        0        0      707 2023-05-19 02:59:20.000000 pyfem-0.0.8/src/pyfem/utils/colors.py
+-rw-rw-rw-   0        0        0     1516 2023-05-08 04:08:44.000000 pyfem-0.0.8/src/pyfem/utils/logger.py
+-rw-rw-rw-   0        0        0     1738 2023-05-19 09:23:55.000000 pyfem-0.0.8/src/pyfem/utils/visualization.py
+-rw-rw-rw-   0        0        0      982 2023-05-19 02:59:20.000000 pyfem-0.0.8/src/pyfem/utils/wrappers.py
+drwxrwxrwx   0        0        0        0 2023-05-22 04:05:01.920823 pyfem-0.0.8/src/pyfem.egg-info/
+-rw-rw-rw-   0        0        0      793 2023-05-22 04:05:01.000000 pyfem-0.0.8/src/pyfem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1510 2023-05-22 04:05:01.000000 pyfem-0.0.8/src/pyfem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 04:05:01.000000 pyfem-0.0.8/src/pyfem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-22 04:05:01.000000 pyfem-0.0.8/src/pyfem.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-05-22 04:05:01.000000 pyfem-0.0.8/src/pyfem.egg-info/top_level.txt
```

### Comparing `pyfem-0.0.7/LICENSE` & `pyfem-0.0.8/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -194,8 +194,8 @@
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
-   limitations under the License.
+   limitations under the License.
```

### Comparing `pyfem-0.0.7/PKG-INFO` & `pyfem-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfem
-Version: 0.0.7
+Version: 0.0.8
 Summary: A finite element package for learning
 Home-page: https://github.com/sunwhale/pyfem
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyfem-0.0.7/setup.py` & `pyfem-0.0.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyfem",
-    version="0.0.7",
+    version="0.0.8",
     author="Jingyu Sun",
     author_email="sun.jingyu@outlook.com",
     description="A finite element package for learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sunwhale/pyfem",
     project_urls={
```

### Comparing `pyfem-0.0.7/src/pyfem/__main__.py` & `pyfem-0.0.8/src/pyfem/solvers/get_solver_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,25 @@
-# -*- coding: utf-8 -*-
-"""
-
-"""
-from pathlib import Path
-
 from pyfem.assembly.Assembly import Assembly
-from pyfem.io.Properties import Properties
-from pyfem.io.arguments import get_arguments
-from pyfem.io.write_vtk import write_vtk
-from pyfem.solvers.get_solver_data import get_solver_data
-from pyfem.utils.wrappers import show_running_time
-
-
-@show_running_time
-def main(base_path: Path = Path.cwd()) -> None:
-    args = get_arguments()
-
-    props = Properties()
-
-    props.base_path = base_path
-
-    input_file = Path(args.i)
-
-    if input_file.is_absolute():
-        abs_input_file = input_file
+from pyfem.io.Solver import Solver
+from pyfem.solvers.BaseSolver import BaseSolver
+from pyfem.solvers.LinearSolver import LinearSolver
+from pyfem.utils.colors import error_style
+
+solver_data_dict = {
+    'LinearSolver': LinearSolver
+}
+
+
+def get_solver_data(assembly: Assembly, solver: Solver) -> BaseSolver:
+    class_name = f'{solver.type}'.strip().replace(' ', '')
+
+    if class_name in solver_data_dict:
+        return solver_data_dict[class_name](assembly=assembly,
+                                            solver=solver)
     else:
-        abs_input_file = base_path.joinpath(input_file)
-
-    props.read_file(abs_input_file)
-
-    props.verify()
-
-    props.show()
-
-    assembly = Assembly(props)
-
-    solver_data = get_solver_data(assembly, props.solver)
+        error_msg = f'{class_name} solver is not supported.\n'
+        error_msg += f'The allowed solver types are {list(solver_data_dict.keys())}.'
+        raise NotImplementedError(error_style(error_msg))
 
-    solver_data.run()
 
-    write_vtk(props, assembly)
+if __name__ == "__main__":
+    pass
```

### Comparing `pyfem-0.0.7/src/pyfem/assembly/Assembly.py` & `pyfem-0.0.8/src/pyfem/assembly/Assembly.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.7/src/pyfem/bc/BaseBC.py` & `pyfem-0.0.8/src/pyfem/bc/BaseBC.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.7/src/pyfem/bc/DirichletBC.py` & `pyfem-0.0.8/src/pyfem/bc/DirichletBC.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.7/src/pyfem/bc/get_bc_data.py` & `pyfem-0.0.8/src/pyfem/bc/get_bc_data.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.7/src/pyfem/elements/BaseElement.py` & `pyfem-0.0.8/src/pyfem/elements/BaseElement.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.7/src/pyfem/elements/IsoElementDiagram.py` & `pyfem-0.0.8/src/pyfem/elements/IsoElementDiagram.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.7/src/pyfem/elements/IsoElementShape.py` & `pyfem-0.0.8/src/pyfem/elements/IsoElementShape.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.7/src/pyfem/elements/SolidPlaneSmallStrain.py` & `pyfem-0.0.8/src/pyfem/elements/SolidPlaneSmallStrain.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.7/src/pyfem/elements/get_element_data.py` & `pyfem-0.0.8/src/pyfem/elements/get_element_data.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.7/src/pyfem/elements/get_iso_element_type.py` & `pyfem-0.0.8/src/pyfem/elements/get_iso_element_type.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.7/src/pyfem/io/BC.py` & `pyfem-0.0.8/src/pyfem/io/BC.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.7/src/pyfem/io/Dof.py` & `pyfem-0.0.8/src/pyfem/io/Dof.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.7/src/pyfem/io/Material.py` & `pyfem-0.0.8/src/pyfem/io/Material.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.7/src/pyfem/io/Mesh.py` & `pyfem-0.0.8/src/pyfem/io/Mesh.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.7/src/pyfem/io/Output.py` & `pyfem-0.0.8/src/pyfem/io/Output.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.7/src/pyfem/io/Properties.py` & `pyfem-0.0.8/src/pyfem/io/Properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,20 +25,19 @@
 
     1. Properties 类的所有属性在首次被赋非None值后不能再被修改和删除，
 
     2. 此时许可的属性关键字存储在self.slots中。
     """
     is_read_only: bool = True
     slots: Tuple = (
-        'base_path', 'work_path', 'input_file', 'toml', 'title', 'mesh', 'dof', 'materials', 'sections', 'bcs',
+        'work_path', 'input_file', 'toml', 'title', 'mesh', 'dof', 'materials', 'sections', 'bcs',
         'solver',
         'outputs', 'nodes', 'elements')
 
     def __init__(self) -> None:
-        self.base_path: Path = None  # type: ignore
         self.work_path: Path = None  # type: ignore
         self.input_file: Path = None  # type: ignore
         self.toml: Dict = None  # type: ignore
         self.title: str = None  # type: ignore
         self.mesh: Mesh = None  # type: ignore
         self.dof: Dof = None  # type: ignore
         self.materials: List[Material] = None  # type: ignore
@@ -69,15 +68,15 @@
         else:
             super().__delattr__(key)
 
     def verify(self) -> None:
         print(info_style('Verifying the input ...'))
         is_error = False
         error_msg = '\nInput error:\n'
-        for key in self.slots[3:]:  # 忽略这3个关键字：'base_path', 'work_path', 'input_file'，它们不是在.toml中定义的
+        for key in self.slots[2:]:  # 忽略这2个关键字：'work_path', 'input_file'，它们不是在.toml中定义的
             if self.__getattribute__(key) is None:
                 is_error = True
                 error_msg += f'  - {key} is missing\n'
 
         if is_error:
             error_msg += f'Please check the input file {self.input_file}'
             raise NotImplementedError(error_style(error_msg))
@@ -250,13 +249,15 @@
             solver_dict = self.toml['solver']
             self.set_solver(solver_dict)
 
         if 'outputs' in toml_keys:
             outputs_dict = self.toml['outputs']
             self.set_outputs(outputs_dict)
 
+        self.verify()
+
 
 if __name__ == "__main__":
     props = Properties()
     # props.show()
     props.read_file(r'F:\Github\pyfem\examples\rectangle\rectangle.toml')
     props.show()
```

### Comparing `pyfem-0.0.7/src/pyfem/io/Section.py` & `pyfem-0.0.8/src/pyfem/io/Section.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.7/src/pyfem/io/arguments.py` & `pyfem-0.0.8/src/pyfem/io/arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     # 添加帮助选项
     parser.add_argument('-h', '--help', action='help', default=SUPPRESS,
                         help='Show this help message and exit.')
 
     # 添加版本选项
     parser.add_argument('-v', '--version', action='version', help='Show program\'s version number and exit.',
-                        version='pyfem 0.0.7')
+                        version='pyfem 0.0.8')
 
     # 解析命令行参数
     args = parser.parse_args()
 
     # 如果未指定程序输入文件，则打印帮助并退出
     if not args.i:
         print('--------------------------------------')
```

### Comparing `pyfem-0.0.7/src/pyfem/io/write_vtk.py` & `pyfem-0.0.8/src/pyfem/io/write_vtk.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         field = SubElement(point_data, "DataArray", {
             "type": "Float64",
             "Name": field_name,
             "NumberOfComponents": "1",
             "format": "ascii"
         })
         field.text = ""
-        for value in assembly.field_variables[field_name]:
+        for value in field_values:
             field.text += f"{value}\n"
 
     #
     points = SubElement(piece, "Points")
     node_coords = SubElement(points, "DataArray", {
         "type": "Float64",
         "NumberOfComponents": "3",
@@ -97,22 +97,8 @@
 
     output_file = props.work_path.joinpath(job_name + '.vtu')
 
     tree.write(output_file, xml_declaration=True, encoding='utf-8')
 
 
 if __name__ == "__main__":
-    from pyfem.io.Properties import Properties
-    from pyfem.assembly.Assembly import Assembly
-    from pyfem.solvers.get_solver_data import get_solver_data
-
-    props = Properties()
-    props.read_file(r'rectangle.toml')
-    props.verify()
-    props.show()
-    assembly = Assembly(props)
-
-    solver_data = get_solver_data(assembly, props.solver)
-
-    solver_data.run()
-
-    write_vtk(props, assembly)
+    pass
```

### Comparing `pyfem-0.0.7/src/pyfem/materials/BaseMaterial.py` & `pyfem-0.0.8/src/pyfem/materials/BaseMaterial.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.7/src/pyfem/materials/ElasticIsotropic.py` & `pyfem-0.0.8/src/pyfem/materials/ElasticIsotropic.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,182 +1,182 @@
-from typing import Optional, Tuple
-
-from numpy import array, outer, diag, float64, ndarray
-
-from pyfem.io.Material import Material
-from pyfem.materials.BaseMaterial import BaseMaterial
-from pyfem.utils.colors import error_style
-
-
-class ElasticIsotropic(BaseMaterial):
-    allowed_option = ['PlaneStress', 'PlaneStrain', None]
-
-    def __init__(self, material: Material, dimension: int, option: Optional[str] = None) -> None:
-        super().__init__(material, dimension, option)
-        self.create_tangent()
-
-    def create_tangent(self):
-        young = self.material.data[0]
-        poisson = self.material.data[1]
-
-        if self.option in self.allowed_option:
-            if self.dimension == 3:
-                self.option = None
-            self.ddsdde = get_stiffness_from_young_poisson(self.dimension, young, poisson, self.option)
-        else:
-            error_msg = f'{self.option} is not the allowed options {self.allowed_option}'
-            raise NotImplementedError(error_style(error_msg))
-
-
-def get_lame_from_young_poisson(young: float, poisson: float, plane: Optional[str]) -> Tuple[float, float]:
-    r"""
-    Compute Lamé parameters from Young's modulus and Poisson's ratio.
-
-    The relationship between Lamé parameters and Young's modulus, Poisson's
-    ratio (see [1],[2]):
-
-    .. math::
-        \lambda = {\nu E \over (1+\nu)(1-2\nu)},\qquad \mu = {E \over 2(1+\nu)}
-
-    The plain stress hypothesis:
-
-    .. math::
-       \bar\lambda = {2\lambda\mu \over \lambda + 2\mu}
-
-    [1] I.S. Sokolnikoff: Mathematical Theory of Elasticity. New York, 1956.
-
-    [2] T.J.R. Hughes: The Finite Element Method, Linear Static and Dynamic
-    Finite Element Analysis. New Jersey, 1987.
-    """
-    mu = young / (2.0 * (1.0 + poisson))
-    lam = young * poisson / ((1.0 + poisson) * (1.0 - 2.0 * poisson))
-
-    if plane == 'PlaneStress':
-        lam = 2 * lam * mu / (lam + 2 * mu)
-
-    return lam, mu
-
-
-def get_stiffness_from_lame(dim: int, lam: float, mu: float) -> ndarray:
-    r"""
-    Compute stiffness tensor corresponding to Lamé parameters.
-
-    .. math::
-        {\bf D}_{(2D)} = \begin{bmatrix} \lambda + 2\mu & \lambda & 0\\
-        \lambda & \lambda + 2\mu & 0\\ 0 & 0 & \mu \end{bmatrix}
-
-    .. math::
-        {\bf D}_{(3D)} = \begin{bmatrix} \lambda + 2\mu & \lambda &
-        \lambda & 0 & 0 & 0\\ \lambda & \lambda + 2\mu & \lambda & 0 & 0 & 0 \\
-        \lambda & \lambda & \lambda + 2\mu & 0 & 0 & 0 \\ 0 & 0 & 0 & \mu & 0 &
-        0 \\ 0 & 0 & 0 & 0 & \mu & 0 \\ 0 & 0 & 0 & 0 & 0 & \mu\\ \end{bmatrix}
-    """
-    sym = (dim + 1) * dim // 2
-    o = array([1.] * dim + [0.] * (sym - dim), dtype=float64)
-    oot = outer(o, o)
-    do1 = diag(o + 1.0)
-
-    lam_array = array(lam)[..., None, None]
-    mu_array = array(mu)[..., None, None]
-    return lam_array * oot + mu_array * do1
-
-
-def get_stiffness_from_young_poisson(dim: int, young: float, poisson: float, plane: Optional[str]) -> ndarray:
-    """
-    Compute stiffness tensor corresponding to Young's modulus and Poisson's
-    ratio.
-    """
-
-    lam, mu = get_lame_from_young_poisson(young, poisson, plane)
-
-    return get_stiffness_from_lame(dim, lam, mu)
-
-
-def get_stiffness_from_lame_mixed(dim: int, lam: float, mu: float) -> ndarray:
-    r"""
-    Compute stiffness tensor corresponding to Lamé parameters for mixed
-    formulation.
-
-    .. math::
-        {\bf D}_{(2D)} = \begin{bmatrix} \widetilde\lambda + 2\mu &
-        \widetilde\lambda & 0\\ \widetilde\lambda & \widetilde\lambda + 2\mu &
-        0\\ 0 & 0 & \mu \end{bmatrix}
-
-    .. math::
-        {\bf D}_{(3D)} = \begin{bmatrix} \widetilde\lambda + 2\mu &
-        \widetilde\lambda & \widetilde\lambda & 0 & 0 & 0\\ \widetilde\lambda &
-        \widetilde\lambda + 2\mu & \widetilde\lambda & 0 & 0 & 0 \\
-        \widetilde\lambda & \widetilde\lambda & \widetilde\lambda + 2\mu & 0 &
-        0 & 0 \\ 0 & 0 & 0 & \mu & 0 & 0 \\ 0 & 0 & 0 & 0 & \mu & 0 \\ 0 & 0 &
-        0 & 0 & 0 & \mu\\ \end{bmatrix}
-
-    where
-
-    .. math::
-       \widetilde\lambda = -{2\over 3} \mu
-    """
-    lam = - 2.0 / 3.0 * mu
-
-    return get_stiffness_from_lame(dim, lam, mu)
-
-
-def get_stiffness_from_young_poisson_mixed(dim: int, young: float, poisson: float, plane) -> ndarray:
-    """
-    Compute stiffness tensor corresponding to Young's modulus and Poisson's
-    ratio for mixed formulation.
-    """
-    lam, mu = get_lame_from_young_poisson(young, poisson, plane)
-
-    return get_stiffness_from_lame_mixed(dim, lam, mu)
-
-
-def get_bulk_from_lame(lam: float, mu: float) -> float:
-    r"""
-    Compute bulk modulus from Lamé parameters.
-
-    .. math::
-        \gamma = \lambda + {2 \over 3} \mu
-    """
-    return lam + 2.0 * mu / 3.0
-
-
-def get_bulk_from_young_poisson(young: float, poisson: float, plane: Optional[str]) -> float:
-    """
-    Compute bulk modulus corresponding to Young's modulus and Poisson's ratio.
-    """
-    lam, mu = get_lame_from_young_poisson(young, poisson, plane)
-
-    return get_bulk_from_lame(lam, mu)
-
-
-def get_lame_from_stiffness(stiffness: ndarray, plane: Optional[str]) -> Tuple[float, float]:
-    """
-    Compute Lamé parameters from an isotropic stiffness tensor.
-    """
-    lam = float(stiffness[..., 0, 1])
-    mu = float(stiffness[..., -1, -1])
-    if plane == 'PlaneStress':
-        lam = - 2.0 * mu * lam / (lam - 2.0 * mu)
-
-    return lam, mu
-
-
-def get_young_poisson_from_stiffness(stiffness: ndarray, plane: Optional[str]) -> Tuple[float, float]:
-    """
-    Compute Young's modulus and Poisson's ratio from an isotropic stiffness
-    tensor.
-    """
-    lam, mu = get_lame_from_stiffness(stiffness, plane)
-    young = (3 * lam * mu + 2 * mu ** 2) / (lam + mu)
-    poisson = lam / (2 * lam + 2 * mu)
-
-    return young, poisson
-
-
-if __name__ == "__main__":
-    from pyfem.io.Properties import Properties
-
-    props = Properties()
-    props.read_file(r'F:\Github\pyfem\examples\rectangle\rectangle.toml')
-
-    material_data = ElasticIsotropic(props.materials[0], 3)
-    print(material_data.to_string())
+from typing import Optional, Tuple
+
+from numpy import array, outer, diag, float64, ndarray
+
+from pyfem.io.Material import Material
+from pyfem.materials.BaseMaterial import BaseMaterial
+from pyfem.utils.colors import error_style
+
+
+class ElasticIsotropic(BaseMaterial):
+    allowed_option = ['PlaneStress', 'PlaneStrain', None]
+
+    def __init__(self, material: Material, dimension: int, option: Optional[str] = None) -> None:
+        super().__init__(material, dimension, option)
+        self.create_tangent()
+
+    def create_tangent(self):
+        young = self.material.data[0]
+        poisson = self.material.data[1]
+
+        if self.option in self.allowed_option:
+            if self.dimension == 3:
+                self.option = None
+            self.ddsdde = get_stiffness_from_young_poisson(self.dimension, young, poisson, self.option)
+        else:
+            error_msg = f'{self.option} is not the allowed options {self.allowed_option}'
+            raise NotImplementedError(error_style(error_msg))
+
+
+def get_lame_from_young_poisson(young: float, poisson: float, plane: Optional[str]) -> Tuple[float, float]:
+    r"""
+    Compute Lamé parameters from Young's modulus and Poisson's ratio.
+
+    The relationship between Lamé parameters and Young's modulus, Poisson's
+    ratio (see [1],[2]):
+
+    .. math::
+        \lambda = {\nu E \over (1+\nu)(1-2\nu)},\qquad \mu = {E \over 2(1+\nu)}
+
+    The plain stress hypothesis:
+
+    .. math::
+       \bar\lambda = {2\lambda\mu \over \lambda + 2\mu}
+
+    [1] I.S. Sokolnikoff: Mathematical Theory of Elasticity. New York, 1956.
+
+    [2] T.J.R. Hughes: The Finite Element Method, Linear Static and Dynamic
+    Finite Element Analysis. New Jersey, 1987.
+    """
+    mu = young / (2.0 * (1.0 + poisson))
+    lam = young * poisson / ((1.0 + poisson) * (1.0 - 2.0 * poisson))
+
+    if plane == 'PlaneStress':
+        lam = 2 * lam * mu / (lam + 2 * mu)
+
+    return lam, mu
+
+
+def get_stiffness_from_lame(dim: int, lam: float, mu: float) -> ndarray:
+    r"""
+    Compute stiffness tensor corresponding to Lamé parameters.
+
+    .. math::
+        {\bf D}_{(2D)} = \begin{bmatrix} \lambda + 2\mu & \lambda & 0\\
+        \lambda & \lambda + 2\mu & 0\\ 0 & 0 & \mu \end{bmatrix}
+
+    .. math::
+        {\bf D}_{(3D)} = \begin{bmatrix} \lambda + 2\mu & \lambda &
+        \lambda & 0 & 0 & 0\\ \lambda & \lambda + 2\mu & \lambda & 0 & 0 & 0 \\
+        \lambda & \lambda & \lambda + 2\mu & 0 & 0 & 0 \\ 0 & 0 & 0 & \mu & 0 &
+        0 \\ 0 & 0 & 0 & 0 & \mu & 0 \\ 0 & 0 & 0 & 0 & 0 & \mu\\ \end{bmatrix}
+    """
+    sym = (dim + 1) * dim // 2
+    o = array([1.] * dim + [0.] * (sym - dim), dtype=float64)
+    oot = outer(o, o)
+    do1 = diag(o + 1.0)
+
+    lam_array = array(lam)[..., None, None]
+    mu_array = array(mu)[..., None, None]
+    return lam_array * oot + mu_array * do1
+
+
+def get_stiffness_from_young_poisson(dim: int, young: float, poisson: float, plane: Optional[str]) -> ndarray:
+    """
+    Compute stiffness tensor corresponding to Young's modulus and Poisson's
+    ratio.
+    """
+
+    lam, mu = get_lame_from_young_poisson(young, poisson, plane)
+
+    return get_stiffness_from_lame(dim, lam, mu)
+
+
+def get_stiffness_from_lame_mixed(dim: int, lam: float, mu: float) -> ndarray:
+    r"""
+    Compute stiffness tensor corresponding to Lamé parameters for mixed
+    formulation.
+
+    .. math::
+        {\bf D}_{(2D)} = \begin{bmatrix} \widetilde\lambda + 2\mu &
+        \widetilde\lambda & 0\\ \widetilde\lambda & \widetilde\lambda + 2\mu &
+        0\\ 0 & 0 & \mu \end{bmatrix}
+
+    .. math::
+        {\bf D}_{(3D)} = \begin{bmatrix} \widetilde\lambda + 2\mu &
+        \widetilde\lambda & \widetilde\lambda & 0 & 0 & 0\\ \widetilde\lambda &
+        \widetilde\lambda + 2\mu & \widetilde\lambda & 0 & 0 & 0 \\
+        \widetilde\lambda & \widetilde\lambda & \widetilde\lambda + 2\mu & 0 &
+        0 & 0 \\ 0 & 0 & 0 & \mu & 0 & 0 \\ 0 & 0 & 0 & 0 & \mu & 0 \\ 0 & 0 &
+        0 & 0 & 0 & \mu\\ \end{bmatrix}
+
+    where
+
+    .. math::
+       \widetilde\lambda = -{2\over 3} \mu
+    """
+    lam = - 2.0 / 3.0 * mu
+
+    return get_stiffness_from_lame(dim, lam, mu)
+
+
+def get_stiffness_from_young_poisson_mixed(dim: int, young: float, poisson: float, plane) -> ndarray:
+    """
+    Compute stiffness tensor corresponding to Young's modulus and Poisson's
+    ratio for mixed formulation.
+    """
+    lam, mu = get_lame_from_young_poisson(young, poisson, plane)
+
+    return get_stiffness_from_lame_mixed(dim, lam, mu)
+
+
+def get_bulk_from_lame(lam: float, mu: float) -> float:
+    r"""
+    Compute bulk modulus from Lamé parameters.
+
+    .. math::
+        \gamma = \lambda + {2 \over 3} \mu
+    """
+    return lam + 2.0 * mu / 3.0
+
+
+def get_bulk_from_young_poisson(young: float, poisson: float, plane: Optional[str]) -> float:
+    """
+    Compute bulk modulus corresponding to Young's modulus and Poisson's ratio.
+    """
+    lam, mu = get_lame_from_young_poisson(young, poisson, plane)
+
+    return get_bulk_from_lame(lam, mu)
+
+
+def get_lame_from_stiffness(stiffness: ndarray, plane: Optional[str]) -> Tuple[float, float]:
+    """
+    Compute Lamé parameters from an isotropic stiffness tensor.
+    """
+    lam = float(stiffness[..., 0, 1])
+    mu = float(stiffness[..., -1, -1])
+    if plane == 'PlaneStress':
+        lam = - 2.0 * mu * lam / (lam - 2.0 * mu)
+
+    return lam, mu
+
+
+def get_young_poisson_from_stiffness(stiffness: ndarray, plane: Optional[str]) -> Tuple[float, float]:
+    """
+    Compute Young's modulus and Poisson's ratio from an isotropic stiffness
+    tensor.
+    """
+    lam, mu = get_lame_from_stiffness(stiffness, plane)
+    young = (3 * lam * mu + 2 * mu ** 2) / (lam + mu)
+    poisson = lam / (2 * lam + 2 * mu)
+
+    return young, poisson
+
+
+if __name__ == "__main__":
+    from pyfem.io.Properties import Properties
+
+    props = Properties()
+    props.read_file(r'F:\Github\pyfem\examples\rectangle\rectangle.toml')
+
+    material_data = ElasticIsotropic(props.materials[0], 3)
+    print(material_data.to_string())
```

### Comparing `pyfem-0.0.7/src/pyfem/materials/get_material_data.py` & `pyfem-0.0.8/src/pyfem/materials/get_material_data.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.7/src/pyfem/mesh/ElementSet.py` & `pyfem-0.0.8/src/pyfem/mesh/ElementSet.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.7/src/pyfem/mesh/NodeSet.py` & `pyfem-0.0.8/src/pyfem/mesh/NodeSet.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,16 @@
 
         mesh = meshio.read(filename, file_format='gmsh')
 
         # 可以通过以下命令查看支持的单元类型
         # print(meshio.gmsh.meshio_to_gmsh_type)
         # print(meshio.gmsh.gmsh_to_meshio_type)
 
-        keywords_1d = ['line']
-        keywords_2d = ['triangle', 'quad']
+        # keywords_1d = ['line']
+        # keywords_2d = ['triangle', 'quad']
         keywords_3d = ['pyramid', 'hexahedron', 'wedge', 'tetra']
 
         self.dimension = 2
 
         # If any 3D mesh type is found, set the dimension to 3
         for cell_name, cell_dict in mesh.cell_sets_dict.items():
             for mesh_type in cell_dict.keys():
```

### Comparing `pyfem-0.0.7/src/pyfem/solvers/BaseSolver.py` & `pyfem-0.0.8/src/pyfem/solvers/BaseSolver.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.7/src/pyfem/solvers/LinearSolver.py` & `pyfem-0.0.8/src/pyfem/solvers/LinearSolver.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from numpy import empty
-from scipy.sparse.linalg import spsolve, gmres  # type: ignore
+from scipy.sparse.linalg import spsolve  # type: ignore
 
 from pyfem.assembly.Assembly import Assembly
 from pyfem.io.Solver import Solver
 from pyfem.solvers.BaseSolver import BaseSolver
 from pyfem.utils.wrappers import show_running_time
```

### Comparing `pyfem-0.0.7/src/pyfem/utils/IntKeyDict.py` & `pyfem-0.0.8/src/pyfem/utils/IntKeyDict.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.7/src/pyfem/utils/colors.py` & `pyfem-0.0.8/src/pyfem/utils/colors.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.7/src/pyfem/utils/logger.py` & `pyfem-0.0.8/src/pyfem/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.7/src/pyfem/utils/visualization.py` & `pyfem-0.0.8/src/pyfem/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.7/src/pyfem/utils/wrappers.py` & `pyfem-0.0.8/src/pyfem/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.7/src/pyfem.egg-info/PKG-INFO` & `pyfem-0.0.8/src/pyfem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfem
-Version: 0.0.7
+Version: 0.0.8
 Summary: A finite element package for learning
 Home-page: https://github.com/sunwhale/pyfem
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyfem-0.0.7/src/pyfem.egg-info/SOURCES.txt` & `pyfem-0.0.8/src/pyfem.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 setup.py
+src/pyfem/Job.py
 src/pyfem/__init__.py
 src/pyfem/__main__.py
 src/pyfem.egg-info/PKG-INFO
 src/pyfem.egg-info/SOURCES.txt
 src/pyfem.egg-info/dependency_links.txt
 src/pyfem.egg-info/entry_points.txt
 src/pyfem.egg-info/top_level.txt
```

