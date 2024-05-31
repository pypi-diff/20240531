# Comparing `tmp/rocketflightsim-0.1.1.tar.gz` & `tmp/rocketflightsim-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocketflightsim-0.1.1.tar", last modified: Mon May 27 00:47:28 2024, max compression
+gzip compressed data, was "rocketflightsim-0.1.2.tar", last modified: Fri May 31 00:00:55 2024, max compression
```

## Comparing `rocketflightsim-0.1.1.tar` & `rocketflightsim-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 00:47:28.322411 rocketflightsim-0.1.1/
--rw-rw-rw-   0        0        0     1095 2024-05-25 02:16:59.000000 rocketflightsim-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      784 2024-05-27 00:47:28.322411 rocketflightsim-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      262 2024-05-25 02:16:59.000000 rocketflightsim-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 00:47:28.262432 rocketflightsim-0.1.1/examples/
--rw-rw-rw-   0        0        0        0 2024-05-25 02:16:59.000000 rocketflightsim-0.1.1/examples/__init__.py
--rw-rw-rw-   0        0        0     7943 2024-05-27 00:45:43.000000 rocketflightsim-0.1.1/examples/example_configurations.py
-drwxrwxrwx   0        0        0        0 2024-05-27 00:47:28.278516 rocketflightsim-0.1.1/rocketflightsim/
--rw-rw-rw-   0        0        0      353 2024-05-27 00:14:19.000000 rocketflightsim-0.1.1/rocketflightsim/__init__.py
--rw-rw-rw-   0        0        0     1350 2024-05-25 04:59:23.000000 rocketflightsim-0.1.1/rocketflightsim/constants.py
--rw-rw-rw-   0        0        0    16006 2024-05-26 22:52:51.000000 rocketflightsim-0.1.1/rocketflightsim/flight_simulation.py
--rw-rw-rw-   0        0        0     8603 2024-05-26 22:52:51.000000 rocketflightsim-0.1.1/rocketflightsim/helper_functions.py
--rw-rw-rw-   0        0        0    14888 2024-05-25 02:16:59.000000 rocketflightsim-0.1.1/rocketflightsim/plotting_functions.py
--rw-rw-rw-   0        0        0     9342 2024-05-26 22:52:51.000000 rocketflightsim-0.1.1/rocketflightsim/rocket_classes.py
-drwxrwxrwx   0        0        0        0 2024-05-27 00:47:28.315425 rocketflightsim-0.1.1/rocketflightsim.egg-info/
--rw-rw-rw-   0        0        0      784 2024-05-27 00:47:28.000000 rocketflightsim-0.1.1/rocketflightsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2024-05-27 00:47:28.000000 rocketflightsim-0.1.1/rocketflightsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 00:47:28.000000 rocketflightsim-0.1.1/rocketflightsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-27 00:47:28.000000 rocketflightsim-0.1.1/rocketflightsim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2024-05-27 00:47:28.000000 rocketflightsim-0.1.1/rocketflightsim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 00:47:28.323406 rocketflightsim-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      778 2024-05-27 00:11:50.000000 rocketflightsim-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-27 00:47:28.320457 rocketflightsim-0.1.1/tests/
--rw-rw-rw-   0        0        0        0 2024-05-25 02:16:59.000000 rocketflightsim-0.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0    30829 2024-05-27 00:25:53.000000 rocketflightsim-0.1.1/tests/test_configs.py
--rw-rw-rw-   0        0        0     3194 2024-05-27 00:25:33.000000 rocketflightsim-0.1.1/tests/test_flight_simulation.py
+drwxrwxrwx   0        0        0        0 2024-05-31 00:00:55.857237 rocketflightsim-0.1.2/
+-rw-rw-rw-   0        0        0     1095 2024-05-25 02:16:59.000000 rocketflightsim-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1125 2024-05-31 00:00:55.857237 rocketflightsim-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      603 2024-05-29 23:05:15.000000 rocketflightsim-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 00:00:55.803643 rocketflightsim-0.1.2/examples/
+-rw-rw-rw-   0        0        0        0 2024-05-25 02:16:59.000000 rocketflightsim-0.1.2/examples/__init__.py
+-rw-rw-rw-   0        0        0     7941 2024-05-29 22:14:56.000000 rocketflightsim-0.1.2/examples/example_configurations.py
+drwxrwxrwx   0        0        0        0 2024-05-31 00:00:55.814836 rocketflightsim-0.1.2/rocketflightsim/
+-rw-rw-rw-   0        0        0      206 2024-05-30 23:51:47.000000 rocketflightsim-0.1.2/rocketflightsim/__init__.py
+-rw-rw-rw-   0        0        0     1481 2024-05-29 23:00:29.000000 rocketflightsim-0.1.2/rocketflightsim/constants.py
+-rw-rw-rw-   0        0        0    14283 2024-05-30 23:33:13.000000 rocketflightsim-0.1.2/rocketflightsim/flight_simulation.py
+-rw-rw-rw-   0        0        0     8603 2024-05-26 22:52:51.000000 rocketflightsim-0.1.2/rocketflightsim/helper_functions.py
+-rw-rw-rw-   0        0        0     9809 2024-05-30 23:59:37.000000 rocketflightsim-0.1.2/rocketflightsim/rocket_classes.py
+drwxrwxrwx   0        0        0        0 2024-05-31 00:00:55.847288 rocketflightsim-0.1.2/rocketflightsim.egg-info/
+-rw-rw-rw-   0        0        0     1125 2024-05-31 00:00:55.000000 rocketflightsim-0.1.2/rocketflightsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2024-05-31 00:00:55.000000 rocketflightsim-0.1.2/rocketflightsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 00:00:55.000000 rocketflightsim-0.1.2/rocketflightsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-31 00:00:55.000000 rocketflightsim-0.1.2/rocketflightsim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2024-05-31 00:00:55.000000 rocketflightsim-0.1.2/rocketflightsim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 00:00:55.858233 rocketflightsim-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      778 2024-05-30 23:53:30.000000 rocketflightsim-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 00:00:55.854247 rocketflightsim-0.1.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-25 02:16:59.000000 rocketflightsim-0.1.2/tests/__init__.py
+-rw-rw-rw-   0        0        0    30808 2024-05-30 23:20:30.000000 rocketflightsim-0.1.2/tests/test_configs.py
+-rw-rw-rw-   0        0        0     4273 2024-05-30 23:52:43.000000 rocketflightsim-0.1.2/tests/test_flight_simulation.py
```

### Comparing `rocketflightsim-0.1.1/LICENSE` & `rocketflightsim-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rocketflightsim-0.1.1/PKG-INFO` & `rocketflightsim-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: rocketflightsim
-Version: 0.1.1
+Version: 0.1.2
 Summary: A lightweight rocket flight simulator.
 Home-page: https://github.com/werocketry/RocketFlightSim
 Author: Giorgio Chassikos, Western Engineering Rocketry Team
 Author-email: werocketry@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RocketFlightSim
 
