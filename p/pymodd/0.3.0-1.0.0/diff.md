# Comparing `tmp/pymodd-0.3.0.tar.gz` & `tmp/pymodd-1.0.0.tar.gz`

## Comparing `pymodd-0.3.0.tar` & `pymodd-1.0.0.tar`

### file list

```diff
@@ -1,39 +1,43 @@
--rw-r--r--   0        0        0      367 1970-01-01 00:00:00.000000 pymodd-0.3.0/Cargo.toml
--rw-r--r--   0      501       20     1513 2023-04-16 22:43:12.000000 pymodd-0.3.0/.github/workflows/CI.yml
--rw-r--r--   0      501       20     3103 2023-04-16 22:43:12.000000 pymodd-0.3.0/.gitignore
--rw-r--r--   0      501       20     1043 2023-04-16 22:43:12.000000 pymodd-0.3.0/LICENSE.txt
--rw-r--r--   0      501       20     2283 2023-04-16 22:43:12.000000 pymodd-0.3.0/README.rst
--rw-r--r--   0      501       20      910 2023-04-16 22:43:12.000000 pymodd-0.3.0/examples/froge/entity_scripts.py
--rw-r--r--   0      501       20     1880 2023-04-16 22:43:12.000000 pymodd-0.3.0/examples/froge/game_variables.py
--rw-r--r--   0      501       20      466 2023-04-16 22:43:12.000000 pymodd-0.3.0/examples/froge/mapping.py
--rw-r--r--   0      501       20     6219 2023-04-16 22:43:12.000000 pymodd-0.3.0/examples/froge/scripts.py
--rw-r--r--   0      501       20    78188 2023-04-16 22:43:12.000000 pymodd-0.3.0/examples/froge/utils/game.json
--rw-r--r--   0      501       20        0 2023-04-16 22:43:12.000000 pymodd-0.3.0/pymodd/__init__.py
--rw-r--r--   0      501       20     1040 2023-04-16 22:43:12.000000 pymodd-0.3.0/pymodd/_pymodd_helper.pyi
--rw-r--r--   0      501       20    43418 2023-04-16 22:43:12.000000 pymodd-0.3.0/pymodd/actions.py
--rw-r--r--   0      501       20     2772 2023-04-16 22:43:12.000000 pymodd-0.3.0/pymodd/console_scripts/pymodd_command.py
--rw-r--r--   0      501       20    52968 2023-04-16 22:43:12.000000 pymodd-0.3.0/pymodd/functions.py
--rw-r--r--   0      501       20       26 2023-04-16 22:43:12.000000 pymodd-0.3.0/pymodd/py.typed
--rw-r--r--   0      501       20     8692 2023-04-16 22:43:12.000000 pymodd-0.3.0/pymodd/script.py
--rw-r--r--   0      501       20      801 2023-04-17 01:03:34.000000 pymodd-0.3.0/pyproject.toml
--rw-r--r--   0      501       20       41 2023-04-16 22:43:12.000000 pymodd-0.3.0/requirements.txt
--rw-r--r--   0      501       20     7772 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/game_data/actions.rs
--rw-r--r--   0      501       20    20091 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/game_data/argument.rs
--rw-r--r--   0      501       20     9678 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/game_data/directory.rs
--rw-r--r--   0      501       20     2135 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/game_data/entity_types.rs
--rw-r--r--   0      501       20    10395 2023-04-17 01:01:26.000000 pymodd-0.3.0/src/game_data/variable_categories.rs
--rw-r--r--   0      501       20     1800 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/game_data.rs
--rw-r--r--   0      501       20     2187 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/lib.rs
--rw-r--r--   0      501       20     4820 2023-04-17 01:01:26.000000 pymodd-0.3.0/src/project_generator/entity_scripts_file.rs
--rw-r--r--   0      501       20      183 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/project_generator/game_json_file.rs
--rw-r--r--   0      501       20     3459 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/project_generator/game_variables_file.rs
--rw-r--r--   0      501       20     6002 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/project_generator/mapping_file.rs
--rw-r--r--   0      501       20    24371 2023-04-16 22:43:22.000000 pymodd-0.3.0/src/project_generator/scripts_file.rs
--rw-r--r--   0      501       20     9767 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/project_generator/utils/iterators/argument_values_iterator.rs
--rw-r--r--   0      501       20     1820 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/project_generator/utils/iterators/directory_iterator.rs
--rw-r--r--   0      501       20       62 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/project_generator/utils/iterators.rs
--rw-r--r--   0      501       20     9420 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/project_generator/utils/to_pymodd_maps.rs
--rw-r--r--   0      501       20     2267 2023-04-17 01:01:26.000000 pymodd-0.3.0/src/project_generator/utils.rs
--rw-r--r--   0      501       20     2400 2023-04-16 22:43:12.000000 pymodd-0.3.0/src/project_generator.rs
--rw-r--r--   0      501       20    12887 2023-04-16 22:43:12.000000 pymodd-0.3.0/Cargo.lock
--rw-r--r--   0        0        0     2869 1970-01-01 00:00:00.000000 pymodd-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      367 1970-01-01 00:00:00.000000 pymodd-1.0.0/Cargo.toml
+-rw-r--r--   0      501       20     1513 2023-04-16 22:43:12.000000 pymodd-1.0.0/.github/workflows/CI.yml
+-rw-r--r--   0      501       20     3103 2023-04-16 22:43:12.000000 pymodd-1.0.0/.gitignore
+-rw-r--r--   0      501       20     1043 2023-04-16 22:43:12.000000 pymodd-1.0.0/LICENSE.txt
+-rw-r--r--   0      501       20     2039 2023-05-21 23:49:14.000000 pymodd-1.0.0/README.rst
+-rw-r--r--   0      501       20     1059 2023-05-21 00:56:47.000000 pymodd-1.0.0/examples/froge/entity_scripts.py
+-rw-r--r--   0      501       20     2823 2023-05-21 02:01:59.000000 pymodd-1.0.0/examples/froge/game_variables.py
+-rw-r--r--   0      501       20      559 2023-05-20 03:48:26.000000 pymodd-1.0.0/examples/froge/mapping.py
+-rw-r--r--   0      501       20     5672 2023-05-21 00:56:47.000000 pymodd-1.0.0/examples/froge/scripts.py
+-rw-r--r--   0      501       20    78239 2023-05-20 03:48:26.000000 pymodd-1.0.0/examples/froge/utils/game.json
+-rw-r--r--   0      501       20        0 2023-04-16 22:43:12.000000 pymodd-1.0.0/pymodd/__init__.py
+-rw-r--r--   0      501       20     1050 2023-05-21 00:56:56.000000 pymodd-1.0.0/pymodd/_pymodd_helper.pyi
+-rw-r--r--   0      501       20    46037 2023-05-21 20:34:51.000000 pymodd-1.0.0/pymodd/actions.py
+-rw-r--r--   0      501       20     3837 2023-05-21 21:43:25.000000 pymodd-1.0.0/pymodd/console_scripts/pymodd_command.py
+-rw-r--r--   0      501       20     2563 2023-05-20 02:49:12.000000 pymodd-1.0.0/pymodd/entity_script.py
+-rw-r--r--   0      501       20    51870 2023-05-21 00:56:47.000000 pymodd-1.0.0/pymodd/functions.py
+-rw-r--r--   0      501       20     6188 2023-05-21 00:56:47.000000 pymodd-1.0.0/pymodd/game.py
+-rw-r--r--   0      501       20       26 2023-04-16 22:43:12.000000 pymodd-1.0.0/pymodd/py.typed
+-rw-r--r--   0      501       20    15438 2023-05-21 20:34:51.000000 pymodd-1.0.0/pymodd/script.py
+-rw-r--r--   0      501       20   122364 2023-05-21 00:56:56.000000 pymodd-1.0.0/pymodd/utils/Default Game.json
+-rw-r--r--   0      501       20    38332 2023-05-21 00:56:47.000000 pymodd-1.0.0/pymodd/variable_types.py
+-rw-r--r--   0      501       20      801 2023-05-21 23:49:58.000000 pymodd-1.0.0/pyproject.toml
+-rw-r--r--   0      501       20       41 2023-04-16 22:43:12.000000 pymodd-1.0.0/requirements.txt
+-rw-r--r--   0      501       20     7772 2023-05-09 00:34:09.000000 pymodd-1.0.0/src/game_data/actions.rs
+-rw-r--r--   0      501       20    20109 2023-05-21 00:56:47.000000 pymodd-1.0.0/src/game_data/argument.rs
+-rw-r--r--   0      501       20     9875 2023-05-21 00:56:47.000000 pymodd-1.0.0/src/game_data/directory.rs
+-rw-r--r--   0      501       20     5295 2023-05-21 00:56:47.000000 pymodd-1.0.0/src/game_data/entity_types.rs
+-rw-r--r--   0      501       20    10379 2023-05-21 00:56:47.000000 pymodd-1.0.0/src/game_data/variable_categories.rs
+-rw-r--r--   0      501       20     1799 2023-05-21 00:56:47.000000 pymodd-1.0.0/src/game_data.rs
+-rw-r--r--   0      501       20     1992 2023-05-21 00:56:56.000000 pymodd-1.0.0/src/lib.rs
+-rw-r--r--   0      501       20    12703 2023-05-21 00:56:47.000000 pymodd-1.0.0/src/project_generator/entity_scripts_file.rs
+-rw-r--r--   0      501       20      183 2023-04-16 22:43:12.000000 pymodd-1.0.0/src/project_generator/game_json_file.rs
+-rw-r--r--   0      501       20    12760 2023-05-21 00:56:47.000000 pymodd-1.0.0/src/project_generator/game_variables_file.rs
+-rw-r--r--   0      501       20     4350 2023-05-19 00:56:39.000000 pymodd-1.0.0/src/project_generator/mapping_file.rs
+-rw-r--r--   0      501       20    44725 2023-05-21 00:56:47.000000 pymodd-1.0.0/src/project_generator/scripts_file.rs
+-rw-r--r--   0      501       20     9842 2023-05-21 00:56:47.000000 pymodd-1.0.0/src/project_generator/utils/iterators/argument_values_iterator.rs
+-rw-r--r--   0      501       20     1820 2023-04-16 22:43:12.000000 pymodd-1.0.0/src/project_generator/utils/iterators/directory_iterator.rs
+-rw-r--r--   0      501       20       62 2023-04-16 22:43:12.000000 pymodd-1.0.0/src/project_generator/utils/iterators.rs
+-rw-r--r--   0      501       20    10069 2023-05-15 23:54:58.000000 pymodd-1.0.0/src/project_generator/utils/to_pymodd_maps.rs
+-rw-r--r--   0      501       20     2518 2023-05-21 00:56:47.000000 pymodd-1.0.0/src/project_generator/utils.rs
+-rw-r--r--   0      501       20     2442 2023-05-21 00:56:47.000000 pymodd-1.0.0/src/project_generator.rs
+-rw-r--r--   0      501       20    12887 2023-04-16 22:43:12.000000 pymodd-1.0.0/Cargo.lock
+-rw-r--r--   0        0        0     2625 1970-01-01 00:00:00.000000 pymodd-1.0.0/PKG-INFO
```

### Comparing `pymodd-0.3.0/.github/workflows/CI.yml` & `pymodd-1.0.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pymodd-0.3.0/.gitignore` & `pymodd-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pymodd-0.3.0/LICENSE.txt` & `pymodd-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pymodd-0.3.0/README.rst` & `pymodd-1.0.0/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,74 +1,54 @@
 ======
 pymodd
 ======
 
 |Build| |Version| |License|
 
-pymodd is a python package used for creating modd.io games in python
+pymodd is a python package for creating and editing modd.io games in python
 
 .. |Build| image:: https://img.shields.io/github/actions/workflow/status/jeff5343/pymodd/CI.yml?label=CI&logo=github&style=plastic
    :alt: GitHub Workflow Status
 .. |Version| image:: https://img.shields.io/pypi/v/pymodd?style=plastic
    :alt: PyPI
 .. |License| image:: https://img.shields.io/pypi/l/pymodd?style=plastic
    :alt: PyPI - License
 
 Features
 --------
 
 - edit global and entity scripts
 - organize folders and scripts with a mapping file
+- edit environment variables
 - a command to generate and compile a pymodd project
 
-Installing
-----------
+Documentation
+-------------
 
-**Python 3.8 or higher is required**
+The pymodd wiki is located at `github.com/jeff5343/pymodd/wiki <https://github.com/jeff5343/pymodd/wiki>`_
 
-To install the library run the following command:
+A brief outline of the wiki:
 
-.. code:: sh
-
-    # Linux/macOS
-    python3 -m pip install -U pymodd
-
-    # Windows
-    py -3 -m pip install -U pymodd
-
-
-Getting Started
----------------
-
-Export your modd game json file from the website and then generate a pymodd project by running the following command:
-
-.. code:: sh
-
-    pymodd generate-project [GAME_JSON_FILE_PATH]
+- `Introduction <https://github.com/jeff5343/pymodd/wiki>`_
+- `Install Guide <https://github.com/jeff5343/pymodd/wiki/Install-Guide>`_
+- `Generating and Compiling a Pymodd Project <https://github.com/jeff5343/pymodd/wiki/Generating-and-Compiling-a-Pymodd-Project>`_
+- `Pymodd Project Structure <https://github.com/jeff5343/pymodd/wiki/Pymodd-Project-Structure>`_
 
 
 Quick Script Example
 --------------------
 
-view the ``examples/froge directory`` for a generated pymodd project
+view the ``examples/froge`` directory for an example of a pymodd project
 
 .. code:: py
 
     @script(triggers=[Trigger.EVERY_SECOND])
-    class EverySecond():
-        def _build(self):
-            self.actions = [
-                if_else((NumberOfUnitsOfUnitType(UnitTypes.FROG) < 5), [
-                    create_unit_for_player_at_position_with_rotation(UnitTypes.FROG, Variables.AI, RandomPositionInRegion(EntireMapRegion()), 0),
-                ], [
-                    if_else((NumberOfUnitsOfUnitType(UnitTypes.FROG_BOSS) == 0), [
-                        if_else((Variables.BOSS_TIMER <= 0), [
-                            create_unit_for_player_at_position_with_rotation(UnitTypes.FROG_BOSS, Variables.AI, RandomPositionInRegion(EntireMapRegion()), 0),
-                            update_ui_target_for_player_for_miliseconds(UiTarget.CENTER, 'BOSS SPAWNED', Undefined(), 5000),
-                            set_variable(Variables.BOSS_TIMER, 200),
-                        ], [
-                        ]),
-                        decrease_variable_by_number(Variables.BOSS_TIMER, 1),
-                    ], [
-                    ]),
-                ]),
-            ]
+    def every_second():
+        if NumberOfUnitsOfUnitType(UnitType.FROG) < 5:
+            create_unit_for_player_at_position_with_rotation(UnitType.FROG, Variable.AI, RandomPositionInRegion(EntireMapRegion()), 0)
+        else:
+            if NumberOfUnitsOfUnitType(UnitType.FROG_BOSS) == 0:
+                if Variable.BOSS_TIMER <= 0:
+                    create_unit_for_player_at_position_with_rotation(UnitType.FROG_BOSS, Variable.AI, RandomPositionInRegion(EntireMapRegion()), 0)
+                    update_ui_target_for_player_for_miliseconds(UiTarget.CENTER, 'BOSS SPAWNED', Undefined(), 5000)
+                decrease_variable_by_number(Variable.BOSS_TIMER, 1)
+
```

### Comparing `pymodd-0.3.0/examples/froge/scripts.py` & `pymodd-1.0.0/examples/froge/scripts.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,147 +2,79 @@
 from pymodd.functions import *
 from pymodd.script import Trigger, UiTarget, Flip, script
 
 from game_variables import *
 
 
 @script(triggers=[Trigger.GAME_START])
-class Initialize():
-	def _build(self):
-		self.actions = [
-			assign_player_to_player_type(Variables.AI, PlayerTypes.AI),
-			
-		]
+def initialize():
+    assign_player_to_player_type(Variable.AI, PlayerType.AI)
 
 
 @script(triggers=[Trigger.PLAYER_JOINS_GAME])
-class PlayerJoins():
-	def _build(self):
-		self.actions = [
-			create_unit_for_player_at_position_with_rotation(UnitTypes.POOPER, LastTriggeringPlayer(), RandomPositionInRegion(EntireMapRegion()), 0),
-			make_camera_of_player_track_unit(LastTriggeringPlayer(), LastCreatedUnit()),
-			assign_player_to_player_type(LastTriggeringPlayer(), PlayerTypes.PLAYER),
-			
-		]
+def player_joins():
+    create_unit_for_player_at_position_with_rotation(UnitType.POOPER, LastTriggeringPlayer(), RandomPositionInRegion(EntireMapRegion()), 0)
+    make_camera_of_player_track_unit(LastTriggeringPlayer(), LastCreatedUnit())
+    assign_player_to_player_type(LastTriggeringPlayer(), PlayerType.PLAYER)
 
 
 @script(triggers=[Trigger.PLAYER_LEAVES_GAME])
-class PlayerLeaves():
-	def _build(self):
-		self.actions = [
-			for_all_units_in(AllUnitsOwnedByPlayer(LastTriggeringPlayer()), [
-				destroy_entity(SelectedUnit()),
-				
-			], comment='when a player leaves, destroy all units owned by that player'),
-			
-		]
+def player_leaves():
+    for unit in AllUnitsOwnedByPlayer(LastTriggeringPlayer()):
+        destroy_entity(unit)
 
 
 @script(triggers=[Trigger.EVERY_SECOND])
-class EverySecond():
-	def _build(self):
-		self.actions = [
-			if_else((NumberOfUnitsOfUnitType(UnitTypes.FROG) < 5), [
-				create_unit_for_player_at_position_with_rotation(UnitTypes.FROG, Variables.AI, RandomPositionInRegion(EntireMapRegion()), 0),
-				
-			], [
-				if_else((NumberOfUnitsOfUnitType(UnitTypes.FROG_BOSS) == 0), [
-					if_else((Variables.BOSS_TIMER <= 0), [
-						create_unit_for_player_at_position_with_rotation(UnitTypes.FROG_BOSS, Variables.AI, RandomPositionInRegion(EntireMapRegion()), 0),
-						update_ui_target_for_player_for_miliseconds(UiTarget.CENTER, 'BOSS SPAWNED', Undefined(), 5000),
-						set_variable(Variables.BOSS_TIMER, 200),
-						
-					], [
-						
-					]),
-					decrease_variable_by_number(Variables.BOSS_TIMER, 1),
-					
-				], [
-					
-				]),
-				
-			]),
-			
-		]
+def every_second():
+    if NumberOfUnitsOfUnitType(UnitType.FROG) < 5:
+        create_unit_for_player_at_position_with_rotation(UnitType.FROG, Variable.AI, RandomPositionInRegion(EntireMapRegion()), 0)
+    else:
+        if NumberOfUnitsOfUnitType(UnitType.FROG_BOSS) == 0:
+            if Variable.BOSS_TIMER <= 0:
+                create_unit_for_player_at_position_with_rotation(UnitType.FROG_BOSS, Variable.AI, RandomPositionInRegion(EntireMapRegion()), 0)
+                update_ui_target_for_player_for_miliseconds(UiTarget.CENTER, 'BOSS SPAWNED', Undefined(), 5000)
+            decrease_variable_by_number(Variable.BOSS_TIMER, 1)
 
 
 @script(triggers=[Trigger.UNIT_ATTRIBUTE_BECOMES_ZERO])
