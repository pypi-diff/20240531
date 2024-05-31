# Comparing `tmp/eflips_depot-3.1.5.tar.gz` & `tmp/eflips_depot-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eflips_depot-3.1.5.tar", max compression
+gzip compressed data, was "eflips_depot-3.2.0.tar", max compression
```

## Comparing `eflips_depot-3.1.5.tar` & `eflips_depot-3.2.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0    34143 2024-05-28 09:46:16.087822 eflips_depot-3.1.5/LICENSE.md
--rw-r--r--   0        0        0     4899 2024-05-28 09:46:16.087822 eflips_depot-3.1.5/README.md
--rw-r--r--   0        0        0     1556 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/__init__.py
--rw-r--r--   0        0        0    51939 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/api/__init__.py
--rw-r--r--   0        0        0     5375 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/api/defaults/default_settings.json
--rw-r--r--   0        0        0        0 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/api/private/__init__.py
--rw-r--r--   0        0        0    17136 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/api/private/depot.py
--rw-r--r--   0        0        0    15362 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/api/private/util.py
--rw-r--r--   0        0        0    35678 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/configuration.py
--rw-r--r--   0        0        0   105566 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/depot.py
--rw-r--r--   0        0        0   140842 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/evaluation.py
--rw-r--r--   0        0        0    16131 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/filters.py
--rw-r--r--   0        0        0     5569 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/input_epex_power_price.py
--rw-r--r--   0        0        0        0 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/doc/__init__.py
--rw-r--r--   0        0        0    22330 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/doc/direct_details.pdf
--rw-r--r--   0        0        0    24855 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/evaluation.py
--rw-r--r--   0        0        0      594 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/opt_tools/__init__.py
--rw-r--r--   0        0        0     1057 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/opt_tools/crossover.py
--rw-r--r--   0        0        0     8230 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/opt_tools/fitness_c_urfd.py
--rw-r--r--   0        0        0     7027 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/opt_tools/fitness_util.py
--rw-r--r--   0        0        0    14707 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/opt_tools/init.py
--rw-r--r--   0        0        0    12238 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/opt_tools/mutation.py
--rw-r--r--   0        0        0     9821 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/optimize_c_urfd.py
--rw-r--r--   0        0        0    56989 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/packing.py
--rw-r--r--   0        0        0      810 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/settings.py
--rw-r--r--   0        0        0     9736 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/template_creation.py
--rw-r--r--   0        0        0     3780 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/layout_opt/util.py
--rw-r--r--   0        0        0     2509 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/plots.py
--rw-r--r--   0        0        0    58757 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/processes.py
--rw-r--r--   0        0        0    16648 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/rating.py
--rw-r--r--   0        0        0    13568 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/resources.py
--rw-r--r--   0        0        0     2527 2024-05-28 09:46:16.091822 eflips_depot-3.1.5/eflips/depot/settings_config.py
--rw-r--r--   0        0        0     9375 2024-05-28 09:46:16.095822 eflips_depot-3.1.5/eflips/depot/simple_vehicle.py
--rw-r--r--   0        0        0    10676 2024-05-28 09:46:16.095822 eflips_depot-3.1.5/eflips/depot/simulation.py
--rw-r--r--   0        0        0    54311 2024-05-28 09:46:16.095822 eflips_depot-3.1.5/eflips/depot/smart_charging.py
--rw-r--r--   0        0        0    22338 2024-05-28 09:46:16.095822 eflips_depot-3.1.5/eflips/depot/standalone.py
--rw-r--r--   0        0        0     7097 2024-05-28 09:46:16.095822 eflips_depot-3.1.5/eflips/depot/validation.py
--rw-r--r--   0        0        0     1215 2024-05-28 09:46:16.095822 eflips_depot-3.1.5/pyproject.toml
--rw-r--r--   0        0        0     5809 1970-01-01 00:00:00.000000 eflips_depot-3.1.5/PKG-INFO
+-rw-r--r--   0        0        0    34143 2024-05-31 15:10:10.053665 eflips_depot-3.2.0/LICENSE.md
+-rw-r--r--   0        0        0     4899 2024-05-31 15:10:10.053665 eflips_depot-3.2.0/README.md
+-rw-r--r--   0        0        0     1556 2024-05-31 15:10:10.053665 eflips_depot-3.2.0/eflips/depot/__init__.py
+-rw-r--r--   0        0        0    57378 2024-05-31 15:10:10.053665 eflips_depot-3.2.0/eflips/depot/api/__init__.py
+-rw-r--r--   0        0        0     5375 2024-05-31 15:10:10.053665 eflips_depot-3.2.0/eflips/depot/api/defaults/default_settings.json
+-rw-r--r--   0        0        0        0 2024-05-31 15:10:10.053665 eflips_depot-3.2.0/eflips/depot/api/private/__init__.py
+-rw-r--r--   0        0        0    17136 2024-05-31 15:10:10.053665 eflips_depot-3.2.0/eflips/depot/api/private/depot.py
+-rw-r--r--   0        0        0    10902 2024-05-31 15:10:10.053665 eflips_depot-3.2.0/eflips/depot/api/private/smart_charging.py
+-rw-r--r--   0        0        0    15362 2024-05-31 15:10:10.053665 eflips_depot-3.2.0/eflips/depot/api/private/util.py
+-rw-r--r--   0        0        0    35678 2024-05-31 15:10:10.053665 eflips_depot-3.2.0/eflips/depot/configuration.py
+-rw-r--r--   0        0        0   105566 2024-05-31 15:10:10.053665 eflips_depot-3.2.0/eflips/depot/depot.py
+-rw-r--r--   0        0        0   140842 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/evaluation.py
+-rw-r--r--   0        0        0    16131 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/filters.py
+-rw-r--r--   0        0        0     5569 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/input_epex_power_price.py
+-rw-r--r--   0        0        0        0 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/layout_opt/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/layout_opt/doc/__init__.py
+-rw-r--r--   0        0        0    22330 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/layout_opt/doc/direct_details.pdf
+-rw-r--r--   0        0        0    24855 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/layout_opt/evaluation.py
+-rw-r--r--   0        0        0      594 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/layout_opt/opt_tools/__init__.py
+-rw-r--r--   0        0        0     1057 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/layout_opt/opt_tools/crossover.py
+-rw-r--r--   0        0        0     8230 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/layout_opt/opt_tools/fitness_c_urfd.py
+-rw-r--r--   0        0        0     7027 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/layout_opt/opt_tools/fitness_util.py
+-rw-r--r--   0        0        0    14707 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/layout_opt/opt_tools/init.py
+-rw-r--r--   0        0        0    12238 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/layout_opt/opt_tools/mutation.py
+-rw-r--r--   0        0        0     9821 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/layout_opt/optimize_c_urfd.py
+-rw-r--r--   0        0        0    56989 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/layout_opt/packing.py
+-rw-r--r--   0        0        0      810 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/layout_opt/settings.py
+-rw-r--r--   0        0        0     9736 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/layout_opt/template_creation.py
+-rw-r--r--   0        0        0     3780 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/layout_opt/util.py
+-rw-r--r--   0        0        0     2509 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/plots.py
+-rw-r--r--   0        0        0    58757 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/processes.py
+-rw-r--r--   0        0        0    16648 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/rating.py
+-rw-r--r--   0        0        0    13568 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/resources.py
+-rw-r--r--   0        0        0     2527 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/settings_config.py
+-rw-r--r--   0        0        0     9375 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/simple_vehicle.py
+-rw-r--r--   0        0        0    10676 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/simulation.py
+-rw-r--r--   0        0        0    54311 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/smart_charging.py
+-rw-r--r--   0        0        0    22338 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/standalone.py
+-rw-r--r--   0        0        0     7097 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/eflips/depot/validation.py
+-rw-r--r--   0        0        0     1233 2024-05-31 15:10:10.057665 eflips_depot-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5848 1970-01-01 00:00:00.000000 eflips_depot-3.2.0/PKG-INFO
```

### Comparing `eflips_depot-3.1.5/LICENSE.md` & `eflips_depot-3.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/README.md` & `eflips_depot-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/__init__.py` & `eflips_depot-3.2.0/eflips/depot/__init__.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/api/__init__.py` & `eflips_depot-3.2.0/eflips/depot/api/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     a. If you are using an external consumption model, run it again making sure it does not create new vehicles.
     b. Run the :func:`simple_consumption_simulation` function again, this time with ``initialize_vehicles=False``.
 """
 import copy
 import os
 import warnings
 from datetime import timedelta
+from enum import Enum, auto
 from math import ceil
 from typing import Any, Dict, Optional, Union
 
 import numpy as np
 import sqlalchemy.orm
 from eflips.model import (
     Area,
@@ -52,23 +53,50 @@
 from eflips.depot import DepotEvaluation, ProcessStatus, SimulationHost
 from eflips.depot.api.private.depot import (
     create_simple_depot,
     delete_depots,
     depot_to_template,
     group_rotations_by_start_end_stop,
 )
+from eflips.depot.api.private.smart_charging import optimize_charging_events_even
 from eflips.depot.api.private.util import (
     create_session,
     repeat_vehicle_schedules,
     start_and_end_times,
     vehicle_type_to_global_constants_dict,
     VehicleSchedule,
 )
 
 
+class SmartChargingStragegy(Enum):
+    """Enum class for different smart charging strategies."""
+
+    NONE = auto
+    """
+    Do not use smart charging.
+
+    Buses are charged with the maximum power available, from the time they arrive at the depot
+    until they are full (or leave the depot).
+    """
+    EVEN = auto
+    """
+    Use smart charging with an even distribution of charging power over the time the bus is at the depot.
+
+    This aims to
+    minimize the peak power demand.
+    """
+    MIN_PRICE = auto
+    """
+    Use smart charging in order to minimize the cost of charging.
+
+    The price profile can be specified using the
+    PRICE_PROFILE environment variable. If this is not set, the price is loaded using an API.
+    """
+
+
 def simple_consumption_simulation(
     scenario: Union[Scenario, int, Any],
     initialize_vehicles: bool,
     database_url: Optional[str] = None,
     calculate_timeseries: bool = False,
 ) -> None:
     """
