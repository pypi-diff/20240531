# Comparing `tmp/objectnat-0.0.3.tar.gz` & `tmp/objectnat-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objectnat-0.0.3.tar", max compression
+gzip compressed data, was "objectnat-0.1.0.tar", max compression
```

## Comparing `objectnat-0.0.3.tar` & `objectnat-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,15 @@
--rw-r--r--   0        0        0     1231 2024-03-11 08:49:52.161769 objectnat-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2354 2024-03-07 18:17:15.789953 objectnat-0.0.3/README.md
--rw-r--r--   0        0        0      438 2024-03-11 08:47:41.514207 objectnat-0.0.3/src/objectnat/__init__.py
--rw-r--r--   0        0        0        0 2024-03-10 20:37:38.615235 objectnat-0.0.3/src/objectnat/methods/__init__.py
--rw-r--r--   0        0        0     1339 2024-03-10 20:37:39.944993 objectnat-0.0.3/src/objectnat/methods/adjacency_matrix.py
--rw-r--r--   0        0        0     2864 2024-03-11 09:10:43.900563 objectnat-0.0.3/src/objectnat/methods/balanced_buildings.py
--rw-r--r--   0        0        0     1633 2024-03-10 20:37:38.610234 objectnat-0.0.3/src/objectnat/methods/demands.py
--rw-r--r--   0        0        0     1453 2024-03-10 20:37:41.358667 objectnat-0.0.3/src/objectnat/methods/isochrones.py
--rw-r--r--   0        0        0     1047 2024-03-10 20:31:25.725502 objectnat-0.0.3/src/objectnat/methods/osm_graph.py
--rw-r--r--   0        0        0     5222 2024-03-10 20:37:39.953994 objectnat-0.0.3/src/objectnat/methods/provision.py
--rw-r--r--   0        0        0     3301 1970-01-01 00:00:00.000000 objectnat-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1498 2024-05-31 18:56:15.185407 objectnat-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     1302 2024-05-31 18:57:14.107422 objectnat-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3856 2024-05-31 18:56:15.185407 objectnat-0.1.0/README.md
+-rw-r--r--   0        0        0      767 2024-05-31 19:00:28.419584 objectnat-0.1.0/src/objectnat/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 18:26:18.453505 objectnat-0.1.0/src/objectnat/methods/__init__.py
+-rw-r--r--   0        0        0     1406 2024-05-31 18:56:15.191406 objectnat-0.1.0/src/objectnat/methods/adjacency_matrix.py
+-rw-r--r--   0        0        0     2864 2024-05-31 18:26:18.474028 objectnat-0.1.0/src/objectnat/methods/balanced_buildings.py
+-rw-r--r--   0        0        0     4650 2024-05-31 18:56:15.191406 objectnat-0.1.0/src/objectnat/methods/cluster_points_in_polygons.py
+-rw-r--r--   0        0        0     3288 2024-05-31 18:56:15.191406 objectnat-0.1.0/src/objectnat/methods/coverage_zones.py
+-rw-r--r--   0        0        0     1633 2024-05-31 18:26:18.452507 objectnat-0.1.0/src/objectnat/methods/demands.py
+-rw-r--r--   0        0        0     2291 2024-05-31 18:56:15.192407 objectnat-0.1.0/src/objectnat/methods/isochrones.py
+-rw-r--r--   0        0        0     1047 2024-05-31 18:26:18.455503 objectnat-0.1.0/src/objectnat/methods/osm_graph.py
+-rw-r--r--   0        0        0     5341 2024-05-31 18:56:15.192407 objectnat-0.1.0/src/objectnat/methods/provision.py
+-rw-r--r--   0        0        0    20662 2024-05-31 18:56:15.192407 objectnat-0.1.0/src/objectnat/methods/visibility_analysis.py
+-rw-r--r--   0        0        0     4933 1970-01-01 00:00:00.000000 objectnat-0.1.0/PKG-INFO
```

### Comparing `objectnat-0.0.3/pyproject.toml` & `objectnat-0.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 [tool.poetry]
 name = "ObjectNat"
-version = "0.0.3"
-description = ""
+version = "0.1.0"
+description = "ObjectNat is an open-source library created for geospatial analysis created by IDU team"
+license = "BSD-3-Clause"
 authors = ["Danila <63115678+DDonnyy@users.noreply.github.com>"]
 readme = "README.md"
 
 packages = [{ include = "objectnat", from = "src" }]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 geopandas = "^0.14.3"
