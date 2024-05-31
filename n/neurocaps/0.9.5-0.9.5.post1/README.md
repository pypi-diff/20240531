# Comparing `tmp/neurocaps-0.9.5.tar.gz` & `tmp/neurocaps-0.9.5.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurocaps-0.9.5.tar", last modified: Thu May 30 18:29:22 2024, max compression
+gzip compressed data, was "neurocaps-0.9.5.post1.tar", last modified: Thu May 30 21:54:52 2024, max compression
```

## Comparing `neurocaps-0.9.5.tar` & `neurocaps-0.9.5.post1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 18:29:22.563119 neurocaps-0.9.5/
--rw-rw-rw-   0        0        0     1077 2024-05-29 20:07:23.000000 neurocaps-0.9.5/LICENSE.md
--rw-rw-rw-   0        0        0       11 2024-05-29 20:41:29.000000 neurocaps-0.9.5/MANIFEST.in
--rw-rw-rw-   0        0        0    18746 2024-05-30 18:29:22.563119 neurocaps-0.9.5/PKG-INFO
--rw-rw-rw-   0        0        0    17191 2024-05-30 18:27:19.000000 neurocaps-0.9.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 18:29:22.486673 neurocaps-0.9.5/neurocaps/
--rw-rw-rw-   0        0        0       72 2024-05-27 18:25:53.000000 neurocaps-0.9.5/neurocaps/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 18:29:22.523719 neurocaps-0.9.5/neurocaps/_utils/
--rw-rw-rw-   0        0        0      363 2024-05-27 18:25:53.000000 neurocaps-0.9.5/neurocaps/_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 18:29:22.534387 neurocaps-0.9.5/neurocaps/_utils/_cap_internals/
--rw-rw-rw-   0        0        0       88 2024-04-28 16:38:21.000000 neurocaps-0.9.5/neurocaps/_utils/_cap_internals/__init__.py
--rw-rw-rw-   0        0        0     2531 2024-05-27 18:25:53.000000 neurocaps-0.9.5/neurocaps/_utils/_cap_internals/_capgetter.py
--rw-rw-rw-   0        0        0      184 2024-05-27 18:25:53.000000 neurocaps-0.9.5/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
-drwxrwxrwx   0        0        0        0 2024-05-30 18:29:22.542200 neurocaps-0.9.5/neurocaps/_utils/_timeseriesextractor_internals/
--rw-rw-rw-   0        0        0      238 2024-05-23 03:16:17.000000 neurocaps-0.9.5/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
--rw-rw-rw-   0        0        0     2187 2024-05-27 18:25:53.000000 neurocaps-0.9.5/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py
--rw-rw-rw-   0        0        0     5777 2024-05-27 18:25:53.000000 neurocaps-0.9.5/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
--rw-rw-rw-   0        0        0     8190 2024-05-27 18:25:53.000000 neurocaps-0.9.5/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
--rw-rw-rw-   0        0        0     2680 2024-05-27 18:25:53.000000 neurocaps-0.9.5/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
-drwxrwxrwx   0        0        0        0 2024-05-30 18:29:22.549153 neurocaps-0.9.5/neurocaps/analysis/
--rw-rw-rw-   0        0        0      139 2024-05-27 18:25:53.000000 neurocaps-0.9.5/neurocaps/analysis/__init__.py
--rw-rw-rw-   0        0        0    75038 2024-05-30 17:55:51.000000 neurocaps-0.9.5/neurocaps/analysis/cap.py
--rw-rw-rw-   0        0        0     4791 2024-05-27 18:25:53.000000 neurocaps-0.9.5/neurocaps/analysis/merge.py
--rw-rw-rw-   0        0        0     1626 2024-05-27 18:25:53.000000 neurocaps-0.9.5/neurocaps/analysis/standardize.py
-drwxrwxrwx   0        0        0        0 2024-05-30 18:29:22.549153 neurocaps-0.9.5/neurocaps/extraction/
--rw-rw-rw-   0        0        0       87 2024-05-27 18:25:53.000000 neurocaps-0.9.5/neurocaps/extraction/__init__.py
--rw-rw-rw-   0        0        0    33356 2024-05-27 18:25:53.000000 neurocaps-0.9.5/neurocaps/extraction/timeseriesextractor.py
-drwxrwxrwx   0        0        0        0 2024-05-30 18:29:22.563119 neurocaps-0.9.5/neurocaps.egg-info/
--rw-rw-rw-   0        0        0    18746 2024-05-30 18:29:22.000000 neurocaps-0.9.5/neurocaps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      955 2024-05-30 18:29:22.000000 neurocaps-0.9.5/neurocaps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 18:29:22.000000 neurocaps-0.9.5/neurocaps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      150 2024-05-30 18:29:22.000000 neurocaps-0.9.5/neurocaps.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-30 18:29:22.000000 neurocaps-0.9.5/neurocaps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1725 2024-05-30 07:32:22.000000 neurocaps-0.9.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-30 18:29:22.563119 neurocaps-0.9.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-30 21:54:52.369709 neurocaps-0.9.5.post1/
+-rw-rw-rw-   0        0        0     1077 2024-05-29 20:07:23.000000 neurocaps-0.9.5.post1/LICENSE.md
+-rw-rw-rw-   0        0        0       11 2024-05-29 20:41:29.000000 neurocaps-0.9.5.post1/MANIFEST.in
+-rw-rw-rw-   0        0        0    18752 2024-05-30 21:54:52.368165 neurocaps-0.9.5.post1/PKG-INFO
+-rw-rw-rw-   0        0        0    17191 2024-05-30 18:27:19.000000 neurocaps-0.9.5.post1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 21:54:52.330006 neurocaps-0.9.5.post1/neurocaps/
+-rw-rw-rw-   0        0        0       72 2024-05-27 18:25:53.000000 neurocaps-0.9.5.post1/neurocaps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 21:54:52.347556 neurocaps-0.9.5.post1/neurocaps/_utils/
+-rw-rw-rw-   0        0        0      363 2024-05-27 18:25:53.000000 neurocaps-0.9.5.post1/neurocaps/_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 21:54:52.352207 neurocaps-0.9.5.post1/neurocaps/_utils/_cap_internals/
+-rw-rw-rw-   0        0        0       88 2024-04-28 16:38:21.000000 neurocaps-0.9.5.post1/neurocaps/_utils/_cap_internals/__init__.py
+-rw-rw-rw-   0        0        0     2531 2024-05-27 18:25:53.000000 neurocaps-0.9.5.post1/neurocaps/_utils/_cap_internals/_capgetter.py
+-rw-rw-rw-   0        0        0      184 2024-05-27 18:25:53.000000 neurocaps-0.9.5.post1/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
+drwxrwxrwx   0        0        0        0 2024-05-30 21:54:52.358292 neurocaps-0.9.5.post1/neurocaps/_utils/_timeseriesextractor_internals/
+-rw-rw-rw-   0        0        0      238 2024-05-23 03:16:17.000000 neurocaps-0.9.5.post1/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
+-rw-rw-rw-   0        0        0     2187 2024-05-27 18:25:53.000000 neurocaps-0.9.5.post1/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py
+-rw-rw-rw-   0        0        0     5777 2024-05-27 18:25:53.000000 neurocaps-0.9.5.post1/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
+-rw-rw-rw-   0        0        0     8190 2024-05-27 18:25:53.000000 neurocaps-0.9.5.post1/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
+-rw-rw-rw-   0        0        0     2680 2024-05-27 18:25:53.000000 neurocaps-0.9.5.post1/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
+drwxrwxrwx   0        0        0        0 2024-05-30 21:54:52.363408 neurocaps-0.9.5.post1/neurocaps/analysis/
+-rw-rw-rw-   0        0        0      139 2024-05-27 18:25:53.000000 neurocaps-0.9.5.post1/neurocaps/analysis/__init__.py
+-rw-rw-rw-   0        0        0    75723 2024-05-30 21:34:56.000000 neurocaps-0.9.5.post1/neurocaps/analysis/cap.py
+-rw-rw-rw-   0        0        0     4791 2024-05-27 18:25:53.000000 neurocaps-0.9.5.post1/neurocaps/analysis/merge.py
+-rw-rw-rw-   0        0        0     1626 2024-05-27 18:25:53.000000 neurocaps-0.9.5.post1/neurocaps/analysis/standardize.py
+drwxrwxrwx   0        0        0        0 2024-05-30 21:54:52.364484 neurocaps-0.9.5.post1/neurocaps/extraction/
+-rw-rw-rw-   0        0        0       87 2024-05-27 18:25:53.000000 neurocaps-0.9.5.post1/neurocaps/extraction/__init__.py
+-rw-rw-rw-   0        0        0    33356 2024-05-27 18:25:53.000000 neurocaps-0.9.5.post1/neurocaps/extraction/timeseriesextractor.py
+drwxrwxrwx   0        0        0        0 2024-05-30 21:54:52.365899 neurocaps-0.9.5.post1/neurocaps.egg-info/
+-rw-rw-rw-   0        0        0    18752 2024-05-30 21:54:52.000000 neurocaps-0.9.5.post1/neurocaps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      955 2024-05-30 21:54:52.000000 neurocaps-0.9.5.post1/neurocaps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 21:54:52.000000 neurocaps-0.9.5.post1/neurocaps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      150 2024-05-30 21:54:52.000000 neurocaps-0.9.5.post1/neurocaps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-30 21:54:52.000000 neurocaps-0.9.5.post1/neurocaps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1731 2024-05-30 21:22:42.000000 neurocaps-0.9.5.post1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 21:54:52.369709 neurocaps-0.9.5.post1/setup.cfg
```

### Comparing `neurocaps-0.9.5/LICENSE.md` & `neurocaps-0.9.5.post1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.5/PKG-INFO` & `neurocaps-0.9.5.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.9.5
+Version: 0.9.5.post1
 Summary: Co-activation Patterns (CAPs) Python package
 Author-email: Donisha Smith <donishasmith@outlook.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
 Project-URL: Issues, https://github.com/donishadsmith/neurocaps/issues
 Project-URL: Changelog, https://github.com/donishadsmith/neurocaps/blob/main/CHANGELOG.md
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
```

### Comparing `neurocaps-0.9.5/README.md` & `neurocaps-0.9.5.post1/README.md`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.5/neurocaps/_utils/_cap_internals/_capgetter.py` & `neurocaps-0.9.5.post1/neurocaps/_utils/_cap_internals/_capgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.5/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py` & `neurocaps-0.9.5.post1/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.5/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py` & `neurocaps-0.9.5.post1/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.5/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py` & `neurocaps-0.9.5.post1/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.5/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py` & `neurocaps-0.9.5.post1/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.5/neurocaps/analysis/cap.py` & `neurocaps-0.9.5.post1/neurocaps/analysis/cap.py`

 * *Files 2% similar despite different names*