@@ -346,18 +374,93 @@
                 cleaning_capacities=max_clean_occupancies,
                 charging_power=charging_power,
                 session=session,
                 cleaning_duration=timedelta(seconds=CLEAN_DURATION),
             )
 
 
+def apply_even_smart_charging(
+    scenario: Union[Scenario, int, Any],
+    database_url: Optional[str] = None,
+    standby_departure_duration: timedelta = timedelta(minutes=5),
+) -> None:
+    """
+    Takes a scenario where depot simulation has been run and applies smart charging to the depot.
+
+    This modifies the
+    time and power of the charging events in the database. The arrival and departure times and SoCs at these times are
+    not modified.
+
+    :param scenario: A :class:`eflips.model.Scenario` object containing the input data for the simulation.
+    :param database_url: An optional database URL. If no database URL is passed and the `scenario` parameter is not a
+        :class:`eflips.model.Scenario` object, the environment variable `DATABASE_URL` must be set to a valid database
+        URL.
+    :param standby_departure_duration: The duration of the STANDBY_DEPARTURE event. This is the time the vehicle is
+        allowed to wait at the depot before it has to leave. The default is 5 minutes.
+    :return: None. The results are added to the database.
+    """
+    with create_session(scenario, database_url) as (session, scenario):
+        depots = session.query(Depot).filter(Depot.scenario_id == scenario.id).all()
+        for depot in depots:
+            # Load all the charging events at this depot
+            charging_events = (
+                session.query(Event)
+                .join(Area)
+                .filter(Area.depot_id == depot.id)
+                .filter(Event.event_type == EventType.CHARGING_DEPOT)
+                .all()
+            )
+
+            # For each event, take the subsequent STANDBY_DEPARTURE event of the same vehicle
+            # Reduce the STANDBY_DEPARTURE events duration to 5 minutes
+            # Move the end time of the charging event to the start time of the STANDBY_DEPARTURE event
+            for charging_event in charging_events:
+                next_event = (
+                    session.query(Event)
+                    .filter(Event.time_start >= charging_event.time_end)
+                    .filter(Event.vehicle_id == charging_event.vehicle_id)
+                    .order_by(Event.time_start)
+                    .first()
+                )
+                assert next_event is not None
+                assert next_event.event_type == EventType.STANDBY_DEPARTURE
+                assert next_event.time_start == charging_event.time_end
+
+                if (
+                    next_event.time_end - next_event.time_start
+                ) > standby_departure_duration:
+                    next_event.time_start = (
+                        next_event.time_end - standby_departure_duration
+                    )
+                    session.flush()
+                    # Add a timeseries to the charging event
+                    assert charging_event.timeseries is None
+                    charging_event.timeseries = {
+                        "time": [
+                            charging_event.time_start.isoformat(),
+                            charging_event.time_end.isoformat(),
+                            next_event.time_start.isoformat(),
+                        ],
+                        "soc": [
+                            charging_event.soc_start,
+                            charging_event.soc_end,
+                            charging_event.soc_end,
+                        ],
+                    }
+                    charging_event.time_end = next_event.time_start
+                    session.flush()
+
+            optimize_charging_events_even(charging_events)
+
+
 def simulate_scenario(
     scenario: Union[Scenario, int, Any],
     repetition_period: Optional[timedelta] = None,
     database_url: Optional[str] = None,
+    smart_charging_strategy: SmartChargingStragegy = SmartChargingStragegy.EVEN,
 ) -> None:
     """
     This method simulates a scenario and adds the results to the database.
 
     It fills in the "Charging Events" in the :class:`eflips.model.Event` table and associates
     :class:`eflips.model.Vehicle` objects with all the existing "Driving Events" in the :class:`eflips.model.Event`
     table.
@@ -371,28 +474,42 @@
         is needed because the result should be a steady-state result. THis can only be achieved by simulating a
         time period before and after our actual simulation, and then only using the "middle". eFLIPS tries to
         automatically detect whether the schedule should be repeated daily or weekly. If this fails, a ValueError is
         raised and repetition needs to be specified manually.
     :param database_url: An optional database URL. If no database URL is passed and the `scenario` parameter is not a
         :class:`eflips.model.Scenario` object, the environment variable `DATABASE_URL` must be set to a valid database
         URL.
+    :param smart_charging_strategy: An optional parameter specifying the smart charging strategy to be used. The
+        default is SmartChargingStragegy.NONE. The following strategies are available:
+        - SmartChargingStragegy.NONE: Do not use smart charging. Buses are charged with the maximum power available,
+        from the time they arrive at the depot until they are full (or leave the depot).
+        - SmartChargingStragegy.EVEN: Use smart charging with an even distribution of charging power over the time the
+        bus is at the depot. This aims to minimize the peak power demand.
 
     :return: Nothing. The results are added to the database.
     """