-RocketFlightSim (RFS) is a light-weight flight simulator for experimental rockets. It currently supports simulation of single-stage rockets in the troposphere, from takeoff to apogee. Simple airbrakes can added to the rocket to induce drag. 
+RocketFlightSim (RFS) is a light-weight flight simulator for experimental rockets. It is designed to be simple to use, understand, and modify, with the goal of providing a platform for students and hobbyists to learn about rocket flight dynamics.
+
+The simulator currently supports simulation of single-stage rockets in the troposphere, from takeoff to apogee. Simple airbrakes can added to the rocket to induce drag. 
+
+A large emphasis is placed on computational efficiency, with the goal of being lightweight enough to run real-time during flight on an onboard microcontroller.
```

### Comparing `rocketflightsim-0.1.1/examples/example_configurations.py` & `rocketflightsim-0.1.2/examples/example_configurations.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,16 +134,15 @@
 altitude_SA = 1401  # m, Spaceport America's elevation
 """ https://www.spaceportamerica.com/faq/#toggle-id-15 """
 launch_angle_SAC = 84  # deg from horizontal
 """ How the standard launch angle at Spaceport America Cup was determined
 DTEG 10.1.1: 
     > Launch vehicles will nominally launch at an elevation angle of 84° ±1°
 DTEG 10.1.2:
-    > Range Safety Officers reserve the right to require certain vehicles’ launch elevation be 
-lower or higher if flight safety issues are identified during pre-launch activities
+    > Range Safety Officers reserve the right to require certain vehicles’ launch elevation be lower or higher if flight safety issues are identified during pre-launch activities
 
 Teams have noted that they've been told to use angles at least as low as 80°. The Range Safety Officer picks the angle based on various factors, including the rocket being launched, the weather, and the location of the launch pad. In the design, simulation, and testing phases, use the nominal angle of 84°, but consider the possibility of the launch angle being more or less than that on competition day.
 """
 
 Spaceport_America_avg_launch_conditions = LaunchConditions(
     launchpad_pressure = launchpad_pressure_SAC,
     launchpad_temp = launchpad_temp_SAC,
@@ -155,16 +154,16 @@
 )
 
 # Default airbrakes model
 default_airbrakes_model = Airbrakes(
     num_flaps = 3,
     A_flap = 0.004,  # m^2  flap area
     Cd_brakes = 1,
-    max_deployment_speed = 5,  # deg/s
-    max_deployment_angle = 45  # deg
+    max_deployment_angle = 45,  # deg
+    max_deployment_rate = 5,  # deg/s
 )
 
 if __name__ == "__main__":
     from rocketflightsim.flight_simulation import simulate_flight, simulate_airbrakes_flight
     from rocketflightsim.plotting_functions import plot_ascent, plot_aerodynamics, plot_airbrakes_ascent
 
     dataset, liftoff_index, launch_rail_cleared_index, burnout_index, apogee_index = simulate_flight(rocket = example_rocket, launch_conditions = Spaceport_America_avg_launch_conditions, timestep = 0.001)
