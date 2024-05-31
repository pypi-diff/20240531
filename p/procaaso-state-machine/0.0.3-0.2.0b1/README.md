# Comparing `tmp/procaaso_state_machine-0.0.3.tar.gz` & `tmp/procaaso_state_machine-0.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "procaaso_state_machine-0.0.3.tar", max compression
+gzip compressed data, was "procaaso_state_machine-0.2.0b1.tar", max compression
```

## Comparing `procaaso_state_machine-0.0.3.tar` & `procaaso_state_machine-0.2.0b1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35821 2024-05-09 22:16:56.731336 procaaso_state_machine-0.0.3/LICENSE
--rw-r--r--   0        0        0        0 2024-05-09 22:16:56.733714 procaaso_state_machine-0.0.3/procaaso_state_machine/__init__.py
--rw-r--r--   0        0        0     3855 2024-05-09 22:16:56.735847 procaaso_state_machine-0.0.3/procaaso_state_machine/procaaso_event.py
--rw-r--r--   0        0        0    13658 2024-05-29 23:59:43.967217 procaaso_state_machine-0.0.3/procaaso_state_machine/procaaso_state.py
--rw-r--r--   0        0        0    25343 2024-05-29 23:42:17.207472 procaaso_state_machine-0.0.3/procaaso_state_machine/procaaso_state_machine.py
--rw-r--r--   0        0        0      389 2024-05-31 19:16:43.765692 procaaso_state_machine-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    18570 2024-05-30 20:21:22.577091 procaaso_state_machine-0.0.3/README.md
--rw-r--r--   0        0        0    18414 1970-01-01 00:00:00.000000 procaaso_state_machine-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35821 2024-05-09 22:16:56.731336 procaaso_state_machine-0.2.0b1/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-09 22:16:56.733714 procaaso_state_machine-0.2.0b1/procaaso_state_machine/__init__.py
+-rw-r--r--   0        0        0     3855 2024-05-09 22:16:56.735847 procaaso_state_machine-0.2.0b1/procaaso_state_machine/procaaso_event.py
+-rw-r--r--   0        0        0    10802 2024-05-29 19:06:27.432467 procaaso_state_machine-0.2.0b1/procaaso_state_machine/procaaso_state.py
+-rw-r--r--   0        0        0    25319 2024-05-29 00:14:16.399345 procaaso_state_machine-0.2.0b1/procaaso_state_machine/procaaso_state_machine.py
+-rw-r--r--   0        0        0      391 2024-05-29 21:57:16.922860 procaaso_state_machine-0.2.0b1/pyproject.toml
+-rw-r--r--   0        0        0    12395 2024-05-09 22:16:56.732365 procaaso_state_machine-0.2.0b1/README.md
+-rw-r--r--   0        0        0    12536 1970-01-01 00:00:00.000000 procaaso_state_machine-0.2.0b1/PKG-INFO
```

### Comparing `procaaso_state_machine-0.0.3/LICENSE` & `procaaso_state_machine-0.2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `procaaso_state_machine-0.0.3/procaaso_state_machine/procaaso_event.py` & `procaaso_state_machine-0.2.0b1/procaaso_state_machine/procaaso_event.py`

 * *Files identical despite different names*

### Comparing `procaaso_state_machine-0.0.3/procaaso_state_machine/procaaso_state.py` & `procaaso_state_machine-0.2.0b1/procaaso_state_machine/procaaso_state.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,25 +6,24 @@
 class State:
     def __init__(self, id: int | str, onEnterEnabled: bool = False, onExitEnabled: bool = False) -> None:
         """
         Initialize a State object. This call will determine if the onEnter and onExit functionality will be disabled or enabled
         All routines and transitions must be added manually through the class methods
 
         Parameters:
-        - id (int | str): The state ID. Each state should only have one ID.
+        - id (int): The state number. Each state should only have one ID.
         - onEnterEnabled (bool): Indicator for if a state should have an on enter function, default to false
         - onExitEnabled (bool): Indicator for if a state should have an on exit function, default to false
 
 
         Raises:
         - TypeError: If the provided ID is not of type 'int'.
 
         Usage:
         - state_instance = State(0)
-        - state_instance = State(1, )
         """
         # A boolean to track if the state is apart of a state machine yet
         self.__apartOfStateMachine = False
 
         # A dictionary containing the routines registered to run
         self.__routines = {}
 
@@ -47,47 +46,18 @@
             self.set_transition(self.id)
         except (TypeError, ValueError) as e:
             # Raise a TypeError if the ID is not of type 'int' or if it can't be converted
             raise TypeError(
                 f"Id should be an integer, but the supplied id is of type {type(id)}"
             ) from e
     def get_on_enter_enabled(self):
-        """
-        Retrieve the current state of the onEnterEnabled attribute.
-
-        Returns:
-            bool: The current value of the __onEnterEnabled attribute, indicating
-                whether the onEnter functionality is enabled (True) or disabled (False).
-        """
         return self.__onEnterEnabled
     def get_on_exit_enabled(self):
-        """
-        Retrieve the current state of the onExitEnabled attribute.
-
-        Returns:
-            bool: The current value of the __onExitEnabled attribute, indicating
-                    whether the onExit functionality is enabled (True) or disabled (False).
-        """
         return self.__onExitEnabled
     def set_on_enter_function(self, routine: Callable):
