# Comparing `tmp/malmoext-0.36.0.0.1-py3-none-any.whl.zip` & `tmp/malmoext-0.36.0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 21761 bytes, number of entries: 14
--rw-r--r--  2.0 unx      430 b- defN 24-May-27 22:22 malmoext/__init__.py
--rw-r--r--  2.0 unx      667 b- defN 24-May-27 22:22 malmoext/__main__.py
--rw-r--r--  2.0 unx    10106 b- defN 24-May-27 22:22 malmoext/agent.py
--rw-r--r--  2.0 unx     8850 b- defN 24-May-27 22:22 malmoext/agent_state.py
--rw-r--r--  2.0 unx     1613 b- defN 24-May-27 22:22 malmoext/malmo_bootstrap.py
--rw-r--r--  2.0 unx     8729 b- defN 24-May-27 22:22 malmoext/scenario.py
--rw-r--r--  2.0 unx    11890 b- defN 24-May-27 22:22 malmoext/scenario_builder.py
--rw-r--r--  2.0 unx    20587 b- defN 24-May-27 22:22 malmoext/types.py
--rw-r--r--  2.0 unx     2598 b- defN 24-May-27 22:22 malmoext/utils.py
--rw-r--r--  2.0 unx     1070 b- defN 24-May-27 22:23 malmoext-0.36.0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      550 b- defN 24-May-27 22:23 malmoext-0.36.0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-27 22:23 malmoext-0.36.0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-May-27 22:23 malmoext-0.36.0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1117 b- defN 24-May-27 22:23 malmoext-0.36.0.0.1.dist-info/RECORD
-14 files, 68308 bytes uncompressed, 19919 bytes compressed:  70.8%
+Zip file size: 22293 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      430 b- defN 24-May-31 18:08 malmoext/__init__.py
+-rw-r--r--  2.0 unx      667 b- defN 24-May-31 18:08 malmoext/__main__.py
+-rw-r--r--  2.0 unx    12031 b- defN 24-May-31 18:08 malmoext/agent.py
+-rw-r--r--  2.0 unx     8850 b- defN 24-May-31 18:08 malmoext/agent_state.py
+-rw-r--r--  2.0 unx     1613 b- defN 24-May-31 18:08 malmoext/malmo_bootstrap.py
+-rw-r--r--  2.0 unx     8848 b- defN 24-May-31 18:08 malmoext/scenario.py
+-rw-r--r--  2.0 unx    11890 b- defN 24-May-31 18:08 malmoext/scenario_builder.py
+-rw-r--r--  2.0 unx    20587 b- defN 24-May-31 18:08 malmoext/types.py
+-rw-r--r--  2.0 unx     2598 b- defN 24-May-31 18:08 malmoext/utils.py
+-rw-r--r--  2.0 unx     1070 b- defN 24-May-31 18:08 malmoext-0.36.0.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      550 b- defN 24-May-31 18:08 malmoext-0.36.0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-31 18:08 malmoext-0.36.0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-May-31 18:08 malmoext-0.36.0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1117 b- defN 24-May-31 18:08 malmoext-0.36.0.0.2.dist-info/RECORD
+14 files, 70352 bytes uncompressed, 20451 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: malmoext/types.py
 Comment: 
 
 Filename: malmoext/utils.py
 Comment: 
 
-Filename: malmoext-0.36.0.0.1.dist-info/LICENSE
+Filename: malmoext-0.36.0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: malmoext-0.36.0.0.1.dist-info/METADATA
+Filename: malmoext-0.36.0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: malmoext-0.36.0.0.1.dist-info/WHEEL
+Filename: malmoext-0.36.0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: malmoext-0.36.0.0.1.dist-info/top_level.txt
+Filename: malmoext-0.36.0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: malmoext-0.36.0.0.1.dist-info/RECORD
+Filename: malmoext-0.36.0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## malmoext/agent.py