-
-    # Step 0: Load the scenario
     with create_session(scenario, database_url) as (session, scenario):
         simulation_host = init_simulation(
             scenario=scenario,
             session=session,
             repetition_period=repetition_period,
         )
         ev = run_simulation(simulation_host)
         add_evaluation_to_database(scenario, ev, session)
 
+    match smart_charging_strategy:
+        case SmartChargingStragegy.NONE:
+            pass
+        case SmartChargingStragegy.EVEN:
+            apply_even_smart_charging(scenario, database_url)
+        case SmartChargingStragegy.MIN_PRICE:
+            raise NotImplementedError("MIN_PRICE strategy is not implemented yet.")
+        case _:
+            raise NotImplementedError()
+
 
 def _init_simulation(
     scenario: Scenario,
     session: Session,
     repetition_period: Optional[timedelta] = None,
     vehicle_count_dict: Optional[Dict[str, int]] = None,
 ) -> SimulationHost:
```

### Comparing `eflips_depot-3.1.5/eflips/depot/api/defaults/default_settings.json` & `eflips_depot-3.2.0/eflips/depot/api/defaults/default_settings.json`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/api/private/depot.py` & `eflips_depot-3.2.0/eflips/depot/api/private/depot.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/api/private/util.py` & `eflips_depot-3.2.0/eflips/depot/api/private/util.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/configuration.py` & `eflips_depot-3.2.0/eflips/depot/configuration.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/depot.py` & `eflips_depot-3.2.0/eflips/depot/depot.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/evaluation.py` & `eflips_depot-3.2.0/eflips/depot/evaluation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/filters.py` & `eflips_depot-3.2.0/eflips/depot/filters.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/input_epex_power_price.py` & `eflips_depot-3.2.0/eflips/depot/input_epex_power_price.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/layout_opt/doc/direct_details.pdf` & `eflips_depot-3.2.0/eflips/depot/layout_opt/doc/direct_details.pdf`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/layout_opt/evaluation.py` & `eflips_depot-3.2.0/eflips/depot/layout_opt/evaluation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/layout_opt/opt_tools/__init__.py` & `eflips_depot-3.2.0/eflips/depot/layout_opt/opt_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/layout_opt/opt_tools/crossover.py` & `eflips_depot-3.2.0/eflips/depot/layout_opt/opt_tools/crossover.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/layout_opt/opt_tools/fitness_c_urfd.py` & `eflips_depot-3.2.0/eflips/depot/layout_opt/opt_tools/fitness_c_urfd.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/layout_opt/opt_tools/fitness_util.py` & `eflips_depot-3.2.0/eflips/depot/layout_opt/opt_tools/fitness_util.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/layout_opt/opt_tools/init.py` & `eflips_depot-3.2.0/eflips/depot/layout_opt/opt_tools/init.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/layout_opt/opt_tools/mutation.py` & `eflips_depot-3.2.0/eflips/depot/layout_opt/opt_tools/mutation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/layout_opt/optimize_c_urfd.py` & `eflips_depot-3.2.0/eflips/depot/layout_opt/optimize_c_urfd.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/layout_opt/packing.py` & `eflips_depot-3.2.0/eflips/depot/layout_opt/packing.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/layout_opt/settings.py` & `eflips_depot-3.2.0/eflips/depot/layout_opt/settings.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/layout_opt/template_creation.py` & `eflips_depot-3.2.0/eflips/depot/layout_opt/template_creation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/layout_opt/util.py` & `eflips_depot-3.2.0/eflips/depot/layout_opt/util.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/plots.py` & `eflips_depot-3.2.0/eflips/depot/plots.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/processes.py` & `eflips_depot-3.2.0/eflips/depot/processes.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/rating.py` & `eflips_depot-3.2.0/eflips/depot/rating.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/resources.py` & `eflips_depot-3.2.0/eflips/depot/resources.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/settings_config.py` & `eflips_depot-3.2.0/eflips/depot/settings_config.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/simple_vehicle.py` & `eflips_depot-3.2.0/eflips/depot/simple_vehicle.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/simulation.py` & `eflips_depot-3.2.0/eflips/depot/simulation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/smart_charging.py` & `eflips_depot-3.2.0/eflips/depot/smart_charging.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/standalone.py` & `eflips_depot-3.2.0/eflips/depot/standalone.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/eflips/depot/validation.py` & `eflips_depot-3.2.0/eflips/depot/validation.py`

 * *Files identical despite different names*

### Comparing `eflips_depot-3.1.5/pyproject.toml` & `eflips_depot-3.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [tool.poetry]
 name = "eflips-depot"