```

### Comparing `rocketflightsim-0.1.1/rocketflightsim/constants.py` & `rocketflightsim-0.1.2/rocketflightsim/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # constants 
-R_universal = 8.3144598  # J/(mol*K)
-MM_air = 0.0289644  # kg/mol
+R_universal = 8.3144598  # universal gas constant, J/(mol*K)
+MM_air = 0.0289644  # molar mass of air, kg/mol
 adiabatic_index_air = 1.4  # unitless
-"""Notes on adiabatic index (also known as the heat capacity ratio (cp/cv)) for air
+"""Notes on adiabatic index (also known as the heat capacity ratio or ratio of specific heats (cp/cv)) for air
+
+As per https://www.grc.nasa.gov/WWW/BGH/realspec.html, air is calorically perfect up to low supersonic Mach numbers, so the adiabatic index doesn't change with airspeed over the speeds that most hobbyist or collegiate team rockets will experience. 
 
 As a function of teperature, for dry air, the adiabatic index according to different sources is:
     https://en.wikipedia.org/wiki/Heat_capacity_ratio
     
         - 1.404 at -15°C
         - 1.403 at 0°C
         - 1.400 at 20°C
         - 1.398 at 200°C
 
     https://www.chemeurope.com/en/encyclopedia/Heat_capacity_ratio.html
 
         - 1.403 at 0°C
         - 1.400 at 20°C
         - 1.401 at 100°C
-        
-The value of 1.4 is a very good approximation for the temperature range the rocket will experience
 
-As per https://www.grc.nasa.gov/WWW/BGH/realspec.html, air is calorically perfect up to low supersonic Mach numbers, so the adiabatic index doesn't change with airspeed over the speeds that the rocket will experience
+The value of 1.4 is a very good approximation for the temperature ranges that most hobbyist or collegiate team rockets will experience.
 """
 
 # derived constants
 R_specific_air = R_universal / MM_air  # J/(kg*K)
 adiabatic_index_air_times_R_specific_air = adiabatic_index_air * R_specific_air  # J/(kg*K)
 
 # conversion factors
```

### Comparing `rocketflightsim-0.1.1/rocketflightsim/flight_simulation.py` & `rocketflightsim-0.1.2/rocketflightsim/flight_simulation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,37 @@
-# Import libraries, define natural constants, helper functions
+# Import libraries
 import sys
 import os
 
 import pandas as pd
 import numpy as np
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..', 'examples')))
 from . import helper_functions as hfunc
 from . import constants as con
 
+# Default timestep for the simulation
 default_timestep = 0.02
 """ Notes on timesteps:
 
 The default for OpenRocket sims is 0.01s for the first while, and then somewhere between 0.02 and 0.05 for a while, and then 0.05 for most of the rest of the ascent. It simulates more complicated dynamics than we do
 
-A timestep of 0.02s gives apogees a few feet different for a 10k launch compared to using 0.001s. 0.001s can still be used for one-off sims, but when running many sims, 0.02s is better.
+A timestep of 0.02s gives apogees a difference of a few feet for a 10k launch compared to using 0.001s. 0.001s can still be used for one-off sims, but when running many sims, 0.02s is better.
 """
+
+# TODO consider splitting simulator into stages. Could be better for readability, but also for allowing more complex simulations with multiple stages, and going beyond the troposphere with different lapse rates, a different gravity model, and a different wind model. Could even use it for educational purposes like showing the importance of having a launch rail
 # Flight simulation function
 def simulate_flight(rocket, launch_conditions, timestep=default_timestep):
     """
     Simulate the flight of a rocket until its apogee given its specifications and launch conditions.
 
     Args:
     - rocket (Rocket): An instance of the Rocket class.
     - launch_conditions (LaunchConditions): An instance of the LaunchConditions class.