```diff
@@ -1,22 +1,26 @@
 import malmo.MalmoPython as MalmoPython
 from typing import Union
 from malmoext.scenario_builder import AgentBuilder
-from malmoext.types import Item, Inventory, Entity, Vector, Rotation
+from malmoext.types import Mob, Item, Inventory, Entity, Vector, Rotation
 from malmoext.utils import Utils
+from enum import Enum
 import math
 
 class Agent:
     '''An Agent wraps a client connection to a Malmo Minecraft instance, and represents a
     player agent in a scenario. The various methods of this class represent the different
     agent actions that can be performed.
     
     Instances of this class should not be constructed directly. Instead, they will be
     automatically constructed when a scenario is ran.'''
 
+    ATTACK_KEEP_DISTANCE = 3
+    '''Distance tolerance (in number of blocks) when attacking an entity'''
+
 
     def __init__(self, builder: AgentBuilder):
         '''Constructor'''
         self.__name = builder.get_name()
         self.__observable_distances = builder.get_observable_distances()
         self.__host = MalmoPython.AgentHost()
         self.state = None   # type: AgentState
@@ -52,14 +56,22 @@
         if self.__host.peekWorldState().number_of_observations_since_last_state > 0:
             self.state = AgentState(self)
             return True
 
         return False
 
 
+    def do_nothing(self):
+        '''Halts all movement and ongoing actions for this agent.'''
+        self.__host.sendCommand('turn 0')
+        self.__host.sendCommand('pitch 0')
+        self.__host.sendCommand('strafe 0')
+        self.__host.sendCommand('move 0')
+
+
     def equip(self, item_type: Item) -> bool:
         '''Equips an item from this agent's inventory. If the item does not already exist in the agent's hotbar,
         it will be swapped with an item from the hotbar. Returns true if successful. Returns false otherwise.'''
         
         inventory_item = self.state.get_inventory_item(item_type)
         if inventory_item is None:
             return False
@@ -80,65 +92,59 @@
 
         # Equip (Malmo keys are 1-indexed)
         self.__host.sendCommand('hotbar.{} 1'.format(target_index + 1))
         self.__host.sendCommand('hotbar.{} 0'.format(target_index + 1))
         return True
 
 
-    def look_at(self, entity: Union[str, Entity]):
+    def look_at(self, entity: Union[str, Mob, Entity]):
         '''Initiates camera movement of this agent's POV to face another entity, specified either by name or by reference.
         If multiple entities exist with the given name, the closest one will be targeted.
         
         Because this transition does not occur instantaneously, this method is intended to be called repeatedly as part
         of the simulation loop.
         
         Returns true if the agent is currently facing the entity (and thus no further camera change will occur). Returns
         false if the agent is not yet facing the entity, or an entity with the given name does not exist.'''
 
-        target = entity
-        if isinstance(target, str):
-            target = self.state.get_entity_by_name(target)
+        target = self.__resolve_entity(entity)
         if target is None:
             return False
         
         turn_rates = self.__compute_turn_rates(target.position)
-        is_looking_at = True
 
         # Modify yaw rate
         if Utils.equal_tol(turn_rates.yaw, 0, 0.001):
             self.__host.sendCommand('turn 0')
         else:
             self.__host.sendCommand('turn {}'.format(turn_rates.yaw))
-            is_looking_at = False
     
         # Modify pitch rate
         if Utils.equal_tol(turn_rates.pitch, 0, 0.001):
             self.__host.sendCommand('pitch 0')
         else:
             self.__host.sendCommand('pitch {}'.format(turn_rates.pitch))
-            is_looking_at = False
 
-        return is_looking_at
+        # Use a slightly higher tolerance for reporting success
+        return Utils.equal_tol(turn_rates.yaw, 0, 0.05) and Utils.equal_tol(turn_rates.pitch, 0, 0.05)
     
 
-    def move_to(self, entity: Union[str, Entity], keep_distance = 2):
+    def move_to(self, entity: Union[str, Mob, Entity], keep_distance = 2):
         '''Initiates movement of this agent to another entity, specified either by name or by reference. If multiple
         entities exist with the given name, the closest one will be targeted. Optionally specify a number of blocks the
         agent should keep away from the target (defaults to 2, since two entities cannot occupy the same block). This
         can be useful in cases where the agent plans to attack or give an item to the target.
         
         Because this transition does not occur instantaneously, this method is inteded to be called repeatedly as part
         of the simulation loop.
         
         Returns true if the agent is currently at the entity (with a tolerance of 2 blocks, given that two entities cannot
         always occupy the same block). Returns false otherwise.'''
 
-        target = entity
-        if isinstance(target, str):
-            target = self.state.get_entity_by_name(target)
+        target = self.__resolve_entity(entity)
         if target is None:
             return False
         
         move_rates = self.__compute_move_rates(target.position, keep_distance)
         is_at = True
 
         # Modify left/right movement rate
@@ -152,15 +158,54 @@
         if Utils.equal_tol(move_rates.z, 0, 0.001):
             self.__host.sendCommand('move 0')
         else:
             self.__host.sendCommand('move {}'.format(move_rates.z))
             is_at = False
 
         return is_at
+    
+
+    def attack(self, entity: Union[str, Mob, Entity]):
+        '''Initiates an attack against another entity, specified either by name or by reference. If multiple entities
+        exist with the given name, the closest one will be targeted. The attack will be performed using the currently-equipped
+        item.
         
+        If the agent is not currently looking or located at the target, this method will default to performing those actions
+        first.
+        
+        Returns true if the attack was performed successfully. Returns false otherwise.'''
+
+        target = self.__resolve_entity(entity)
+        if target is None:
+            return False
+        
+        # Ensure we are first looking and located at the entity
+        looking_at = self.look_at(entity)
+        located_at = self.move_to(entity, Agent.ATTACK_KEEP_DISTANCE)
+        if not looking_at or not located_at:
+            return False
+        
+        # Perform the attack
+        self.__host.sendCommand('attack 1')
+        self.__host.sendCommand('attack 0')
+        return True
+        
+
+    def __resolve_entity(self, entity: Union[str, Entity]):
+        '''If given the name of an entity, this method will return the closest entity to the agent containing that name (or None if
+        no entity with that name could be located). If given an entity reference, this method will return that reference as-is.'''
+        
+        target = entity
+        if isinstance(target, Enum):
+            target = target.value
+        if isinstance(target, str):
+            target = self.state.get_entity_by_name(target)
+
+        return target
+
     
     def __compute_turn_rates(self, target_position: Vector):
         '''Calculates proposed yaw and pitch angle rotations for the camera, in order to face the given position.'''
 
         # Compute signed angle differences
         angle_diffs = self.__compute_angle_diffs(target_position)
         yaw_turn_direction = 1 if angle_diffs.yaw >= 0 else -1
```

