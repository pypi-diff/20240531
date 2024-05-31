# Comparing `tmp/sorcerun-0.4.1.tar.gz` & `tmp/sorcerun-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sorcerun-0.4.1.tar", last modified: Mon May 13 22:53:47 2024, max compression
+gzip compressed data, was "sorcerun-0.4.2.tar", last modified: Fri May 31 21:08:21 2024, max compression
```

## Comparing `sorcerun-0.4.1.tar` & `sorcerun-0.4.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:53:47.540440 sorcerun-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-13 22:53:43.000000 sorcerun-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-13 22:53:47.540440 sorcerun-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-13 22:53:43.000000 sorcerun-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 22:53:47.540440 sorcerun-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-13 22:53:43.000000 sorcerun-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:53:47.540440 sorcerun-0.4.1/sorcerun/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 22:53:43.000000 sorcerun-0.4.1/sorcerun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-13 22:53:43.000000 sorcerun-0.4.1/sorcerun/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-13 22:53:43.000000 sorcerun-0.4.1/sorcerun/auth_mongodb_option.py
--rw-r--r--   0 runner    (1001) docker     (127)    19333 2024-05-13 22:53:43.000000 sorcerun-0.4.1/sorcerun/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-13 22:53:43.000000 sorcerun-0.4.1/sorcerun/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 22:53:43.000000 sorcerun-0.4.1/sorcerun/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-13 22:53:43.000000 sorcerun-0.4.1/sorcerun/grid_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9050 2024-05-13 22:53:43.000000 sorcerun-0.4.1/sorcerun/grid_plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-05-13 22:53:43.000000 sorcerun-0.4.1/sorcerun/incense_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-13 22:53:43.000000 sorcerun-0.4.1/sorcerun/mongodb_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-13 22:53:43.000000 sorcerun-0.4.1/sorcerun/sacred_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:53:47.540440 sorcerun-0.4.1/sorcerun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-13 22:53:47.000000 sorcerun-0.4.1/sorcerun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-13 22:53:47.000000 sorcerun-0.4.1/sorcerun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 22:53:47.000000 sorcerun-0.4.1/sorcerun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-13 22:53:47.000000 sorcerun-0.4.1/sorcerun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-13 22:53:47.000000 sorcerun-0.4.1/sorcerun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-13 22:53:47.000000 sorcerun-0.4.1/sorcerun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:08:21.966900 sorcerun-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-31 21:08:13.000000 sorcerun-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-31 21:08:21.966900 sorcerun-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-31 21:08:13.000000 sorcerun-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 21:08:21.966900 sorcerun-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-31 21:08:13.000000 sorcerun-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:08:21.966900 sorcerun-0.4.2/sorcerun/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 21:08:13.000000 sorcerun-0.4.2/sorcerun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-31 21:08:13.000000 sorcerun-0.4.2/sorcerun/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-31 21:08:13.000000 sorcerun-0.4.2/sorcerun/auth_mongodb_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19333 2024-05-31 21:08:13.000000 sorcerun-0.4.2/sorcerun/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-31 21:08:13.000000 sorcerun-0.4.2/sorcerun/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-31 21:08:13.000000 sorcerun-0.4.2/sorcerun/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-31 21:08:13.000000 sorcerun-0.4.2/sorcerun/grid_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-05-31 21:08:13.000000 sorcerun-0.4.2/sorcerun/grid_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10981 2024-05-31 21:08:13.000000 sorcerun-0.4.2/sorcerun/incense_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-31 21:08:13.000000 sorcerun-0.4.2/sorcerun/mongodb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-31 21:08:13.000000 sorcerun-0.4.2/sorcerun/sacred_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:08:21.966900 sorcerun-0.4.2/sorcerun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-31 21:08:21.000000 sorcerun-0.4.2/sorcerun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-31 21:08:21.000000 sorcerun-0.4.2/sorcerun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 21:08:21.000000 sorcerun-0.4.2/sorcerun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-31 21:08:21.000000 sorcerun-0.4.2/sorcerun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-31 21:08:21.000000 sorcerun-0.4.2/sorcerun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 21:08:21.000000 sorcerun-0.4.2/sorcerun.egg-info/top_level.txt
```

### Comparing `sorcerun-0.4.1/LICENSE` & `sorcerun-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sorcerun-0.4.1/PKG-INFO` & `sorcerun-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sorcerun
-Version: 0.4.1
+Version: 0.4.2
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: sacred
 Requires-Dist: pymongo
 Requires-Dist: pyyaml
 Requires-Dist: scikit-learn
 Requires-Dist: incense