-class WhenAUnitsAttributeBecomes0OrLess():
-	def _build(self):
-		self.actions = [
-			if_else((AttributeTypeOfAttribute(LastTriggeringAttribute()) == AttributeTypes.HEALTH), [
-				if_else((PlayerTypeOfPlayer(OwnerOfEntity(LastTriggeringUnit())) == PlayerTypes.PLAYER), [
-					set_entity_attribute(AttributeTypes.HEALTH, LastTriggeringUnit(), AttributeMaxOfEntity(AttributeTypes.HEALTH, LastTriggeringUnit())),
-					set_entity_variable(EntityVariables.TARGET_UNIT, LastTriggeringUnit(), Undefined()),
-					move_entity_to_position(LastTriggeringUnit(), CenterOfRegion(EntireMapRegion())),
-					
-				], [
-					if_else((UnitTypeOfUnit(LastTriggeringUnit()) == UnitTypes.FROG_BOSS), [
-						set_player_attribute(AttributeTypes.FROG_KILLS, OwnerOfEntity(LastAttackingUnit()), PlayerAttribute(AttributeTypes.FROG_KILLS, OwnerOfEntity(LastAttackingUnit())) + 7),
-						
-					], [
-						set_player_attribute(AttributeTypes.FROG_KILLS, OwnerOfEntity(LastAttackingUnit()), PlayerAttribute(AttributeTypes.FROG_KILLS, OwnerOfEntity(LastAttackingUnit())) + 1),
-						
-					]),
-					destroy_entity(LastTriggeringUnit()),
-					
-				]),
-				
-			], [
-				if_else((AttributeTypeOfAttribute(LastTriggeringAttribute()) == AttributeTypes.MOVE), [
-					set_entity_variable(EntityVariables.TARGET_UNIT, LastTriggeringUnit(), Undefined()),
-					for_all_entities_in(AllEntitiesInRegion(DynamicRegion(XCoordinateOfPosition(PositionOfEntity(LastTriggeringUnit())) - (ValueOfEntityVariable(EntityVariables.SENSOR_RADIUS, LastTriggeringUnit()) / 2), YCoordinateOfPosition(PositionOfEntity(LastTriggeringUnit())) - (ValueOfEntityVariable(EntityVariables.SENSOR_RADIUS, LastTriggeringUnit()) / 2), ValueOfEntityVariable(EntityVariables.SENSOR_RADIUS, LastTriggeringUnit()), ValueOfEntityVariable(EntityVariables.SENSOR_RADIUS, LastTriggeringUnit()))), [
-						if_else((PlayerTypeOfPlayer(OwnerOfEntity(SelectedEntity())) == PlayerTypes.PLAYER), [
-							if_else(((ValueOfEntityVariable(EntityVariables.TARGET_UNIT, LastTriggeringUnit()) == Undefined()) | (DistanceBetweenPositions(PositionOfEntity(SelectedEntity()), PositionOfEntity(LastTriggeringUnit())) > DistanceBetweenPositions(PositionOfEntity(ValueOfEntityVariable(EntityVariables.TARGET_UNIT, LastTriggeringUnit())), PositionOfEntity(LastTriggeringUnit())))), [
-								create_floating_text_at_position_with_color('Froge sense', PositionOfEntity(LastTriggeringUnit()), '#327117', disabled=True),
-								set_entity_variable(EntityVariables.TARGET_UNIT, LastTriggeringUnit(), SelectedEntity()),
-								
-							], [
-								
-							]),
-							
-						], [
-							
-						]),
-						
-					]),
-					if_else((ValueOfEntityVariable(EntityVariables.TARGET_UNIT, LastTriggeringUnit()) != Undefined()), [
-						rotate_entity_instantly_to_face_position(LastTriggeringUnit(), PositionOfEntity(ValueOfEntityVariable(EntityVariables.TARGET_UNIT, LastTriggeringUnit()))),
-						if_else((UnitTypeOfUnit(LastTriggeringUnit()) == UnitTypes.FROG_BOSS), [
-							apply_force_on_entity_at_angle(RandomNumberBetween(3000, 6000), LastTriggeringUnit(), UnitsFacingAngle(LastTriggeringUnit())),
-							
-						], [
-							apply_force_on_entity_at_angle(RandomNumberBetween(300, 600), LastTriggeringUnit(), UnitsFacingAngle(LastTriggeringUnit())),
-							
-						]),
-						use_item_continuously_until_stopped(ItemCurrentlyHeldByUnit(LastTriggeringUnit())),
-						
-					], [
-						rotate_entity_instantly_to_face_position(LastTriggeringUnit(), RandomPositionInRegion(EntityBounds(LastTriggeringUnit()))),
-						if_else((UnitTypeOfUnit(LastTriggeringUnit()) == UnitTypes.FROG_BOSS), [
-							apply_force_on_entity_at_angle(RandomNumberBetween(1500, 3500), LastTriggeringUnit(), UnitsFacingAngle(LastTriggeringUnit())),
-							
-						], [
-							apply_force_on_entity_at_angle(RandomNumberBetween(150, 400), LastTriggeringUnit(), UnitsFacingAngle(LastTriggeringUnit())),
-							
-						]),
-						stop_using_item(ItemCurrentlyHeldByUnit(LastTriggeringUnit())),
-						
-					]),
-					set_entity_attribute(AttributeTypes.MOVE, LastTriggeringUnit(), RandomNumberBetween(35, 100)),
-					
-				], [
-					
-				]),
-				
-			]),
-			
-		]
+def when_a_units_attribute_becomes_0_or_less():
+    if AttributeTypeOfAttribute(LastTriggeringAttribute()) == AttributeType.HEALTH:
+        if PlayerTypeOfPlayer(OwnerOfEntity(LastTriggeringUnit())) == PlayerType.PLAYER:
+            set_entity_attribute(AttributeType.HEALTH, LastTriggeringUnit(), AttributeMaxOfEntity(AttributeType.HEALTH, LastTriggeringUnit()))
+            set_entity_variable(EntityVariable.TARGET_UNIT, LastTriggeringUnit(), Undefined())
+            move_entity_to_position(LastTriggeringUnit(), CenterOfRegion(EntireMapRegion()))
+        else:
+            if UnitTypeOfUnit(LastTriggeringUnit()) == UnitType.FROG_BOSS:
+                set_variable(Variable.BOSS_TIMER, 200)
+                set_player_attribute(AttributeType.FROG_KILLS, OwnerOfEntity(LastAttackingUnit()), ValueOfPlayerAttribute(AttributeType.FROG_KILLS, OwnerOfEntity(LastAttackingUnit())) + 7)
+            else:
+                set_player_attribute(AttributeType.FROG_KILLS, OwnerOfEntity(LastAttackingUnit()), ValueOfPlayerAttribute(AttributeType.FROG_KILLS, OwnerOfEntity(LastAttackingUnit())) + 1)
+            destroy_entity(LastTriggeringUnit())
+    else:
+        if AttributeTypeOfAttribute(LastTriggeringAttribute()) == AttributeType.MOVE:
+            set_entity_variable(EntityVariable.TARGET_UNIT, LastTriggeringUnit(), Undefined())
+            for entity in AllEntitiesInRegion(DynamicRegion(XCoordinateOfPosition(PositionOfEntity(LastTriggeringUnit())) - (ValueOfEntityVariable(EntityVariable.SENSOR_RADIUS, LastTriggeringUnit()) / 2), YCoordinateOfPosition(PositionOfEntity(LastTriggeringUnit())) - (ValueOfEntityVariable(EntityVariable.SENSOR_RADIUS, LastTriggeringUnit()) / 2), ValueOfEntityVariable(EntityVariable.SENSOR_RADIUS, LastTriggeringUnit()), ValueOfEntityVariable(EntityVariable.SENSOR_RADIUS, LastTriggeringUnit()))):
+                if PlayerTypeOfPlayer(OwnerOfEntity(entity)) == PlayerType.PLAYER:
+                    if ValueOfEntityVariable(EntityVariable.TARGET_UNIT, LastTriggeringUnit()) == Undefined() or DistanceBetweenPositions(PositionOfEntity(entity), PositionOfEntity(LastTriggeringUnit())) > DistanceBetweenPositions(PositionOfEntity(ValueOfEntityVariable(EntityVariable.TARGET_UNIT, LastTriggeringUnit())), PositionOfEntity(LastTriggeringUnit())):
+                        create_floating_text_at_position_with_color('Froge sense', PositionOfEntity(LastTriggeringUnit()), '#327117', disabled=True)
+                        set_entity_variable(EntityVariable.TARGET_UNIT, LastTriggeringUnit(), entity)
+            if ValueOfEntityVariable(EntityVariable.TARGET_UNIT, LastTriggeringUnit()) != Undefined():
+                rotate_entity_instantly_to_face_position(LastTriggeringUnit(), PositionOfEntity(ValueOfEntityVariable(EntityVariable.TARGET_UNIT, LastTriggeringUnit())))
+                if UnitTypeOfUnit(LastTriggeringUnit()) == UnitType.FROG_BOSS:
+                    apply_force_on_entity_at_angle(RandomNumberBetween(3000, 6000), LastTriggeringUnit(), UnitsFacingAngle(LastTriggeringUnit()))
+                else:
+                    apply_force_on_entity_at_angle(RandomNumberBetween(300, 600), LastTriggeringUnit(), UnitsFacingAngle(LastTriggeringUnit()))
+                use_item_continuously_until_stopped(ItemCurrentlyHeldByUnit(LastTriggeringUnit()))
+            else:
+                rotate_entity_instantly_to_face_position(LastTriggeringUnit(), RandomPositionInRegion(EntityBounds(LastTriggeringUnit())))
+                if UnitTypeOfUnit(LastTriggeringUnit()) == UnitType.FROG_BOSS:
+                    apply_force_on_entity_at_angle(RandomNumberBetween(1500, 3500), LastTriggeringUnit(), UnitsFacingAngle(LastTriggeringUnit()))
+                else:
+                    apply_force_on_entity_at_angle(RandomNumberBetween(150, 400), LastTriggeringUnit(), UnitsFacingAngle(LastTriggeringUnit()))
+                stop_using_item(ItemCurrentlyHeldByUnit(LastTriggeringUnit()))
+            set_entity_attribute(AttributeType.MOVE, LastTriggeringUnit(), RandomNumberBetween(35, 100))
 
 
 @script(triggers=[])
-class OpenShop():
-	def _build(self):
-		self.actions = [
-			open_shop_for_player(Shops.FROGE_SHOP, OwnerOfEntity(LastCastingUnit())),
-			
-		]
+def open_shop():
+    open_shop_for_player(Shop.FROGE_SHOP, OwnerOfEntity(LastCastingUnit()))
+
```

### Comparing `pymodd-0.3.0/examples/froge/utils/game.json` & `pymodd-1.0.0/examples/froge/utils/game.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8816980127488185%*

 * *Differences: {"'__v'": '851',*

 * * "'_id'": "'6311661c535ef4072260feb2'",*

 * * "'backupOn'": '1677200135429',*

 * * "'clientSidePredictionEnabled'": 'False',*

 * * "'cover'": "'https://cache.modd.io/asset/spriteImage/1662091460423_1588259290955_Small_Machete_Knife.png'",*

 * * "'createdAt'": "'2022-09-02T02:10:36.829Z'",*

 * * "'data'": "{'playerTypeVariables': {replace: OrderedDict([('targetUnit', "*

 * *           "OrderedDict([('dataType', 'unit')]))])}, 'playerTypes': {'humanPlayer': {'variables': "*

 * *           "{replace: OrderedDict([('targetUnit', […]*

```diff
@@ -1,27 +1,26 @@
 {
-    "__v": 229,
-    "_id": "63816c35103812aeda0c69b8",
+    "__v": 851,
+    "_id": "6311661c535ef4072260feb2",
     "access": "private",
     "allowDuplicateIPS": false,
     "allowGuestMode": false,
     "allowLateJoining": false,
     "allowVerifiedUserToChat": false,
     "androidLink": null,
     "autoSave": true,
-    "backupOn": 1678936212479,
+    "backupOn": 1677200135429,
     "banChat": [],
     "banIps": [],
     "banUsers": [],
     "canHostPrivateServers": false,
     "clientPhysicsEngine": "planck",
-    "clientSidePredictionEnabled": true,
-    "cover": "https://cache.modd.io/asset/spriteImage/1589327274851_cover_blank.png",
-    "coverUpdated": false,
-    "createdAt": "2022-11-26T01:30:29.896Z",
+    "clientSidePredictionEnabled": false,
+    "cover": "https://cache.modd.io/asset/spriteImage/1662091460423_1588259290955_Small_Machete_Knife.png",
+    "createdAt": "2022-09-02T02:10:36.829Z",
     "dailyCoinTransferLimit": 0,
     "data": {
         "abilities": {},
         "animationTypes": {
             "B1cWOYKvNL": {
                 "frames": [
                     2,
@@ -5737,15 +5736,19 @@
                     "minVector": {
                         "x": -1,
                         "y": -1
                     }
                 }
             }
         },
-        "playerTypeVariables": {},
+        "playerTypeVariables": {
+            "targetUnit": {
+                "dataType": "unit"
+            }
+        },
         "playerTypes": {
             "eA9ZwoweVz": {
                 "attributes": {},
                 "color": "white",
                 "name": "ai",
                 "relationships": {
                     "humanPlayer": "hostile"
@@ -5771,15 +5774,19 @@
                 },
                 "color": "#ffffff",
                 "name": "Player",
                 "relationships": {
                     "humanPlayer": "friendly"
                 },
                 "showNameLabel": true,
-                "variables": {}
+                "variables": {
+                    "targetUnit": {
+                        "dataType": "unit"
+                    }
+                }
             }
         },
         "projectileTypes": {},
         "scripts": {
             "5BUXtByxVf": {
                 "actions": [
                     {
@@ -5802,15 +5809,15 @@
                         "operator": "=="
                     },
                     true,
                     true
                 ],
                 "key": "5BUXtByxVf",
                 "name": "open shop",
-                "order": 5,
+                "order": 6,
                 "parent": null,
                 "triggers": []
             },
             "CE0PBg1VWG": {
                 "actions": [
                     {
                         "conditions": [
@@ -5891,15 +5898,15 @@
                                         "value": {
                                             "function": "undefinedValue"
                                         },
                                         "variable": {
                                             "function": "getEntityVariable",
                                             "variable": {
                                                 "dataType": "unit",
-                                                "entity": "null",
+                                                "entity": "oTDQ3jlcMa",
                                                 "key": "targetUnit",
                                                 "text": "targetUnit"
                                             }
                                         },
                                         "vars": [
                                             {
                                                 "id": "getTriggeringUnit",
@@ -6002,15 +6009,15 @@
                                                                         "function": "getTriggeringUnit"
                                                                     },
                                                                     "function": "getValueOfEntityVariable",
                                                                     "variable": {
                                                                         "function": "getEntityVariable",
                                                                         "variable": {
                                                                             "dataType": "unit",
-                                                                            "entity": "null",
+                                                                            "entity": "oTDQ3jlcMa",
                                                                             "key": "targetUnit",
                                                                             "text": "targetUnit"
                                                                         }
                                                                     }
                                                                 },
                                                                 {
                                                                     "function": "undefinedValue"
@@ -6044,15 +6051,15 @@
                                                                                 "function": "getTriggeringUnit"
                                                                             },
                                                                             "function": "getValueOfEntityVariable",
                                                                             "variable": {
                                                                                 "function": "getEntityVariable",
                                                                                 "variable": {
                                                                                     "dataType": "unit",
-                                                                                    "entity": "null",
+                                                                                    "entity": "oTDQ3jlcMa",
                                                                                     "key": "targetUnit",
                                                                                     "text": "targetUnit"
                                                                                 }
                                                                             }
                                                                         },
                                                                         "function": "getEntityPosition"
                                                                     },
@@ -6141,15 +6148,15 @@
                                                                 "value": {
                                                                     "function": "getSelectedEntity"
                                                                 },
                                                                 "variable": {
                                                                     "function": "getEntityVariable",
                                                                     "variable": {
                                                                         "dataType": "unit",
-                                                                        "entity": "null",
+                                                                        "entity": "oTDQ3jlcMa",
                                                                         "key": "targetUnit",
                                                                         "text": "targetUnit"
                                                                     }
                                                                 },
                                                                 "vars": [
                                                                     {
                                                                         "id": "getTriggeringUnit",
@@ -6239,15 +6246,15 @@
                                                         ]
                                                     },
                                                     "function": "getValueOfEntityVariable",
                                                     "variable": {
                                                         "function": "getEntityVariable",
                                                         "variable": {
                                                             "dataType": "number",
-                                                            "entity": "null",
+                                                            "entity": "oTDQ3jlcMa",
                                                             "key": "sensorRadius",
                                                             "text": "sensorRadius"
                                                         },
                                                         "vars": [
                                                             {
                                                                 "id": "getTriggeringUnit",
                                                                 "source": "trigger"
@@ -6326,15 +6333,15 @@
                                                         ]
                                                     },
                                                     "function": "getValueOfEntityVariable",
                                                     "variable": {
                                                         "function": "getEntityVariable",
                                                         "variable": {
                                                             "dataType": "number",
-                                                            "entity": "null",
+                                                            "entity": "oTDQ3jlcMa",
                                                             "key": "sensorRadius",
                                                             "text": "sensorRadius"
                                                         },
                                                         "vars": [
                                                             {
                                                                 "id": "getTriggeringUnit",
                                                                 "source": "trigger"
@@ -6398,15 +6405,15 @@
                                                                         "function": "getTriggeringUnit"
                                                                     },
                                                                     "function": "getValueOfEntityVariable",
                                                                     "variable": {
                                                                         "function": "getEntityVariable",
                                                                         "variable": {
                                                                             "dataType": "number",
-                                                                            "entity": "null",
+                                                                            "entity": "oTDQ3jlcMa",
                                                                             "key": "sensorRadius",
                                                                             "text": "sensorRadius"
                                                                         }
                                                                     }
                                                                 },
                                                                 2
                                                             ]
@@ -6457,15 +6464,15 @@
                                                                         "function": "getTriggeringUnit"
                                                                     },
                                                                     "function": "getValueOfEntityVariable",
                                                                     "variable": {
                                                                         "function": "getEntityVariable",
                                                                         "variable": {
                                                                             "dataType": "number",
-                                                                            "entity": "null",
+                                                                            "entity": "oTDQ3jlcMa",
                                                                             "key": "sensorRadius",
                                                                             "text": "sensorRadius"
                                                                         }
                                                                     }
                                                                 },
                                                                 2
                                                             ]
@@ -6529,15 +6536,15 @@
                                                 "source": "forAllEntities"
                                             }
                                         ]
                                     },
                                     {
                                         "conditions": [
                                             {
-                                                "operandType": "unit",
+                                                "operandType": "unitType",
                                                 "operator": "!="
                                             },
                                             {
                                                 "entity": {
                                                     "function": "getTriggeringUnit",
                                                     "vars": [
                                                         {
@@ -6551,15 +6558,15 @@
                                                     ]
                                                 },
                                                 "function": "getValueOfEntityVariable",
                                                 "variable": {
                                                     "function": "getEntityVariable",
                                                     "variable": {
                                                         "dataType": "unit",
-                                                        "entity": "null",
+                                                        "entity": "oTDQ3jlcMa",
                                                         "key": "targetUnit",
                                                         "text": "targetUnit"
                                                     },
                                                     "vars": [
                                                         {
                                                             "id": "getTriggeringUnit",
                                                             "source": "trigger"
@@ -6917,15 +6924,15 @@
                                                             ]
                                                         },
                                                         "function": "getValueOfEntityVariable",
                                                         "variable": {
                                                             "function": "getEntityVariable",
                                                             "variable": {
                                                                 "dataType": "unit",
-                                                                "entity": "null",
+                                                                "entity": "oTDQ3jlcMa",
                                                                 "key": "targetUnit",
                                                                 "text": "targetUnit"
                                                             },
                                                             "vars": [
                                                                 {
                                                                     "id": "getTriggeringUnit",
                                                                     "source": "trigger"
@@ -7606,15 +7613,15 @@
                                         "value": {
                                             "function": "undefinedValue"
                                         },
                                         "variable": {
                                             "function": "getEntityVariable",
                                             "variable": {
                                                 "dataType": "unit",
-                                                "entity": "null",
+                                                "entity": "oTDQ3jlcMa",
                                                 "key": "targetUnit",
                                                 "text": "targetUnit"
                                             }
                                         },
                                         "vars": [
                                             {
                                                 "id": "getTriggeringUnit",
@@ -7710,15 +7717,15 @@
                         "operandType": "boolean",
                         "operator": "=="
                     },
                     true,
                     true
                 ],
                 "key": "CE0PBg1VWG",
-                "name": "when a units attribute becomes 0 or less",
+                "name": "when a unit's attribute becomes 0 or less",
                 "order": 4,
                 "parent": null,
                 "triggers": [
                     {
                         "type": "unitAttributeBecomesZero"
                     }
                 ]
@@ -7802,19 +7809,15 @@
                                         ],
                                         "type": "condition",
                                         "vars": []
                                     },
                                     {
                                         "number": 1,
                                         "type": "decreaseVariableByNumber",
-                                        "variable": {
-                                            "function": "getVariable",
-                                            "variableName": "bossTimer",
-                                            "vars": []
-                                        },
+                                        "variable": "bossTimer",
                                         "vars": []
                                     }
                                 ],
                                 "type": "condition",
                                 "vars": []
                             }
                         ],
@@ -7870,22 +7873,15 @@
                             "vars": []
                         },
                         "playerType": "eA9ZwoweVz",
                         "type": "assignPlayerType",
                         "vars": []
                     }
                 ],
-                "conditions": [
-                    {
-                        "operandType": "boolean",
-                        "operator": "=="
-                    },
-                    true,
-                    true
-                ],
+                "isProtected": true,
                 "key": "initialize",
                 "name": "initialize",
                 "order": -1,
                 "parent": null,
                 "triggers": [
                     {
                         "type": "gameStart"
@@ -7929,14 +7925,17 @@
                             {
                                 "id": "getTriggeringPlayer",
                                 "source": "trigger"
                             }
                         ]
                     },
                     {
+                        "fighter": {
+                            "function": "getTriggeringPlayer"
+                        },
                         "player": {
                             "function": "getTriggeringPlayer",
                             "vars": [
                                 {
                                     "id": "getTriggeringPlayer",
                                     "source": "trigger"
                                 }
@@ -7975,22 +7974,15 @@
                             {
                                 "id": "getTriggeringPlayer",
                                 "source": "trigger"
                             }
                         ]
                     }
                 ],
-                "conditions": [
-                    {
-                        "operandType": "boolean",
-                        "operator": "=="
-                    },
-                    true,
-                    true
-                ],
+                "conditions": [],
                 "key": "playerJoinsGame",
                 "name": "player joins",
                 "order": 1,
                 "parent": null,
                 "triggers": [
                     {
                         "type": "playerJoinsGame"
@@ -8035,14 +8027,17 @@
                                     }
                                 ]
                             }
                         ],
                         "comment": "when a player leaves, destroy all units owned by that player",
                         "type": "forAllUnits",
                         "unitGroup": {
+                            "fighter": {
+                                "function": "getTriggeringPlayer"
+                            },
                             "function": "allUnitsOwnedByPlayer",
                             "player": {
                                 "function": "getTriggeringPlayer",
                                 "vars": [
                                     {
                                         "id": "getTriggeringPlayer",
                                         "source": "trigger"
@@ -8958,15 +8953,15 @@
                                 "operator": "=="
                             },
                             true,
                             true
                         ],
                         "key": "umIqJLd7De",
                         "name": "use item",
-                        "order": 0,
+                        "order": -1,
                         "parent": null,
                         "triggers": []
                     }
                 },
                 "skin": "https://s3-us-west-1.amazonaws.com/modd/halloween-0.18/spritesheet/man.png",
                 "sound": {
                     "KK9JlU1UQy": {
@@ -9331,16 +9326,16 @@
                                 "operandType": "boolean",
                                 "operator": "=="
                             },
                             true,
                             true
                         ],
                         "key": "XUAEBhSryo",
-                        "name": "new script",
-                        "order": 0,
+                        "name": "New Script",
+                        "order": -1,
                         "parent": null,
                         "triggers": []
                     }
                 },
                 "skin": "https://s3-us-west-1.amazonaws.com/modd/halloween-0.18/spritesheet/man.png",
                 "sound": {
                     "KK9JlU1UQy": {
@@ -9440,56 +9435,56 @@
     "enablePersistedData": false,
     "enableVideoChat": false,
     "extrapolation": true,
     "facebookLink": null,
     "featuredOrderNo": -1,
     "frameRate": 15,
     "gamePlayInstructions": "",
-    "gameSlug": "p2H8kqy9c",
+    "gameSlug": "froge",
     "heightBasedZIndex": false,
-    "hidden": false,
+    "hidden": true,
     "highScores": [],
     "invitedUsers": [],
     "iosLink": null,
     "isDeleted": false,
     "isFeatured": false,
     "isGuestPlayerAllowed": true,
     "isLobbyEnabled": false,
-    "isMod": true,
+    "isMod": false,
     "isModdable": false,
-    "lastPlayedAt": "2023-03-08T23:50:55.198Z",
+    "lastPlayedAt": "2023-02-17T14:59:38.654Z",
     "lifeSpanHours": 5,
     "link": null,
     "lobbyUnitKey": "",
     "mapBackgroundColor": "#000000",
     "maxLobbySize": 4,
     "minLobbySize": 2,
     "mobileReady": false,
     "moreIoGames": false,
     "owner": "5dc7aca54006dc3c67a150c8",
-    "parentGameId": "634e14bfb4b75e6d3e7730ee",
+    "parentGameId": null,
     "patchNotes": null,
     "physicsEngine": "planck",
-    "playCount": 1,
-    "preferredRegion": "us",
+    "playCount": 4,
+    "preferredRegion": "",
     "privateServerIdleTimeout": 0.1,
     "reasonForTakingDown": "",
     "redirect": "off",
     "releases": [
         {
-            "_id": "63816c35103812aeda0c69b9",
+            "_id": "6311661c535ef4072260feb3",
             "isStable": false,
-            "release": "63816c35103812aeda0c69b6",
+            "release": "6311661c535ef4072260feb0",
             "version": 0.01
         }
     ],
     "revenueSharing": false,
     "sandboxMode": "advanced",
     "solanaWalletLoginEnabled": false,
     "tier": "1",
     "title": "Froge",
-    "totalPlayCount": 15,
+    "totalPlayCount": 110,
     "twitterLink": null,
-    "updatedAt": "2023-03-16T03:09:51.493Z",
+    "updatedAt": "2023-02-24T00:37:58.233Z",
     "version": 0.01,
     "youtubeLink": null
 }
```

### Comparing `pymodd-0.3.0/pymodd/actions.py` & `pymodd-1.0.0/pymodd/actions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 import functools
 
-from .functions import Condition, Number, String
-from .script import Script, to_dict
+from pymodd.functions import Condition, Number, String
+from pymodd.script import Script, to_dict
 
 
 def action(func):
     @functools.wraps(func)
     def wrapper_action(*args, **kwargs):
         action_dictionary = (func(*args))
         action_dictionary.update(
@@ -26,24 +26,14 @@
         dictionary['disabled'] = True
     if run_on_client:
         dictionary['runOnClient'] = True
     return dictionary
 
 
 @action
-def if_else(condition: Condition, then_actions=[], else_actions=[], comment=None, disabled=False, run_on_client=False):
-    return {
-        'type': 'condition',
-        'conditions': to_dict(condition),
-        'then': then_actions,
-        'else': else_actions,
-    }
-
-
-@action
 def set_player_variable(variable_type, player, value, comment=None, disabled=False, run_on_client=False):
     return {
         'type': 'setPlayerVariable',
         'player': to_dict(player),
         'variable': to_dict(variable_type),
         'value': to_dict(value)
     }
@@ -64,23 +54,14 @@
     return {
         'type': 'playAdForPlayer',
         'entity': to_dict(entity),
     }
 
 
 @action
-def set_time_out(duration: Number, actions=[], comment=None, disabled=False, run_on_client=False):
-    return {
-        'type': 'setTimeOut',
-        'duration': to_dict(duration),
-        'actions': actions,
-    }
-
-
-@action
 def rotate_entity_instantly_to_face_position(entity, position, comment=None, disabled=False, run_on_client=False):
     return {
         'type': 'rotateEntityToFacePosition',
         'entity': to_dict(entity),
         'position': to_dict(position),
     }
 
@@ -171,21 +152,14 @@
         'type': 'openDialogueForPlayer',
         'dialogue': to_dict(dialogue),
         'player': to_dict(player),
     }
 
 
 @action
-def continue_loop(comment=None, disabled=False, run_on_client=False):
-    return {
-        'type': 'continue',
-    }
-
-
-@action
 def open_website_for_player(string: String, player, comment=None, disabled=False, run_on_client=False):
     return {
         'type': 'openWebsiteForPlayer',
         'string': to_dict(string),
         'player': to_dict(player),
     }
 
@@ -303,23 +277,14 @@
         'type': 'moveDebris',
         'entity': to_dict(entity),
         'position': to_dict(position),
     }
 
 
 @action
