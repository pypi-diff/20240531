# Comparing `tmp/LearningNashQLearning-0.3.tar.gz` & `tmp/LearningNashQLearning-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LearningNashQLearning-0.3.tar", last modified: Tue May 28 11:06:03 2024, max compression
+gzip compressed data, was "LearningNashQLearning-0.4.tar", last modified: Fri May 31 11:51:11 2024, max compression
```

## Comparing `LearningNashQLearning-0.3.tar` & `LearningNashQLearning-0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 11:06:03.921835 LearningNashQLearning-0.3/
-drwxrwxrwx   0        0        0        0 2024-05-28 11:06:03.889946 LearningNashQLearning-0.3/LearningNashQLearning/
-drwxrwxrwx   0        0        0        0 2024-05-28 11:06:03.906827 LearningNashQLearning-0.3/LearningNashQLearning/Model/
--rw-rw-rw-   0        0        0      888 2024-05-28 08:48:57.000000 LearningNashQLearning-0.3/LearningNashQLearning/Model/Agent.py
--rw-rw-rw-   0        0        0    11859 2024-05-28 08:48:57.000000 LearningNashQLearning-0.3/LearningNashQLearning/Model/Environment.py
--rw-rw-rw-   0        0        0     1232 2024-05-28 08:48:57.000000 LearningNashQLearning-0.3/LearningNashQLearning/Model/History.py
--rw-rw-rw-   0        0        0    26997 2024-05-28 11:05:01.000000 LearningNashQLearning-0.3/LearningNashQLearning/Model/NashQLearning.py
--rw-rw-rw-   0        0        0        0 2024-05-25 16:18:54.000000 LearningNashQLearning-0.3/LearningNashQLearning/Model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 11:06:03.921835 LearningNashQLearning-0.3/LearningNashQLearning/View/
--rw-rw-rw-   0        0        0     3964 2024-05-25 16:38:41.000000 LearningNashQLearning-0.3/LearningNashQLearning/View/EnvGraphDisplay.py
--rw-rw-rw-   0        0        0    18670 2024-05-25 17:54:57.000000 LearningNashQLearning-0.3/LearningNashQLearning/View/FinalDisplay.py
--rw-rw-rw-   0        0        0    14709 2024-05-25 16:33:28.000000 LearningNashQLearning-0.3/LearningNashQLearning/View/GameEditor.py
--rw-rw-rw-   0        0        0     3457 2024-05-25 16:32:45.000000 LearningNashQLearning-0.3/LearningNashQLearning/View/GraphClass.py
--rw-rw-rw-   0        0        0    11881 2024-05-28 09:30:52.000000 LearningNashQLearning-0.3/LearningNashQLearning/View/PresetGames.py
--rw-rw-rw-   0        0        0        0 2024-05-25 16:35:10.000000 LearningNashQLearning-0.3/LearningNashQLearning/View/__init__.py
--rw-rw-rw-   0        0        0       43 2024-05-25 16:35:28.000000 LearningNashQLearning-0.3/LearningNashQLearning/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 11:06:03.906827 LearningNashQLearning-0.3/LearningNashQLearning.egg-info/
--rw-rw-rw-   0        0        0      423 2024-05-28 11:06:03.000000 LearningNashQLearning-0.3/LearningNashQLearning.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      747 2024-05-28 11:06:03.000000 LearningNashQLearning-0.3/LearningNashQLearning.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 11:06:03.000000 LearningNashQLearning-0.3/LearningNashQLearning.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-28 11:06:03.000000 LearningNashQLearning-0.3/LearningNashQLearning.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-05-28 11:06:03.000000 LearningNashQLearning-0.3/LearningNashQLearning.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      423 2024-05-28 11:06:03.921835 LearningNashQLearning-0.3/PKG-INFO
--rw-rw-rw-   0        0        0       23 2024-04-15 18:26:09.000000 LearningNashQLearning-0.3/README.md
--rw-rw-rw-   0        0        0      698 2024-05-28 11:05:31.000000 LearningNashQLearning-0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-28 11:06:03.921835 LearningNashQLearning-0.3/setup.cfg
--rw-rw-rw-   0        0        0      380 2024-05-28 11:05:39.000000 LearningNashQLearning-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:51:11.663005 LearningNashQLearning-0.4/
+drwxrwxrwx   0        0        0        0 2024-05-31 11:51:11.527145 LearningNashQLearning-0.4/LearningNashQLearning/
+drwxrwxrwx   0        0        0        0 2024-05-31 11:51:11.597004 LearningNashQLearning-0.4/LearningNashQLearning/Model/
+-rw-rw-rw-   0        0        0      888 2024-05-30 08:19:52.000000 LearningNashQLearning-0.4/LearningNashQLearning/Model/Agent.py
+-rw-rw-rw-   0        0        0    11859 2024-05-30 08:19:52.000000 LearningNashQLearning-0.4/LearningNashQLearning/Model/Environment.py
+-rw-rw-rw-   0        0        0     1232 2024-05-30 08:19:52.000000 LearningNashQLearning-0.4/LearningNashQLearning/Model/History.py
+-rw-rw-rw-   0        0        0    26997 2024-05-30 08:19:52.000000 LearningNashQLearning-0.4/LearningNashQLearning/Model/NashQLearning.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 08:19:52.000000 LearningNashQLearning-0.4/LearningNashQLearning/Model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:51:11.663005 LearningNashQLearning-0.4/LearningNashQLearning/View/
+-rw-rw-rw-   0        0        0     3964 2024-05-30 08:19:52.000000 LearningNashQLearning-0.4/LearningNashQLearning/View/EnvGraphDisplay.py
+-rw-rw-rw-   0        0        0    18664 2024-05-31 11:50:27.000000 LearningNashQLearning-0.4/LearningNashQLearning/View/FinalDisplay.py
+-rw-rw-rw-   0        0        0    14709 2024-05-30 08:19:52.000000 LearningNashQLearning-0.4/LearningNashQLearning/View/GameEditor.py
+-rw-rw-rw-   0        0        0     3437 2024-05-31 11:50:16.000000 LearningNashQLearning-0.4/LearningNashQLearning/View/GraphClass.py
+-rw-rw-rw-   0        0        0    11881 2024-05-30 08:19:52.000000 LearningNashQLearning-0.4/LearningNashQLearning/View/PresetGames.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 08:19:52.000000 LearningNashQLearning-0.4/LearningNashQLearning/View/__init__.py
+-rw-rw-rw-   0        0        0       43 2024-05-30 08:19:52.000000 LearningNashQLearning-0.4/LearningNashQLearning/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:51:11.578997 LearningNashQLearning-0.4/LearningNashQLearning.egg-info/
+-rw-rw-rw-   0        0        0      423 2024-05-31 11:51:11.000000 LearningNashQLearning-0.4/LearningNashQLearning.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      747 2024-05-31 11:51:11.000000 LearningNashQLearning-0.4/LearningNashQLearning.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 11:51:11.000000 LearningNashQLearning-0.4/LearningNashQLearning.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-31 11:51:11.000000 LearningNashQLearning-0.4/LearningNashQLearning.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-31 11:51:11.000000 LearningNashQLearning-0.4/LearningNashQLearning.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      423 2024-05-31 11:51:11.663005 LearningNashQLearning-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       23 2024-05-30 08:19:52.000000 LearningNashQLearning-0.4/README.md
+-rw-rw-rw-   0        0        0      698 2024-05-31 11:50:37.000000 LearningNashQLearning-0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-31 11:51:11.663005 LearningNashQLearning-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      380 2024-05-31 11:50:55.000000 LearningNashQLearning-0.4/setup.py
```

### Comparing `LearningNashQLearning-0.3/LearningNashQLearning/Model/Agent.py` & `LearningNashQLearning-0.4/LearningNashQLearning/Model/Agent.py`

 * *Files identical despite different names*

### Comparing `LearningNashQLearning-0.3/LearningNashQLearning/Model/Environment.py` & `LearningNashQLearning-0.4/LearningNashQLearning/Model/Environment.py`

 * *Files identical despite different names*

### Comparing `LearningNashQLearning-0.3/LearningNashQLearning/Model/History.py` & `LearningNashQLearning-0.4/LearningNashQLearning/Model/History.py`

 * *Files identical despite different names*

### Comparing `LearningNashQLearning-0.3/LearningNashQLearning/Model/NashQLearning.py` & `LearningNashQLearning-0.4/LearningNashQLearning/Model/NashQLearning.py`

 * *Files identical despite different names*

### Comparing `LearningNashQLearning-0.3/LearningNashQLearning/View/EnvGraphDisplay.py` & `LearningNashQLearning-0.4/LearningNashQLearning/View/EnvGraphDisplay.py`

 * *Files identical despite different names*

### Comparing `LearningNashQLearning-0.3/LearningNashQLearning/View/FinalDisplay.py` & `LearningNashQLearning-0.4/LearningNashQLearning/View/FinalDisplay.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,15 +254,15 @@
             return
 
         for i, qTable in enumerate(qTables):
             for j, game in enumerate(qTable):
                 for k, q in enumerate(game):
                     for l, qCouple in enumerate(q):
                         for m, qValue in enumerate(qCouple):