```

### Comparing `sorcerun-0.4.1/README.md` & `sorcerun-0.4.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -14,11 +14,11 @@
 
 It also has tools to run **grids** of experiments and then analyze results from experiment grids.
 
 # TODO
 
 -   [x] Add example and documentation (top priority)
     -   [ ] Document the JL example
--   [ ] Add ability to add and edit tags to `grid_plotter` to filter experiments
+-   [x] Add ability to add and edit tags to `grid_plotter` to filter experiments
 -   [ ] Improve `grid_plotter` with more features for plot customization
 -   [ ] Fix the incense version dependency for `FileStorageObserver`
 -   [ ] Cleaner source file and other meta info tracking
```

### Comparing `sorcerun-0.4.1/setup.py` & `sorcerun-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="sorcerun",
-    version="0.4.1",
+    version="0.4.2",
     packages=find_packages(),
     install_requires=[
         "click",
         # "sacred @ git+https://github.com/rajatvd/sacred.git",
         "sacred",
         "pymongo",
         "pyyaml",
```

### Comparing `sorcerun-0.4.1/sorcerun/adapter.py` & `sorcerun-0.4.2/sorcerun/adapter.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.4.1/sorcerun/auth_mongodb_option.py` & `sorcerun-0.4.2/sorcerun/auth_mongodb_option.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.4.1/sorcerun/cli.py` & `sorcerun-0.4.2/sorcerun/cli.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.4.1/sorcerun/config.py` & `sorcerun-0.4.2/sorcerun/config.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.4.1/sorcerun/grid_config.py` & `sorcerun-0.4.2/sorcerun/grid_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 repo = Repo(".", search_parent_directories=True)
 dirty = repo.is_dirty()
 commit_hash = repo.git.rev_parse("HEAD")
 short_length = 8
 short_hash = commit_hash[:short_length]
 time_str = time.strftime("%Y-%m-%d-%H-%M-%S", time.localtime())
 extra = "jlTest"
-grid_id = f"{time_str}-{extra}-{short_hash}-dirty={dirty}"
+grid_id = f"{time_str}_{extra}_{short_hash}_dirty={dirty}"
 
 ns = (np.logspace(1, 3, 20, dtype=int)).tolist()
 ds = (np.logspace(1, 3, 3, dtype=int)).tolist()
 ks = (np.logspace(1, 3, 20, dtype=int)).tolist()
 num_repeats = 10
 
 grid_config = {
```

### Comparing `sorcerun-0.4.1/sorcerun/grid_plotter.py` & `sorcerun-0.4.2/sorcerun/grid_plotter.py`

 * *Files 7% similar despite different names*

```diff
@@ -82,38 +82,42 @@
 ]
 
 
 # create a list of strings showing shorted coordinate values
 # (if the length of the coordinate is greater than 10, then it is shortened)
 MAX_LEN = 100
 shortened_coords = {
-    dim: str(data.coords[dim].values)
-    if len(str(data.coords[dim].values)) < MAX_LEN
-    else str(data.coords[dim].values)[: MAX_LEN // 2]
-    + "..."
-    + str(data.coords[dim].values)[-MAX_LEN // 2 :]
+    dim: (
+        str(data.coords[dim].values)
+        if len(str(data.coords[dim].values)) < MAX_LEN
+        else str(data.coords[dim].values)[: MAX_LEN // 2]
+        + "..."
+        + str(data.coords[dim].values)[-MAX_LEN // 2 :]
+    )
     for dim in dims
 }
 
 st.subheader("Dimensions with more than 1 coordinate value")
 st.write("Select a reduction option for each dimension")
 # create a dictionary of reduction options for each dimension
 # if the dim is `repeat`, then the default reduction option is `mean` by default
 reduce_options_dict = {
-    dim: st.radio(
-        f"`{dim}`: {shortened_coords[dim]}",
-        reduce_options,
-        horizontal=True,
-    )
-    if dim != "repeat"
-    else st.radio(
-        f"`{dim}`: {shortened_coords[dim]}",
-        reduce_options,
-        horizontal=True,
-        index=1,
+    dim: (
+        st.radio(
+            f"`{dim}`: {shortened_coords[dim]}",
+            reduce_options,
+            horizontal=True,
+        )
+        if dim != "repeat"
+        else st.radio(
+            f"`{dim}`: {shortened_coords[dim]}",
+            reduce_options,
+            horizontal=True,
+            index=1,
+        )
     )
     for dim in dims
 }
 
 # apply the reduction to the data
 for dim, reduce_option in reduce_options_dict.items():
     if reduce_option == "mean":
@@ -127,41 +131,54 @@
 new_dims = [dim for dim in data.dims if len(data[dim]) > 1]
 
 metric_names = list(data["metric"].values)
 st.subheader("Metrics")
 st.write(metric_names)
 
 st.subheader("Choose axes for each plot")
+xlim = None
+ylim = None
 # Choose an x and y axis from both dimensions and metrics
 with st.container():
-    col1x, col2x, col3x = st.columns(3)
+    # add a column for setting xlim and ylim
+    col1x, col2x, col3x, col4x = st.columns(4)
     with col1x:
         x_axis = st.selectbox(
             "X axis",
             new_dims,
             index=new_dims.index("step") if "step" in new_dims else 0,
         )
     with col2x:
         st.text("")
         st.text("")
         log_x = st.checkbox("Log scale x axis", value=False)
 
     with col3x:
         x_label = st.text_input("X label", value=x_axis)
 
-    col1y, col2y, col3y = st.columns(3)
+    with col4x:
+        xlim = st.text_input("X limits", value="")
+        if xlim:
+            xlim = [float(x) for x in xlim.split(",")]
+
+    col1y, col2y, col3y, col4y = st.columns(4)
     # Choose multiple y axes from the metrics
     with col1y:
         y_axes = st.multiselect("Y axis", metric_names)
     with col2y:
         st.text("")
         st.text("")
         log_y = st.checkbox("Log scale y axis", value=False)
     with col3y:
         y_label = st.text_input("Y label", value="metric")
+    with col4y:
+        ylim = st.text_input("Y limits", value="")
+        if ylim:
+            ylim = [float(y) for y in ylim.split(",")]
+
 # Remaining dims
 remaining_dims = sorted(list(set(new_dims) - set([x_axis, "metric"])))
 
 # Choose a style for the plot
 style = st.text_input("Line style", value="o-")
 
 # Choose plot dimensions to include within a single plot
@@ -175,24 +192,28 @@
 other_dims = fixed_dims_per_plot
 st.write("Dimensions that vary in each plot:")
 st.write(dims_used_in_plot)
 
 # Boolean on whether to show regression line slope
 show_slope = st.checkbox("Show regression line slope", value=False)
 
+# Boolean on whether to have axis grids
+axis_grids = st.checkbox("Show axis grids", value=True)
+
 # Boolean on whether to save the plots
 save_plots = st.checkbox("Save plots", value=False)
 
 if save_plots:
     # Select a save type (png, eps, pdf)
     save_type = st.selectbox("Save type", ["png", "eps", "pdf"])
     save_dir = f"figures/{grid_id}/{save_type}"
     st.write(f"Saving plots to: `{save_dir}`")
     os.makedirs(save_dir, exist_ok=True)
 
+# TODO: auto change ylabel is there is only one metric and dont include that in legend
 
 # Add a button to actually make the plots
 # check if other_dims is empty
 if not other_dims:
     out = data
     groups = [()]
 else:
@@ -211,30 +232,31 @@
     for i, group in enumerate(groups):
         title = "--".join(
             [
                 f"{TITLE_NAME[key]}={val}"
                 for key, val in zip(other_dims, group)
                 if key in title_keys
             ]
+            + [f"metrics={'-'.join(y_axes)}"]
         )
         xarr = out[group]
 
         fig, ax = plt.subplots()
         plt.title(title)
         # use itertools product to iterate over all coordinate combinations of dims_used_in_plot
         for coord in itertools.product(
             *[xarr.coords[dim].values for dim in dims_used_in_plot]
         ):
             d = {dim: coord[i] for i, dim in enumerate(dims_used_in_plot)}
             ys = xarr.loc[d]
             for y_axis in y_axes:
                 y = ys.loc[dict(metric=y_axis)].squeeze().to_numpy()
-                label = " ".join(
-                    [f"{y_axis}", ", ".join([f"{k}={v}" for k, v in d.items()])]
-                )
+                label = ", ".join([f"{k}={v}" for k, v in d.items()])
+                if len(y_axes) > 1:
+                    label = y_axis + " " + label
 
                 # check if y is all nans or infs, if so, don't plot
                 good_inds = np.isfinite(y)
 
                 # dont_plot = y.isnull().all().item() or (y == float("inf")).all().item()
                 dont_plot = not np.any(good_inds)
                 if not dont_plot:
@@ -269,14 +291,28 @@
 
         if log_x:
             plt.xscale("log")
         if log_y:
             plt.yscale("log")
         plt.ylabel(y_label)
         plt.xlabel(x_label)
-        plt.legend()
+        if xlim:
+            plt.xlim(xlim)
+        if ylim:
+            plt.ylim(ylim)
+
+        # place legend outside plot to the right using axis
+        leg = fig.legend(loc="center left", bbox_to_anchor=(0.92, 0.5))
+        # plt.legend()
+
+        if axis_grids:
+            plt.grid(True)
 
         # display plot in streamlit
+        if save_plots:
+            fig.savefig(
+                f"{save_dir}/{i:03d}--{title}.{save_type}",
+                bbox_extra_artists=[leg],
+                bbox_inches="tight",
+            )
         st.write(f"Plot {i+1}: {title}")
         st.pyplot(fig)
-        if save_plots:
-            plt.savefig(f"{save_dir}/{i:03d}--{title}.{save_type}")
```

### Comparing `sorcerun-0.4.1/sorcerun/incense_utils.py` & `sorcerun-0.4.2/sorcerun/incense_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,15 +320,18 @@
     else:
         print(f"The size of '{file_path}' is: {size_in_bytes / 1024**3:.2f} GB")
 
 
 def process_and_save_grid_to_netcdf(gid, file_root=FILE_STORAGE_ROOT):
     # loader = get_incense_loader()
     # grid_exps = loader.find_by_config_key("grid_id", gid)
-    grid_exps = load_filesystem_expts_by_config_keys(grid_id=gid, runs_dir=os.path.join(file_root, RUNS_DIR))
+    grid_exps = load_filesystem_expts_by_config_keys(
+        grid_id=gid,
+        runs_dir=os.path.join(file_root, RUNS_DIR),
+    )
     e = grid_exps[0]
 
     print(f"Found {len(grid_exps)} experiments with grid_id {gid}")
 
     grid_exps_xr, grid_metrics_xr = exps_to_xarray(grid_exps)
     metrics_reduced_xr = grid_metrics_xr
```

### Comparing `sorcerun-0.4.1/sorcerun/mongodb_utils.py` & `sorcerun-0.4.2/sorcerun/mongodb_utils.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.4.1/sorcerun/sacred_utils.py` & `sorcerun-0.4.2/sorcerun/sacred_utils.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.4.1/sorcerun.egg-info/PKG-INFO` & `sorcerun-0.4.2/sorcerun.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sorcerun
-Version: 0.4.1
+Version: 0.4.2
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: sacred
 Requires-Dist: pymongo
 Requires-Dist: pyyaml
 Requires-Dist: scikit-learn
 Requires-Dist: incense
```