-def for_all_items_in(item_group, actions=[], comment=None, disabled=False, run_on_client=False):
-    return {
-        'type': 'forAllItems',
-        'itemGroup': to_dict(item_group),
-        'actions': actions,
-    }
-
-
-@action
 def remove_player_from_player_group(player, player_group, comment=None, disabled=False, run_on_client=False):
     return {
         'type': 'removePlayerFromPlayerGroup',
         'player': to_dict(player),
         'playerGroup': to_dict(player_group),
     }
 
@@ -367,21 +332,14 @@
         'type': 'hideUnitInPlayerMinimap',
         'unit': to_dict(unit),
         'player': to_dict(player),
     }
 
 
 @action
-def return_loop(comment=None, disabled=False, run_on_client=False):
-    return {
-        'type': 'return',
-    }
-
-
-@action
 def run_script(script: Script, comment=None, disabled=False, run_on_client=False):
     return {
         'type': 'runScript',
         'scriptName': to_dict(script.key),
     }
 
 
@@ -440,15 +398,15 @@
     }
 
 
 @action
 def set_variable(variable, value, comment=None, disabled=False, run_on_client=False):
     return {
         'type': 'setVariable',
-        'variableName': variable.name,
+        'variableName': variable.id,
         'value': to_dict(value),
     }
 
 
 @action
 def increase_variable_by_number(variable, number: Number, comment=None, disabled=False, run_on_client=False):
     return {
@@ -482,23 +440,14 @@
         'type': 'playEntityAnimation',
         'entity': to_dict(entity),
         'animation': to_dict(animation),
     }
 
 
 @action
-def while_do(conditions, actions=[], comment=None, disabled=False, run_on_client=False):
-    return {
-        'type': 'while',
-        'conditions': to_dict(conditions),
-        'actions': actions,
-    }
-
-
-@action
 def apply_force_on_entity_xy(force_x: Number, force_y: Number, entity, comment=None, disabled=False, run_on_client=False):
     return {
         'type': 'applyForceOnEntityXY',
         'force': {
             'x': to_dict(force_x),
             'y': to_dict(force_y),
         },
@@ -575,23 +524,14 @@
         'type': 'attachDebrisToUnit',
         'entity': to_dict(debris),
         'unit': to_dict(unit),
     }
 
 
 @action
-def repeat(count: Number, actions=[], comment=None, disabled=False, run_on_client=False):
-    return {
-        'type': 'repeat',
-        'count': to_dict(count),
-        'actions': actions,
-    }
-
-
-@action
 def stop_music_for_everyone(comment=None, disabled=False, run_on_client=False):
     return {
         'type': 'stopMusic',
     }
 
 
 @action
@@ -600,14 +540,24 @@
         'type': 'emitParticleOnceAtPosition',
         'particleType': to_dict(particle_type),
         'position': to_dict(position),
     }
 
 
 @action
+def emit_particle_attached_to_entity(particle_type, angle, entity, comment=None, disabled=False, run_on_client=False):
+    return {
+        'type': 'emitParticleAttachedToEntity',
+        'particle_type': to_dict(particle_type),
+        'angle': to_dict(angle),
+        'entity': to_dict(entity),
+    }
+
+
+@action
 def set_velocity_of_entity(velocity_x: Number, velocity_y: Number, entity, comment=None, disabled=False, run_on_client=False):
     return {
         'type': 'setVelocityOfEntityXY',
         'velocity': {
             'x': to_dict(velocity_x),
             'y': to_dict(velocity_y),
         },
@@ -654,23 +604,14 @@
 def start_accepting_players(comment=None, disabled=False, run_on_client=False):
     return {
         'type': 'startAcceptingPlayers',
     }
 
 
 @action
-def for_all_entities_in(entity_group, actions=[], comment=None, disabled=False, run_on_client=False):
-    return {
-        'type': 'forAllEntities',
-        'entityGroup': to_dict(entity_group),
-        'actions': actions,
-    }
-
-
-@action
 def make_player_select_unit(player, unit, comment=None, disabled=False, run_on_client=False):
     return {
         'type': 'makePlayerSelectUnit',
         'player': to_dict(player),
         'unit': to_dict(unit),
     }
 
@@ -682,23 +623,14 @@
         'attribute': to_dict(attribute),
         'entity': to_dict(entity),
         'value': to_dict(value),
     }
 
 
 @action
-def for_all_item_types_in(item_type_group, actions=[], comment=None, disabled=False, run_on_client=False):
-    return {
-        'type': 'forAllItemTypes',
-        'itemTypeGroup': to_dict(item_type_group),
-        'actions': actions,
-    }
-
-
-@action
 def create_entity_for_player_at_position_with_dimensions(entity, player, position, height: Number, width: Number, angle: Number, comment=None, disabled=False, run_on_client=False):
     return {
         'type': 'createEntityForPlayerAtPositionWithDimensions',
         'entity': to_dict(entity),
         'player': to_dict(player),
         'position': to_dict(position),
         'height': to_dict(height),
@@ -720,32 +652,14 @@
         'type': 'updateUiTextForEveryone',
         'target': to_dict(target),
         'value': to_dict(value),
     }
 
 
 @action
-def for_all_units_in(unit_group, actions=[], comment=None, disabled=False, run_on_client=False):
-    return {
-        'type': 'forAllUnits',
-        'unitGroup': to_dict(unit_group),
-        'actions': actions,
-    }
-
-
-@action
-def for_all_projectiles_in(projectile_group, actions=[], comment=None, disabled=False, run_on_client=False):
-    return {
-        'type': 'forAllProjectiles',
-        'projectileGroup': to_dict(projectile_group),
-        'actions': actions,
-    }
-
-
-@action
 def stop_music_for_player(player, comment=None, disabled=False, run_on_client=False):
     return {
         'type': 'stopMusicForPlayer',
         'player': to_dict(player),
     }
 
 
@@ -793,23 +707,14 @@
         'type': 'changeScaleOfEntityBody',
         'entity': to_dict(entity),
         'scale': to_dict(scale),
     }
 
 
 @action
-def for_all_regions_in(region_group, actions=[], comment=None, disabled=False, run_on_client=False):
-    return {
-        'type': 'forAllRegions',
-        'regionGroup': to_dict(region_group),
-        'actions': actions,
-    }
-
-
-@action
 def rotate_entity_loss_tolerant_to_radians(entity, radians: Number, comment=None, disabled=False, run_on_client=False):
     return {
         'type': 'rotateEntityToRadiansLT',
         'entity': to_dict(entity),
         'radians': to_dict(radians),
     }
 
@@ -831,23 +736,14 @@
         'attributeType': to_dict(attribute_type),
         'player': to_dict(player),
         'number': to_dict(number),
     }
 
 
 @action
-def for_all_unit_types_in(unit_type_group, actions=[], comment=None, disabled=False, run_on_client=False):
-    return {
-        'type': 'forAllUnitTypes',
-        'unitTypeGroup': to_dict(unit_type_group),
-        'actions': actions,
-    }
-
-
-@action
 def decrease_variable_by_number(variable, number: Number, comment=None, disabled=False, run_on_client=False):
     return {
         'type': 'decreaseVariableByNumber',
         'variable': to_dict(variable),
         'number': to_dict(number),
     }
 
@@ -857,37 +753,32 @@
     return {
         'type': 'kickPlayer',
         'entity': to_dict(entity),
     }
 
 
 @action
-def for_all_players_in(player_group, actions=[], comment=None, disabled=False, run_on_client=False):
-    return {
-        'type': 'forAllPlayers',
-        'playerGroup': to_dict(player_group),
-        'actions': actions,
-    }
-
-
-@action
 def remove_unit_from_unit_group(unit, unit_group, comment=None, disabled=False, run_on_client=False):
     return {
         'type': 'removeUnitFromUnitGroup',
         'unit': to_dict(unit),
         'unitGroup': to_dict(unit_group),
     }
 
 
 @action
-def flip_sprite_of_entity(flip, entity, comment=None, disabled=False, run_on_client=False):
+def flip_sprite_of_entity(entity, flip, comment=None, disabled=False, run_on_client=False):
     '''Flip the sprite of an entity
 
+    example:
+        `flip_sprite_of_entity(LastTriggeringUnit(), Flip.HORIZONTAL)`
+
     Args:
         entity (Entity): the entity that will be flipped
+
         flip (Flip): the flip direction from `Flip` enum class
     '''
     return {
         'type': 'flipEntitySprite',
         'entity': to_dict(entity),
         'flip': to_dict(flip),
     }
@@ -942,25 +833,14 @@
         'type': 'moveEntity',
         'entity': to_dict(entity),
         'position': to_dict(position),
     }
 
 
 @action
-def for_range(variable, start: Number, stop: Number, actions=[], comment=None, disabled=False, run_on_client=False):
-    return {
-        'type': 'for',
-        'variableName': variable.name,
-        'start': to_dict(start),
-        'stop': to_dict(stop),
-        'actions': actions,
-    }
-
-
-@action
 def show_menu_to_player_and_select_best_server(player, comment=None, disabled=False, run_on_client=False):
     return {
         'type': 'showMenuAndSelectBestServer',
         'player': to_dict(player),
     }
 
 
@@ -1011,23 +891,14 @@
         'type': 'changeUnitType',
         'entity': to_dict(entity),
         'unitType': to_dict(unit_type),
     }
 
 
 @action
-def for_all_debris_in(debris_group, actions=[], comment=None, disabled=False, run_on_client=False):
-    return {
-        'type': 'forAllDebris',
-        'debrisGroup': to_dict(debris_group),
-        'actions': actions,
-    }
-
-
-@action
 def play_music_for_player_repeatedly(music, player, comment=None, disabled=False, run_on_client=False):
     return {
         'type': 'playMusicForPlayerRepeatedly',
         'music': to_dict(music),
         'player': to_dict(player),
     }
 
@@ -1080,21 +951,14 @@
 def make_unit_invisible_to_hostile_players(entity, comment=None, disabled=False, run_on_client=False):
     return {
         'type': 'makeUnitInvisible',
         'entity': to_dict(entity),
     }
 
 
-@action
-def break_loop(comment=None, disabled=False, run_on_client=False):
-    return {
-        'type': 'break',
-    }
-
-
 @ action
 def change_scale_of_sprite_for_entity(scale: Number, entity, comment=None, disabled=False, run_on_client=False):
     return {
         'type': 'changeScaleOfEntitySprite',
         'entity': to_dict(entity),
         'scale': to_dict(scale),
     }
@@ -1609,7 +1473,249 @@
 
 @ action
 def command_ai_to_idle(unit, comment=None, disabled=False, run_on_client=False):
     return {
         'type': 'aiGoIdle',
         'unit': to_dict(unit),
     }
+
+
+# ---------------------------------------------------------------------------- #
+#                              Deprecated Actions                              #
+# ---------------------------------------------------------------------------- #
+
+
+@action
+def break_loop(comment=None, disabled=False, run_on_client=False):
+    '''Deprecated, use the python `break` keyword instead'''
+    return {
+        'type': 'break',
+    }
+
+
+@action
+def continue_loop(comment=None, disabled=False, run_on_client=False):
+    '''Deprecated, use the python `continue` keyword instead'''
+    return {
+        'type': 'continue',
+    }
+
+
+@action
+def return_loop(comment=None, disabled=False, run_on_client=False):
+    '''Deprecated, use the python `return` keyword instead'''
+    return {
+        'type': 'return',
+    }
+
+
+@action
+def if_else(condition: Condition, then_actions=[], else_actions=[], comment=None, disabled=False, run_on_client=False):
+    '''Deprecated, use a python if statement instead:
+    ```
+    if NumberOfPlayers() > 10 & Variables.TIMER <= 0:
+        ...
+    ```
+    '''
+    return {
+        'type': 'condition',
+        'conditions': to_dict(condition),
+        'then': then_actions,
+        'else': else_actions,
+    }
+
+
+@action
+def repeat(count: Number, actions=[], comment=None, disabled=False, run_on_client=False):
+    '''Deprecated, use a python for loop instead:
+    ```
+    for _ in repeat(5):
+        ...
+    ```
+    '''
+    return {
+        'type': 'repeat',
+        'count': to_dict(count),
+        'actions': actions,
+    }
+
+
+@action
+def range(start: Number, stop: Number, variable=None, actions=[], comment=None, disabled=False, run_on_client=False):
+    '''Deprecated, use a python for loop instead:
+    ```
+    for Variables.I in range(5):
+        ...
+    ```
+    '''
+    return {
+        'type': 'for',
+        'variableName': '',
+        'start': to_dict(start),
+        'stop': to_dict(stop),
+        'actions': actions,
+    }
+
+
+@action
+def for_all_entities_in(entity_group, actions=[], comment=None, disabled=False, run_on_client=False):
+    '''Deprecated, use a python for loop instead:
+    ```
+    for entity in AllEntitiesInTheGame()
+        ...
+    ```
+    '''
+    return {
+        'type': 'forAllEntities',
+        'entityGroup': to_dict(entity_group),
+        'actions': actions,
+    }
+
+
+@action
+def for_all_projectiles_in(projectile_group, actions=[], comment=None, disabled=False, run_on_client=False):
+    '''Deprecated, use a python for loop instead:
+    ```
+    for projectile in AllProjectilesInTheGame()
+        ...
+    ```
+    '''
+    return {
+        'type': 'forAllProjectiles',
+        'projectileGroup': to_dict(projectile_group),
+        'actions': actions,
+    }
+
+
+@action
+def for_all_items_in(item_group, actions=[], comment=None, disabled=False, run_on_client=False):
+    '''Deprecated, use a python for loop instead:
+    ```
+    for items in AllItemsInTheGame()
+        ...
+    ```
+    '''
+    return {
+        'type': 'forAllItems',
+        'itemGroup': to_dict(item_group),
+        'actions': actions,
+    }
+
+
+@action
+def for_all_units_in(unit_group, actions=[], comment=None, disabled=False, run_on_client=False):
+    '''Deprecated, use a python for loop instead:
+    ```
+    for unit in AllUnitsInTheGame()
+        ...
+    ```
+    '''
+    return {
+        'type': 'forAllUnits',
+        'unitGroup': to_dict(unit_group),
+        'actions': actions,
+    }
+
+
+@action
+def for_all_players_in(player_group, actions=[], comment=None, disabled=False, run_on_client=False):
+    '''Deprecated, use a python for loop instead:
+    ```
+    for player in AllPlayersInTheGame()
+        ...
+    ```
+    '''
+    return {
+        'type': 'forAllPlayers',
+        'playerGroup': to_dict(player_group),
+        'actions': actions,
+    }
+
+
+@action
+def for_all_item_types_in(item_type_group, actions=[], comment=None, disabled=False, run_on_client=False):
+    '''Deprecated, use a python for loop instead:
+    ```
+    for item_type in AllItemTypesInTheGame()
+        ...
+    ```
+    '''
+    return {
+        'type': 'forAllItemTypes',
+        'itemTypeGroup': to_dict(item_type_group),
+        'actions': actions,
+    }
+
+
+@action
+def for_all_unit_types_in(unit_type_group, actions=[], comment=None, disabled=False, run_on_client=False):
+    '''Deprecated, use a python for loop instead:
+    ```
+    for unit_type in AllUnitTypesInTheGame()
+        ...
+    ```
+    '''
+    return {
+        'type': 'forAllUnitTypes',
+        'unitTypeGroup': to_dict(unit_type_group),
+        'actions': actions,
+    }
+
+
+@action
+def for_all_regions_in(region_group, actions=[], comment=None, disabled=False, run_on_client=False):
+    '''Deprecated, use a python for loop instead:
+    ```
+    for region in AllRegionsInTheGame()
+        ...
+    ```
+    '''
+    return {
+        'type': 'forAllRegions',
+        'regionGroup': to_dict(region_group),
+        'actions': actions,
+    }
+
+
+@action
+def for_all_debris_in(debris_group, actions=[], comment=None, disabled=False, run_on_client=False):
+    '''Deprecated, use a python for loop instead:
+    ```
+    for debris in AllDebrisInTheGame()
+        ...
+    ```
+    '''
+    return {
+        'type': 'forAllDebris',
+        'debrisGroup': to_dict(debris_group),
+        'actions': actions,
+    }
+
+
+@action
+def while_do(conditions, actions=[], comment=None, disabled=False, run_on_client=False):
+    '''Deprecated, use a python while loop instead:
+    ```
+    while NumberOfPlayers() < 5:
+        ...
+    ```
+    '''
+    return {
+        'type': 'while',
+        'conditions': to_dict(conditions),
+        'actions': actions,
+    }
+
+
+@action
+def after_timeout(duration_milliseconds: Number, actions=[], comment=None, disabled=False, run_on_client=False):
+    '''Deprecated, use a python with statement instead:
+    ```
+    with after_timeout(1000):
+        ...
+    ```
+    '''
+    return {
+        'type': 'setTimeOut',
+        'duration': to_dict(duration_milliseconds),
+        'actions': actions,
+    }
```

### Comparing `pymodd-0.3.0/pymodd/functions.py` & `pymodd-1.0.0/pymodd/functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import pymodd
 from caseconverter import camelcase
 