-    - timestep (float): The time increment for the simulation in seconds.
+    - timestep (float, optional): The time increment for the simulation in seconds.
 
     Returns:
     - tuple: A tuple containing the dataset of simulation results and indices of key flight events.
     """
 
     # Initialize rocket parameters and launch conditions
     dry_mass = rocket.dry_mass
@@ -43,16 +46,17 @@
     L_launch_rail = launch_conditions.L_launch_rail
     launch_angle = launch_conditions.launch_angle
     
     T_lapse_rate = launch_conditions.local_T_lapse_rate
     F_gravity = launch_conditions.local_gravity
 
     # Initialize simulation variables
-    time, height, speed, a_y, a_x, v_y, v_x, Cd_A_rocket, Ma, q = 0, 0, 0, 0, 0, 0, 0, 0, 0, 0
+    time, height, speed, a_y, a_x, v_y, v_x, Ma, q = 0, 0, 0, 0, 0, 0, 0, 0, 0
     angle_to_vertical = np.deg2rad(90 - launch_angle)
+
     # Calculate constants to be used in air density function, set initial air density
     multiplier = launchpad_pressure / (con.R_specific_air * pow(launchpad_temp, - F_gravity / (con.R_specific_air * T_lapse_rate)))
     exponent = - F_gravity / (con.R_specific_air * T_lapse_rate) - 1
     air_density = hfunc.air_density_optimized(launchpad_temp, multiplier, exponent)
 
     # Store the initial state of the rocket
     simulated_values = [
@@ -64,24 +68,28 @@
             a_x,
             v_y,
             v_x,
             launchpad_temp,
             air_density,
             q,
             Ma,
-            Cd_A_rocket, # why is this being saved?
             angle_to_vertical,
         ]
     ]
 
+    # Calculate trigonometric ratios on the launch rail
+    cos_rail_angle_to_vertical = np.cos(angle_to_vertical)
+    sin_rail_angle_to_vertical = np.sin(angle_to_vertical)
+
     # Simulate motor burn until liftoff
+    takeoff_thrust = F_gravity * cos_rail_angle_to_vertical
     while (
         hfunc.thrust_at_time(time, engine_thrust_lookup)
         / hfunc.mass_at_time(time, dry_mass, fuel_mass_lookup)
-        <= F_gravity
+        <= takeoff_thrust
     ):
         time += timestep
         # Append simulation values for each timestep
         simulated_values.append(
             [
                 time,
                 height, # 0
@@ -90,25 +98,24 @@
                 a_x, # 0
                 v_y, # 0
                 v_x, # 0
                 launchpad_temp,
                 air_density,
                 q, # 0
                 Ma, # 0
-                Cd_A_rocket, # 0
                 angle_to_vertical,
             ]
         )
 
     liftoff_index = len(simulated_values)
 
     # Liftoff until launch rail cleared
     time += timestep
     effective_L_launch_rail = L_launch_rail - rocket.h_second_rail_button
-    effective_h_launch_rail = effective_L_launch_rail * np.cos(angle_to_vertical)
+    effective_h_launch_rail = effective_L_launch_rail * cos_rail_angle_to_vertical
 
     # Simulate flight from liftoff until the launch rail is cleared
     while height < effective_h_launch_rail:
         # Update environmental conditions based on height
         temperature = hfunc.temp_at_height(height, launchpad_temp, lapse_rate = T_lapse_rate)
         air_density = hfunc.air_density_optimized(temperature, multiplier,exponent)
 
@@ -117,16 +124,17 @@
         Cd_A_rocket = Cd_A_rocket_fn(Ma)
         q = hfunc.calculate_dynamic_pressure(air_density, speed)
         F_drag = q * Cd_A_rocket
 
         # Update rocket's motion parameters
         mass = hfunc.mass_at_time(time, dry_mass, fuel_mass_lookup)
         thrust = hfunc.thrust_at_time(time, engine_thrust_lookup)
-        a_y = (thrust - F_drag) * np.cos(angle_to_vertical) / mass - F_gravity
-        a_x = (thrust - F_drag) * np.sin(angle_to_vertical) / mass
+        a_rail = (thrust - F_drag) / mass - F_gravity * cos_rail_angle_to_vertical
+        a_y = a_rail * cos_rail_angle_to_vertical
+        a_x = a_rail * sin_rail_angle_to_vertical
         v_y += a_y * timestep
         v_x += a_x * timestep
         speed = np.sqrt(v_y**2 + v_x**2)
         height += v_y * timestep
 
         # Append updated simulation values
         simulated_values.append(
@@ -138,15 +146,14 @@
                 a_x,
                 v_y,
                 v_x,
                 temperature,
                 air_density,
                 q,
                 Ma,
-                Cd_A_rocket,
                 angle_to_vertical,
             ]
         )
         time += timestep
 
     launch_rail_cleared_index = len(simulated_values)
 
@@ -185,15 +192,14 @@
                 a_x,
                 v_y,
                 v_x,
                 temperature,
                 air_density,
                 q,
                 Ma,
-                Cd_A_rocket,
                 angle_to_vertical,
             ]
         )
 
         time += timestep
 
     burnout_index = len(simulated_values)
@@ -232,42 +238,41 @@
                 a_x,
                 v_y,
                 v_x,
                 temperature,
                 air_density,
                 q,
                 Ma,
-                Cd_A_rocket,
                 angle_to_vertical,
             ]
         )
 
         time += timestep
 
-    # Mark the index at apogee (highest point)
+    # Mark the index at apogee
     apogee_index = len(simulated_values)
-    simulated_values[-1][12] = simulated_values[-2][12]
+    simulated_values[-1][11] = simulated_values[-2][11]
 
     # Convert the list of simulation values to a DataFrame for easier analysis and visualization
     dataset = pd.DataFrame(
-        {
-            "time": [row[0] for row in simulated_values],
-            "height": [row[1] for row in simulated_values],
-            "speed": [row[2] for row in simulated_values],
-            "a_y": [row[3] for row in simulated_values],
-            "a_x": [row[4] for row in simulated_values],
-            "v_y": [row[5] for row in simulated_values],
-            "v_x": [row[6] for row in simulated_values],
-            "temperature": [row[7] for row in simulated_values],
-            "air_density": [row[8] for row in simulated_values],
-            "q": [row[9] for row in simulated_values],
-            "Ma": [row[10] for row in simulated_values],
-            "Cd_A_rocket": [row[11] for row in simulated_values],
-            "angle_to_vertical": [row[12] for row in simulated_values],
-        }
+        simulated_values,
+        columns=[
+            "time",
+            "height",
+            "speed",
+            "a_y",
+            "a_x",
+            "v_y",
+            "v_x",
+            "temperature",
+            "air_density",
+            "q",
+            "Ma",
+            "angle_to_vertical",
+        ],
     )
 
     return (
         dataset,
         liftoff_index,
         launch_rail_cleared_index,
         burnout_index,
@@ -277,22 +282,22 @@
 
 # Flight with airbrakes simulation function
 def simulate_airbrakes_flight(pre_brake_flight, rocket, launch_conditions, airbrakes, timestep = default_timestep):
     """
     Simulate the flight of a rocket during its post-burnout ascent with airbrakes deployed until apogee, given its specifications and environmental conditions.
 
     Args:
-    - pre_brake_flight (DataFrame): A DataFrame containing the simulation results from the rocket's ascent until burnout. # TODO: change to a tuple of the dataset at the time to start the simulation
+    - pre_brake_flight (DataFrame): A DataFrame containing the simulation results from the rocket's ascent until burnout. # TODO: maybe change to a tuple of the dataset at the time to start the simulation?
     - rocket (Rocket): An instance of the Rocket class.
     - launch_conditions (LaunchConditions): An instance of the LaunchConditions class.
     - airbrakes (Airbrakes): An instance of the Airbrakes class.
-    - timestep (float): The time increment for the simulation in seconds.
+    - timestep (float, optional): The time increment for the simulation in seconds.
 
     Returns:
-    - tuple: A tuple containing the dataset of simulation results and the time at which the airbrakes are fully deployed.
+    - DataFrame: A DataFrame containing the simulation results from the rocket's post-burnout ascent with airbrakes deployed until apogee.
     """
     # Extract rocket parameters
     mass = rocket.dry_mass
     Cd_A_rocket_fn = rocket.Cd_A_rocket
 
     # Extract launch condition parameters
     launchpad_temp = pre_brake_flight.temperature.iloc[0]
@@ -303,50 +308,44 @@
 
     # Calculate constants to be used in air density function
     multiplier = launchpad_pressure / (con.R_specific_air * pow(launchpad_temp, - F_gravity / (con.R_specific_air * T_lapse_rate)))
     exponent = - F_gravity / (con.R_specific_air * T_lapse_rate) - 1
 
     # Extract airbrakes parameters
     Cd_brakes = airbrakes.Cd_brakes
-    max_deployment_speed = np.deg2rad(airbrakes.max_deployment_speed)
+    max_deployment_rate = np.deg2rad(airbrakes.max_deployment_rate)
     max_deployment_angle = np.deg2rad(airbrakes.max_deployment_angle)
     A_brakes = airbrakes.num_flaps * airbrakes.A_flap
 
     pre_brake_flight["deployment_angle"] = 0
 
     # Initialize simulation variables
     height = pre_brake_flight["height"].iloc[-1]
     speed = pre_brake_flight["speed"].iloc[-1]
     v_y = pre_brake_flight["v_y"].iloc[-1]
     v_x = pre_brake_flight["v_x"].iloc[-1]
     time = pre_brake_flight["time"].iloc[-1]
     angle_to_vertical = np.arctan(v_x / v_y)
 
     deployment_angle = 0
-    time_recorded = False
 
     # for efficiency, may be removed if/when the simulation is made more accurate by the cd of the brakes changing during the sim:
     A_Cd_brakes = A_brakes * Cd_brakes
 
     simulated_values = []
     while v_y > 0:
         time += timestep
 
         temperature = hfunc.temp_at_height(height, launchpad_temp, lapse_rate = T_lapse_rate)
         air_density = hfunc.air_density_optimized(temperature, multiplier,exponent)
         Ma = hfunc.mach_number_fn(speed, temperature)
         Cd_A_rocket = Cd_A_rocket_fn(Ma)
         q = hfunc.calculate_dynamic_pressure(air_density, speed)
 
-        deployment_angle = min(max_deployment_angle, deployment_angle + max_deployment_speed * timestep)
-
-        if deployment_angle >= max_deployment_angle and not time_recorded:
-            time_of_max_deployment = time
-            time_recorded = True
-
+        deployment_angle = min(max_deployment_angle, deployment_angle + max_deployment_rate * timestep)
 
         F_drag = q * (np.sin(deployment_angle) * A_Cd_brakes + Cd_A_rocket)
         a_y = -F_drag * np.cos(angle_to_vertical) / mass - F_gravity
         a_x = -F_drag * np.sin(angle_to_vertical) / mass
         v_y += a_y * timestep
         v_x += a_x * timestep
         speed = np.sqrt(v_y**2 + v_x**2)
@@ -363,58 +362,35 @@
                 a_x,
                 v_y,
                 v_x,
                 temperature,
                 air_density,
                 q,
                 Ma,
-                Cd_A_rocket,
                 angle_to_vertical,
                 deployment_angle,
             ]
         )
 
-    simulated_values[-1][12] = simulated_values[-2][12]
-
-    data = {
-        "time": [row[0] for row in simulated_values],
-        "height": [row[1] for row in simulated_values],
-        "speed": [row[2] for row in simulated_values],
-        "a_y": [row[3] for row in simulated_values],
-        "a_x": [row[4] for row in simulated_values],
-        "v_y": [row[5] for row in simulated_values],
-        "v_x": [row[6] for row in simulated_values],
-        "temperature": [row[7] for row in simulated_values],
-        "air_density": [row[8] for row in simulated_values],
-        "q": [row[9] for row in simulated_values],
-        "Ma": [row[10] for row in simulated_values],
-        "Cd_A_rocket": [row[11] for row in simulated_values],
-        "angle_to_vertical": [row[12] for row in simulated_values],
-        "deployment_angle": [row[13] for row in simulated_values],
-    }
-
-    ascent = pd.concat([pre_brake_flight, pd.DataFrame(data)], ignore_index=True)
-
-    if not time_recorded:
-        time_of_max_deployment = time
+    simulated_values[-1][11] = simulated_values[-2][11]
 
-    return ascent, time_of_max_deployment
+    airbrakes_ascent = pd.DataFrame(
+        simulated_values,
+        columns=[
+            "time",
+            "height",
+            "speed",
+            "a_y",
+            "a_x",
+            "v_y",
+            "v_x",
+            "temperature",
+            "air_density",
+            "q",
+            "Ma",
+            "angle_to_vertical",
+            "deployment_angle",
+        ],
+    )
 
+    return airbrakes_ascent
 
-# TODO: move this to a test file
-    # run a couple hundred different timesteps in logspace between 0.001 and 0.1 to see how it changes to help pick a good timestep
-    
-"""    apogees = []
-    for timestep in np.logspace(-3, -1, 200):
-        dataset, liftoff_index, launch_rail_cleared_index, burnout_index, apogee_index = simulate_flight(rocket=Juno3_rocket, timestep=timestep)
-        ascent, time_of_max_deployment = simulate_airbrakes_flight(dataset.iloc[:burnout_index].copy(), rocket=Juno3_rocket, launch_conditions=Juno3_launch_conditions, timestep=0.001)
-        apogees.append(ascent["height"].iloc[-1]*3.28084)
-        print(len(apogees))
-    # plot them
-    import matplotlib.pyplot as plt
-    plt.plot(np.logspace(-3, -1, 200), apogees)
-    plt.xscale("log")
-    plt.xlabel("Timestep (s)")
-    plt.ylabel("Apogee (ft)")
-    plt.title("Apogee vs Timestep")
-    plt.show()"""
-
```

### Comparing `rocketflightsim-0.1.1/rocketflightsim/helper_functions.py` & `rocketflightsim-0.1.2/rocketflightsim/helper_functions.py`

 * *Files identical despite different names*

### Comparing `rocketflightsim-0.1.1/rocketflightsim/rocket_classes.py` & `rocketflightsim-0.1.2/rocketflightsim/rocket_classes.py`

 * *Files 16% similar despite different names*

```diff
@@ -180,49 +180,57 @@
     ----------
     num_flaps : int
         Number of airbrake flaps.
     A_flap : float
         Cross-sectional area of each flap (m^2).
     Cd_brakes : float
         Coefficient of drag of the airbrakes.
-    max_deployment_speed : float
-        Maximum speed at which the airbrakes can be deployed (deg/s).
     max_deployment_angle : float
-        Maximum angle that the flaps can deploy to (deg).
+        Maximum angle that the flaps can deploy to (deg).    
+    max_deployment_rate : float
+        Maximum rate at which the airbrakes can be deployed (deg/s).
+    max_retraction_rate : float
+        Maximum rate at which the airbrakes can be retracted (deg/s).
     """
 
     def __init__(
         self, 
         num_flaps : int,
         A_flap : float,
         Cd_brakes : float,
-        max_deployment_speed : float,
         max_deployment_angle : float,
+        max_deployment_rate : float,
+        max_retraction_rate : float = None,
     ):
         """Initializes the Airbrakes object.
 
         Parameters
         ----------
         num_flaps : int
             Number of airbrake flaps.
         A_flap : float
             Cross-sectional area of each flap (m^2).
         Cd_brakes : float
             Coefficient of drag of the airbrakes.
-        max_deployment_speed : float
-            Maximum speed at which the airbrakes can be deployed (deg/s).
         max_deployment_angle : float
             Maximum angle that the flaps can deploy to (deg).
+        max_deployment_rate : float
+            Maximum rate at which the airbrakes can be deployed (deg/s).
+        max_retraction_rate : float, optional
+            Maximum rate at which the airbrakes can be retracted (deg/s). Defaults to max_deployment_rate.
         """
         self.num_flaps = num_flaps
         self.A_flap = A_flap
         self.Cd_brakes = Cd_brakes