```diff
@@ -330,14 +330,16 @@
                 Rotation angle for x-axis labels.
             - "ylabel_rotation": int, default=0
                 Rotation angle for y-axis labels.
             - "annot": bool, default=False
                 Add values to cells on the outer product heatmap at the region level only.
             - "linewidths": float, default=0
                 Padding between each cell in the plot.
+            - "linecolor": str, default="black"
+                Color of the line that seperates each cell.
             - "cmap": str, Class, or function, default="coolwarm"
                 Color map for the cells in the plot. For this parameter, you can use premade color palettes or create custom ones.
                 Below is a list of valid options:
                 - Strings to call seaborn's premade palettes. Refer to seaborn's documentation for valid options.
                 - Seaborn's diverging_palette function to generate custom palettes.
                 - Matplotlib's LinearSegmentedColormap to generate custom palettes.
                 - Other classes or functions compatible with seaborn.
@@ -411,14 +413,15 @@
                         tight_layout = kwargs["tight_layout"] if kwargs and "tight_layout" in kwargs.keys() else True,
                         rect = kwargs["rect"] if kwargs and "rect" in kwargs.keys() else [0, 0.03, 1, 0.95],
                         sharey = kwargs["sharey"] if kwargs and "sharey" in kwargs.keys() else True,
                         xlabel_rotation = kwargs["xlabel_rotation"] if kwargs and "xlabel_rotation" in kwargs.keys() else 0,
                         ylabel_rotation = kwargs["ylabel_rotation"] if kwargs and "ylabel_rotation" in kwargs.keys() else 0,
                         annot = kwargs["annot"] if kwargs and "annot" in kwargs.keys() else False,
                         linewidths = kwargs["linewidths"] if kwargs and "linewidths" in kwargs.keys() else 0,
+                        linecolor = kwargs["linecolor"] if kwargs and "linecolor" in kwargs.keys() else "black",
                         cmap = kwargs["cmap"] if kwargs and "cmap" in kwargs.keys() else "coolwarm"
                         )
         
         if kwargs:
             invalid_kwargs = {key : value for key, value in kwargs.items() if key not in plot_dict.keys()}
             if len(invalid_kwargs.keys()) > 0:
                 print(f"Invalid kwargs arguments used and will be ignored {invalid_kwargs}.")
@@ -537,17 +540,17 @@
                         starting_value += frequency_dict[names_list[num-1]] 
                         labels[starting_value] = name
 
             if subplots: 
                 ax = axes[axes_y] if nrow == 1 else axes[axes_x,axes_y]
                 # Modify tick labels based on scope
                 if scope == "regions":
-                    display = heatmap(ax=ax, data=self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], xticklabels=columns, yticklabels=columns, cbar_kws={"shrink": plot_dict["shrink"]}, annot=plot_dict["annot"])
+                    display = heatmap(ax=ax, data=self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], linecolor=plot_dict["linecolor"], xticklabels=columns, yticklabels=columns, cbar_kws={"shrink": plot_dict["shrink"]}, annot=plot_dict["annot"])
                 else:
-                    display = heatmap(ax=ax, data=self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], cbar_kws={"shrink": plot_dict["shrink"]})
+                    display = heatmap(ax=ax, data=self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], linecolor=plot_dict["linecolor"], cbar_kws={"shrink": plot_dict["shrink"]})
 
                     ticks = [i for i, label in enumerate(labels) if label]  
 
                     ax.set_xticks(ticks)  
                     ax.set_xticklabels([label for label in labels if label]) 
                     ax.set_yticks(ticks)  
                     ax.set_yticklabels([label for label in labels if label]) 
@@ -571,17 +574,17 @@
                     axes_y += 1
 
             else:
                 # Create new plot for each iteration when not subplot
                 plt.figure(figsize=plot_dict["figsize"])
 
                 plot_title = f"{group} {cap} {task_title}" if task_title else f"{group} {cap}"
-                if scope == "regions": display = heatmap(self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], xticklabels=columns, yticklabels=columns, cbar_kws={'shrink': plot_dict["shrink"]})
+                if scope == "regions": display = heatmap(self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], linecolor=plot_dict["linecolor"], xticklabels=columns, yticklabels=columns, cbar_kws={'shrink': plot_dict["shrink"]})
                 else: 
-                    display = heatmap(self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], xticklabels=[], yticklabels=[], cbar_kws={'shrink': plot_dict["shrink"]})
+                    display = heatmap(self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], linecolor=plot_dict["linecolor"], xticklabels=[], yticklabels=[], cbar_kws={'shrink': plot_dict["shrink"]})
                     ticks = [i for i, label in enumerate(labels) if label]  
 
                     display.set_xticks(ticks)  
                     display.set_xticklabels([label for label in labels if label]) 
                     display.set_yticks(ticks)  
                     display.set_yticklabels([label for label in labels if label]) 
                 
@@ -612,15 +615,15 @@
         import matplotlib.pyplot as plt, os, pandas as pd
         from seaborn import heatmap
         
         # Initialize new grid
         plt.figure(figsize=plot_dict["figsize"])
 
         if scope == "regions": 
-            display = heatmap(pd.DataFrame(cap_dict[group], index=columns), xticklabels=True, yticklabels=True, cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], cbar_kws={'shrink': plot_dict["shrink"]}) 
+            display = heatmap(pd.DataFrame(cap_dict[group], index=columns), xticklabels=True, yticklabels=True, cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], linecolor=plot_dict["linecolor"], cbar_kws={'shrink': plot_dict["shrink"]}) 
         else: 
             # Create Labels
             import collections
             if list(self._parcel_approach.keys())[0] == "Schaefer":
                 frequency_dict = dict(collections.Counter([names[0] + " " + names[1] for names in [name.split("_")[0:2] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]]]))
             elif list(self._parcel_approach.keys())[0] == "AAL":
                 frequency_dict = collections.Counter([name.split("_")[0] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]])
@@ -640,15 +643,15 @@
                 if num == 0:
                     labels[0] = name
                 else:
                     # Shifting to previous frequency of the preceding netwerk to obtain the new starting value of the subsequent region and hemosphere pair
                     starting_value += frequency_dict[names_list[num-1]] 
                     labels[starting_value] = name
 
-            display = heatmap(pd.DataFrame(cap_dict[group], columns=cap_dict[group].keys()), xticklabels=True, yticklabels=True, cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], cbar_kws={'shrink': plot_dict["shrink"]})
+            display = heatmap(pd.DataFrame(cap_dict[group], columns=cap_dict[group].keys()), xticklabels=True, yticklabels=True, cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], linecolor=plot_dict["linecolor"], cbar_kws={'shrink': plot_dict["shrink"]})
 
             plt.yticks(ticks=[pos for pos, label in enumerate(labels) if label], labels=names_list)  
 
         display.set_xticklabels(display.get_xticklabels(), size = plot_dict["xticklabels_size"], rotation=plot_dict["xlabel_rotation"])
         display.set_yticklabels(display.get_yticklabels(), size = plot_dict["yticklabels_size"], rotation=plot_dict["ylabel_rotation"])
 
         plot_title = f"{group} CAPs {task_title}" if task_title else f"{group} CAPs" 
@@ -878,14 +881,16 @@
                 Rotation angle for x-axis labels.
             - "ylabel_rotation": int, default=0
                 Rotation angle for y-axis labels.
             - "annot": bool, default=False
                 Add values to each cell.
             - "linewidths": float, default=0
                 Padding between each cell in the plot.
+            - "linecolor": str, default="black"
+                Color of the line that seperates each cell.
             - "cmap": str, Class, or function, default="coolwarm"
                 Color map for the cells in the plot. For this parameter, you can use premade color palettes or create custom ones.
                 Below is a list of valid options:
                 - Strings to call seaborn's premade palettes. Refer to seaborn's documentation for valid options.
                 - Seaborn's diverging_palette function to generate custom palettes.
                 - Matplotlib's LinearSegmentedColormap to generate custom palettes.
                 - Other classes or functions compatible with seaborn.
@@ -903,28 +908,29 @@
                         xticklabels_size = kwargs["xticklabels_size"] if kwargs and "xticklabels_size" in kwargs.keys() else 8,
                         yticklabels_size = kwargs["yticklabels_size"] if kwargs and "yticklabels_size" in kwargs.keys() else 8,
                         shrink = kwargs["shrink"] if kwargs and "shrink" in kwargs.keys() else 0.8,
                         xlabel_rotation = kwargs["xlabel_rotation"] if kwargs and "xlabel_rotation" in kwargs.keys() else 0,
                         ylabel_rotation = kwargs["ylabel_rotation"] if kwargs and "ylabel_rotation" in kwargs.keys() else 0,
                         annot = kwargs["annot"] if kwargs and "annot" in kwargs.keys() else False,
                         linewidths = kwargs["linewidths"] if kwargs and "linewidths" in kwargs.keys() else 0,
+                        linecolor = kwargs["linecolor"] if kwargs and "linecolor" in kwargs.keys() else "black",
                         cmap = kwargs["cmap"] if kwargs and "cmap" in kwargs.keys() else "coolwarm"
                         )
         
         if kwargs:
             invalid_kwargs = {key : value for key, value in kwargs.items() if key not in plot_dict.keys()}
             if len(invalid_kwargs.keys()) > 0:
                 print(f"Invalid kwargs arguments used and will be ignored {invalid_kwargs}.")
 
         for group in self.caps.keys():
             # Refresh grid for each iteration
             plt.figure(figsize=plot_dict["figsize"])
 
             df = pd.DataFrame(self.caps[group])
-            display = heatmap(df.corr(), xticklabels=True, yticklabels=True, cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], 
+            display = heatmap(df.corr(), xticklabels=True, yticklabels=True, cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], linecolor=plot_dict["linecolor"],
                               cbar_kws={'shrink': plot_dict["shrink"]}, annot=plot_dict["annot"]) 
             # Modify label sizes
             display.set_xticklabels(display.get_xticklabels(), size = plot_dict["xticklabels_size"], rotation=plot_dict["xlabel_rotation"])
             display.set_yticklabels(display.get_yticklabels(), size = plot_dict["yticklabels_size"], rotation=plot_dict["ylabel_rotation"])
             # Set plot name
             plot_title = f"{group} - CAPs Correlation Matrix" 
             display.set_title(plot_title, fontdict= {'fontsize': plot_dict["fontsize"]})
```