-from .script import Base, to_dict
+from pymodd.script import Base, to_dict
 
 
 class Function(Base):
     def __init__(self):
         self.function = None
         self.options = {}
 
@@ -16,33 +17,14 @@
         data = {
             'function': self.function
         }
         if self.options is not None:
             data.update(self.options)
         return data
 
-    # condition functions
-    def __eq__(self, other):
-        return Condition(self, '==', other)
-
-    def __ne__(self, other):
-        return Condition(self, '!=', other)
-
-    def __ge__(self, other):
-        return Condition(self, '>=', other)
-
-    def __gt__(self, other):
-        return Condition(self, '>', other)
-
-    def __le__(self, other):
-        return Condition(self, '<=', other)
-
-    def __lt__(self, other):
-        return Condition(self, '<', other)
-
     # calculation functions
     def __add__(self, other):
         if 'string' in [type_of_item(self).lower(), type_of_item(other).lower()]:
             return Concat(self, other)
         else:
             return Calculation(self, '+', other)
 
@@ -51,14 +33,17 @@
 
     def __mul__(self, other):
         return Calculation(self, '*', other)
 
     def __truediv__(self, other):
         return Calculation(self, '/', other)
 
+    def __mod__(self, other):
+        return Calculation(self, '%', other)
+
     def __pow__(self, other):
         return Exponent(self, other)
 
     def __radd__(self, other):
         if 'string' in [type_of_item(self).lower(), type_of_item(other).lower()]:
             return Concat(other, self)
         else:
@@ -69,95 +54,66 @@
 
     def __rmul__(self, other):
         return Calculation(other, '*', self)
 
     def __rtruediv__(self, other):
         return Calculation(other, '/', self)
 
+    def __rmod__(self, other):
+        return Calculation(other, '%', self)
+
     def __rpow__(self, other):
         return Exponent(other, self)
 
 
+# only subclasses of Function requires these types
+# (also prevents a circular import)
+from .variable_types import (VariableType, AttributeTypeBase, EntityVariableBase, ItemTypeBase, PlayerTypeBase,
+                             PlayerVariableBase, ProjectileTypeBase, StateBase, UnitTypeBase, VariableBase)
+
+
 # ---------------------------------------------------------------------------- #
 #                                     Other                                    #
 # ---------------------------------------------------------------------------- #
 
 
 def type_of_item(item):
     primitive_to_type = {
         int: 'number',
+        float: 'number',
+        complex: 'number',
         bool: 'boolean',
         str: 'string',
     }
 
-    if isinstance(item, (Undefined, Null)):
+    if isinstance(item, Undefined):
         return None
     if (primitive := primitive_to_type.get(type(item))):
         return primitive
-    if isinstance(item, Variable):
-        return camelcase(item.type)
+    if isinstance(item, VariableBase):
+        return item.data_type.value
+    if isinstance(item, VariableType):
+        base_classes = item.__class__.mro()
+        for i, base_class in enumerate(base_classes):
+            if base_class.__name__ == 'VariableType':
+                return camelcase(base_classes[i-1].__name__)
     if isinstance(item, Function):
         base_classes = item.__class__.mro()
         for i, base_class in enumerate(base_classes):
             if base_class.__name__ == 'Function':
                 return camelcase(base_classes[i-1].__name__)
     return None
 
 
-class Condition(Function):
-    def __init__(self, item_a: Base, operator: str, item_b: Base):
-        """The comparison type of the condition is determined based on the type of item_a
-
-        Args:
-            item_a (Base): any object
-            operator (str): can be regular comparisons (==, !=, >=, ...) or 'AND' and 'OR'
-            item_b (Base): any object
-        """
-
-        self.item_a = item_a
-        self.operator = operator.upper()
-        self.item_b = item_b
-        comparison = None
-        if (operator := operator.lower()) == 'and' or operator == 'or':
-            comparison = operator
-        else:
-            comparison = type_of_item(item_a) or type_of_item(item_b)
-        self.comparison = comparison
-
-    def to_dict(self):
-        return [
-            {
-                'operandType': self.comparison,
-                'operator': self.operator,
-            },
-            to_dict(self.item_a),
-            to_dict(self.item_b)
-        ]
-
-    def __and__(self, other):
-        return Condition(self, 'AND', other)
-
-    def __or__(self, other):
-        return Condition(self, 'OR', other)
-
-
 class Undefined(Function):
     def __init__(self):
         self.function = 'undefinedValue'
         self.options = {}
 
 
-class Null(Function):
-    def __init__(self):
-        self.function = {
-            'direct': True,
-            'value': None,
-        }
-
-
 # ---------------------------------------------------------------------------- #
 #                                    Entitys                                   #
 # ---------------------------------------------------------------------------- #
 
 
 class Entity(Function):
     pass
@@ -583,23 +539,15 @@
 
 
 # ---------------------------------------------------------------------------- #
 #                                    States                                    #
 # ---------------------------------------------------------------------------- #
 
 
-class State(Function):
-    def __init__(self, state_id):
-        self.function = {
-            'direct': True,
-            'value': state_id,
-        }
-
-
-class EntityState(State):
+class CurrentStateOfEntity(StateBase):
     def __init__(self, entity):
         self.function = 'getEntityState'
         self.options = {
             'entity': to_dict(entity),
         }
 
 
@@ -677,15 +625,15 @@
         self.function = 'playerAttributeMax'
         self.options = {
             'attribute': to_dict(attribute),
             'entity': to_dict(entity),
         }
 
 
-class PlayerAttribute(Number):
+class ValueOfPlayerAttribute(Number):
     def __init__(self, attribute, entity):
         self.function = 'getPlayerAttribute'
         self.options = {
             'attribute': to_dict(attribute),
             'entity': to_dict(entity),
         }
 
@@ -911,15 +859,15 @@
     def __init__(self, number):
         self.function = 'absoluteValueOfNumber'
         self.options = {
             'number': to_dict(number),
         }
 
 
-class EntityAttribute(Number):
+class ValueOfEntityAttribute(Number):
     def __init__(self, attribute, entity):
         self.function = 'getEntityAttribute'
         self.options = {
             'attribute': to_dict(attribute),
             'entity': to_dict(entity),
         }
 
@@ -951,15 +899,15 @@
         self.function = 'getQuantityOfItemTypeInItemTypeGroup'
         self.options = {
             'itemType': to_dict(item_type),
             'itemTypeGroup': to_dict(item_type_group),
         }
 
 
-class NumberOfItemsPresent(Number):
+class NumberOfItems(Number):
     def __init__(self):
         self.function = 'getNumberOfItemsPresent'
         self.options = {}
 
 
 class Min(Number):
     def __init__(self, num_a, num_b):
@@ -1047,28 +995,14 @@
     def __init__(self, unit):
         self.function = 'unitSensorRadius'
         self.options = {
             'unit': to_dict(unit),
         }
 
 
-class Calculation(Number):
-    def __init__(self, item_a: Number, operator: str, item_b: Number):
-        self.function = 'calculate'
-        self.options = {
-            'items': [
-                {
-                    'operator': operator
-                },
-                to_dict(item_a),
-                to_dict(item_b),
-            ]
-        }
-
-
 # ---------------------------------------------------------------------------- #
 #                                    Strings                                   #
 # ---------------------------------------------------------------------------- #
 
 
 class String(Function):
     def __init__(self, string):
@@ -1090,23 +1024,14 @@
     def __init__(self, player):
         self.function = 'playerCustomInput'
         self.options = {
             'player': to_dict(player),
         }
 
 
-class Concat(String):
-    def __init__(self, text_a, text_b):
-        self.function = 'concat'
-        self.options = {
-            'textA': to_dict(text_a),
-            'textB': to_dict(text_b),
-        }
-
-
 class NameOfPlayer(String):
     def __init__(self, entity):
         self.function = 'getPlayerName'
         self.options = {
             'entity': to_dict(entity),
         }
 
@@ -1169,15 +1094,15 @@
             'sourceString': to_dict(source_string),
             'newString': to_dict(new_string),
         }
 
 
 class UnixTimeToFormattedString(String):
     def __init__(self, seconds):
-        """formats to (hh::mm:ss)"""
+        '''formats to (hh::mm:ss)'''
         self.function = 'getTimeString'
         self.options = {
             'seconds': to_dict(seconds),
         }
 
 
 class DescriptionOfItem(String):
@@ -1448,76 +1373,38 @@
 
 
 # ---------------------------------------------------------------------------- #
 #                                   Variables                                  #
 # ---------------------------------------------------------------------------- #
 
 
-class Variable(Function):
-    def __init__(self, variable_name, variable_type=None):
-        self.function = 'getVariable'
-        self.name = variable_name
-        self.type = variable_type
-        self.options = {
-            'variableName': variable_name
-        }
-
-
 # ---------------------------------------------------------------------------- #
 #                               Entity Variables                               #
 # ---------------------------------------------------------------------------- #
 
 
-class EntityVariable(Variable):
-    def __init__(self, variable_name, variable_type):
-        self.function = 'getEntityVariable'
-        self.type = variable_type
-        self.options = {
-            'variable': {
-                'text': f'{variable_name}',
-                'dataType': f'{variable_type}',
-                'entity': 'null',
-                'key': f'{variable_name}'
-            }
-        }
-
-
-class ValueOfEntityVariable(Variable):
+class ValueOfEntityVariable(EntityVariableBase):
     def __init__(self, entity_variable_type, entity):
         self.function = 'getValueOfEntityVariable'
-        self.type = entity_variable_type.type
+        self.data_type = entity_variable_type.data_type
         self.options = {
             'variable': to_dict(entity_variable_type),
             'entity': to_dict(entity)
         }
 
 
 # ---------------------------------------------------------------------------- #
 #                               Player Variables                               #
 # ---------------------------------------------------------------------------- #
 
 
-class PlayerVariable(Variable):
-    def __init__(self, variable_name, variable_type):
-        self.function = 'getPlayerVariable'
-        self.type = variable_type
-        self.options = {
-            'variable': {
-                'text': f'{variable_name}',
-                'dataType': f'{variable_type}',
-                'entity': 'null',
-                'key': f'{variable_name}'
-            }
-        }
-
-
-class ValueOfPlayerVariable(Variable):
+class ValueOfPlayerVariable(PlayerVariableBase):
     def __init__(self, player_variable_type, player):
         self.function = 'getValueOfPlayerVariable'
-        self.type = player_variable_type.type
+        self.data_type = player_variable_type.data_type
         self.options = {
             'variable': to_dict(player_variable_type),
             'player': to_dict(player)
         }
 
 
 # ---------------------------------------------------------------------------- #
@@ -1567,173 +1454,141 @@
 
 
 # ---------------------------------------------------------------------------- #
 #                                  Unit Types                                  #
 # ---------------------------------------------------------------------------- #
 
 
-class UnitType(Function):
-    def __init__(self, unit_type_id):
-        self.function = {
-            'direct': True,
-            'value': unit_type_id,
-        }
-
-
-class UnitTypeOfUnit(UnitType):
+class UnitTypeOfUnit(UnitTypeBase):
     def __init__(self, entity):
         self.function = 'getUnitTypeOfUnit'
         self.options = {
             'entity': to_dict(entity),
         }
 
 
-class IdOfLastPurchasedUnitTypet(UnitType):
+class IdOfLastPurchasedUnitTypet(UnitTypeBase):
     def __init__(self):
         self.function = 'lastPurchasedUnitTypetId'
         self.options = {}
 
 
-class RandomUnitTypeFromUnitTypeGroup(UnitType):
+class RandomUnitTypeFromUnitTypeGroup(UnitTypeBase):
     def __init__(self, unit_type_group):
         self.function = 'getRandomUnitTypeFromUnitTypeGroup'
         self.options = {
             'unitTypeGroup': to_dict(unit_type_group),
         }
 
 
-class SelectedUnitType(UnitType):
+class SelectedUnitType(UnitTypeBase):
     def __init__(self):
         self.function = 'selectedUnitType'
         self.options = {}
 
 
 # ---------------------------------------------------------------------------- #
 #                                  Item Types                                  #
 # ---------------------------------------------------------------------------- #
 
 
-class ItemType(Function):
-    def __init__(self, item_type_id):
-        self.function = {
-            'direct': True,
-            'value': item_type_id,
-        }
-
-
-class SelectedItemType(ItemType):
+class SelectedItemType(ItemTypeBase):
     def __init__(self):
         self.function = 'selectedItemType'
         self.options = {}
 
 
-class ItemTypeOfItem(ItemType):
+class ItemTypeOfItem(ItemTypeBase):
     def __init__(self, entity):
         self.function = 'getItemTypeOfItem'
         self.options = {
             'entity': to_dict(entity),
         }
 
 
-class RandomItemTypeFromItemTypeGroup(ItemType):
+class RandomItemTypeFromItemTypeGroup(ItemTypeBase):
     def __init__(self, item_type_group):
         self.function = 'getRandomItemTypeFromItemTypeGroup'
         self.options = {
             'itemTypeGroup': to_dict(item_type_group),
         }
 
 
 # ---------------------------------------------------------------------------- #
 #                               Projectile Types                               #
 # ---------------------------------------------------------------------------- #
 
 
-class ProjectileType(Function):
-    def __init__(self, projectile_type_id):
-        self.function = {
-            'direct': True,
-            'value': projectile_type_id,
-        }
-
-
-class ProjectileTypeOfProjectile(ProjectileType):
+class ProjectileTypeOfProjectile(ProjectileTypeBase):
     def __init__(self, entity):
         self.function = 'getProjectileTypeOfProjectile'
         self.options = {
             'entity': to_dict(entity),
         }
 
 
 # ---------------------------------------------------------------------------- #
 #                                 Player Types                                 #
 # ---------------------------------------------------------------------------- #
 
 
-class PlayerType(Function):
-    def __init__(self, player_type_id):
-        self.function = {
-            'direct': True,
-            'value': player_type_id,
-        }
-
-
-class PlayerTypeOfPlayer(PlayerType):
+class PlayerTypeOfPlayer(PlayerTypeBase):
     def __init__(self, player):
         self.function = 'playerTypeOfPlayer'
         self.options = {
             'player': to_dict(player),
         }
 
 
 # ---------------------------------------------------------------------------- #
 #                                Attribute Types                               #
 # ---------------------------------------------------------------------------- #
 
 
-class AttributeType(Function):
-    def __init__(self, attribute_type_id):
-        self.function = {
-            'direct': True,
-            'value': attribute_type_id,
-        }
-
-
-class AttributeTypeOfAttribute(AttributeType):
+class AttributeTypeOfAttribute(AttributeTypeBase):
     def __init__(self, entity):
         self.function = 'getAttributeTypeOfAttribute'
         self.options = {
             'entity': to_dict(entity),
         }
 
 
 # ---------------------------------------------------------------------------- #
 #                                    Groups                                    #
 # ---------------------------------------------------------------------------- #
 
 
 class Group(Function):
-    pass
+    def _get_iterating_action(self):
+        raise NotImplementedError('_get_iteration_object not implemented')
+
+    def _get_iteration_object(self):
+        raise NotImplementedError('_get_iteration_object not implemented')
 
 
 # ---------------------------------------------------------------------------- #
 #                                 Entity Groups                                #
 # ---------------------------------------------------------------------------- #
 
 
 class EntityGroup(Group):
-    pass
+    def _get_iterating_action(self):
+        return pymodd.actions.for_all_entities_in
+
+    def _get_iteration_object(self):
+        return SelectedEntity()
 
 
 class AllEntitiesCollidingWithLastRaycast(EntityGroup):
     def __init__(self):
         self.function = 'entitiesCollidingWithLastRaycast'
         self.options = {}
 
 
-class AllEntitesInTheGame(EntityGroup):
+class AllEntitiesInTheGame(EntityGroup):
     def __init__(self):
         self.function = 'allEntities'
         self.options = {}
 
 
 class AllEntitiesInRegion(EntityGroup):
     def __init__(self, region):
@@ -1765,15 +1620,19 @@
 
 # ---------------------------------------------------------------------------- #
 #                                  Unit Groups                                 #
 # ---------------------------------------------------------------------------- #
 
 
 class UnitGroup(Group):