-                            self.qTableWidget.children[i].children[j].children[k*len(qCouple) + l].children[m].value = str(
+                            self.qTableWidget.children[i].children[j].children[k*len(q) + l].children[m].value = str(
                                 qValue)
 
     def setCurrentPolicy(self, policy):
         self.currentPolicyWidget.children = []
         for i, playerPolicy in enumerate(policy):
             playerPolicyWidget = widgets.HBox()
             label = widgets.Label(value='Player ' + str(i) + ':')
```

### Comparing `LearningNashQLearning-0.3/LearningNashQLearning/View/GameEditor.py` & `LearningNashQLearning-0.4/LearningNashQLearning/View/GameEditor.py`

 * *Files identical despite different names*

### Comparing `LearningNashQLearning-0.3/LearningNashQLearning/View/GraphClass.py` & `LearningNashQLearning-0.4/LearningNashQLearning/View/GraphClass.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,16 @@
             self.edge_colors.update({edge: 'black'})
 
         return self
 
     def plotGraph(self, ax: plt.Axes):
         ax.cla()
         self.updateLabelsFromActionLabels()
-        Graph(self.graph, node_labels=True, node_layout='circular', edge_labels=self.edge_labels, edge_label_fontdict=dict(size=10, fontweight='bold'), edge_layout='arc', node_size=10,
-              edge_width=0.5, arrows=True, ax=ax, node_edge_color=self.node_colors, node_label_fontdict=dict(size=10), edge_label_position=0.5, edge_labels_rotate=False, edge_color=self.edge_colors)
+        Graph(self.graph, node_labels=True, node_layout='circular', edge_labels=self.edge_labels, edge_label_fontdict=dict(size=8), edge_layout='arc', node_size=10,
+              edge_width=0.5, arrows=True, ax=ax, node_edge_color=self.node_colors, node_label_fontdict=dict(size=10), edge_label_position=0.3, edge_labels_rotate=False, edge_color=self.edge_colors)
 
     def current_state_set(self, state):
         for node in list(self.graph.nodes):
             if node == state:
                 self.node_colors.update({node: 'red'})
             else:
                 self.node_colors.update({node: 'blue'})
```

### Comparing `LearningNashQLearning-0.3/LearningNashQLearning/View/PresetGames.py` & `LearningNashQLearning-0.4/LearningNashQLearning/View/PresetGames.py`

 * *Files identical despite different names*

### Comparing `LearningNashQLearning-0.3/LearningNashQLearning.egg-info/SOURCES.txt` & `LearningNashQLearning-0.4/LearningNashQLearning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LearningNashQLearning-0.3/pyproject.toml` & `LearningNashQLearning-0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "LearningNashQLearning"
-version = "0.3"
+version = "0.4"
 description = "A simple NashQ-learning implementation in Python"
 readme = "README.md"
 authors = [{ name = "Paolo Ginefra" }, { name = "Federico Rocca"}, { name = "Andrea Tarabotto" }]
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