### Comparing `neurocaps-0.9.5/neurocaps/analysis/merge.py` & `neurocaps-0.9.5.post1/neurocaps/analysis/merge.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.5/neurocaps/analysis/standardize.py` & `neurocaps-0.9.5.post1/neurocaps/analysis/standardize.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.5/neurocaps/extraction/timeseriesextractor.py` & `neurocaps-0.9.5.post1/neurocaps/extraction/timeseriesextractor.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.5/neurocaps.egg-info/PKG-INFO` & `neurocaps-0.9.5.post1/neurocaps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.9.5
+Version: 0.9.5.post1
 Summary: Co-activation Patterns (CAPs) Python package
 Author-email: Donisha Smith <donishasmith@outlook.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
 Project-URL: Issues, https://github.com/donishadsmith/neurocaps/issues
 Project-URL: Changelog, https://github.com/donishadsmith/neurocaps/blob/main/CHANGELOG.md
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
```

### Comparing `neurocaps-0.9.5/neurocaps.egg-info/SOURCES.txt` & `neurocaps-0.9.5.post1/neurocaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.5/pyproject.toml` & `neurocaps-0.9.5.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,107 +2,108 @@
 00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
 00000020: 7570 746f 6f6c 7322 2c20 2277 6865 656c  uptools", "wheel
 00000030: 225d 0d0a 6275 696c 642d 6261 636b 656e  "]..build-backen
 00000040: 6420 3d20 2273 6574 7570 746f 6f6c 732e  d = "setuptools.
 00000050: 6275 696c 645f 6d65 7461 220d 0a0d 0a5b  build_meta"....[
 00000060: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000070: 2022 6e65 7572 6f63 6170 7322 0d0a 7665   "neurocaps"..ve