-        """
-        Set the routine to be executed when the state is entered, if onEnter functionality is enabled.
-
-        Args:
-            routine (Callable): The function to be executed on entering the state. This function must accept keyword arguments.
-
-        Raises:
-            Exception: If the state is already part of a state machine, the onEnter functionality is disabled, 
-                    or the supplied routine does not accept keyword arguments.
-
-        Notes:
-            - Ensures that the state is not yet part of a state machine.
-            - Checks if the onEnter functionality is enabled.
-            - Verifies that the supplied routine is a callable and accepts keyword arguments.
-        """
         # Ensure this state is not yet apart of the state machine
         if not self.__apartOfStateMachine:
             # Ensure that the on enter functionality is enabled 
             if self.__onEnterEnabled:
                 if isinstance(routine, Callable):
                     if self.__accepts_kwargs(routine) == True:
                         self.__onEnterRoutine = routine
@@ -98,45 +68,21 @@
                     f"On Enter function disabled, enable onEnterEnabled to set this routine"
                 )
         else:
             raise Exception(
                 f"Once state object is apart of StateMachine object, it may no longer be modified"
             )
     def get_on_enter_function(self):
-        """
-        Retrieve the routine to be executed when the state is entered.
-
-        Returns:
-            Callable: The function to be executed on entering the state, if onEnter functionality is enabled.
-
-        Raises:
-            Exception: If the onEnter functionality is not enabled, an exception is raised indicating that no function may be returned.
-        """
         if self.get_on_enter_enabled():
             return self.__onEnterRoutine
         else:
             raise Exception(
                 f"onEnter functionality is not enabled, no function may be returned"
             )
     def set_on_exit_function(self, routine: Callable):
-        """
-        Set the routine to be executed when the state is exited, if onExit functionality is enabled.
-
-        Args:
-            routine (Callable): The function to be executed on exiting the state. This function must accept keyword arguments.
-
-        Raises:
-            Exception: If the state is already part of a state machine, the onExit functionality is disabled,
-                    or the supplied routine does not accept keyword arguments.
-
-        Notes:
-            - Ensures that the state is not yet part of a state machine.
-            - Checks if the onExit functionality is enabled.
-            - Verifies that the supplied routine is a callable and accepts keyword arguments.
-        """
         # Ensure this state is not yet apart of the state machine
         if not self.__apartOfStateMachine:
             # Ensure that the on enter functionality is enabled 
             if self.__onExitEnabled:
                 if isinstance(routine, Callable):
                     if self.__accepts_kwargs(routine) == True:
                         self.__onExitRoutine = routine
@@ -147,30 +93,20 @@
                     f"onExit function disabled, enable onExitEnabled to set this routine"
                 )
         else:
             raise Exception(
                 f"Once state object is apart of StateMachine object, it may no longer be modified"
             )
     def get_on_exit_function(self):
-        """
-        Retrieve the routine to be executed when the state is exited.
-
-        Returns:
-            Callable: The function to be executed on exiting the state, if onExit functionality is enabled.
-
-        Raises:
-            Exception: If the onExit functionality is not enabled, an exception is raised indicating that no function may be returned.
-        """
         if self.get_on_exit_enabled():
             return self.__onExitRoutine
         else:
             raise Exception(
                 f"onExit functionality is not enabled, no function may be returned"
             )
-
     def set_routine(self, routineName: str, routine: Callable):
         """
         Set a routine with a given name in the object's routines dictionary.
         The order in which the routines are added determines the order in which they will be executed.
         If a routine name is already present in the states dictionary of routines, the routine will be updated, not added.
         Thus, routine names must be unique within a state object.
         It is required that all routines accept kwargs by default, such that on call the routines can be passed information.
```

### Comparing `procaaso_state_machine-0.0.3/procaaso_state_machine/procaaso_state_machine.py` & `procaaso_state_machine-0.2.0b1/procaaso_state_machine/procaaso_state_machine.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,20 +224,20 @@
         - states_dict = state_machine_instance.get_states()
         """
         try:
             return self.__states
         except Exception as e:
             raise Exception(f"Failed to get state dictionary: {e}")
 
-    def __set_current_state_id(self, newStateId: int | str):
+    def __set_current_state_id(self, newStateId: int):
         """
         Set the ID of the current state.
 
         Parameters:
-        - newStateId (int | str): The ID of the new state.
+        - newStateId (int): The ID of the new state.
 
         Raises:
         - Exception: If an unexpected exception occurs during the process.
 
         Usage:
         - state_machine_instance._StateMachine__set_current_state_id(2)
         """
@@ -249,15 +249,15 @@
             )
 
     def get_current_state_id(self):
         """
         Get the ID of the current state.
 
         Returns:
-        - int | str: The ID of the current state.
+        - int: The ID of the current state.
 
         Raises:
         - Exception: If an unexpected exception occurs during the process.
 
         Usage:
         - current_state_id = state_machine_instance.get_current_state_id()
         """
@@ -318,15 +318,15 @@
             - If true, run the on enter function, 
                 - If the routine fails, stay in the current state and throw error.
                 - If routine succeeds exit the transition_state routine
             - If false, exit the transition_state routine \n
         Return values are allowed, if the function returns a non-None values, the return value(s) from onEnter and onExit will be 
 
         Parameters:
-        - newStateId (int | str): The ID of the new state.
+        - newStateId (int): The ID of the new state.
         - onEnterParameters (dict[str, any]) OPTIONAL: A structure to contain any variables for the on enter function
         - onExitParameters (dict[str, any]) OPTIONAL: A struture to contain any variables for the on exit function
 
         Raises:
         - Exception: If an unexpected exception occurs during the process.
         Returns:
         - Dict['onExitReturn': onExitReturnValue, 'onEnterReturn': onEnterReturnValue]
```