-        self.max_deployment_speed = max_deployment_speed
+        self.max_deployment_rate = max_deployment_rate
         self.max_deployment_angle = max_deployment_angle
-
+        if max_retraction_rate:
+            self.max_retraction_rate = max_retraction_rate
+        else:
+            self.max_retraction_rate = max_deployment_rate
 
 class PastFlight ():
     """
     Stores the rocket, launch conditions, and apogee of a past flight
     likely add more things like max speed, max acceleration later
     """
```

### Comparing `rocketflightsim-0.1.1/rocketflightsim.egg-info/PKG-INFO` & `rocketflightsim-0.1.2/rocketflightsim.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: rocketflightsim
-Version: 0.1.1
+Version: 0.1.2
 Summary: A lightweight rocket flight simulator.
 Home-page: https://github.com/werocketry/RocketFlightSim
 Author: Giorgio Chassikos, Western Engineering Rocketry Team
 Author-email: werocketry@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RocketFlightSim
 
-RocketFlightSim (RFS) is a light-weight flight simulator for experimental rockets. It currently supports simulation of single-stage rockets in the troposphere, from takeoff to apogee. Simple airbrakes can added to the rocket to induce drag. 
+RocketFlightSim (RFS) is a light-weight flight simulator for experimental rockets. It is designed to be simple to use, understand, and modify, with the goal of providing a platform for students and hobbyists to learn about rocket flight dynamics.
+
+The simulator currently supports simulation of single-stage rockets in the troposphere, from takeoff to apogee. Simple airbrakes can added to the rocket to induce drag. 
+
+A large emphasis is placed on computational efficiency, with the goal of being lightweight enough to run real-time during flight on an onboard microcontroller.
```

### Comparing `rocketflightsim-0.1.1/rocketflightsim.egg-info/SOURCES.txt` & `rocketflightsim-0.1.2/rocketflightsim.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 setup.py
 examples/__init__.py
 examples/example_configurations.py
 rocketflightsim/__init__.py
 rocketflightsim/constants.py
 rocketflightsim/flight_simulation.py
 rocketflightsim/helper_functions.py