-00000080: 7273 696f 6e20 3d20 2230 2e39 2e35 220d  rsion = "0.9.5".
-00000090: 0a6c 6963 656e 7365 203d 207b 7465 7874  .license = {text
-000000a0: 203d 2022 4d49 5420 4c69 6365 6e73 6522   = "MIT License"
-000000b0: 7d0d 0a61 7574 686f 7273 203d 205b 7b6e  }..authors = [{n
-000000c0: 616d 6520 3d20 2244 6f6e 6973 6861 2053  ame = "Donisha S
-000000d0: 6d69 7468 222c 2065 6d61 696c 203d 2022  mith", email = "
-000000e0: 646f 6e69 7368 6173 6d69 7468 406f 7574  donishasmith@out
-000000f0: 6c6f 6f6b 2e63 6f6d 227d 5d0d 0a64 6573  look.com"}]..des
-00000100: 6372 6970 7469 6f6e 203d 2022 436f 2d61  cription = "Co-a
-00000110: 6374 6976 6174 696f 6e20 5061 7474 6572  ctivation Patter
-00000120: 6e73 2028 4341 5073 2920 5079 7468 6f6e  ns (CAPs) Python
-00000130: 2070 6163 6b61 6765 220d 0a72 6561 646d   package"..readm
-00000140: 6520 3d20 2252 4541 444d 452e 6d64 220d  e = "README.md".
-00000150: 0a72 6571 7569 7265 732d 7079 7468 6f6e  .requires-python
-00000160: 203d 2022 3e3d 332e 392e 3022 0d0a 6b65   = ">=3.9.0"..ke
-00000170: 7977 6f72 6473 203d 205b 2270 7974 686f  ywords = ["pytho
-00000180: 6e22 2c20 2243 6f2d 4163 7469 7661 7469  n", "Co-Activati
-00000190: 6f6e 2050 6174 7465 726e 7322 2c20 2243  on Patterns", "C
-000001a0: 4150 7322 2c20 226e 6575 726f 696d 6167  APs", "neuroimag
-000001b0: 696e 6722 2c20 2266 6d72 6922 2c20 2264  ing", "fmri", "d
-000001c0: 6663 222c 2022 6479 6e61 6d69 6320 6675  fc", "dynamic fu
-000001d0: 6e63 7469 6f6e 616c 2063 6f6e 6e65 6374  nctional connect
-000001e0: 6976 6974 7922 2c20 2266 4d52 4950 7265  ivity", "fMRIPre
-000001f0: 7022 5d0d 0a63 6c61 7373 6966 6965 7273  p"]..classifiers
-00000200: 203d 205b 0d0a 2020 2020 2249 6e74 656e   = [..    "Inten
-00000210: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
-00000220: 4564 7563 6174 696f 6e22 2c0d 0a20 2020  Education",..   
-00000230: 2022 496e 7465 6e64 6564 2041 7564 6965   "Intended Audie
-00000240: 6e63 6520 3a3a 2053 6369 656e 6365 2f52  nce :: Science/R
-00000250: 6573 6561 7263 6822 2c0d 0a20 2020 2022  esearch",..    "
-00000260: 546f 7069 6320 3a3a 2053 6369 656e 7469  Topic :: Scienti
-00000270: 6669 632f 456e 6769 6e65 6572 696e 6722  fic/Engineering"
-00000280: 2c0d 0a20 2020 2022 4c69 6365 6e73 6520  ,..    "License 
-00000290: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-000002a0: 3a3a 204d 4954 204c 6963 656e 7365 222c  :: MIT License",
-000002b0: 0d0a 2020 2020 2250 726f 6772 616d 6d69  ..    "Programmi
-000002c0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000002d0: 7974 686f 6e20 3a3a 2033 2e39 222c 0d0a  ython :: 3.9",..
-000002e0: 2020 2020 2250 726f 6772 616d 6d69 6e67      "Programming
-000002f0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000300: 686f 6e20 3a3a 2033 2e31 3022 2c0d 0a20  hon :: 3.10",.. 
-00000310: 2020 2022 5072 6f67 7261 6d6d 696e 6720     "Programming 
-00000320: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000330: 6f6e 203a 3a20 332e 3131 222c 0d0a 2020  on :: 3.11",..  
-00000340: 2020 2250 726f 6772 616d 6d69 6e67 204c    "Programming L
-00000350: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000360: 6e20 3a3a 2033 2e31 3222 2c0d 0a20 2020  n :: 3.12",..   
-00000370: 2022 4f70 6572 6174 696e 6720 5379 7374   "Operating Syst
-00000380: 656d 203a 3a20 4d61 634f 5320 3a3a 204d  em :: MacOS :: M
-00000390: 6163 4f53 2058 222c 0d0a 2020 2020 224f  acOS X",..    "O
-000003a0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-000003b0: 3a3a 2050 4f53 4958 203a 3a20 4c69 6e75  :: POSIX :: Linu
-000003c0: 7822 2c0d 0a20 2020 2022 4f70 6572 6174  x",..    "Operat
-000003d0: 696e 6720 5379 7374 656d 203a 3a20 4d69  ing System :: Mi
-000003e0: 6372 6f73 6f66 7420 3a3a 2057 696e 646f  crosoft :: Windo
-000003f0: 7773 203a 3a20 5769 6e64 6f77 7320 3131  ws :: Windows 11
-00000400: 222c 0d0a 2020 2020 2244 6576 656c 6f70  ",..    "Develop
-00000410: 6d65 6e74 2053 7461 7475 7320 3a3a 2034  ment Status :: 4
-00000420: 202d 2042 6574 6122 0d0a 5d0d 0a64 6570   - Beta"..]..dep
-00000430: 656e 6465 6e63 6965 7320 3d20 5b22 6e75  endencies = ["nu
-00000440: 6d70 7922 2c0d 0a20 2020 2020 2020 2020  mpy",..         
-00000450: 2020 2020 2020 2022 7061 6e64 6173 222c         "pandas",
-00000460: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000470: 2020 226d 6174 706c 6f74 6c69 6222 2c0d    "matplotlib",.
-00000480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000490: 2022 7365 6162 6f72 6e22 2c0d 0a20 2020   "seaborn",..   
-000004a0: 2020 2020 2020 2020 2020 2020 2022 6b6e               "kn
-000004b0: 6565 6422 2c0d 0a20 2020 2020 2020 2020  eed",..         
-000004c0: 2020 2020 2020 2022 6e69 6261 6265 6c22         "nibabel"
-000004d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000004e0: 2020 2022 6e69 6c65 6172 6e3e 3d30 2e31     "nilearn>=0.1
-000004f0: 302e 312c 2021 3d30 2e31 302e 3322 2c0d  0.1, !=0.10.3",.
-00000500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000510: 2022 7363 696b 6974 2d6c 6561 726e 3e3d   "scikit-learn>=
-00000520: 312e 342e 3022 2c0d 0a20 2020 2020 2020  1.4.0",..       
-00000530: 2020 2020 2020 2020 2022 7375 7266 706c           "surfpl
-00000540: 6f74 222c 0d0a 2020 2020 2020 2020 2020  ot",..          
-00000550: 2020 2020 2020 226e 6575 726f 6d61 7073        "neuromaps
-00000560: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00000570: 2020 2020 2270 7962 6964 733b 2070 6c61      "pybids; pla
-00000580: 7466 6f72 6d5f 7379 7374 656d 2021 3d20  tform_system != 
-00000590: 2757 696e 646f 7773 2722 0d0a 2020 2020  'Windows'"..    
-000005a0: 2020 2020 2020 2020 2020 2020 5d0d 0a0d              ]...
-000005b0: 0a5b 7072 6f6a 6563 742e 7572 6c73 5d0d  .[project.urls].
-000005c0: 0a48 6f6d 6570 6167 6520 3d20 2268 7474  .Homepage = "htt
-000005d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000005e0: 646f 6e69 7368 6164 736d 6974 682f 6e65  donishadsmith/ne
-000005f0: 7572 6f63 6170 7322 2020 0d0a 4973 7375  urocaps"  ..Issu
-00000600: 6573 203d 2022 6874 7470 733a 2f2f 6769  es = "https://gi
-00000610: 7468 7562 2e63 6f6d 2f64 6f6e 6973 6861  thub.com/donisha
-00000620: 6473 6d69 7468 2f6e 6575 726f 6361 7073  dsmith/neurocaps
-00000630: 2f69 7373 7565 7322 2020 0d0a 4368 616e  /issues"  ..Chan
-00000640: 6765 6c6f 6720 3d20 2268 7474 7073 3a2f  gelog = "https:/
-00000650: 2f67 6974 6875 622e 636f 6d2f 646f 6e69  /github.com/doni
-00000660: 7368 6164 736d 6974 682f 6e65 7572 6f63  shadsmith/neuroc
-00000670: 6170 732f 626c 6f62 2f6d 6169 6e2f 4348  aps/blob/main/CH
-00000680: 414e 4745 4c4f 472e 6d64 220d 0a0d 0a5b  ANGELOG.md"....[
-00000690: 746f 6f6c 2e64 6973 7475 7469 6c73 2e62  tool.distutils.b
-000006a0: 6469 7374 5f77 6865 656c 5d0d 0a75 6e69  dist_wheel]..uni
-000006b0: 7665 7273 616c 203d 2074 7275 65         versal = true
+00000080: 7273 696f 6e20 3d20 2230 2e39 2e35 2e70  rsion = "0.9.5.p
+00000090: 6f73 7431 220d 0a6c 6963 656e 7365 203d  ost1"..license =
+000000a0: 207b 7465 7874 203d 2022 4d49 5420 4c69   {text = "MIT Li
+000000b0: 6365 6e73 6522 7d0d 0a61 7574 686f 7273  cense"}..authors
+000000c0: 203d 205b 7b6e 616d 6520 3d20 2244 6f6e   = [{name = "Don
+000000d0: 6973 6861 2053 6d69 7468 222c 2065 6d61  isha Smith", ema
+000000e0: 696c 203d 2022 646f 6e69 7368 6173 6d69  il = "donishasmi
+000000f0: 7468 406f 7574 6c6f 6f6b 2e63 6f6d 227d  th@outlook.com"}
+00000100: 5d0d 0a64 6573 6372 6970 7469 6f6e 203d  ]..description =
+00000110: 2022 436f 2d61 6374 6976 6174 696f 6e20   "Co-activation 
+00000120: 5061 7474 6572 6e73 2028 4341 5073 2920  Patterns (CAPs) 
+00000130: 5079 7468 6f6e 2070 6163 6b61 6765 220d  Python package".
+00000140: 0a72 6561 646d 6520 3d20 2252 4541 444d  .readme = "READM
+00000150: 452e 6d64 220d 0a72 6571 7569 7265 732d  E.md"..requires-
+00000160: 7079 7468 6f6e 203d 2022 3e3d 332e 392e  python = ">=3.9.
+00000170: 3022 0d0a 6b65 7977 6f72 6473 203d 205b  0"..keywords = [
+00000180: 2270 7974 686f 6e22 2c20 2243 6f2d 4163  "python", "Co-Ac
+00000190: 7469 7661 7469 6f6e 2050 6174 7465 726e  tivation Pattern
+000001a0: 7322 2c20 2243 4150 7322 2c20 226e 6575  s", "CAPs", "neu
+000001b0: 726f 696d 6167 696e 6722 2c20 2266 6d72  roimaging", "fmr
+000001c0: 6922 2c20 2264 6663 222c 2022 6479 6e61  i", "dfc", "dyna
+000001d0: 6d69 6320 6675 6e63 7469 6f6e 616c 2063  mic functional c
+000001e0: 6f6e 6e65 6374 6976 6974 7922 2c20 2266  onnectivity", "f
+000001f0: 4d52 4950 7265 7022 5d0d 0a63 6c61 7373  MRIPrep"]..class
+00000200: 6966 6965 7273 203d 205b 0d0a 2020 2020  ifiers = [..    
+00000210: 2249 6e74 656e 6465 6420 4175 6469 656e  "Intended Audien
+00000220: 6365 203a 3a20 4564 7563 6174 696f 6e22  ce :: Education"
+00000230: 2c0d 0a20 2020 2022 496e 7465 6e64 6564  ,..    "Intended
+00000240: 2041 7564 6965 6e63 6520 3a3a 2053 6369   Audience :: Sci
+00000250: 656e 6365 2f52 6573 6561 7263 6822 2c0d  ence/Research",.
+00000260: 0a20 2020 2022 546f 7069 6320 3a3a 2053  .    "Topic :: S
+00000270: 6369 656e 7469 6669 632f 456e 6769 6e65  cientific/Engine
+00000280: 6572 696e 6722 2c0d 0a20 2020 2022 4c69  ering",..    "Li
+00000290: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
+000002a0: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
+000002b0: 656e 7365 222c 0d0a 2020 2020 2250 726f  ense",..    "Pro
+000002c0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000002d0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000002e0: 2e39 222c 0d0a 2020 2020 2250 726f 6772  .9",..    "Progr
+000002f0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000300: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
+00000310: 3022 2c0d 0a20 2020 2022 5072 6f67 7261  0",..    "Progra
+00000320: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000330: 3a20 5079 7468 6f6e 203a 3a20 332e 3131  : Python :: 3.11
+00000340: 222c 0d0a 2020 2020 2250 726f 6772 616d  ",..    "Program
+00000350: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000360: 2050 7974 686f 6e20 3a3a 2033 2e31 3222   Python :: 3.12"
+00000370: 2c0d 0a20 2020 2022 4f70 6572 6174 696e  ,..    "Operatin
+00000380: 6720 5379 7374 656d 203a 3a20 4d61 634f  g System :: MacO
+00000390: 5320 3a3a 204d 6163 4f53 2058 222c 0d0a  S :: MacOS X",..
+000003a0: 2020 2020 224f 7065 7261 7469 6e67 2053      "Operating S
+000003b0: 7973 7465 6d20 3a3a 2050 4f53 4958 203a  ystem :: POSIX :
+000003c0: 3a20 4c69 6e75 7822 2c0d 0a20 2020 2022  : Linux",..    "
+000003d0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+000003e0: 203a 3a20 4d69 6372 6f73 6f66 7420 3a3a   :: Microsoft ::
+000003f0: 2057 696e 646f 7773 203a 3a20 5769 6e64   Windows :: Wind
+00000400: 6f77 7320 3131 222c 0d0a 2020 2020 2244  ows 11",..    "D
+00000410: 6576 656c 6f70 6d65 6e74 2053 7461 7475  evelopment Statu
+00000420: 7320 3a3a 2034 202d 2042 6574 6122 0d0a  s :: 4 - Beta"..
+00000430: 5d0d 0a64 6570 656e 6465 6e63 6965 7320  ]..dependencies 
+00000440: 3d20 5b22 6e75 6d70 7922 2c0d 0a20 2020  = ["numpy",..   
+00000450: 2020 2020 2020 2020 2020 2020 2022 7061               "pa
+00000460: 6e64 6173 222c 0d0a 2020 2020 2020 2020  ndas",..        
+00000470: 2020 2020 2020 2020 226d 6174 706c 6f74          "matplot
+00000480: 6c69 6222 2c0d 0a20 2020 2020 2020 2020  lib",..         
+00000490: 2020 2020 2020 2022 7365 6162 6f72 6e22         "seaborn"
+000004a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000004b0: 2020 2022 6b6e 6565 6422 2c0d 0a20 2020     "kneed",..   
+000004c0: 2020 2020 2020 2020 2020 2020 2022 6e69               "ni
+000004d0: 6261 6265 6c22 2c0d 0a20 2020 2020 2020  babel",..       
+000004e0: 2020 2020 2020 2020 2022 6e69 6c65 6172           "nilear
+000004f0: 6e3e 3d30 2e31 302e 312c 2021 3d30 2e31  n>=0.10.1, !=0.1
+00000500: 302e 3322 2c0d 0a20 2020 2020 2020 2020  0.3",..         
+00000510: 2020 2020 2020 2022 7363 696b 6974 2d6c         "scikit-l
+00000520: 6561 726e 3e3d 312e 342e 3022 2c0d 0a20  earn>=1.4.0",.. 
+00000530: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000540: 7375 7266 706c 6f74 222c 0d0a 2020 2020  surfplot",..    
+00000550: 2020 2020 2020 2020 2020 2020 226e 6575              "neu
+00000560: 726f 6d61 7073 222c 0d0a 2020 2020 2020  romaps",..      
+00000570: 2020 2020 2020 2020 2020 2270 7962 6964            "pybid
+00000580: 733b 2070 6c61 7466 6f72 6d5f 7379 7374  s; platform_syst
+00000590: 656d 2021 3d20 2757 696e 646f 7773 2722  em != 'Windows'"
+000005a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000005b0: 2020 5d0d 0a0d 0a5b 7072 6f6a 6563 742e    ]....[project.
+000005c0: 7572 6c73 5d0d 0a48 6f6d 6570 6167 6520  urls]..Homepage 
+000005d0: 3d20 2268 7474 7073 3a2f 2f67 6974 6875  = "https://githu
+000005e0: 622e 636f 6d2f 646f 6e69 7368 6164 736d  b.com/donishadsm
+000005f0: 6974 682f 6e65 7572 6f63 6170 7322 2020  ith/neurocaps"  
+00000600: 0d0a 4973 7375 6573 203d 2022 6874 7470  ..Issues = "http
+00000610: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+00000620: 6f6e 6973 6861 6473 6d69 7468 2f6e 6575  onishadsmith/neu
+00000630: 726f 6361 7073 2f69 7373 7565 7322 2020  rocaps/issues"  
+00000640: 0d0a 4368 616e 6765 6c6f 6720 3d20 2268  ..Changelog = "h
+00000650: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000660: 6d2f 646f 6e69 7368 6164 736d 6974 682f  m/donishadsmith/
+00000670: 6e65 7572 6f63 6170 732f 626c 6f62 2f6d  neurocaps/blob/m
+00000680: 6169 6e2f 4348 414e 4745 4c4f 472e 6d64  ain/CHANGELOG.md
+00000690: 220d 0a0d 0a5b 746f 6f6c 2e64 6973 7475  "....[tool.distu
+000006a0: 7469 6c73 2e62 6469 7374 5f77 6865 656c  tils.bdist_wheel
+000006b0: 5d0d 0a75 6e69 7665 7273 616c 203d 2074  ]..universal = t
+000006c0: 7275 65                                  rue
```