-osmnx = "^1.9.1"
 tqdm = "^4.66.2"
-osm2geojson = "^0.2.4"
-pydantic = "^2.6.1"
-momepy = "^0.7.0"
 networkit = "^11.0"
 numpy = "^1.23.5"
 pandas = "^2.2.0"
 networkx = "^3.2.1"
 population-restorator = "^0.2.3"
-dongraphio = "^0.2.5"
-provisio = "^0.1.5"
-
-
-
+dongraphio = "^0.3.9"
+provisio = "^0.1.7"
+joblib = "^1.4.2"
+pandarallel = "^1.6.5"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.2.0"
 pylint = "^3.0.3"
 isort = "^5.13.2"
 jupyter = "^1.0.0"
```

### Comparing `objectnat-0.0.3/README.md` & `objectnat-0.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,74 @@
 # ObjectNat - Meta Library
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-
 <p align="center">
-<img src="./docs/img/logo.png" alt="test-logo" width="400"></a>
+<img src="https://i.ibb.co/FWtHNQv/logo.png" alt="logo" width="400">
 </p>
 
-**ObjectNat** is an open-source library created for geospatial analysis created by IDU team
+#### **ObjectNat** is an open-source library created for geospatial analysis created by **IDU team**
 
 ## ObjectNat Components
 
 - [dongraphio](https://github.com/DDonnyy/dongraphio) : `dongraphio` provides graph functions
 - [provisio](https://github.com/DDonnyy/provisio) : `provisio` provides main provisio fuctions
 - [population-restorator](https://github.com/kanootoko/population-restorator) : `restorator` provides city resettlement
 
 ## Features and how to use
 
-1. [City graph from OSM](./examples/graph_generator.ipynb) - Function to assemble a road, pedestrian, and public
+1. **[City graph from OSM](./examples/graph_generator.ipynb)** - Function to assemble a road, pedestrian, and public
    transport graph from OpenStreetMap (OSM) and creating Intermodal graph.
 
-   <img src="./docs/img/graphTara.png" alt="city_graph" width="300"></a>
-   
-2. [Adjacency matrix](./examples/calculate_adjacency_matrix.ipynb) - Calculate adjacency matrix based on the provided
+   <img src="https://i.ibb.co/VpsPgL1/Graph-generator-v1.webp" alt="Graph-generator-v1" height="250">
+
+2. **[Adjacency matrix](./examples/calculate_adjacency_matrix.ipynb)** - Calculate adjacency matrix based on the provided
    graph and edge weight type (time or distance). The intermodal graph can be obtained using the previous example.
-3. [Isochrones,transport accessibility](./examples/isochrone_generator.ipynb) - Function for generating isochrones to
+3. **[Isochrones,transport accessibility](./examples/isochrone_generator.ipynb)** - Function for generating isochrones to
    analyze transportation accessibility from specified starting coordinates. Isochrones can be constructed based on
    pedestrian, automobile, or public transport graphs, or a combination thereof.
 
-   <img src="./docs/img/isochronesTara.png" alt="isochrones" width="300"></a>
+   <img src="https://i.ibb.co/QM0tmZ2/isochrones-from-2-points.webp" alt="isochrones-from-2-points" height="250">
 
-4. [Population restoration](./examples/restore_population.ipynb) - Function for resettling population into the provided
+4. **[Population restoration](./examples/restore_population.ipynb)** - Function for resettling population into the provided
    layer of residential buildings. This function distributes people among dwellings based on the total city population
    and the living area of each house.
-5. [Service provision](./examples/calculate_provision.ipynb) - Function for calculating the provision of residential
+5. **[Service provision](./examples/calculate_provision.ipynb)** - Function for calculating the provision of residential
    buildings and population with services. In case of missing data, this function utilizes previously described
    functionality to retrieve the necessary information.
 
-   <img src="./docs/img/provisioTara.png" alt="isochrones" width="300"></a>
+   <img src="https://i.ibb.co/CW7Xj5F/Burger-Provision5min.webp" alt="Burger-Provision5min" height="250">
+   
+6. **[Visibility analysis](./examples/visibility_analysis.ipynb)** - Function to get a quick estimate of visibility from a
+   given point(s) to buildings within a given distance. Also, there is a visibility catchment area calculator for a
+   large
+   urban area. This function is designed to work with at least 1000 points spaced 10-20 meters apart for optimal
+   results. Points can be generated using a road graph and random point distribution along edges.
+
+   <img src="https://i.ibb.co/LxcGTfN/visibility-from-point.webp" alt="visibility-from-point" height="250"> 
+
+   <img src="https://i.ibb.co/zNRzXc5/visibility-catchment-area.webp" alt="visibility-catchment-area" height="250">
+
+7. **[Point clusterization](./examples/point_clusterization.ipynb)** - Function to generate cluster polygons for given
+   points based on a specified minimum distance and minimum points per cluster. Optionally, calculate the relative ratio
+   between types of services within the clusters.
+
+   <img src="https://i.ibb.co/fF3c4YC/service-clusterization.webp" alt="service-clusterization" height="250">
 
 ## Installation
 
-**ObjectNat** soon ~~can be installed with~~ ``pip``:
+**ObjectNat** can be installed with ``pip``:
 
 ```
 pip install ObjectNat
 ```
 
 ## Contacts
 
+- [NCCR](https://actcognitive.org/) - National
+  Center for Cognitive Research
+- [IDU](https://idu.itmo.ru/) - Institute of
+  Design and Urban Studies
+- [Natalya Chichkova](https://t.me/nancy_nat) - project manager
+- [Danila Oleynikov (Donny)](https://t.me/ddonny_dd) - lead software engineer
+
 ## Publications
```

### Comparing `objectnat-0.0.3/src/objectnat/methods/adjacency_matrix.py` & `objectnat-0.1.0/src/objectnat/methods/adjacency_matrix.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 def get_adjacency_matrix(
     buildings_from: gpd.GeoDataFrame,
     services_to: gpd.GeoDataFrame,
     weight: str,
     city_crs: int | None = None,
     nx_graph: nx.MultiDiGraph | None = None,
     dongraphio: DonGraphio | None = None,
+    graph_type=None,
 ) -> pd.DataFrame:
     """
     Get the adjacency matrix for the specified city graph, buildings, and services.
 
     Args:
         nx_graph (nx.Graph): The networkx graph.
         buildings_from (gpd.GeoDataFrame): GeoDataFrame representing buildings to build matrix from.
@@ -24,15 +25,15 @@
         weight (str): The weight attribute, could be only "time_min" or "length_meter".
 
     Returns:
         pd.DataFrame: The adjacency matrix.
     """
     try:
         if dongraphio:
-            return dongraphio.get_adjacency_matrix(buildings_from, services_to, weight)
+            return dongraphio.get_adjacency_matrix(buildings_from, services_to, weight, graph_type=graph_type)
 
         dongraphio = DonGraphio(city_crs)
         dongraphio.set_graph(nx_graph)
-        return dongraphio.get_adjacency_matrix(buildings_from, services_to, weight)
+        return dongraphio.get_adjacency_matrix(buildings_from, services_to, weight, graph_type=graph_type)
     except ValidationError as e:
         logger.error("Function get_adjacency_matrix() missing 'weight' argument")
         raise e
```

### Comparing `objectnat-0.0.3/src/objectnat/methods/balanced_buildings.py` & `objectnat-0.1.0/src/objectnat/methods/balanced_buildings.py`

 * *Files identical despite different names*

### Comparing `objectnat-0.0.3/src/objectnat/methods/demands.py` & `objectnat-0.1.0/src/objectnat/methods/demands.py`

 * *Files identical despite different names*

### Comparing `objectnat-0.0.3/src/objectnat/methods/osm_graph.py` & `objectnat-0.1.0/src/objectnat/methods/osm_graph.py`

 * *Files identical despite different names*

### Comparing `objectnat-0.0.3/src/objectnat/methods/provision.py` & `objectnat-0.1.0/src/objectnat/methods/provision.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,8 +122,14 @@
         city_graph = dngraph.get_intermodal_graph_from_osm(city_osm_id)
 
     dngraph.set_graph(city_graph)
 
     if calculate_matrix:
         adjacency_matrix = dngraph.get_adjacency_matrix(buildings, services, weight_adjacency_matrix)
 
-    return get_service_provision(services, adjacency_matrix, buildings, threshold, calculation_type)
+    return get_service_provision(
+        services=services,
+        adjacency_matrix=adjacency_matrix,
+        demanded_buildings=buildings,
+        threshold=threshold,
+        calculation_type=calculation_type,
+    )
```