-rocketflightsim/plotting_functions.py
 rocketflightsim/rocket_classes.py
 rocketflightsim.egg-info/PKG-INFO
 rocketflightsim.egg-info/SOURCES.txt
 rocketflightsim.egg-info/dependency_links.txt
 rocketflightsim.egg-info/requires.txt
 rocketflightsim.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `rocketflightsim-0.1.1/setup.py` & `rocketflightsim-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rocketflightsim',
-    version='0.1.1',
+    version='0.1.2',
     description='A lightweight rocket flight simulator.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Giorgio Chassikos, Western Engineering Rocketry Team',
     author_email='werocketry@gmail.com',
     url='https://github.com/werocketry/RocketFlightSim',
     packages=find_packages(),
```

### Comparing `rocketflightsim-0.1.1/tests/test_configs.py` & `rocketflightsim-0.1.2/tests/test_configs.py`

 * *Files 0% similar despite different names*

```diff
@@ -918,21 +918,21 @@
 )
 """ TODO: investigate why the sim performs so poorly on this flight compared to the others
 This is the flight that the sim is furthest off from predicting well. Possible reasons:
 - weak motor, short and quick flight leads to:
     - various small effects not accounted for in the sim made more significant
     - can't put the energy into wording it right now, but intuition
     - try simulating from burnout to apogee to see if the sim is more accurate there
-    - would wind have a larger effect?
+    - wind would have a larger effect
 - not confident in the values the notebook provides for the motor:
     - adding on the motor mass from thrustcurve.org, the sim gives an error of -14.76, instead of +24.63
         - also lended some credence due to the sim also underestimating the other 3 flights
     - was it even the K828FJ that was used?
         - the RocketPy paper says that total impulse of the "class K solid motor" used for the flight was 2120 Ns, but the notebook says 2070.99 Ns
             - https://www.researchgate.net/publication/354034513_RocketPy_Six_Degree-of-Freedom_Rocket_Trajectory_Simulator
 - using a constant Cd may not be a great approximation for a rocket hitting about Mach 0.25 
     - also, no mention of where the Cd value comes from. If it's ork or RasAero, it's likely not accurate. If it was CFD, they likely would have given a curve
 - no local variation in lapse rate from the standard lapse rate accounted for. Based on how it affects a 10k launch, it can improve the accuracy by about 0.3%, which might be another small factor
-Could diagnose more by comparing plots of data from the flight computer to plots from the sim, but a bit busy atm
+Could diagnose more by comparing plots of data from the flight computer to plots from the sim
 """
 
 past_flights = [NDRT_2020_flight, Valetudo_flight, Juno3_flight, Bella_Lui_flight]
```