-version = "3.1.5"
+version = "3.2.0"
 description = "Depot Simulation for eFLIPS"
 authors = ["Enrico Lauth <enrico.lauth@tu-berlin.de>",
     "Ludger Heide <ludger.heide@tu-berlin.de",
     "Shuyao Guo <shuyao.guo@tu-berlin.de"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/mpm-tu-berlin/eflips-depot"
 repository = "https://github.com/mpm-tu-berlin/eflips-depot"
 packages = [{ include = "eflips/depot" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 simpy = "^4.0.1"
-eflips-model = "^3.2.0"
+eflips-model = "^3.3.0"
 # Legacy dependencies, which are still needed until we refactor the code
 eflips = "^0.1.3"
 xlsxwriter = "^3.1.9"
 pandas = "^2.1.4"
 xlrd = "<=1.2.0"
+scipy = "^1.13.1"
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
 
 [tool.pydocstringformatter]
```

### Comparing `eflips_depot-3.1.5/PKG-INFO` & `eflips_depot-3.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: eflips-depot
-Version: 3.1.5
+Version: 3.2.0
 Summary: Depot Simulation for eFLIPS
 Home-page: https://github.com/mpm-tu-berlin/eflips-depot
 License: AGPL-3.0-or-later
 Author: Enrico Lauth
 Author-email: enrico.lauth@tu-berlin.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: eflips (>=0.1.3,<0.2.0)
-Requires-Dist: eflips-model (>=3.2.0,<4.0.0)
+Requires-Dist: eflips-model (>=3.3.0,<4.0.0)
 Requires-Dist: pandas (>=2.1.4,<3.0.0)
+Requires-Dist: scipy (>=1.13.1,<2.0.0)
 Requires-Dist: simpy (>=4.0.1,<5.0.0)
 Requires-Dist: xlrd (<=1.2.0)
 Requires-Dist: xlsxwriter (>=3.1.9,<4.0.0)
 Project-URL: Repository, https://github.com/mpm-tu-berlin/eflips-depot
 Description-Content-Type: text/markdown
 
 [![Tests](https://github.com/mpm-tu-berlin/eflips-depot/actions/workflows/unittests.yml/badge.svg)](https://github.com/mpm-tu-berlin/eflips-depot/actions/workflows/unittests.yml)
```