-    pass
+    def _get_iterating_action(self):
+        return pymodd.actions.for_all_units_in
+
+    def _get_iteration_object(self):
+        return SelectedUnit()
 
 
 class AllUnitsOwnedByPlayer(UnitGroup):
     def __init__(self, player):
         self.function = 'allUnitsOwnedByPlayer'
         self.options = {
             'player': to_dict(player),
@@ -1820,15 +1679,19 @@
 
 # ---------------------------------------------------------------------------- #
 #                               Projectile Groups                              #
 # ---------------------------------------------------------------------------- #
 
 
 class ProjectileGroup(Group):
-    pass
+    def _get_iterating_action(self):
+        return pymodd.actions.for_all_projectiles_in
+
+    def _get_iteration_object(self):
+        return SelectedProjectile()
 
 
 class AllProjectilesAttachedToUnit(ProjectileGroup):
     def __init__(self, entity):
         self.function = 'allProjectilesAttachedToUnit'
         self.options = {
             'entity': to_dict(entity),
@@ -1843,15 +1706,19 @@
 
 # ---------------------------------------------------------------------------- #
 #                                  Item Groups                                 #
 # ---------------------------------------------------------------------------- #
 
 
 class ItemGroup(Group):
-    pass
+    def _get_iterating_action(self):
+        return pymodd.actions.for_all_items_in
+
+    def _get_iteration_object(self):
+        return SelectedItem()
 
 
 class AllItemsDroppedOnGround(ItemGroup):
     def __init__(self):
         self.function = 'allItemsDroppedOnGround'
         self.options = {}
 
@@ -1880,157 +1747,192 @@
 
 # ---------------------------------------------------------------------------- #
 #                                 Player Groups                                #
 # ---------------------------------------------------------------------------- #
 
 
 class PlayerGroup(Group):
-    pass
+    def _get_iterating_action(self):
+        return pymodd.actions.for_all_players_in
 
+    def _get_iteration_object(self):
+        return SelectedPlayer()
 
-class AllHumanPlayers(PlayerGroup):
+
+class AllHumanPlayersInTheGame(PlayerGroup):
     def __init__(self):
         self.function = 'humanPlayers'
         self.options = {}
 
 
-class AllComputerPlayers(PlayerGroup):
+class AllComputerPlayersInTheGame(PlayerGroup):
     def __init__(self):
         self.function = 'computerPlayers'
         self.options = {}
 
 
-class AllPlayers(PlayerGroup):
+class AllPlayersInTheGame(PlayerGroup):
     def __init__(self):
         self.function = 'allPlayers'
         self.options = {}
 
 
-class AllBotPlayers(PlayerGroup):
+class AllBotPlayersInTheGame(PlayerGroup):
     def __init__(self):
         self.function = 'botPlayers'
         self.options = {}
 
 
 # ---------------------------------------------------------------------------- #
 #                               Item Type Groups                               #
 # ---------------------------------------------------------------------------- #
 
 
 class ItemTypeGroup(Group):
-    pass
+    def _get_iterating_action(self):
+        return pymodd.actions.for_all_item_types_in
+
+    def _get_iteration_object(self):
+        return SelectedItemType()
 
 
-class AllItemTypesInGame(ItemTypeGroup):
+class AllItemTypesInTheGame(ItemTypeGroup):
     def __init__(self):
         self.function = 'allItemTypesInGame'
         self.options = {}
 
 
 # ---------------------------------------------------------------------------- #
 #                               Unit Type Groups                               #
 # ---------------------------------------------------------------------------- #
 
 
 class UnitTypeGroup(Group):
-    pass
+    def _get_iterating_action(self):
+        return pymodd.actions.for_all_unit_types_in
+
+    def _get_iteration_object(self):
+        return SelectedUnitType()
 
 
-class AllUnitTypesInGame(UnitTypeGroup):
+class AllUnitTypesInTheGame(UnitTypeGroup):
     def __init__(self):
         self.function = 'allUnitTypesInGame'
         self.options = {}
 
 
 # ---------------------------------------------------------------------------- #
 #                                 Debris Groups                                #
 # ---------------------------------------------------------------------------- #
 
 
 class DebrisGroup(Group):
-    pass
+    def _get_iterating_action(self):
+        return pymodd.actions.for_all_debris_in
 
+    def _get_iteration_object(self):
+        return SelectedDebris()
 
-class AllDebris(DebrisGroup):
+
+class AllDebrisInTheGame(DebrisGroup):
     def __init__(self):
         self.function = 'allDebris'
         self.options = {}
 
 
 # ---------------------------------------------------------------------------- #
 #                                 Region Groups                                #
 # ---------------------------------------------------------------------------- #
 
 
 class RegionGroup(Group):
-    pass
+    def _get_iterating_action(self):
+        return pymodd.actions.for_all_regions_in
+
+    def _get_iteration_object(self):
+        return SelectedRegion()
 
 
 class AllRegionsInTheGame(RegionGroup):
     def __init__(self):
         self.function = 'allRegions'
         self.options = {}
 
 
 # ---------------------------------------------------------------------------- #
 #                                     Shops                                    #
 # ---------------------------------------------------------------------------- #
 
 
-class Shop(Function):
-    def __init__(self, shop_id):
-        self.function = {
-            'direct': True,
-            'value': shop_id,
-        }
-
-
 # ---------------------------------------------------------------------------- #
 #                                  Animations                                  #
 # ---------------------------------------------------------------------------- #
 
 
-class AnimationType(Function):
-    def __init__(self, animation_type_id):
-        self.function = {
-            'direct': True,
-            'value': animation_type_id,
-        }
-
-
 # ---------------------------------------------------------------------------- #
 #                                     Music                                    #
 # ---------------------------------------------------------------------------- #
 
 
-class Music(Function):
-    def __init__(self, music_id):
-        self.function = {
-            'direct': True,
-            'value': music_id,
-        }
-
-
 # ---------------------------------------------------------------------------- #
 #                                    Sounds                                    #
 # ---------------------------------------------------------------------------- #
 
 
-class Sound(Function):
-    def __init__(self, sound_id):
-        self.function = {
-            'direct': True,
-            'value': sound_id,
-        }
+# ---------------------------------------------------------------------------- #
+#                                   Dialogues                                  #
+# ---------------------------------------------------------------------------- #
 
 
 # ---------------------------------------------------------------------------- #
-#                                   Dialogues                                  #
+#                              Deprecated Actions                              #
 # ---------------------------------------------------------------------------- #
 
 
-class Dialogue(Function):
-    def __init__(self, dialogue_id):
-        self.function = {
-            'direct': True,
-            'value': dialogue_id,
+class Condition(Function):
+    '''Deprecated, use python comparison operators instead'''
+
+    def __init__(self, item_a: Base, operator: str, item_b: Base):
+        self.item_a = item_a
+        self.operator = operator.upper()
+        self.item_b = item_b
+        if self.operator == 'AND' or self.operator == 'OR':
+            self.comparison = operator.lower()
+        else:
+            self.comparison = type_of_item(item_a) or type_of_item(item_b)
+
+    def to_dict(self):
+        return [
+            {
+                'operandType': self.comparison,
+                'operator': self.operator,
+            },
+            to_dict(self.item_a),
+            to_dict(self.item_b)
+        ]
+
+
+class Calculation(Number):
+    '''Deprecated, use python arithmetic operators instead'''
+
+    def __init__(self, item_a: Number, operator: str, item_b: Number):
+        self.function = 'calculate'
+        self.options = {
+            'items': [
+                {
+                    'operator': operator
+                },
+                to_dict(item_a),
+                to_dict(item_b),
+            ]
+        }
+
+
+class Concat(String):
+    '''Deprecated, use python `+` operator instead'''
+
+    def __init__(self, text_a, text_b):
+        self.function = 'concat'
+        self.options = {
+            'textA': to_dict(text_a),
+            'textB': to_dict(text_b),
         }
```

### Comparing `pymodd-0.3.0/pyproject.toml` & `pymodd-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "pymodd"
-version = "0.3.0"
+version = "1.0.0"
 description = "A package for creating modd.io games using python!"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
     {name = "Jeff"}
 ]
```

### Comparing `pymodd-0.3.0/src/game_data/actions.rs` & `pymodd-1.0.0/src/game_data/actions.rs`

 * *Files identical despite different names*

### Comparing `pymodd-0.3.0/src/game_data/argument.rs` & `pymodd-1.0.0/src/game_data/argument.rs`

 * *Files 0% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 use crate::project_generator::utils::to_pymodd_maps::{
     PymoddStructure, FLIP_CONSTANTS_TO_PYMODD_ENUM, FUNCTIONS_TO_PYMODD_STRUCTURE,
     UI_TARGET_CONSTANTS_TO_PYMODD_ENUM,
 };
 
 use super::actions::{parse_actions, Action};
 
-const ARGS_TO_IGNORE: [&str; 8] = [
+const ARGS_TO_IGNORE: [&str; 9] = [
     "type",
     "entityType",
     "vars",
     "function",
     "comment",
     "disabled",
     "runOnClient",
     "hasFixedCSP",
+    "isExpanded",
 ];
 
 /// Accepts both pymodd action and pymodd function data
 pub fn parse_arguments_of_object_data(object_data: &Map<String, Value>) -> Vec<Argument> {
     let mut args = Vec::new();
     object_data
         .iter()
```

### Comparing `pymodd-0.3.0/src/game_data/directory.rs` & `pymodd-1.0.0/src/game_data/directory.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use heck::ToPascalCase;
+use heck::ToSnakeCase;
 use serde_json::{map::Values, Map, Value};
 
 use crate::project_generator::utils::{
     is_valid_class_name, iterators::directory_iterator::DirectoryIterItem,
     to_pymodd_maps::TRIGGERS_TO_PYMODD_ENUM,
 };
 
@@ -147,20 +147,25 @@
     pub name: String,
     pub key: String,
     pub triggers: Vec<String>,
     pub actions: Vec<Action>,
 }
 
 impl Script {
-    pub fn pymodd_class_name(&self) -> String {
-        let class_name = self.name.replace("'", "").to_pascal_case().to_string();
-        if !is_valid_class_name(&class_name) {
-            return format!("q{class_name}");
+    pub fn pymodd_function_name(&self) -> String {
+        let mut function_name = self.name.replace(['\'', '\"'], "").to_snake_case();
+        // use script key as name if script name is empty
+        if function_name.is_empty() {
+            function_name = self.key.to_string().to_lowercase()
+        }
+        if !is_valid_class_name(&function_name) {
+            format!("q{function_name}")
+        } else {
+            function_name
         }
-        class_name
     }
 
     pub fn triggers_into_pymodd_enums(&self) -> Vec<String> {
         self.triggers
             .iter()
             .map(|trigger| {
                 TRIGGERS_TO_PYMODD_ENUM
```

### Comparing `pymodd-0.3.0/src/game_data/variable_categories.rs` & `pymodd-1.0.0/src/game_data/variable_categories.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 use std::collections::HashMap;
 
-use heck::ToPascalCase;
 use serde_json::{Map, Value};
 
 use crate::project_generator::utils::enum_name_of;
 
 pub const VARIABLE_CATEGORIES: [&str; 13] = [
     "animationTypes",
     "attributeTypes",
@@ -23,31 +22,31 @@
 
 pub const VARIABLES_CATEGORY_NAME: &str = "variables";
 // modd.io holds these categories in the "variables" category
 pub const SEPERATED_VARIABLE_CATEGORIES: [&str; 3] =
     ["regions", "itemTypeGroups", "unitTypeGroups"];
 
 const VARIABLE_CATEGORIES_ITERATION_ORDER: [&str; 17] = [
-    "unitTypes",
-    "playerTypes",
     "itemTypes",
     "projectileTypes",
-    "regions",
+    "unitTypes",
+    "playerTypes",
+    "itemTypeGroups",
+    "unitTypeGroups",
     "variables",
     "entityTypeVariables",
     "playerTypeVariables",
-    "animationTypes",
-    "attributeTypes",
-    "itemTypeGroups",
-    "unitTypeGroups",
-    "states",
+    "regions",
     "shops",
     "dialogues",
     "music",
     "sound",
+    "states",
+    "animationTypes",
+    "attributeTypes",
 ];
 
 pub struct CategoriesToVariables {
     pub categories_to_variables: HashMap<&'static str, Vec<Variable>>,
 }
 
 impl CategoriesToVariables {
@@ -101,54 +100,72 @@
                 .position(|element| &element == category)
                 .unwrap()
         });
         categories_of_variables.into_iter()
     }
 }
 
+#[derive(Debug, PartialEq, Eq)]
+pub struct Variable {
+    pub id: String,
+    pub name: String,
+    data: Map<String, Value>,
+}
+
+impl Variable {
+    pub fn enum_name(&self) -> String {
+        enum_name_of(&self.name)
+    }
+
+    pub fn data_type(&self) -> Option<String> {
+        Some(
+            self.get_key("dataType")?
+                .as_str()
+                .filter(|value| !value.is_empty())?
+                .to_string(),
+        )
+    }
+
+    pub fn get_key(&self, key: &str) -> Option<&Value> {
+        self.data.get(key)
+    }
+}
+
 fn variables_from_category_data(category_data: &Value) -> Vec<Variable> {
     category_data
         .as_object()
         .unwrap_or(&Map::new())
         .iter()
-        .map(|(var_id, var)| Variable {
-            id: var_id.clone(),
-            enum_name: enum_name_of(
-                var.get("name")
-                    .unwrap_or(&Value::String(var_id.clone()))
-                    .as_str()
-                    .unwrap(),
-            )
-            .to_string(),
-            data_type: parse_data_type(var.get("dataType")),
+        .map(|(var_id, var)| {
+            let var_name = var
+                .get("name")
+                .unwrap_or(&Value::Null)
+                .as_str()
+                .unwrap_or(var_id);
+            Variable {
+                id: var_id.clone(),
+                name: var_name.to_string(),
+                data: var.as_object().unwrap_or(&Map::new()).clone(),
+            }
         })
         .collect()
 }
 
-fn parse_data_type(data_type: Option<&Value>) -> Option<String> {
-    Some(
-        data_type?
-            .as_str()
-            .filter(|value| !value.is_empty())?
-            .to_string(),
-    )
-}
-
 fn resolve_duplicate_variable_enum_names(variables: Vec<Variable>) -> Vec<Variable> {
     let mut enum_names_to_count: HashMap<String, u32> = HashMap::new();
     variables
         .into_iter()
-        .map(|mut var| {
+        .map(|var| {
             enum_names_to_count.insert(
-                var.enum_name.clone(),
-                enum_names_to_count.get(&var.enum_name).unwrap_or(&0) + 1,
+                var.enum_name(),
+                enum_names_to_count.get(&var.enum_name()).unwrap_or(&0) + 1,
             );
-            if let Some(&count) = enum_names_to_count.get(&var.enum_name) {
+            if let Some(&count) = enum_names_to_count.get(&var.enum_name()) {
                 if count > 1 {
-                    var.enum_name.push_str(format!("_{}", count - 1).as_str());
+                    var.enum_name().push_str(format!("_{}", count - 1).as_str());
                 }
             }
             var
         })
         .collect()
 }
 
@@ -167,82 +184,47 @@
     variables_from_category_data(&variables_category_data)
         .into_iter()
         .for_each(|variable| {
             let seperated_category_of_variable =
                 SEPERATED_VARIABLE_CATEGORIES.iter().find(|&category| {
                     category.eq(&format!(
                         "{}s",
-                        &variable.data_type.as_ref().unwrap_or(&String::new())
+                        &variable.data_type().unwrap_or(String::new())
                     ))
                 });
 
             seperated_category_to_variables
                 .get_mut(seperated_category_of_variable.unwrap_or(&VARIABLES_CATEGORY_NAME))
                 .unwrap()
                 .push(variable);
         });
     seperated_category_to_variables
 }
 
-pub fn pymodd_class_name_of_category(category: &'static str) -> String {
-    let mut class_name = match category {
-        "entityTypeVariables" => "EntityVariables",
-        "playerTypeVariables" => "PlayerVariables",
-        _ => category,
-    }
-    .to_pascal_case()
-    .to_string();
-    if !class_name.ends_with("s") {
-        class_name.push('s')
-    }
-    class_name
-}
-
-pub fn pymodd_class_type_of_category(category: &'static str) -> String {
-    // in order to match with classes defined in pymodd/functions.py
-    if VARIABLES_CATEGORY_NAME == category || SEPERATED_VARIABLE_CATEGORIES.contains(&category) {
-        return String::from("Variable");
-    }
-    pymodd_class_name_of_category(&category)
-        .strip_suffix('s')
-        .unwrap()
-        .to_string()
-}
-
-pub fn is_category_of_variable_type(category: &'static str) -> bool {
-    category.to_lowercase().contains("variables")
-        || SEPERATED_VARIABLE_CATEGORIES.contains(&category)
-}
-
-#[derive(Debug, PartialEq, Eq)]
-pub struct Variable {
-    pub id: String,
-    pub enum_name: String,
-    pub data_type: Option<String>,
-}
-
 #[cfg(test)]
 mod tests {
     use std::collections::HashMap;
 
-    use serde_json::json;
+    use serde_json::{json, Map, Value};
 
     use crate::game_data::variable_categories::seperated_variables_categories;
 
     use super::{
         resolve_duplicate_variable_enum_names, variables_from_category_data, CategoriesToVariables,
         Variable,
     };
 
     impl Variable {
-        pub fn new(id: &str, enum_name: &str, data_type: Option<&str>) -> Variable {
+        pub fn new(id: &str, name: &str, additonal_data: Value) -> Variable {
+            let mut data = additonal_data.as_object().unwrap_or(&Map::new()).clone();
+            data.insert(String::from("name"), Value::String(name.to_string()));
             Variable {
                 id: id.to_string(),
-                enum_name: enum_name.to_string(),
-                data_type: data_type.map(|val| val.to_string()),
+                name: name.to_string(),
+                data,
             }
         }
     }
 
     impl CategoriesToVariables {
         pub fn new(map: HashMap<&'static str, Vec<Variable>>) -> CategoriesToVariables {
             CategoriesToVariables {
@@ -253,61 +235,69 @@
 
     #[test]
     fn find_variable_with_key() {
         assert_eq!(
             CategoriesToVariables::new(HashMap::from([
                 (
                     "unitTypeGroups",
-                    vec![Variable::new("O23FJW2", "BANANA", Some("unitTypeGroup"))]
+                    vec![Variable::new(
+                        "O23FJW2",
+                        "banana",
+                        json!({"dataType": "unitTypeGroup"})
+                    )]
                 ),
                 (
                     "regions",
-                    vec![Variable::new("WDWI313", "WATER", Some("region"))]
+                    vec![Variable::new(
+                        "WDWI313",
+                        "water",
+                        json!({"dataType": "region"})
+                    )]
                 ),
                 ("variables", vec![]),
             ]))
             .find_categoried_variable_with_id("WDWI313")
             .unwrap(),
             (
                 "regions",
-                &Variable::new("WDWI313", "WATER", Some("region"))
+                &Variable::new("WDWI313", "water", json!({"dataType": "region"}))
             )
         );
     }
 
     #[test]
     fn parse_variables_from_category_data() {
         assert_eq!(
             variables_from_category_data(&json!({
                 "FW3513W": { "name": "apple", "dataType": None::<&str> },
                 "O23FJW2": { "name": "banana", "dataType": "" },
                 "WDWI313": { "name": "water", "dataType": "region" },
             }))
             .as_slice(),
             [
-                Variable::new("FW3513W", "APPLE", None),
-                Variable::new("O23FJW2", "BANANA", None),
-                Variable::new("WDWI313", "WATER", Some("region")),
+                Variable::new("FW3513W", "apple", json!({ "dataType": null })),
+                Variable::new("O23FJW2", "banana", json!({"dataType": ""})),
+                Variable::new("WDWI313", "water", json!({"dataType": "region"})),
             ]
         );
     }
 
     #[test]
     fn ensure_no_duplicated_enum_names() {
         assert_eq!(
             resolve_duplicate_variable_enum_names(vec![
-                Variable::new("FW3513W", "APPLE", None),
-                Variable::new("O23FJW2", "APPLE", None),
-                Variable::new("WDWI313", "APPLE", None),
+                Variable::new("FW3513W", "apple", json!({})),
+                Variable::new("O23FJW2", "apple", json!({})),
+                Variable::new("WDWI313", "apple", json!({})),
             ])
             .as_slice(),
             [
-                Variable::new("FW3513W", "APPLE", None),
-                Variable::new("O23FJW2", "APPLE_1", None),
-                Variable::new("WDWI313", "APPLE_2", None),
+                Variable::new("FW3513W", "apple", json!({})),
+                Variable::new("O23FJW2", "apple", json!({})),
+                Variable::new("WDWI313", "apple", json!({})),
             ]
         );
     }
 
     #[test]
     fn seperate_variables_category_into_multiple() {
         assert_eq!(
@@ -315,22 +305,34 @@
                 "FW3513W": { "name": "apple", "dataType": "itemTypeGroup" },
                 "O23FJW2": { "name": "banana", "dataType": "unitTypeGroup" },
                 "WDWI313": { "name": "water", "dataType": "region" },
             })),
             HashMap::from([
                 (
                     "itemTypeGroups",
-                    vec![Variable::new("FW3513W", "APPLE", Some("itemTypeGroup"))]
+                    vec![Variable::new(
+                        "FW3513W",
+                        "apple",
+                        json!({"dataType": "itemTypeGroup"})
+                    )]
                 ),
                 (
                     "unitTypeGroups",
-                    vec![Variable::new("O23FJW2", "BANANA", Some("unitTypeGroup"))]
+                    vec![Variable::new(
+                        "O23FJW2",
+                        "banana",
+                        json!({"dataType": "unitTypeGroup"})
+                    )]
                 ),
                 (
                     "regions",
-                    vec![Variable::new("WDWI313", "WATER", Some("region"))]
+                    vec![Variable::new(
+                        "WDWI313",
+                        "water",
+                        json!({"dataType": "region"})
+                    )]
                 ),
                 ("variables", vec![]),
             ])
         );
     }
 }
```

### Comparing `pymodd-0.3.0/src/game_data.rs` & `pymodd-1.0.0/src/game_data.rs`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 }
 
 impl GameData {
     pub fn parse(game_json_file_content: String) -> Result<GameData, &'static str> {
         let mut deserializer = serde_json::Deserializer::from_str(&game_json_file_content);
         deserializer.disable_recursion_limit();
         let deserializer = serde_stacker::Deserializer::new(&mut deserializer);
-        let game_json = Value::deserialize(deserializer)
-            .map_err(|_| "error parsing modd.io json file!")?;
+        let game_json =
+            Value::deserialize(deserializer).map_err(|_| "error parsing modd.io json file!")?;
         let game_data = &game_json["data"];
         Ok(GameData {
             name: game_json
                 .get("title")
                 .ok_or("invalid modd.io json file! missing key: title")?
                 .to_string(),
             categories_to_variables: CategoriesToVariables::parse(&game_data),
```

### Comparing `pymodd-0.3.0/src/lib.rs` & `pymodd-1.0.0/src/lib.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,17 @@
 mod game_data;
 mod project_generator;
 
-use std::fs;
-
 use crossterm::style::Stylize;
 use game_data::GameData;
 use project_generator::ProjectGenerator;
 use pyo3::prelude::*;
 
 #[pyfunction]
-fn generate_project_from_json_file_path(json_file_path: String) {
-    let json_file_content = match fs::read_to_string(&json_file_path) {
-        Err(_) => {
-            log_error("invalid json file path!");
-            return;
-        }
-        Ok(content) => content,
-    };
-
+fn generate_project_from_json_file_content(json_file_content: String) {
     let game_data = match GameData::parse(json_file_content) {
         Err(err_msg) => {
             log_error(err_msg);
             return;
         }
         Ok(data) => data,
     };
@@ -66,14 +56,17 @@
         }
         .dark_green()
     );
 }
 
 #[pymodule]
 fn _pymodd_helper(_py: Python, m: &PyModule) -> PyResult<()> {
-    m.add_function(wrap_pyfunction!(generate_project_from_json_file_path, m)?)?;
+    m.add_function(wrap_pyfunction!(
+        generate_project_from_json_file_content,
+        m
+    )?)?;
     m.add_function(wrap_pyfunction!(log_success, m)?)?;
     m.add_function(wrap_pyfunction!(log_error, m)?)?;
     m.add_function(wrap_pyfunction!(log_cli_start_message, m)?)?;
     m.add_function(wrap_pyfunction!(log_cli_end_message, m)?)?;
     Ok(())
 }
```

### Comparing `pymodd-0.3.0/src/project_generator/entity_scripts_file.rs` & `pymodd-1.0.0/src/project_generator/mapping_file.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,130 +1,120 @@
-use crate::game_data::{
-    entity_types::EntityType, variable_categories::pymodd_class_name_of_category, GameData,
-};
+use std::ops::Add;
+
+use heck::ToPascalCase;
 
-use super::{
-    mapping_file::build_directory_items_contents,
-    scripts_file::{build_directory_content, ScriptsContentBuilder},
-    utils::enum_name_of,
+use crate::game_data::{directory::Directory, entity_types::CategoriesToEntityTypes, GameData};
+
+use super::utils::{
+    iterators::directory_iterator::DirectoryIterItem, surround_string_with_quotes, TAB_SIZE,
 };
 
-pub struct EntityScriptsFile {}
+pub struct MappingFile {}
 
-impl EntityScriptsFile {
+impl MappingFile {
     pub fn build_content(game_data: &GameData) -> String {
+        let game_class_name = game_data.name.to_pascal_case().to_string();
         let mut content = format!(
-            "from pymodd.actions import *\n\
-            from pymodd.functions import *\n\
-            from pymodd.script import EntityScripts, Folder, Trigger, UiTarget, Flip, script\n\n\
-            from game_variables import *\n\n\n"
+            "from pymodd.game import Game, Folder\n\n\
+            from scripts import *\n\
+            from entity_scripts import * \n\n\n\
+            class {game_class_name}(Game):\n\
+                \tdef _build(self):\n\
+                    \t\tself.entity_scripts = [{}]\n\
+                    \t\tself.scripts = [\n",
+            retrieve_clases_of_entity_scripts(&game_data.categories_to_entity_types).join(", ")
         );
-        let scripts_class_content_builder = ScriptsContentBuilder::new(
-            &game_data.categories_to_variables,
-            &game_data.root_directory,
+        content.push_str(
+            &build_directory_items_contents(&game_data.root_directory)
+                .into_iter()
+                .map(|element| format!("{}{element}\n", "\t".repeat(3)))
+                .collect::<String>()
+                .as_str(),
         );
-
-        game_data
-            .categories_to_entity_types
-            .iter()
-            .for_each(|(category, entity_types)| {
-                entity_types
-                    .iter()
-                    .filter(|entity_type| !entity_type.directory.is_empty())
-                    .for_each(|entity_type| {
-                        content.push_str(&format!(
-                            "{}\n{}\n\n",
-                            build_class_content_of_entity_type_in_category(&entity_type, category),
-                            build_directory_content(
-                                &entity_type.directory,
-                                &scripts_class_content_builder
-                            )
-                            .lines()
-                            .map(|line| { format!("\t{line}\n") })
-                            .collect::<String>()
-                            // remove one line in between the scripts of the entity_type
-                            .replace("\t\n\t\n", "\n")
-                        ));
-                    });
-            });
-        content
+        content.add(
+            &format!(
+                "\t\t\t\n\
+                \t\t]\n\n\n\
+                # run `pymodd compile` within this project directory to generate this game's json files\n\
+                # example:\n\
+                \"\"\"\n\
+                $ cd {}\n\
+                $ pymodd compile\n\
+                \"\"\"\n",
+                game_data.pymodd_project_name()
+            )
+            .as_str(),
+        ).replace("\t", &" ".repeat(TAB_SIZE))
     }
 }
 
-fn build_class_content_of_entity_type_in_category(
-    entity_type: &EntityType,
-    category: &'static str,
-) -> String {
-    let (entity_type_class_name, category_class_name) = (
-        entity_type.pymodd_class_name(),
-        pymodd_class_name_of_category(category),
-    );
-    format!(
-        "class {entity_type_class_name}(EntityScripts):\n\
-            \tdef _build(self):\n\
-                \t\tself.entity_type = {category_class_name}.{}\n\
-                \t\tself.scripts = [\n\
-                {}\
-                \t\t\t\n\
-                \t\t]\n",
-        enum_name_of(&entity_type.name),
-        build_directory_elements_for_entity_type(&entity_type)
-            .into_iter()
-            .map(|element| format!("{}{element}\n", "\t".repeat(3)))
-            .collect::<String>()
-    )
+fn retrieve_clases_of_entity_scripts(
+    entity_type_categories: &CategoriesToEntityTypes,
+) -> Vec<String> {
+    entity_type_categories
+        .iter()
+        .flat_map(|(_category, entity_types)| entity_types)
+        .filter(|entity_type| !entity_type.directory.is_empty())
+        .map(|entity_type| entity_type.pymodd_class_name().add("()"))
+        .collect()
 }
 
-fn build_directory_elements_for_entity_type(entity_type: &EntityType) -> Vec<String> {
-    build_directory_items_contents(&entity_type.directory)
-        .into_iter()
-        .map(|mut element| {
-            if !element.trim_start().starts_with("Folder") && !element.trim_start().starts_with("]")
-            {
-                element.insert_str(element.find(char::is_alphabetic).unwrap_or(0), "self.")
+pub fn build_directory_items_contents(directory: &Directory) -> Vec<String> {
+    let mut elements = Vec::new();
+    let mut curr_depth = 0;
+    directory.iter_flattened().for_each(|game_item| {
+        elements.push(match game_item {
+            DirectoryIterItem::StartOfDirectory(directory) => {
+                curr_depth += 1;
+                format!(
+                    "{}Folder({}, [",
+                    "\t".repeat(curr_depth - 1),
+                    surround_string_with_quotes(&directory.name)
+                )
+            }
+            DirectoryIterItem::Script(script) => {
+                format!(
+                    "{}{}(),",
+                    "\t".repeat(curr_depth),
+                    script.pymodd_function_name()
+                )
+            }
+            DirectoryIterItem::DirectoryEnd => {
+                curr_depth -= 1;
+                format!("{}]),", "\t".repeat(curr_depth))
             }
-            element
         })
-        .collect()
+    });
+    elements
 }
 
 #[cfg(test)]
 mod tests {
     use serde_json::json;
 
     use crate::{
-        game_data::{directory::Directory, entity_types::EntityType},
-        project_generator::entity_scripts_file::build_class_content_of_entity_type_in_category,
+        game_data::directory::Directory,
+        project_generator::mapping_file::build_directory_items_contents,
     };
 
     #[test]
-    fn simple_entity_scripts_class_content() {
+    fn directory_content() {
         assert_eq!(
-            build_class_content_of_entity_type_in_category(
-                &EntityType {
-                    name: "bob".to_string(),
-                    directory: Directory::parse(&json!({
-                        "DF31W32": { "name": "initialize", "key": "DF31W32", "actions": [{
-                            "type": null
-                        }], "parent": null, "order": 1 },
-                        "31IAD2B": { "triggers": [], "folderName": "utils",
-                            "key": "31IAD2B", "parent": null, "order": 2 },
-                        "SDUW31W": { "triggers": [], "name": "change_state",
-                            "key": "SDUW31W", "actions": [], "parent": "31IAD2B", "order": 1 }
-                    }))
-                },
-                "unitTypes"
-            )
-            .as_str(),
-            "class Bob(EntityScripts):\n\
-                \tdef _build(self):\n\
-                    \t\tself.entity_type = UnitTypes.BOB\n\
-                    \t\tself.scripts = [\n\
-                        \t\t\tself.Initialize(),\n\
-                        \t\t\tFolder('utils', [\n\
-                            \t\t\t\tself.ChangeState(),\n\
-                        \t\t\t]),\n\
-                        \t\t\t\n\
-                    \t\t]\n"
+            build_directory_items_contents(&Directory::parse(&json!({
+                "WI31HDK": { "name": "initialize", "key": "WI31HDK", "actions": [], "parent": None::<&str>, "order": 1},
+                "31IAD2B": { "folderName": "utils", "key": "31IAD2B", "parent": None::<&str>, "order": 2 },
+                "SDUW31W": { "name": "change_state", "key": "SDUW31W", "actions": [], "parent": "31IAD2B", "order": 1 },
+                "Q31E2RS": { "name": "check_players", "key": None::<&str>, "actions": [], "parent": "31IAD2B", "order": 2 },
+                "HWI31WQ": { "folderName": "other", "key": "HWI31WQ", "parent": "31IAD2B", "order": 3 },
+                "JK32Q03": { "name": "destroy_server", "key": "JK32Q03", "actions": [], "parent": "HWI31WQ", "order": 1},
+            }))).into_iter().collect::<String>(),
+            "initialize(),\
+            Folder('utils', [\
+                \tchange_state(),\
+                \tcheck_players(),\
+                \tFolder('other', [\
+                    \t\tdestroy_server(),\
+                \t]),\
+            ]),"
         );
     }
 }
```

### Comparing `pymodd-0.3.0/src/project_generator/scripts_file.rs` & `pymodd-1.0.0/src/project_generator/scripts_file.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 use std::ops::Add;
 
+use heck::{ToSnakeCase, ToUpperCamelCase};
 use serde_json::Value;
 
 use crate::game_data::{
     actions::Action,
     directory::{Directory, Script},
-    variable_categories::{pymodd_class_name_of_category, CategoriesToVariables},
+    variable_categories::CategoriesToVariables,
     GameData,
 };
 
-use super::utils::{
-    iterators::{
-        argument_values_iterator::{ArgumentValueIterItem, ArgumentValuesIterator, Operation},
-        directory_iterator::DirectoryIterItem,
+use super::{
+    game_variables_file::pymodd_class_name_of_category,
+    utils::{
+        iterators::{
+            argument_values_iterator::{ArgumentValueIterItem, ArgumentValuesIterator, Operation},
+            directory_iterator::DirectoryIterItem,
+        },
+        surround_string_with_quotes, TAB_SIZE,
     },
-    surround_string_with_quotes,
 };
 
 pub struct ScriptsFile {}
 
 impl ScriptsFile {
     pub fn build_content(game_data: &GameData) -> String {
-        let content = format!(
+        format!(
             "from pymodd.actions import *\n\
             from pymodd.functions import *\n\
             from pymodd.script import Trigger, UiTarget, Flip, script\n\n\
-            from game_variables import *\n\n\n"
-        );
-        content.add(&build_directory_content(
-            &game_data.root_directory,
-            &ScriptsContentBuilder::new(
-                &game_data.categories_to_variables,
+            from game_variables import *\n\n\n\
+            {}\n\n",
+            &build_directory_content(
                 &game_data.root_directory,
-            ),
-        ))
+                &ScriptsContentBuilder::new(
+                    &game_data.categories_to_variables,
+                    &game_data.root_directory,
+                ),
+            )
+        )
+        .replace("\t", &" ".repeat(TAB_SIZE))
     }
 }
 
 pub fn build_directory_content(
     directory: &Directory,
     scripts_class_content_builder: &ScriptsContentBuilder,
 ) -> String {
@@ -76,129 +82,319 @@
         ScriptsContentBuilder {
             categories_to_variables,
             root_directory,
         }
     }
 
     pub fn build_script_content(&self, script: &Script) -> String {
-        let class_name = script.pymodd_class_name();
+        let function_name = script.pymodd_function_name();
         format!(
             "@script(triggers=[{}]{})\n\
-            class {class_name}():\n\
-            \tdef _build(self):\n\
-                \t\tself.actions = [\n\
-                {}\
-                \t\t\t\n\
-                \t\t]\n",
+            def {function_name}():\n\
+                {}",
             script.triggers_into_pymodd_enums().join(", "),
-            if !script.name.is_ascii() {
-                format!(", name={}", surround_string_with_quotes(&script.name))
-            } else {
+            if script.name.is_ascii() {
                 String::new()
+            } else {
+                format!(", name={}", surround_string_with_quotes(&script.name))
             },
-            self.build_actions_content(&script.actions)
-                .lines()
-                .map(|action| format!("{}{action}\n", "\t".repeat(3)))
-                .collect::<String>(),
+            if script.actions.len() > 0 {
+                let content = self
+                    .build_actions_content(&script.actions)
+                    .lines()
+                    .map(|action| format!("{}{action}\n", "\t"))
+                    .collect::<String>();
+                // generate pass statements for functions with commented bodies
+                if self.is_body_commented_out(&format!("def func:\n{content}")) {
+                    content.to_string().add("\tpass\n")
+                } else {
+                    content
+                }
+            } else {
+                String::from("\tpass\n")
+            }
         )
     }
 
     fn build_actions_content(&self, actions: &Vec<Action>) -> String {
         actions
             .iter()
             .map(|action| self.build_action_content(&action))
             .collect::<String>()
     }
 
     fn build_action_content(&self, action: &Action) -> String {
+        // for use while converting arguments of special actions
+        let (none, pass) = (String::from("None"), String::from("\t\tpass\n"));
+
+        // convert actions into python statements
+        let statement_content = match action.name.as_str() {
+            // convert condition actions into if statements
+            "condition" => {
+                let args = self.build_arguments_of_action_individually(action);
+                let (condition, then_actions, else_actions) = (
+                    args.get(0).unwrap_or(&none),
+                    args.get(1).unwrap_or(&pass),
+                    args.get(2).unwrap_or(&pass),
+                );
+                Some(format!(
+                    "if {condition}:{}{}",
+                    then_actions.strip_suffix("\n").unwrap(),
+                    if else_actions != "\n\tpass\n" {
+                        format!("\nelse:{else_actions}")
+                    } else {
+                        String::from("\n")
+                    }
+                ))
+            }
+
+            // convert variable for loop actions into for loops
+            "for" => {
+                let args = self.build_arguments_of_action_individually(action);
+                let (start, stop, variable, actions) = (
+                    args.get(0).unwrap_or(&none),
+                    args.get(1).unwrap_or(&none),
+                    args.get(2).unwrap_or(&none),
+                    args.get(3).unwrap_or(&pass),
+                );
+                Some(format!(
+                    "for {variable} in range({start}, {stop}):{actions}"
+                ))
+            }
+
+            // convert for each type in function/variable actions into for loops
+            "forAllEntities" | "forAllProjectiles" | "forAllItems" | "forAllUnits"
+            | "forAllPlayers" | "forAllItemTypes" | "forAllUnitTypes" | "forAllRegions"
+            | "forAllDebris" => {
+                let args = self.build_arguments_of_action_individually(action);
+                let (group, actions) = (args.get(0).unwrap_or(&none), args.get(1).unwrap_or(&pass));
+                let group_type = match action
+                    .name
+                    .strip_prefix("forAll")
+                    .unwrap()
+                    .to_snake_case()
+                    .strip_suffix("s")
+                    .unwrap()
+                {
+                    "entitie" => "entity",
+                    "debri" => "debris",
+                    group_type => group_type,
+                }
+                .to_string();
+                // use the variable provided by the for loop instead of functions
+                let actions = actions.replace(
+                    &format!("Selected{}()", group_type.to_upper_camel_case()),
+                    &group_type,
+                );
+                Some(format!("for {group_type} in {group}:{actions}"))
+            }
+
+            // convert repeat actions into for loops
+            "repeat" => {
+                let args = self.build_arguments_of_action_individually(action);
+                let (count, actions) = (args.get(0).unwrap_or(&none), args.get(1).expect(&pass));
+                Some(format!("for _ in repeat({count}):{actions}"))
+            }
+
+            // convert while actions into while loops
+            "while" => {
+                let args = self.build_arguments_of_action_individually(action);
+                let (condition, actions) =
+                    (args.get(0).unwrap_or(&none), args.get(1).unwrap_or(&pass));
+                Some(format!("while {condition}:{actions}"))
+            }
+
+            // convert set timeout actions into with loops
+            "setTimeOut" => {
+                let args = self.build_arguments_of_action_individually(action);
+                let (duration, actions) =
+                    (args.get(0).unwrap_or(&none), args.get(1).unwrap_or(&pass));
+                Some(format!("with after_timeout({duration}):{actions}"))
+            }
+
+            _ => None,
+        };
+        if let Some(statement_content) = statement_content {
+            return match action.disabled {
+                true => self.comment_out_statement_content(statement_content),
+                false => {
+                    self.append_pass_keyword_to_commented_bodies_of_statement(statement_content)
+                }
+            };
+        }
+
         match action.name.as_str() {
+            // convert break, continue, and return actions into python keywords
+            "break" | "continue" | "return" => {
+                format!(
+                    "{}{}\n",
+                    if action.disabled { "# " } else { "" },
+                    &action.name
+                )
+            }
+
             "comment" => {
                 format!(
-                    "{}({}{}),\n",
+                    "{}({}{})\n",
                     action.pymodd_class_name(),
                     // set argument manually for comments
                     surround_string_with_quotes(
                         action.comment.as_ref().unwrap_or(&String::from("None"))
                     ),
                     self.build_optional_arguments_contents(&action)
                         .into_iter()
                         .skip(1) // skip over optional comment argument
                         .map(|arg| String::from(", ") + &arg)
                         .collect::<String>(),
                 )
             }
+
             _ => format!(
-                "{}({}",
+                "{}({}{})\n",
                 action.pymodd_class_name(),
-                self.build_arguments_content(action.iter_flattened_argument_values())
-            )
-            .add(
+                self.build_arguments_content(action.iter_flattened_argument_values()),
                 &self
                     .build_optional_arguments_contents(&action)
                     .into_iter()
                     .enumerate()
                     .map(|(i, arg)| {
                         if action.args.is_empty() && i == 0 {
                             arg
                         } else {
                             String::from(", ") + &arg
                         }
                     })
                     .collect::<String>(),
-            )
-            .add("),\n"),
+            ),
+        }
+    }
+
+    fn comment_out_statement_content(&self, statement_content: String) -> String {
+        statement_content
+            .lines()
+            .map(|line| {
+                if line.trim().starts_with("# ") {
+                    format!("# \t{}", line.trim().strip_prefix("# ").unwrap())
+                } else {
+                    format!("# {line}")
+                }
+                .add("\n")
+            })
+            .collect()
+    }
+
+    fn append_pass_keyword_to_commented_bodies_of_statement(
+        &self,
+        statement_content: String,
+    ) -> String {
+        let bodies: Vec<&str> = statement_content.trim().split("\nelse:").collect();
+        let (mut then_body, mut else_body) = (
+            bodies.get(0).unwrap_or(&"").to_string(),
+            format!("else:{}", bodies.get(1).unwrap_or(&"").to_string()),
+        );
+        if self.is_body_commented_out(&then_body) {
+            then_body = then_body.add("\n\tpass")
+        }
+        if self.is_body_commented_out(&else_body) {
+            else_body = else_body.add("\n\tpass")
         }
+        format!(
+            "{then_body}{}\n",
+            // add else body if it is not empty
+            if else_body != String::from("else:") {
+                format!("\n{else_body}")
+            } else {
+                String::new()
+            }
+        )
+    }
+
+    fn is_body_commented_out(&self, body_content: &String) -> bool {
+        let body_lines = body_content.lines();
+        if body_lines.collect::<Vec<&str>>().len() == 1 {
+            return false;
+        }
+        !body_content
+            .lines()
+            .skip(1)
+            .any(|line| line.starts_with("\t") & !line.starts_with("\t# "))
+    }
+
+    /// used while parsing if statements, for loops, and while loops
+    fn build_arguments_of_action_individually(&self, action: &Action) -> Vec<String> {
+        action
+            .args
+            .iter()
+            .map(|arg| {
+                self.build_arguments_content(ArgumentValuesIterator::new(&vec![arg.clone()]))
+            })
+            .collect::<Vec<String>>()
     }
 
     fn build_arguments_content(&self, args_iter: ArgumentValuesIterator) -> String {
         args_iter
             .fold(String::from("("), |pymodd_args, arg| {
                 let include_seperator =
                     !pymodd_args.ends_with("(") && arg != ArgumentValueIterItem::FunctionEnd;
                 pymodd_args
-                    + &format!(
-                        "{}{}",
-                        String::from(if include_seperator { ", " } else { "" }),
-                        match arg {
-                            // surround entire condition with parenthesis
-                            ArgumentValueIterItem::Condition(_) =>
-                                format!("({})", self.build_argument_content(arg)),
-                            _ => self.build_argument_content(arg),
+                    .add(if include_seperator { ", " } else { "" })
+                    .add(&{
+                        // remove parentheses surrounding the outermost layer of conditions
+                        if let ArgumentValueIterItem::Condition(_) = arg {
+                            let condition_content = self.build_argument_content(arg);
+                            if condition_content.starts_with("(")
+                                && condition_content.ends_with(")")
+                            {
+                                condition_content
+                                    .strip_prefix("(")
+                                    .unwrap()
+                                    .strip_suffix(")")
+                                    .unwrap()
+                                    .to_string()
+                            } else {
+                                condition_content
+                            }
+                        } else {
+                            self.build_argument_content(arg)
                         }
-                    )
+                    })
             })
             .strip_prefix("(")
             .unwrap()
             .to_string()
     }
 
-    fn build_argument_content(&self, arg: ArgumentValueIterItem) -> String {
+    pub(crate) fn build_argument_content(&self, arg: ArgumentValueIterItem) -> String {
         match arg {
             ArgumentValueIterItem::StartOfFunction(function) => {
                 format!("{}(", function.pymodd_class_name())
             }
             ArgumentValueIterItem::Actions(actions) => {
                 format!(
-                    "[\n{}\t\n]",
-                    self.build_actions_content(actions)
-                        .lines()
-                        .map(|line| format!("\t{line}\n"))
-                        .collect::<String>()
+                    "\n{}",
+                    if actions.len() > 0 {
+                        self.build_actions_content(actions)
+                            .lines()
+                            .map(|line| format!("\t{line}\n"))
+                            .collect::<String>()
+                    } else {
+                        String::from("\tpass\n")
+                    }
                 )
             }
             ArgumentValueIterItem::Value(value) => match value {
                 Value::String(string) => {
                     match self
                         .categories_to_variables
                         .find_categoried_variable_with_id(string)
                     {
                         Some((category, variable)) => format!(
                             "{}.{}",
                             pymodd_class_name_of_category(category),
-                            variable.enum_name
+                            variable.enum_name()
                         ),
                         _ => surround_string_with_quotes(string),
                     }
                 }
                 Value::Bool(boolean) => String::from(match boolean {
                     true => "True",
                     false => "False",
@@ -213,46 +409,55 @@
                 self.build_operation_content(&operation)
             }
             ArgumentValueIterItem::ScriptKey(key) => {
                 let item_with_key = self.root_directory.find_item_with_key(&key);
                 if item_with_key.is_some() {
                     if let DirectoryIterItem::Script(script) = item_with_key.unwrap() {
                         // run_script action accepts Script objects, not keys
-                        return format!("{}()", script.pymodd_class_name());
+                        return format!("{}()", script.pymodd_function_name());
                     }
                 }
                 String::from("None")
             }
+            ArgumentValueIterItem::None => String::from("None"),
             ArgumentValueIterItem::FunctionEnd => String::from(")"),
         }
     }
 
     fn build_operation_content(&self, operator: &Operation) -> String {
         let (item_a, operator, item_b) = (
             ArgumentValueIterItem::from_argument(&operator.item_a),
             ArgumentValueIterItem::from_argument(&operator.operator),
             ArgumentValueIterItem::from_argument(&operator.item_b),
         );
 
-        format!(
+        let operator = if let ArgumentValueIterItem::Value(operator_val) = operator {
+            into_operator(operator_val.as_str().unwrap_or("")).unwrap_or("")
+        } else {
+            ""
+        };
+
+        let content = format!(
             "{} {} {}",
             self.build_operation_item_content(item_a),
-            if let ArgumentValueIterItem::Value(operator_value) = operator {
-                into_operator(operator_value.as_str().unwrap_or("")).unwrap_or("")
-            } else {
-                ""
-            },
+            operator,
             self.build_operation_item_content(item_b)
-        )
+        );
+        // surround `and` and `or` conditions with parentheses
+        if ["and", "or"].contains(&operator) {
+            format!("({content})")
+        } else {
+            content
+        }
     }
 
     fn build_operation_item_content(&self, operation_item: ArgumentValueIterItem) -> String {
         match operation_item {
-            // only surround conditions and calculations with parenthesis
-            ArgumentValueIterItem::Condition(_) | ArgumentValueIterItem::Calculation(_) => {
+            // surround calculations with parentheses
+            ArgumentValueIterItem::Calculation(_) => {
                 format!("({})", self.build_argument_content(operation_item))
             }
             ArgumentValueIterItem::StartOfFunction(_) => self.build_arguments_content(
                 ArgumentValuesIterator::from_argument_iter_value(operation_item),
             ),
             _ => self.build_argument_content(operation_item),
         }
@@ -273,32 +478,36 @@
             optional_arguments.push(String::from("run_on_client=True"));
         }
         optional_arguments
     }
 }
 
 fn into_operator(string: &str) -> Option<&str> {
-    if ["==", "!=", "<=", "<", ">", ">=", "+", "-", "/", "*", "**"].contains(&string) {
+    if [
+        "==", "!=", "<=", "<", ">", ">=", "+", "-", "/", "*", "%", "**",
+    ]
+    .contains(&string)
+    {
         return Some(string);
     }
     match string.to_lowercase().as_str() {
-        "and" => Some("&"),
-        "or" => Some("|"),
+        "and" => Some("and"),
+        "or" => Some("or"),
         _ => None,
     }
 }
 
 #[cfg(test)]
 mod tests {
     use std::collections::HashMap;
 
     use serde_json::json;
 
     use crate::game_data::{
-        actions::parse_actions,
+        actions::{parse_actions, Action},
         directory::{Directory, DirectoryItem, Script},
         variable_categories::{CategoriesToVariables, Variable},
     };
 
     use super::ScriptsContentBuilder;
 
     #[test]
@@ -312,169 +521,246 @@
                 "initialize",
                 "WI31HDK",
                 vec!["gameStart"],
                 Vec::new()
             )),
             String::from(format!(
                 "@script(triggers=[Trigger.GAME_START])\n\
-                class Initialize():\n\
-                    \tdef _build(self):\n\
-                        \t\tself.actions = [\n\
-                        \t\t\t\n\
-                        \t\t]\n",
+                def initialize():\n\
+                    \tpass\n",
             ))
         );
     }
 
     #[test]
-    fn script_with_weird_name_content() {
+    fn script_with_non_ascii_name_content() {
         assert_eq!(
             ScriptsContentBuilder::new(
                 &CategoriesToVariables::new(HashMap::new()),
                 &Directory::new("root", "null", Vec::new())
             )
             .build_script_content(&Script::new(
                 "【 𝚒𝚗𝚒𝚝𝚒𝚊𝚕𝚒𝚣𝚎 イ】",
                 "WI31HDK",
                 vec!["gameStart"],
                 Vec::new()
             )),
             String::from(format!(
                 "@script(triggers=[Trigger.GAME_START], name='【 𝚒𝚗𝚒𝚝𝚒𝚊𝚕𝚒𝚣𝚎 イ】')\n\
-                class q():\n\
-                    \tdef _build(self):\n\
-                        \t\tself.actions = [\n\
-                        \t\t\t\n\
-                        \t\t]\n",
+                def wi31hdk():\n\
+                    \tpass\n",
+            ))
+        );
+    }
+
+    #[test]
+    fn script_with_no_name() {
+        assert_eq!(
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::new()),
+                &Directory::new("root", "null", Vec::new())
+            )
+            .build_script_content(&Script::new(
+                "",
+                "WI31HDK",
+                vec![],
+                Vec::new()
+            )),
+            String::from(format!(
+                "@script(triggers=[])\n\
+                def wi31hdk():\n\
+                    \tpass\n",
+            ))
+        );
+    }
+
+    #[test]
+    fn script_content_with_commented_body() {
+        assert_eq!(
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::new()),
+                &Directory::new("root", "null", Vec::new())
+            )
+            .build_script_content(&Script::new(
+                "initialize",
+                "WI31HDK",
+                vec!["gameStart"],
+                vec![Action::new("break", vec![], None, false, true)]
+            )),
+            String::from(format!(
+                "@script(triggers=[Trigger.GAME_START])\n\
+                def initialize():\n\
+                    \t# break\n\
+                    \tpass\n",
             ))
         );
     }
 
     #[test]
     fn parse_action_with_variable_into_pymodd() {
         assert_eq!(
             ScriptsContentBuilder::new(
                 &CategoriesToVariables::new(HashMap::from([(
                     "shops",
-                    vec![Variable::new("OJbEQyc7is", "WEAPONS", None)]
+                    vec![Variable::new("OJbEQyc7is", "weapons", json!({}))]
                 )])),
                 &Directory::new("root", "null", Vec::new())
             )
             .build_actions_content(&parse_actions(
                 &json!([
                     {
                         "type": "openShopForPlayer",
                             "player": {
                                 "function": "getOwner",
-                                "entity": {
-                                    "function": "getLastCastingUnit",
-                                    "vars": []
-                                },
+                                "entity": { "function": "getLastCastingUnit", "vars": [] },
                                 "vars": []
                             },
                         "shop": "OJbEQyc7is",
                         "vars": []
                     }
                 ])
                 .as_array()
                 .unwrap()
             )),
-            "open_shop_for_player(Shops.WEAPONS, OwnerOfEntity(LastCastingUnit())),\n"
+            "open_shop_for_player(Shop.WEAPONS, OwnerOfEntity(LastCastingUnit()))\n"
         )
     }
 
     #[test]
     fn parse_action_with_optional_arguments_into_pymodd() {
         assert_eq!(
             ScriptsContentBuilder::new(
                 &CategoriesToVariables::new(HashMap::new()),
                 &Directory::new("root", "null", Vec::new())
             )
             .build_actions_content(&parse_actions(
                 &json!([
                     {
                         "type": "startUsingItem",
-                        "entity": {
-                            "function": "getTriggeringItem"
-                        },
+                        "entity": { "function": "getTriggeringItem" },
                         "comment": "hi!",
                         "runOnClient": true,
                         "disabled": true,
                     }
                 ])
                 .as_array()
                 .unwrap()
             )),
-            "use_item_continuously_until_stopped(LastTriggeringItem(), comment='hi!', disabled=True, run_on_client=True),\n"
+            "use_item_continuously_until_stopped(LastTriggeringItem(), comment='hi!', disabled=True, run_on_client=True)\n"
         )
     }
 
     #[test]
     fn parse_action_with_only_optional_arguments_into_pymodd() {
         assert_eq!(
             ScriptsContentBuilder::new(
                 &CategoriesToVariables::new(HashMap::new()),
                 &Directory::new("root", "null", Vec::new())
             )
             .build_actions_content(&parse_actions(
                 &json!([
-                    {
-                        "type": "return",
-                        "comment": "hi!",
-                        "runOnClient": true,
-                        "disabled": false,
-                    }
+                    { "type": "stopMusic", "comment": "hi!", "runOnClient": true, "disabled": false, }
                 ])
                 .as_array()
                 .unwrap()
             )),
-            "return_loop(comment='hi!', run_on_client=True),\n"
+            "stop_music_for_everyone(comment='hi!', run_on_client=True)\n"
         )
     }
 
     #[test]
     fn parse_action_with_constant_into_pymodd() {
         assert_eq!(
             ScriptsContentBuilder::new(
                 &CategoriesToVariables::new(HashMap::new()),
                 &Directory::new("root", "null", Vec::new())
             )
             .build_actions_content(&parse_actions(
                 &json!([
-                    {
-                        "type": "updateUiTextForEveryone",
-                        "target": "top",
-                        "value": "Hello!"
-                    }
+                    { "type": "updateUiTextForEveryone", "target": "top", "value": "Hello!" }
                 ])
                 .as_array()
                 .unwrap()
             )),
-            "update_ui_text_for_everyone(UiTarget.TOP, 'Hello!'),\n"
+            "update_ui_text_for_everyone(UiTarget.TOP, 'Hello!')\n"
         )
     }
 
     #[test]
+    fn parse_action_with_null_into_pymodd() {
+        assert_eq!(
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::new()),
+                &Directory::new("root", "null", Vec::new())
+            )
+            .build_actions_content(&parse_actions(
+                &json!([
+                    { "type": "updateUiTextForEveryone", "target": "top", "value": null }
+                ])
+                .as_array()
+                .unwrap()
+            )),
+            "update_ui_text_for_everyone(UiTarget.TOP, None)\n"
+        )
+    }
+    #[test]
     fn parse_comment_action_into_pymodd() {
         assert_eq!(
             ScriptsContentBuilder::new(
                 &CategoriesToVariables::new(HashMap::new()),
                 &Directory::new("root", "null", Vec::new())
             )
             .build_actions_content(&parse_actions(
                 &json!([
-                    {
-                        "type": "comment",
-                        "comment": "hey there",
-                    }
+                    { "type": "comment", "comment": "hey there", }
+                ])
+                .as_array()
+                .unwrap()
+            )),
+            "comment('hey there')\n"
+        );
+    }
+
+    #[test]
+    fn parse_keyword_actions_into_pymodd() {
+        assert_eq!(
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::new()),
+                &Directory::new("root", "null", Vec::new())
+            )
+            .build_actions_content(&parse_actions(
+                &json!([ { "type": "break" }, { "type": "continue" }, { "type": "return" } ])
+                    .as_array()
+                    .unwrap()
+            )),
+            "break\n\
+            continue\n\
+            return\n"
+        );
+    }
+
+    #[test]
+    fn parse_disabled_keyword_actions_into_pymodd() {
+        assert_eq!(
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::new()),
+                &Directory::new("root", "null", Vec::new())
+            )
+            .build_actions_content(&parse_actions(
+                &json!([
+                    { "type": "break", "disabled": true },
+                    { "type": "continue", "disabled": true },
+                    { "type": "return", "disabled": true }
                 ])
                 .as_array()
                 .unwrap()
             )),
-            "comment('hey there'),\n"
+            "# break\n\
+            # continue\n\
+            # return\n"
         );
     }
 
     #[test]
     fn parse_nested_calculations_into_pymodd() {
         assert_eq!(
             ScriptsContentBuilder::new(
@@ -483,32 +769,34 @@
             )
                 .build_actions_content(&parse_actions(
                     &json!([
                         {
                             "type": "increaseVariableByNumber",
                             "variable": null,
                             "number": {
-                                "function": "calculate",
+                                "function": "calculate", 
                                 "items": [
-                                    { "operator": "*" },
-                                    { "function": "getRandomNumberBetween", "min": 0, "max": 5 },
-                                    { "function": "calculate", "items": [
-                                            { "operator": "+" },
-                                            { "function": "getExponent", "base": { "function": "currentTimeStamp" }, "power": 2 },
-                                            3
-                                       ]
-                                    }
+                                    { "operator": "%" }, 10, { "function": "calculate", "items": [
+                                            { "operator": "+" }, 5, { "function": "calculate", "items": [
+                                                    { "operator": "-" }, 3, { "function": "calculate", "items": [ 
+                                                            { "operator": "*" }, 3, { "function": "calculate", "items": [ 
+                                                                    { "operator": "/" }, 2,
+                                                                    { "function": "getExponent", "base": 5, "power": 2 }
+                                                            ] }
+                                                        ] }
+                                                ] }
+                                        ] }
                                 ]
                             }
                         }
                     ])
                     .as_array()
                     .unwrap()
                 )),
-            "increase_variable_by_number(None, RandomNumberBetween(0, 5) * ((CurrentUnixTimeStamp() ** 2) + 3)),\n"
+            "increase_variable_by_number(None, 10 % (5 + (3 - (3 * (2 / (5 ** 2))))))\n"
         );
     }
 
     #[test]
     fn parse_nested_concatenations_into_pymodd() {
         assert_eq!(
             ScriptsContentBuilder::new(
@@ -522,135 +810,381 @@
                             "message": {
                                 "function": "concat",
                                 "textA": "hi ",
                                 "textB": {
                                     "function": "concat",
                                     "textA": {
                                         "function": "getPlayerId",
-                                        "player": {
-                                            "function": "getTriggeringPlayer"
-                                        }
+                                        "player": { "function": "getTriggeringPlayer" }
                                     },
                                     "textB": " player!"
                                 }
                             }
                         }
                     ])
                     .as_array()
                     .unwrap()
                 )),
-            "send_chat_message_to_everyone('hi ' + IdOfPlayer(LastTriggeringPlayer()) + ' player!'),\n"
+            "send_chat_message_to_everyone('hi ' + IdOfPlayer(LastTriggeringPlayer()) + ' player!')\n"
         );
     }
 
     #[test]
     fn parse_nested_if_statements_into_pymodd() {
         assert_eq!(
             ScriptsContentBuilder::new(
                 &CategoriesToVariables::new(HashMap::new()),
                 &Directory::new("root", "null", Vec::new())
             )
             .build_actions_content(&parse_actions(
                 json!([
                      {
                         "type": "condition",
-                        "conditions": [
-                            { "operandType": "boolean", "operator": "==" },
-                            true,
-                            true
-                        ],
+                        "conditions": [ { "operandType": "boolean", "operator": "==" }, true, true ],
                         "then": [
                             {
                                 "type": "condition",
-                                "conditions": [
-                                    { "operandType": "boolean", "operator": "==" },
-                                    true,
-                                    true
-                                ],
+                                "conditions": [ { "operandType": "boolean", "operator": "==" }, true, true ],
                                 "then": [
                                     {
                                         "type": "condition",
-                                        "conditions": [
-                                            { "operandType": "boolean", "operator": "==" },
-                                            true,
-                                            true
-                                        ],
-                                        "then": [],
-                                        "else": []
+                                        "conditions": [ { "operandType": "boolean", "operator": "==" }, true, true ],
+                                        "then": [ { "type": "sendChatMessage", "message": "hi" } ],
+                                        "else": [ { "type": "sendChatMessage", "message": "hi" } ]
                                     }
                                 ],
-                                "else": []
-                               }
-                          ],
-                          "else": []
+                                "else": [ { "type": "sendChatMessage", "message": "hi" } ]
+                            }
+                        ],
+                        "else": [ { "type": "sendChatMessage", "message": "hi" } ]
                      }
                 ])
                 .as_array()
                 .unwrap(),
             ))
             .as_str(),
-            "if_else((True == True), [\n\
-                \tif_else((True == True), [\n\
-    		        \t\tif_else((True == True), [\n\
-		                \t\t\t\n\
-		            \t\t], [\n\
-		                \t\t\t\n\
-		            \t\t]),\n\
-                    \t\t\n\
-                \t], [\n\
-                    \t\t\n\
-                \t]),\n\
-                \t\n\
-            ], [\n\
-                \t\n\
-            ]),\n"
+            "if True == True:\n\
+                \tif True == True:\n\
+    		        \t\tif True == True:\n\
+		                \t\t\tsend_chat_message_to_everyone('hi')\n\
+                    \t\telse:\n\
+		                \t\t\tsend_chat_message_to_everyone('hi')\n\
+                \telse:\n\
+		            \t\tsend_chat_message_to_everyone('hi')\n\
+            else:\n\
+                \tsend_chat_message_to_everyone('hi')\n"
         )
     }
 
     #[test]
     fn parse_nested_conditions_into_pymodd() {
         assert_eq!(
             ScriptsContentBuilder::new(
                 &CategoriesToVariables::new(HashMap::new()),
                 &Directory::new("root", "null", Vec::new())
             )
-                .build_actions_content(&parse_actions(
-                    json!([
-                         {
-                            "type": "condition",
-                            "conditions": [
-                                { "operandType": "and", "operator": "AND" },
-                                [
-                                    { "operandType": "boolean", "operator": "==" },
-                                    { "function": "getNumberOfUnitsOfUnitType", "unitType": "oTDQ3jlcMa" },
-                                    5
-                                ],
-                                [
-                                    { "operandType": "boolean", "operator": "==" },
-                                    true,
-                                    true
-                                ]
-                            ],
-                            "then": [],
-                            "else": []
-                         }
-                    ])
-                    .as_array()
-                    .unwrap(),
-                ))
-                .as_str(),
-            "if_else(((NumberOfUnitsOfUnitType('oTDQ3jlcMa') == 5) & (True == True)), [\n\
-                \t\n\
-            ], [\n\
-                \t\n\
-            ]),\n"
+            .build_actions_content(&parse_actions(
+                json!([
+                    {
+                        "type": "condition",
+                        "conditions": [
+                              { "operandType": "and", "operator": "AND" },
+                              [ { "operandType": "boolean", "operator": "==" }, true, true ],
+                              [
+                                   { "operandType": "or", "operator": "OR" },
+                                   [ { "operandType": "boolean", "operator": "==" }, true, true ],
+                                   [ { "operandType": "boolean", "operator": "==" }, true, true ]
+                              ]
+                         ],
+                         "then": [],
+                         "else": []
+                }])
+                .as_array()
+                .unwrap(),
+            ))
+            .as_str(),
+            "if True == True and (True == True or True == True):\n\
+                \tpass\n"
         );
     }
 
     #[test]
+    fn parse_variable_for_loop_into_pymodd() {
+        assert_eq!(
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::from([(
+                    "variables",
+                    vec![Variable::new("i", "i", json!({"dataType": "number"}))]
+                )])),
+                &Directory::new("root", "null", Vec::new())
+            )
+            .build_actions_content(&parse_actions(
+                json!([
+                    { "type": "for", "variableName": "i", "start": 0, "stop": 5, "actions": [] }
+                ])
+                .as_array()
+                .unwrap(),
+            ))
+            .as_str(),
+            "for Variable.I in range(0, 5):\n\
+                \tpass\n"
+        );
+    }
+
+    #[test]
+    fn parse_for_each_type_in_function_action_into_pymodd() {
+        assert_eq!(
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::new()),
+                &Directory::new("root", "null", Vec::new())
+            )
+            .build_actions_content(&parse_actions(
+                json!([
+                    { "type": "forAllEntities", "entityGroup": { "function": "allEntities" }, "actions": [
+                        { "type": "destroyEntity", "entity": { "function": "getSelectedEntity" } }
+                    ] }
+                ])
+                .as_array()
+                .unwrap(),
+            ))
+            .as_str(),
+            "for entity in AllEntitiesInTheGame():\n\
+                \tdestroy_entity(entity)\n"
+        );
+    }
+
+    #[test]
+    fn parse_for_each_type_in_variable_action_into_pymodd() {
+        assert_eq!(
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::from([(
+                    "itemTypeGroups",
+                    vec![Variable::new("specialItemTypes", "specialItemTypes", json![{}])]
+                )])),
+                &Directory::new("root", "null", Vec::new())
+            )
+            .build_actions_content(&parse_actions(
+                json!([
+                    {
+                        "type": "forAllItemTypes",
+                        "itemTypeGroup": { "function": "getVariable", "variableName": "specialItemTypes" },
+                        "actions": []
+                     }
+                ])
+                .as_array()
+                .unwrap(),
+            ))
+            .as_str(),
+            "for item_type in ItemTypeGroup.SPECIAL_ITEM_TYPES:\n\
+                \tpass\n"
+        );
+    }
+
+    #[test]
+    fn parse_for_each_type_in_multi_arg_function_action_into_pymodd() {
+        assert_eq!(
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::new()),
+                &Directory::new("root", "null", Vec::new())
+            )
+            .build_actions_content(&parse_actions(
+                json!([
+                    {
+                        "type": "forAllUnits",
+                        "unitGroup": { "function": "allUnitsInRegion", "region": {
+                                "function": "dynamicRegion",
+                                "x": 0, "y": 0, "width": 5, "height": 5 }
+                        },
+                        "actions": []
+                    }
+                ])
+                .as_array()
+                .unwrap(),
+            ))
+            .as_str(),
+            "for unit in AllUnitsInRegion(DynamicRegion(0, 0, 5, 5)):\n\
+                \tpass\n"
+        );
+    }
+
+    #[test]
+    fn parse_repeat_action_into_python() {
+        assert_eq!(
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::new()),
+                &Directory::new("root", "null", Vec::new())
+            )
+            .build_actions_content(&parse_actions(
+                json!([
+                    { "type": "repeat", "count": 5, "actions": [] }
+                ])
+                .as_array()
+                .unwrap(),
+            ))
+            .as_str(),
+            "for _ in repeat(5):\n\
+                \tpass\n"
+        );
+    }
+
+    #[test]
+    fn parse_while_action_into_python() {
+        assert_eq!(
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::new()),
+                &Directory::new("root", "null", Vec::new())
+            )
+            .build_actions_content(&parse_actions(
+                json!([
+                    {
+                        "type": "while",
+                        "conditions": [
+                            { "operandType": "boolean", "operator": "==" },
+                            { "function": "entityExists", "entity": { "function": "getTriggeringUnit" } },
+                            true
+                        ],
+                        "actions": []
+                    }
+                ])
+                .as_array()
+                .unwrap(),
+            ))
+            .as_str(),
+            "while EntityExists(LastTriggeringUnit()) == True:\n\
+                \tpass\n"
+        );
+    }
+
+    #[test]
+    fn parse_set_timeout_action_into_python() {
+        assert_eq!(
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::new()),
+                &Directory::new("root", "null", Vec::new())
+            )
+            .build_actions_content(&parse_actions(
+                json!([
+                    { "type": "setTimeOut", "duration": 1000, "actions": [ { "type": "stopMusic" } ] } 
+                ])
+                .as_array()
+                .unwrap(),
+            ))
+            .as_str(),
+            "with after_timeout(1000):\n\
+                \tstop_music_for_everyone()\n"
+        );
+    }
+
+    #[test]
+    fn parse_disabled_while_action_into_python() {
+        assert_eq!(
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::new()),
+                &Directory::new("root", "null", Vec::new())
+            )
+            .build_actions_content(&parse_actions(
+                json!([
+                    {
+                        "type": "while", "conditions": [ { "operandType": "boolean", "operator": "==" }, true, true ], "actions": [],
+                        "disabled": true
+                    }
+                ])
+                .as_array()
+                .unwrap(),
+            ))
+            .as_str(),
+            "# while True == True:\n\
+                # \tpass\n"
+        );
+    }
+
+    #[test]
+    fn parse_while_action_with_disabled_actions_into_python() {
+        assert_eq!(
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::new()),
+                &Directory::new("root", "null", Vec::new())
+            )
+            .build_actions_content(&parse_actions(
+                json!([
+                    {
+                        "type": "while", 
+                        "conditions": [ { "operandType": "boolean", "operator": "==" }, true, true ], 
+                        "actions": [
+                            {
+                                "type": "while", "conditions": [ { "operandType": "boolean", "operator": "==" }, true, true ], "actions": [],
+                                "disabled": true
+                            }
+                        ],
+                    }
+                ])
+                .as_array()
+                .unwrap(),
+            ))
+            .as_str(),
+            "while True == True:\n\
+                \t# while True == True:\n\
+                \t# \tpass\n\
+                \tpass\n"
+        );
+    }
+
+    #[test]
+    fn parse_nested_disabled_if_statements_into_pymodd() {
+        assert_eq!(
+            ScriptsContentBuilder::new(
+                &CategoriesToVariables::new(HashMap::new()),
+                &Directory::new("root", "null", Vec::new())
+            )
+            .build_actions_content(&parse_actions(
+                json!([
+                     {
+                        "type": "condition", "conditions": [ { "operandType": "boolean", "operator": "==" }, true, true ],
+                        "then": [ {
+                                "type": "condition", "conditions": [ { "operandType": "boolean", "operator": "==" }, true, true ],
+                                "then": [ {
+                                        "type": "condition", "conditions": [ { "operandType": "boolean", "operator": "==" }, true, true ],
+                                        "then": [ { "type": "sendChatMessage", "message": "hi" } ],
+                                        "else": [ { "type": "sendChatMessage", "message": "hi" } ],
+                                        "disabled": true
+                                    } ],
+                                "else": [ { "type": "sendChatMessage", "message": "hi" } ],
+                                "disabled": true
+                            } ],
+                        "else": [ {
+                                "type": "condition", "conditions": [ { "operandType": "boolean", "operator": "==" }, true, true ],
+                                "then": [ { "type": "sendChatMessage", "message": "hi" } ],
+                                "else": [ { "type": "sendChatMessage", "message": "hi" } ],
+                                "disabled": true
+                            } ]
+                     }
+                ])
+                .as_array()
+                .unwrap(),
+            ))
+            .as_str(),
+            "if True == True:\n\
+                \t# if True == True:\n\
+    		        \t# \tif True == True:\n\
+		                \t# \t\tsend_chat_message_to_everyone('hi')\n\
+                    \t# \telse:\n\
+		                \t# \t\tsend_chat_message_to_everyone('hi')\n\
+                \t# else:\n\
+		            \t# \tsend_chat_message_to_everyone('hi')\n\
+                \tpass\n\
+            else:\n\
+                \t# if True == True:\n\
+                    \t# \tsend_chat_message_to_everyone('hi')\n\
+                \t# else:\n\
+                    \t# \tsend_chat_message_to_everyone('hi')\n\
+                \tpass\n"
+        )
+    }
+
+    #[test]
     fn parse_run_script_action_into_pymodd() {
         assert_eq!(
             ScriptsContentBuilder::new(
                 &CategoriesToVariables::new(HashMap::new()),
                 &Directory::new(
                     "root",
                     "null",
@@ -664,20 +1198,17 @@
                             actions: Vec::new()
                         })]
                     ))]
                 )
             )
             .build_actions_content(&parse_actions(
                 json!([
-                     {
-                        "type": "runScript",
-                        "scriptName": "If2aW3B"
-                     }
+                     { "type": "runScript", "scriptName": "If2aW3B" }
                 ])
                 .as_array()
                 .unwrap(),
             ))
             .as_str(),