## malmoext/scenario.py

```diff
@@ -116,28 +116,25 @@
         # Wait for mission to start
         self.__wait_for_mission_start()
 
         # While mission is running, repeatedly synchronize the local state with the remote server state,
         # and execute agent actions (assume the time limit is the same across all agents)
         while (agentZero.is_mission_active()):
 
-            # Avoid handing off control while we are still waiting to receive observations for agents
-            all_agents_have_observations = True
-            for agent in self.__agents.values():
-                num_observations = agent.get_host().peekWorldState().number_of_observations_since_last_state
-                all_agents_have_observations = all_agents_have_observations and num_observations > 0
-            if not all_agents_have_observations:
+            # Avoid handing off control while we are still waiting to receive observations for one or more agents
+            if not self.__all_agents_have_observations():
                 continue
 
             # Sync agent states
             for agent in self.__agents.values():
                 agent.sync()
 
             # Call handler to perform agent actions
             self.on_tick(self.__agents)
+
             time.sleep(0.05)
 
         print('Mission has ended.')
 
 
     def __start_host_mission(self, agent, mission, client_pool, recording, role, experimentId) -> None:
         '''Attempts to start a mission for an agent host. Will automatically retry on failure. After multiple,
@@ -172,14 +169,15 @@
                     print("Waiting will not help here - bailing immediately.")
                     exit(1)
             if used_attempts == max_attempts:
                 print("All chances used up - bailing now.")
                 exit(1)
         print("startMission called okay.")
 
+
     def __wait_for_mission_start(self) -> None:
         '''This method will block execution until all given hosts have succesfully started their mission. If any host
         fails to begin their mission, a timeout error will occur and the program will exit.'''
         print("Waiting for the mission to start", end=' ')
         agents = self.__agents.values()
         start_flags = [False for a in agents]
         start_time = time.time()
@@ -196,8 +194,18 @@
                 exit(1)
             time.sleep(0.1)
             print(".", end=' ')
         print()
         if time.time() - start_time >= time_out:
             print("Timed out waiting for mission to begin. Bailing.")
             exit(1)
-        print("Mission has started.")
+        print("Mission has started.")
+
+
+    def __all_agents_have_observations(self):
+        '''Returns true if all agents have a received a new observation from the server. Returns false otherwise.'''
+
+        for agent in self.__agents.values():
+            num_observations = agent.get_host().peekWorldState().number_of_observations_since_last_state
+            if num_observations == 0:
+                return False
+        return True
```