### Comparing `rocketflightsim-0.1.1/tests/test_flight_simulation.py` & `rocketflightsim-0.1.2/tests/test_flight_simulation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import sys
 import os
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
 
 import unittest
-# from rocketflightsim import constants as con
-# from rocketflightsim import helper_functions as hfunc
+
 from rocketflightsim.rocket_classes import Motor, Rocket, LaunchConditions
 from rocketflightsim.flight_simulation import simulate_flight, simulate_airbrakes_flight
 
-from test_configs import past_flights
+from .test_configs import past_flights
+from .test_configs import Juno3_rocket, Juno3_launch_conditions
+
+from example_configurations import default_airbrakes_model
 
 class TestFlightSimulation(unittest.TestCase):
     def test_flight_simulation(self):
             print("Testing flight simulation")
 
             for flight in past_flights:
                 dataset, liftoff_index, launch_rail_cleared_index, burnout_index, apogee_index = simulate_flight(rocket=flight.rocket, launch_conditions=flight.launch_conditions, timestep=0.001)
@@ -22,26 +24,48 @@
                 difference = abs(apogee_simulated - apogee_actual)
                 proportional_difference = difference / apogee_actual
                 print(f"Flight {flight.name}: \n\tSimulated apogee: {round(apogee_simulated,2)} m\n\tActual apogee: {round(apogee_actual,2)} m\n\tDifference: {round(difference,2)} m\n\tPercent difference: {round(proportional_difference*100,2)}%\n")
 
                 assert proportional_difference < 0.1
             print("\n--------------------")
 
+class TestDefaultTimestep(unittest.TestCase):
+     def test_default_timestep(self):
+            print("Testing default timestep")
+            # TODO test to verify slight changes from the default timestep don't have a significant effect on the simulation results
+# from flight simulation file, used to pick the default timestep:
+
+# run a couple hundred different timesteps in logspace between 0.001 and 0.1 to see how it changes to help pick a good timestep
+"""apogees = []
+for timestep in np.logspace(-3, -1, 200):
+    dataset, liftoff_index, launch_rail_cleared_index, burnout_index, apogee_index = simulate_flight(rocket=Juno3_rocket, timestep=timestep)
+    ascent, time_of_max_deployment = simulate_airbrakes_flight(dataset.iloc[:burnout_index].copy(), rocket=Juno3_rocket, launch_conditions=Juno3_launch_conditions, timestep=0.001)
+    apogees.append(ascent["height"].iloc[-1]*3.28084)
+    print(len(apogees))
+# plot them
+import matplotlib.pyplot as plt
+plt.plot(np.logspace(-3, -1, 200), apogees)
+plt.xscale("log")
+plt.xlabel("Timestep (s)")
+plt.ylabel("Apogee (ft)")
+plt.title("Apogee vs Timestep")
+plt.show()"""
+
+# add a test to verify that the simulation doesn't take too long to run
+
 class TestAirbrakesFlightSimulation(unittest.TestCase):
      def test_airbrakes_flight_simulation(self):
             print("\n--------------------")
             print("Testing airbrakes flight simulation")
-            from test_configs import Juno3_rocket, Juno3_launch_conditions
-            from example_configurations import default_airbrakes_model
-    
+            
             dataset, liftoff_index, launch_rail_cleared_index, burnout_index, apogee_index = simulate_flight(rocket=Juno3_rocket, launch_conditions=Juno3_launch_conditions, timestep=0.001)
             print(f"Burnout: \n\tHeight: {dataset['height'].iloc[burnout_index - 1]} m\n\tSpeed: {dataset['speed'].iloc[burnout_index - 1]} m/s\n\tTime: {dataset['time'].iloc[burnout_index - 1]} s\n")
             print(f"No-airbraking apogee: \n\tHeight: {dataset['height'].iloc[apogee_index - 1]} m\n\tTime: {dataset['time'].iloc[apogee_index - 1]} s\n")
             # TODO: make it take the actual flight data at burnout and sim from there
-            ascent, time_of_max_deployment = simulate_airbrakes_flight(dataset.iloc[:burnout_index].copy(), rocket=Juno3_rocket, launch_conditions=Juno3_launch_conditions, airbrakes=default_airbrakes_model, timestep=0.001)
+            ascent = simulate_airbrakes_flight(dataset.iloc[:burnout_index].copy(), rocket=Juno3_rocket, launch_conditions=Juno3_launch_conditions, airbrakes=default_airbrakes_model, timestep=0.001)
             print(f"Airbrakes apogee: \n\tHeight: {ascent['height'].iloc[-1]} m\n\tTime: {ascent['time'].iloc[-1]} s\n\n")
             print("--------------------")
 
             assert ascent["height"].iloc[-1] > 1000
             assert ascent["height"].iloc[-1] < dataset["height"].iloc[apogee_index - 1]
             assert ascent["time"].iloc[-1] < dataset["time"].iloc[apogee_index - 1]
             # assert ascent["speed"].iloc[-1] < dataset["speed"].iloc[apogee_index - 1] ?
```