-            "run_script(SpawnBoss()),\n"
+            "run_script(spawn_boss())\n"
         )
     }
 }
```

### Comparing `pymodd-0.3.0/src/project_generator/utils/iterators/argument_values_iterator.rs` & `pymodd-1.0.0/src/project_generator/utils/iterators/argument_values_iterator.rs`

 * *Files 1% similar despite different names*

```diff
@@ -3,27 +3,26 @@
 use crate::game_data::{
     actions::Action,
     argument::{Argument, ArgumentValue, Function},
 };
 
 impl Action {
     pub fn iter_flattened_argument_values(&self) -> ArgumentValuesIterator {
-        ArgumentValuesIterator::new(self)
+        ArgumentValuesIterator::new(&self.args)
     }
 }
 
 pub struct ArgumentValuesIterator<'a> {
     stack: Vec<ArgumentValueIterItem<'a>>,
 }
 
 impl<'a> ArgumentValuesIterator<'a> {
-    fn new(action: &Action) -> ArgumentValuesIterator {
+    pub fn new(arguments: &Vec<Argument>) -> ArgumentValuesIterator {
         ArgumentValuesIterator {
-            stack: action
-                .args
+            stack: arguments
                 .iter()
                 .map(|arg| ArgumentValueIterItem::from_argument(arg))
                 .collect(),
         }
     }
 
     pub fn from_argument_iter_value(argument: ArgumentValueIterItem) -> ArgumentValuesIterator {
@@ -64,25 +63,27 @@
     Actions(&'a Vec<Action>),
     Value(&'a Value),
     Constant(&'a String),
     Condition(Operation),
     Concatenation(Operation),
     Calculation(Operation),
     ScriptKey(String),
+    None,
     FunctionEnd,
 }
 
 impl<'a> ArgumentValueIterItem<'a> {
     pub fn from_argument(argument: &Argument) -> ArgumentValueIterItem {
         match &argument.value {
             ArgumentValue::Function(function) => {
                 match (function.name.as_str(), Operation::from_function(function)) {
                     ("condition", Some(operation)) => ArgumentValueIterItem::Condition(operation),
                     ("concat", Some(operation)) => ArgumentValueIterItem::Concatenation(operation),
                     (_, Some(operation)) => ArgumentValueIterItem::Calculation(operation),
+                    ("null", _) => ArgumentValueIterItem::None,
                     _ => ArgumentValueIterItem::StartOfFunction(&function),
                 }
             }
             ArgumentValue::Constant(constant) => ArgumentValueIterItem::Constant(&constant),
             ArgumentValue::Value(value) => {
                 if value.is_string() && argument.name.as_str() == "scriptName" {
                     ArgumentValueIterItem::ScriptKey(value.as_str().unwrap().to_string())
```

### Comparing `pymodd-0.3.0/src/project_generator/utils/iterators/directory_iterator.rs` & `pymodd-1.0.0/src/project_generator/utils/iterators/directory_iterator.rs`

 * *Files identical despite different names*

### Comparing `pymodd-0.3.0/src/project_generator/utils/to_pymodd_maps.rs` & `pymodd-1.0.0/src/project_generator/utils/to_pymodd_maps.rs`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,24 @@
 
 use std::collections::HashMap;
 
 use lazy_static::lazy_static;
 
 // pymodd files
 const PYMODD_SCRIPT_FILE_CONTENT: &str = include_str!("../../../pymodd/script.py");
+const PYMODD_ENTITY_SCRIPT_FILE_CONTENT: &str = include_str!("../../../pymodd/entity_script.py");
 const PYMODD_ACTIONS_FILE_CONTENT: &str = include_str!("../../../pymodd/actions.py");
 const PYMODD_FUNCTIONS_FILE_CONTENT: &str = include_str!("../../../pymodd/functions.py");
+const PYMODD_VARIABLE_TYPES_FILE_CONTENT: &str = include_str!("../../../pymodd/variable_types.py");
 
 lazy_static! {
     // enum maps
     pub static ref TRIGGERS_TO_PYMODD_ENUM: HashMap<String, String> = generate_to_pymodd_enums_map_for_type("Trigger", PYMODD_SCRIPT_FILE_CONTENT);
+    pub static ref VARIABLE_DATA_TYPES_TO_PYMODD_ENUM: HashMap<String, String> = generate_to_pymodd_enums_map_for_type("DataType", PYMODD_VARIABLE_TYPES_FILE_CONTENT);
+    pub static ref KEYS_TO_PYMODD_ENUM: HashMap<String, String> = generate_to_pymodd_enums_map_for_type("Key", PYMODD_ENTITY_SCRIPT_FILE_CONTENT);
     pub static ref UI_TARGET_CONSTANTS_TO_PYMODD_ENUM:HashMap<String, String> = generate_to_pymodd_enums_map_for_type("UiTarget", PYMODD_SCRIPT_FILE_CONTENT);
     pub static ref FLIP_CONSTANTS_TO_PYMODD_ENUM:HashMap<String, String> = generate_to_pymodd_enums_map_for_type("Flip", PYMODD_SCRIPT_FILE_CONTENT);
 
     // action/function maps
     pub static ref ACTIONS_TO_PYMODD_STRUCTURE: HashMap<String, PymoddStructure> = generate_actions_to_pymodd_structure_map();
     pub static ref FUNCTIONS_TO_PYMODD_STRUCTURE: HashMap<String, PymoddStructure> = generate_functions_to_pymodd_structure_map();
 }
@@ -43,15 +47,15 @@
 
 // CONSTANTS
 fn generate_to_pymodd_enums_map_for_type(
     type_name: &str,
     file_content: &str,
 ) -> HashMap<String, String> {
     let mut modd_names_to_pymodd_enums: HashMap<String, String> = HashMap::new();
-    parse_class_content_from_file(type_name, file_content)
+    parse_enum_class_content_from_file(type_name, file_content)
         .lines()
         .for_each(|line| match line.split_once("=") {
             Some((enum_name, modd_name)) => {
                 modd_names_to_pymodd_enums.insert(
                     strip_quotes(modd_name),
                     strip_quotes(&format!("{type_name}.{}", enum_name.trim())),
                 );
@@ -65,18 +69,21 @@
 fn generate_actions_to_pymodd_structure_map() -> HashMap<String, PymoddStructure> {
     let mut actions_to_structure: HashMap<String, PymoddStructure> = HashMap::new();
     let action_functions: Vec<&str> = PYMODD_ACTIONS_FILE_CONTENT
         .split("\n\n\n")
         .skip(3)
         .collect();
     action_functions.into_iter().for_each(|function_content| {
-        actions_to_structure.insert(
-            parse_action_name_of_pymodd_action_function(&function_content),
-            parse_pymodd_structure_of_pymodd_action_function(&function_content),
-        );
+        // skip over divider comments
+        if !function_content.starts_with("# ------") {
+            actions_to_structure.insert(
+                parse_action_name_of_pymodd_action_function(&function_content),
+                parse_pymodd_structure_of_pymodd_action_function(&function_content),
+            );
+        }
     });
     actions_to_structure
 }
 
 fn parse_action_name_of_pymodd_action_function(action_function_content: &str) -> String {
     strip_quotes(
         &action_function_content
@@ -191,18 +198,18 @@
         .expect("class line could not be found")
         .split([' ', '('])
         .nth(1)
         .expect("class name could not be parsed")
         .to_string()
 }
 
-fn parse_class_content_from_file(class_name: &str, file_content: &str) -> String {
+fn parse_enum_class_content_from_file(class_name: &str, file_content: &str) -> String {
     file_content
         .lines()
-        .skip_while(|line| !line.starts_with(&format!("class {class_name}")))
+        .skip_while(|line| !line.starts_with(&format!("class {class_name}(Enum):")))
         .skip(1)
         .take_while(|line| !line.starts_with("class"))
         .map(|line| format!("{line}\n"))
         .collect::<String>()
 }
 
 fn strip_quotes(string: &str) -> String {
```

### Comparing `pymodd-0.3.0/src/project_generator/utils.rs` & `pymodd-1.0.0/src/project_generator/utils.rs`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 use heck::{ToLowerCamelCase, ToShoutySnakeCase};
 
 use crate::game_data::variable_categories::{
     SEPERATED_VARIABLE_CATEGORIES, VARIABLES_CATEGORY_NAME, VARIABLE_CATEGORIES,
 };
 
+pub(crate) const TAB_SIZE: usize = 4;
+
 pub(crate) fn is_valid_class_name(class_name: &str) -> bool {
     !(class_name.is_empty()
         || string_starts_with_a_number(&class_name)
         || type_conflicts_with_a_category_class_name(&class_name))
 }
 
 fn string_starts_with_a_number(string: &str) -> bool {
@@ -37,15 +39,25 @@
     } else if string.contains('\'') {
         return "\"";
     }
     "'"
 }
 
 pub(crate) fn enum_name_of(name: &str) -> String {
-    name.to_shouty_snake_case()
+    let enum_name: String = name.to_shouty_snake_case();
+    if enum_name
+        .chars()
+        .next()
+        .map(|c| c.is_ascii_digit())
+        .unwrap_or(true)
+    {
+        format!("_{enum_name}")
+    } else {
+        enum_name
+    }
 }
 
 #[cfg(test)]
 mod tests {
     use crate::project_generator::utils::{is_valid_class_name, surrounding_quote_for_string};
 
     #[test]
```

### Comparing `pymodd-0.3.0/src/project_generator.rs` & `pymodd-1.0.0/src/project_generator.rs`

 * *Files 3% similar despite different names*

```diff
@@ -50,18 +50,20 @@
             // insert project directory as parent to all file paths
             path: PathBuf::from(game_data.pymodd_project_name()).join(file.path),
             content: file.content,
         }) {
             // unwrap is fine as all files have the project directory as parent
             let parent = file.path.parent().unwrap();
             if !parent.exists() {
-                fs::create_dir_all(parent).map_err(|_| "error creating a pymodd project directories!")?;
+                fs::create_dir_all(parent)
+                    .map_err(|_| "error creating a pymodd project directories!")?;
             }
             write!(
-                fs::File::create(&file.path).map_err(|_| "error creating a pymodd project file!")?,
+                fs::File::create(&file.path)
+                    .map_err(|_| "error creating a pymodd project file!")?,
                 "{}",
                 file.content
             )
             .map_err(|_| "error writing to a pymodd project file!")?;
             generation_logger(file);
         }
         Ok(())
```

### Comparing `pymodd-0.3.0/Cargo.lock` & `pymodd-1.0.0/Cargo.lock`

 * *Files identical despite different names*

### Comparing `pymodd-0.3.0/PKG-INFO` & `pymodd-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodd
-Version: 0.3.0
+Version: 1.0.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: case-converter==1.1.0
 License-File: LICENSE.txt
 Summary: A package for creating modd.io games using python!
 Author: Jeff
@@ -16,75 +16,56 @@
 
 ======
 pymodd
 ======
 
 |Build| |Version| |License|
 
-pymodd is a python package used for creating modd.io games in python
+pymodd is a python package for creating and editing modd.io games in python
 
 .. |Build| image:: https://img.shields.io/github/actions/workflow/status/jeff5343/pymodd/CI.yml?label=CI&logo=github&style=plastic
    :alt: GitHub Workflow Status
 .. |Version| image:: https://img.shields.io/pypi/v/pymodd?style=plastic
    :alt: PyPI
 .. |License| image:: https://img.shields.io/pypi/l/pymodd?style=plastic
    :alt: PyPI - License
 
 Features
 --------
 
 - edit global and entity scripts
 - organize folders and scripts with a mapping file
+- edit environment variables
 - a command to generate and compile a pymodd project
 
-Installing
-----------
+Documentation
+-------------
 
-**Python 3.8 or higher is required**
+The pymodd wiki is located at `github.com/jeff5343/pymodd/wiki <https://github.com/jeff5343/pymodd/wiki>`_
 
-To install the library run the following command:
+A brief outline of the wiki:
 
-.. code:: sh
-
-    # Linux/macOS
-    python3 -m pip install -U pymodd
-
-    # Windows
-    py -3 -m pip install -U pymodd
-
-
-Getting Started
----------------
-
-Export your modd game json file from the website and then generate a pymodd project by running the following command:
-
-.. code:: sh
-
-    pymodd generate-project [GAME_JSON_FILE_PATH]
+- `Introduction <https://github.com/jeff5343/pymodd/wiki>`_
+- `Install Guide <https://github.com/jeff5343/pymodd/wiki/Install-Guide>`_
+- `Generating and Compiling a Pymodd Project <https://github.com/jeff5343/pymodd/wiki/Generating-and-Compiling-a-Pymodd-Project>`_
+- `Pymodd Project Structure <https://github.com/jeff5343/pymodd/wiki/Pymodd-Project-Structure>`_
 
 
 Quick Script Example
 --------------------
 
-view the ``examples/froge directory`` for a generated pymodd project
+view the ``examples/froge`` directory for an example of a pymodd project
 
 .. code:: py
 
     @script(triggers=[Trigger.EVERY_SECOND])
-    class EverySecond():
-        def _build(self):
-            self.actions = [
-                if_else((NumberOfUnitsOfUnitType(UnitTypes.FROG) < 5), [
-                    create_unit_for_player_at_position_with_rotation(UnitTypes.FROG, Variables.AI, RandomPositionInRegion(EntireMapRegion()), 0),
-                ], [
-                    if_else((NumberOfUnitsOfUnitType(UnitTypes.FROG_BOSS) == 0), [
-                        if_else((Variables.BOSS_TIMER <= 0), [
-                            create_unit_for_player_at_position_with_rotation(UnitTypes.FROG_BOSS, Variables.AI, RandomPositionInRegion(EntireMapRegion()), 0),
-                            update_ui_target_for_player_for_miliseconds(UiTarget.CENTER, 'BOSS SPAWNED', Undefined(), 5000),
-                            set_variable(Variables.BOSS_TIMER, 200),
-                        ], [
-                        ]),
-                        decrease_variable_by_number(Variables.BOSS_TIMER, 1),
-                    ], [
-                    ]),
-                ]),
-            ]
+    def every_second():
+        if NumberOfUnitsOfUnitType(UnitType.FROG) < 5:
+            create_unit_for_player_at_position_with_rotation(UnitType.FROG, Variable.AI, RandomPositionInRegion(EntireMapRegion()), 0)
+        else:
+            if NumberOfUnitsOfUnitType(UnitType.FROG_BOSS) == 0:
+                if Variable.BOSS_TIMER <= 0:
+                    create_unit_for_player_at_position_with_rotation(UnitType.FROG_BOSS, Variable.AI, RandomPositionInRegion(EntireMapRegion()), 0)
+                    update_ui_target_for_player_for_miliseconds(UiTarget.CENTER, 'BOSS SPAWNED', Undefined(), 5000)
+                decrease_variable_by_number(Variable.BOSS_TIMER, 1)
+
+
```