## Comparing `malmoext-0.36.0.0.1.dist-info/LICENSE` & `malmoext-0.36.0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `malmoext-0.36.0.0.1.dist-info/METADATA` & `malmoext-0.36.0.0.2.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malmoext
-Version: 0.36.0.0.1
+Version: 0.36.0.0.2
 Summary: A wrapper for Microsoft's Malmo Platform capable of creating automated agent action sequences in Minecraft.
 Home-page: https://github.com/NateRex/malmoext
 Author: Nate Rex
 Author-email: UNKNOWN
 License: MIT License
 Keywords: malmoext
 Platform: UNKNOWN
```

## Comparing `malmoext-0.36.0.0.1.dist-info/RECORD` & `malmoext-0.36.0.0.2.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 malmoext/__init__.py,sha256=4f9sqJVo1ldMv-rXzp-G9B5NsS-lpxIpGgBjHAQ7E0U,430
 malmoext/__main__.py,sha256=t08AD471eofTc2AJXfM_Fbei2-d0R_BMEscCCbj96Ho,667
-malmoext/agent.py,sha256=SaF5P6Csq_PBKcKuD3ZZAG9dAwxRkhkyVzRWALuiTQw,10106
+malmoext/agent.py,sha256=CAnlZdeg36hfUv7On_x_iVJNaskl4DrK_Pwol4q-PdA,12031
 malmoext/agent_state.py,sha256=Y2hDVsEIfhCeRlDz5wwWzTqpUjOJfVWjV5ahCOcIWG0,8850
 malmoext/malmo_bootstrap.py,sha256=kjR1hhgJCwtzG6MyzxAuDpTXAjw9-w0xT1ZfhOlelsI,1613
-malmoext/scenario.py,sha256=GVT7gJxSo7-8to2P0OQSszqQOWSBhLNk2GsYeQ53YLs,8729
+malmoext/scenario.py,sha256=jFL2UppHmsazwYgy77MUwa26NYCVWoanHgpOFex77Wo,8848
 malmoext/scenario_builder.py,sha256=6iFYNBdDbw6OIELIjvSXsW6AVfbKEesLTRfo4w9OPnI,11890
 malmoext/types.py,sha256=Dkg6YdGirEFw3BwJXXbS2KwQeqY38om7q_v5SWtB8AM,20587
 malmoext/utils.py,sha256=svLJsuMeDsOeaZTlkttK-Oo42OtIG7k98MNpAFfODco,2598
-malmoext-0.36.0.0.1.dist-info/LICENSE,sha256=I4zaWkcNiCu8UyKainEMhG57jr1Ht8MGgLWNDpfxEbU,1070
-malmoext-0.36.0.0.1.dist-info/METADATA,sha256=u-ubwUBW9yERXX7iIe9yiCiTMf0oXqWOQaKoYdd-qLw,550
-malmoext-0.36.0.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-malmoext-0.36.0.0.1.dist-info/top_level.txt,sha256=8vhP_P8bgE-zPDzdl41LLizkQD3GiRJjOrJJpq6FafQ,9
-malmoext-0.36.0.0.1.dist-info/RECORD,,
+malmoext-0.36.0.0.2.dist-info/LICENSE,sha256=I4zaWkcNiCu8UyKainEMhG57jr1Ht8MGgLWNDpfxEbU,1070
+malmoext-0.36.0.0.2.dist-info/METADATA,sha256=AuNAu6VeIYtziO3wimwumTqUVgPEuTJoz3PukB6oaas,550
+malmoext-0.36.0.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+malmoext-0.36.0.0.2.dist-info/top_level.txt,sha256=8vhP_P8bgE-zPDzdl41LLizkQD3GiRJjOrJJpq6FafQ,9
+malmoext-0.36.0.0.2.dist-info/RECORD,,
```

