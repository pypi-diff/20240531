# Comparing `tmp/ammico-0.2.0.tar.gz` & `tmp/ammico-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ammico-0.2.0.tar", last modified: Wed Sep 13 12:33:17 2023, max compression
+gzip compressed data, was "ammico-0.2.1.tar", last modified: Fri May 31 10:27:31 2024, max compression
```

## Comparing `ammico-0.2.0.tar` & `ammico-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,27 @@
-drwxrwxr-x   0 inga      (1001) inga      (1001)        0 2023-09-13 12:33:17.773593 ammico-0.2.0/
--rw-rw-r--   0 inga      (1001) inga      (1001)     1060 2023-05-04 11:56:20.000000 ammico-0.2.0/LICENSE
--rw-r--r--   0 inga      (1001) inga      (1001)     9300 2023-09-13 12:33:17.773593 ammico-0.2.0/PKG-INFO
--rw-rw-r--   0 inga      (1001) inga      (1001)     7630 2023-09-07 11:01:05.000000 ammico-0.2.0/README.md
-drwxrwxr-x   0 inga      (1001) inga      (1001)        0 2023-09-13 12:33:17.769593 ammico-0.2.0/ammico/
--rw-rw-r--   0 inga      (1001) inga      (1001)      951 2023-09-07 11:01:05.000000 ammico-0.2.0/ammico/__init__.py
--rw-rw-r--   0 inga      (1001) inga      (1001)     5236 2023-09-01 12:08:41.000000 ammico-0.2.0/ammico/colors.py
--rw-rw-r--   0 inga      (1001) inga      (1001)    13362 2023-07-09 12:13:35.000000 ammico-0.2.0/ammico/cropposts.py
-drwxrwxr-x   0 inga      (1001) inga      (1001)        0 2023-09-13 12:33:17.769593 ammico-0.2.0/ammico/data/
--rw-rw-r--   0 inga      (1001) inga      (1001)     3079 2023-07-09 12:13:35.000000 ammico-0.2.0/ammico/data/Color_tables.csv
--rw-rw-r--   0 inga      (1001) inga      (1001)  1467471 2023-06-15 07:52:40.000000 ammico-0.2.0/ammico/data/test-crop-image.png
--rw-rw-r--   0 inga      (1001) inga      (1001)    20171 2023-09-01 12:08:41.000000 ammico-0.2.0/ammico/display.py
--rw-rw-r--   0 inga      (1001) inga      (1001)    10706 2023-09-01 12:08:41.000000 ammico-0.2.0/ammico/faces.py
--rw-rw-r--   0 inga      (1001) inga      (1001)    37502 2023-09-01 12:08:41.000000 ammico-0.2.0/ammico/multimodal_search.py
--rw-rw-r--   0 inga      (1001) inga      (1001)     1623 2023-06-15 07:52:40.000000 ammico-0.2.0/ammico/objects.py
--rw-rw-r--   0 inga      (1001) inga      (1001)     1893 2023-07-09 12:13:35.000000 ammico-0.2.0/ammico/objects_cvlib.py
--rw-rw-r--   0 inga      (1001) inga      (1001)     9977 2023-07-09 18:21:21.000000 ammico-0.2.0/ammico/summary.py
--rw-rw-r--   0 inga      (1001) inga      (1001)    17207 2023-09-07 11:00:54.000000 ammico-0.2.0/ammico/text.py
--rw-rw-r--   0 inga      (1001) inga      (1001)     8443 2023-09-07 11:01:05.000000 ammico-0.2.0/ammico/utils.py
-drwxrwxr-x   0 inga      (1001) inga      (1001)        0 2023-09-13 12:33:17.769593 ammico-0.2.0/ammico.egg-info/
--rw-r--r--   0 inga      (1001) inga      (1001)     9300 2023-09-13 12:33:17.000000 ammico-0.2.0/ammico.egg-info/PKG-INFO
--rw-rw-r--   0 inga      (1001) inga      (1001)      493 2023-09-13 12:33:17.000000 ammico-0.2.0/ammico.egg-info/SOURCES.txt
--rw-rw-r--   0 inga      (1001) inga      (1001)        1 2023-09-13 12:33:17.000000 ammico-0.2.0/ammico.egg-info/dependency_links.txt
--rw-rw-r--   0 inga      (1001) inga      (1001)       79 2023-09-13 12:33:17.000000 ammico-0.2.0/ammico.egg-info/entry_points.txt
--rw-rw-r--   0 inga      (1001) inga      (1001)      500 2023-09-13 12:33:17.000000 ammico-0.2.0/ammico.egg-info/requires.txt
--rw-rw-r--   0 inga      (1001) inga      (1001)        7 2023-09-13 12:33:17.000000 ammico-0.2.0/ammico.egg-info/top_level.txt
--rw-rw-r--   0 inga      (1001) inga      (1001)     1814 2023-09-13 12:33:10.000000 ammico-0.2.0/pyproject.toml
--rw-rw-r--   0 inga      (1001) inga      (1001)       38 2023-09-13 12:33:17.773593 ammico-0.2.0/setup.cfg
--rw-rw-r--   0 inga      (1001) inga      (1001)       39 2023-05-04 11:56:20.000000 ammico-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:27:31.235110 ammico-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-31 10:27:22.000000 ammico-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13389 2024-05-31 10:27:31.235110 ammico-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11841 2024-05-31 10:27:22.000000 ammico-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:27:31.231110 ammico-0.2.1/ammico/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-31 10:27:22.000000 ammico-0.2.1/ammico/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-05-31 10:27:22.000000 ammico-0.2.1/ammico/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13494 2024-05-31 10:27:22.000000 ammico-0.2.1/ammico/cropposts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:27:31.231110 ammico-0.2.1/ammico/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-31 10:27:22.000000 ammico-0.2.1/ammico/data/Color_tables.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1467471 2024-05-31 10:27:22.000000 ammico-0.2.1/ammico/data/test-crop-image.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20772 2024-05-31 10:27:22.000000 ammico-0.2.1/ammico/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11011 2024-05-31 10:27:22.000000 ammico-0.2.1/ammico/faces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37535 2024-05-31 10:27:22.000000 ammico-0.2.1/ammico/multimodal_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25825 2024-05-31 10:27:22.000000 ammico-0.2.1/ammico/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19175 2024-05-31 10:27:22.000000 ammico-0.2.1/ammico/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-05-31 10:27:22.000000 ammico-0.2.1/ammico/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:27:31.235110 ammico-0.2.1/ammico.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13389 2024-05-31 10:27:31.000000 ammico-0.2.1/ammico.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-31 10:27:31.000000 ammico-0.2.1/ammico.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 10:27:31.000000 ammico-0.2.1/ammico.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-31 10:27:31.000000 ammico-0.2.1/ammico.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-31 10:27:31.000000 ammico-0.2.1/ammico.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-31 10:27:31.000000 ammico-0.2.1/ammico.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-31 10:27:22.000000 ammico-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 10:27:31.235110 ammico-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-31 10:27:22.000000 ammico-0.2.1/setup.py
```

### Comparing `ammico-0.2.0/LICENSE` & `ammico-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ammico-0.2.0/ammico/__init__.py` & `ammico-0.2.1/ammico/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,29 +3,27 @@
 except ImportError:
     # Running on pre-3.8 Python; use importlib-metadata package
     import importlib_metadata as metadata  # type: ignore
 from ammico.cropposts import crop_media_posts, crop_posts_from_refs
 from ammico.display import AnalysisExplorer
 from ammico.faces import EmotionDetector
 from ammico.multimodal_search import MultimodalSearch
-from ammico.objects import ObjectDetector
 from ammico.summary import SummaryDetector
 from ammico.text import TextDetector, PostprocessText
 from ammico.utils import find_files, get_dataframe
 
 # Export the version defined in project metadata
 __version__ = metadata.version(__package__)
 del metadata
 
 __all__ = [
     "crop_media_posts",
     "crop_posts_from_refs",
     "AnalysisExplorer",
     "EmotionDetector",
     "MultimodalSearch",
-    "ObjectDetector",
     "SummaryDetector",
     "TextDetector",
     "PostprocessText",
     "find_files",
     "get_dataframe",
 ]
```

### Comparing `ammico-0.2.0/ammico/colors.py` & `ammico-0.2.1/ammico/colors.py`

 * *Files identical despite different names*

### Comparing `ammico-0.2.0/ammico/cropposts.py` & `ammico-0.2.1/ammico/cropposts.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,27 +321,29 @@
             Defaults to False.
         plt_image (Bool, optional): Display the image part of the social media post.
             Defaults to False.
     """
 
     # get the reference images with regions that signify areas to crop
     ref_views = []
-    for ref_file in ref_files:
-        ref_view = cv2.imread(ref_file)
+    for ref_file in ref_files.values():
+        ref_file_path = ref_file["filename"]
+        ref_view = cv2.imread(ref_file_path)
         ref_views.append(ref_view)
     # parse through the social media posts to be cropped
-    for crop_file in files:
-        view = cv2.imread(crop_file)
-        print("Doing file {}".format(crop_file))
+    for crop_file in files.values():
+        crop_file_path = crop_file["filename"]
+        view = cv2.imread(crop_file_path)
+        print("Doing file {}".format(crop_file_path))
         crop_view = crop_posts_from_refs(
             ref_views,
             view,
             plt_match=plt_match,
             plt_crop=plt_crop,
             plt_image=plt_image,
         )
         if crop_view is not None:
             # save the image to the provided folder
-            filename = ntpath.basename(crop_file)
+            filename = ntpath.basename(crop_file_path)
             save_path = os.path.join(save_crop_dir, filename)
             save_path = save_path.replace("\\", "/")
             cv2.imwrite(save_path, crop_view)
```

### Comparing `ammico-0.2.0/ammico/data/Color_tables.csv` & `ammico-0.2.1/ammico/data/Color_tables.csv`

 * *Files identical despite different names*

### Comparing `ammico-0.2.0/ammico/data/test-crop-image.png` & `ammico-0.2.1/ammico/data/test-crop-image.png`

 * *Files identical despite different names*

### Comparing `ammico-0.2.0/ammico/display.py` & `ammico-0.2.1/ammico/display.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import ammico.faces as faces
 import ammico.text as text
-import ammico.objects as objects
 import ammico.colors as colors
 from ammico.utils import is_interactive
 import ammico.summary as summary
-import dash_renderjson
+import pandas as pd
 from dash import html, Input, Output, dcc, State, Dash
 from PIL import Image
 import dash_bootstrap_components as dbc
 
 
 COLOR_SCHEMES = [
     "CIE 1976",
@@ -88,15 +87,15 @@
         self.app.callback(
             Output("img_middle_picture_id", "src"),
             Input("left_select_id", "value"),
             prevent_initial_call=True,
         )(self.update_picture)
 
         self.app.callback(
-            Output("right_json_viewer", "data"),
+            Output("right_json_viewer", "children"),
             Input("button_run", "n_clicks"),
             State("left_select_id", "options"),
             State("left_select_id", "value"),
             State("Dropdown_select_Detector", "value"),
             State("setting_Text_analyse_text", "value"),
             State("setting_Text_model_names", "value"),
             State("setting_Text_revision_numbers", "value"),
@@ -328,15 +327,14 @@
             [
                 dbc.Col(
                     [
                         dbc.Row(
                             dcc.Dropdown(
                                 options=[
                                     "TextDetector",
-                                    "ObjectDetector",
                                     "EmotionDetector",
                                     "SummaryDetector",
                                     "ColorDetector",
                                 ],
                                 value="TextDetector",
                                 id="Dropdown_select_Detector",
                                 style={"width": "60%"},
@@ -361,21 +359,16 @@
                             ),
                             justify="start",
                         ),
                         dbc.Row(
                             dcc.Loading(
                                 id="loading-2",
                                 children=[
-                                    dash_renderjson.DashRenderjson(
-                                        id="right_json_viewer",
-                                        data={},
-                                        max_depth=-1,
-                                        theme=self.theme,
-                                        invert_theme=True,
-                                    ),
+                                    # This is where the json is shown.
+                                    html.Div(id="right_json_viewer"),
                                 ],
                                 type="circle",
                             ),
                             justify="start",
                         ),
                     ],
                     align="start",
@@ -461,15 +454,14 @@
 
         Returns:
             dict: The analysis output for the selected image.
         """
         identify_dict = {
             "EmotionDetector": faces.EmotionDetector,
             "TextDetector": text.TextDetector,
-            "ObjectDetector": objects.ObjectDetector,
             "SummaryDetector": summary.SummaryDetector,
             "ColorDetector": colors.ColorDetector,
         }
 
         # Get image ID from dropdown value, which is the filepath
         if current_img_value is None:
             return {}
@@ -483,38 +475,65 @@
         if detector_value == "TextDetector":
             analyse_text = (
                 True if settings_text_analyse_text == ["Analyse text"] else False
             )
             detector_class = identify_function(
                 image_copy,
                 analyse_text=analyse_text,
-                model_names=[settings_text_model_names]
-                if (settings_text_model_names is not None)
-                else None,
-                revision_numbers=[settings_text_revision_numbers]
-                if (settings_text_revision_numbers is not None)
-                else None,
+                model_names=(
+                    [settings_text_model_names]
+                    if (settings_text_model_names is not None)
+                    else None
+                ),
+                revision_numbers=(
+                    [settings_text_revision_numbers]
+                    if (settings_text_revision_numbers is not None)
+                    else None
+                ),
             )
         elif detector_value == "EmotionDetector":
-            print("test")
             detector_class = identify_function(
                 image_copy,
                 race_threshold=setting_emotion_race_threshold,
                 emotion_threshold=setting_emotion_emotion_threshold,
             )
         elif detector_value == "ColorDetector":
             detector_class = identify_function(
                 image_copy,
                 delta_e_method=setting_color_delta_e_method,
             )
         elif detector_value == "SummaryDetector":
             detector_class = identify_function(
                 image_copy,
                 analysis_type=setting_summary_analysis_type,
-                summary_model_type=setting_summary_model,
-                list_of_questions=[setting_summary_list_of_questions]
-                if (setting_summary_list_of_questions is not None)
-                else None,
+                model_type=setting_summary_model,
+                list_of_questions=(
+                    [setting_summary_list_of_questions]
+                    if (setting_summary_list_of_questions is not None)
+                    else None
+                ),
             )
         else:
             detector_class = identify_function(image_copy)
-        return detector_class.analyse_image()
+        analysis_dict = detector_class.analyse_image()
+
+        # Initialize an empty dictionary
+        new_analysis_dict = {}
+
+        # Iterate over the items in the original dictionary
+        for k, v in analysis_dict.items():
+            # Check if the value is a list
+            if isinstance(v, list):
+                # If it is, convert each item in the list to a string and join them with a comma
+                new_value = ", ".join([str(f) for f in v])
+            else:
+                # If it's not a list, keep the value as it is
+                new_value = v
+
+            # Add the new key-value pair to the new dictionary
+            new_analysis_dict[k] = new_value
+
+        df = pd.DataFrame([new_analysis_dict]).set_index("filename").T
+        df.index.rename("filename", inplace=True)
+        return dbc.Table.from_dataframe(
+            df, striped=True, bordered=True, hover=True, index=True
+        )
```

### Comparing `ammico-0.2.0/ammico/faces.py` & `ammico-0.2.1/ammico/faces.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,14 +93,19 @@
         Args:
             subdict (dict): The dictionary to store the analysis results.
             emotion_threshold (float): The threshold for detecting emotions (default: 50.0).
             race_threshold (float): The threshold for detecting race (default: 50.0).
         """
         super().__init__(subdict)
         self.subdict.update(self.set_keys())
+        # check if thresholds are valid
+        if emotion_threshold < 0 or emotion_threshold > 100:
+            raise ValueError("Emotion threshold must be between 0 and 100.")
+        if race_threshold < 0 or race_threshold > 100:
+            raise ValueError("Race threshold must be between 0 and 100.")
         self.emotion_threshold = emotion_threshold
         self.race_threshold = race_threshold
         self.emotion_categories = {
             "angry": "Negative",
             "disgust": "Negative",
             "fear": "Negative",
             "sad": "Negative",
@@ -194,15 +199,15 @@
         self.subdict["face"] = "Yes"
         self.subdict["multiple_faces"] = "Yes" if len(faces) > 1 else "No"
         self.subdict["no_faces"] = len(faces) if len(faces) <= 15 else 99
         # note number of faces being identified
         result = {"number_faces": len(faces) if len(faces) <= 3 else 3}
         # We limit ourselves to three faces
         for i, face in enumerate(faces[:3]):
-            result[f"person{ i+1 }"] = self.analyze_single_face(face)
+            result[f"person{i+1}"] = self.analyze_single_face(face)
         self.clean_subdict(result)
         return self.subdict
 
     def clean_subdict(self, result: dict) -> dict:
         """
         Cleans the subdict dictionary by converting results into appropriate formats.
```

### Comparing `ammico-0.2.0/ammico/multimodal_search.py` & `ammico-0.2.1/ammico/multimodal_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,15 +328,16 @@
             image_names (list): sorted list of image names.
             features_image_stacked (torch.Tensor): tensors of images features stacked in device.
         """
         if model_type in ("clip_base", "clip_vitl14_336", "clip_vitl14"):
             path_to_lib = lavis.__file__[:-11] + "models/clip_models/"
             url = "https://raw.githubusercontent.com/salesforce/LAVIS/main/lavis/models/clip_models/bpe_simple_vocab_16e6.txt.gz"
             r = requests.get(url, allow_redirects=False)
-            open(path_to_lib + "bpe_simple_vocab_16e6.txt.gz", "wb").write(r.content)
+            with open(path_to_lib + "bpe_simple_vocab_16e6.txt.gz", "wb") as f:
+                f.write(r.content)
 
         image_keys = sorted(self.subdict.keys())
         image_names = [self.subdict[k]["filename"] for k in image_keys]
 
         select_model = {
             "blip2": MultimodalSearch.load_feature_extractor_model_blip2,
             "blip": MultimodalSearch.load_feature_extractor_model_blip,
@@ -530,17 +531,17 @@
                     and similarity[key][q].item() > filter_val_limit
                     and 100 * abs(max_val - similarity[key][q].item()) / max_val
                     < filter_rel_error
                 ):
                     self.subdict[image_keys[key]][
                         "rank " + list(search_query[q].values())[0]
                     ] = places[q][key]
-                    self.subdict[image_keys[key]][
-                        list(search_query[q].values())[0]
-                    ] = similarity[key][q].item()
+                    self.subdict[image_keys[key]][list(search_query[q].values())[0]] = (
+                        similarity[key][q].item()
+                    )
                 else:
                     self.subdict[image_keys[key]][
                         "rank " + list(search_query[q].values())[0]
                     ] = None
                     self.subdict[image_keys[key]][list(search_query[q].values())[0]] = 0
         return similarity, sorted_lists
 
@@ -911,17 +912,17 @@
                     self.subdict[image_keys[key]][
                         "itm_rank " + list(search_query[index_text_query].values())[0]
                     ] = None
 
             avg_gradcams.append(local_avg_gradcams)
             itm_scores.append(local_itm_scores)
             itm_scores2.append(local_itm_scores2)
-            image_gradcam_with_itm[
-                list(search_query[index_text_query].values())[0]
-            ] = localimage_gradcam_with_itm
+            image_gradcam_with_itm[list(search_query[index_text_query].values())[0]] = (
+                localimage_gradcam_with_itm
+            )
         del (
             itm_model,
             vis_processor_itm,
             text_processor,
             raw_images,
             images,
             tokenizer,
```

### Comparing `ammico-0.2.0/ammico/text.py` & `ammico-0.2.1/ammico/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -216,30 +216,33 @@
         """Generate Spacy doc object for further text analysis."""
         self.doc = self.nlp(self.subdict["text_english"])
 
     def clean_text(self):
         """Clean the text from unrecognized words and any numbers."""
         templist = []
         for token in self.doc:
-            templist.append(
-                token.text
-            ) if token.pos_ != "NUM" and token.has_vector else None
+            (
+                templist.append(token.text)
+                if token.pos_ != "NUM" and token.has_vector
+                else None
+            )
         self.subdict["text_clean"] = " ".join(templist).rstrip().lstrip()
 
     def text_summary(self):
         """Generate a summary of the text using the Transformers pipeline."""
         # use the transformers pipeline to summarize the text
         # use the current default model - 03/2023
         max_number_of_characters = 3000
         pipe = pipeline(
             "summarization",
             model=self.model_summary,
             revision=self.revision_summary,
             min_length=5,
             max_length=20,
+            framework="pt",
         )
         try:
             summary = pipe(self.subdict["text_english"][0:max_number_of_characters])
             self.subdict["text_summary"] = summary[0]["summary_text"]
         except IndexError:
             print(
                 "Cannot provide summary for this object - please check that the text has been translated correctly."
@@ -252,37 +255,91 @@
         # use the transformers pipeline for text classification
         # use the current default model - 03/2023
         pipe = pipeline(
             "text-classification",
             model=self.model_sentiment,
             revision=self.revision_sentiment,
             truncation=True,
+            framework="pt",
         )
         result = pipe(self.subdict["text_english"])
         self.subdict["sentiment"] = result[0]["label"]
         self.subdict["sentiment_score"] = round(result[0]["score"], 2)
 
     def text_ner(self):
         """Perform named entity recognition on the text using the Transformers pipeline."""
         # use the transformers pipeline for named entity recognition
         # use the current default model - 03/2023
         pipe = pipeline(
             "token-classification",
             model=self.model_ner,
             revision=self.revision_ner,
             aggregation_strategy="simple",
+            framework="pt",
         )
         result = pipe(self.subdict["text_english"])
         self.subdict["entity"] = []
         self.subdict["entity_type"] = []
         for entity in result:
             self.subdict["entity"].append(entity["word"])
             self.subdict["entity_type"].append(entity["entity_group"])
 
 
+class TextAnalyzer:
+    """Used to get text from a csv and then run the TextDetector on it."""
+
+    def __init__(self, csv_path: str, column_key: str = None) -> None:
+        """Init the TextTranslator class.
+
+        Args:
+            csv_path (str): Path to the CSV file containing the text entries.
+            column_key (str): Key for the column containing the text entries.
+                Defaults to None.
+        """
+        self.csv_path = csv_path
+        self.column_key = column_key
+        self._check_valid_csv_path()
+        self._check_file_exists()
+
+    def _check_valid_csv_path(self):
+        if not isinstance(self.csv_path, str):
+            raise ValueError("The provided path to the CSV file is not a string.")
+        if not self.csv_path.endswith(".csv"):
+            raise ValueError("The provided file is not a CSV file.")
+
+    def _check_file_exists(self):
+        try:
+            with open(self.csv_path, "r") as file:  # noqa
+                pass
+        except FileNotFoundError:
+            raise FileNotFoundError("The provided CSV file does not exist.")
+
+    def read_csv(self) -> dict:
+        """Read the CSV file and return the dictionary with the text entries.
+
+        Returns:
+            dict: The dictionary with the text entries.
+        """
+        df = pd.read_csv(self.csv_path, encoding="utf8")
+        if not self.column_key:
+            self.column_key = "text"
+
+        if self.column_key not in df:
+            raise ValueError(
+                "The provided column key is not in the CSV file. Please check."
+            )
+        self.mylist = df[self.column_key].to_list()
+        self.mydict = {}
+        for i, text in enumerate(self.mylist):
+            self.mydict[self.csv_path + "row-" + str(i)] = {
+                "filename": self.csv_path,
+                "text": text,
+            }
+
+
 class PostprocessText:
     def __init__(
         self,
         mydict: dict = None,
         use_csv: bool = False,
         csv_path: str = None,
         analyze_text: str = "text_english",
```

### Comparing `ammico-0.2.0/ammico/utils.py` & `ammico-0.2.1/ammico/utils.py`

 * *Files identical despite different names*

### Comparing `ammico-0.2.0/pyproject.toml` & `ammico-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=61",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ammico"
-version = "0.2.0"
+version = "0.2.1"
 description = "AI Media and Misinformation Content Analysis Tool"
 readme = "README.md"
 maintainers = [
     { name = "Inga Ulusoy", email = "ssc@iwr.uni-heidelberg.de" },
     { name = "Petr Andriushchenko", email = "ssc@iwr.uni-heidelberg.de" },
 ]
 requires-python = ">=3.8"
@@ -19,17 +19,16 @@
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: MIT License",
 ]
 
 dependencies = [
     "bertopic<=0.14.1",
-    "cvlib",
     "dash>=2.11.0",
-    "dash_renderjson",
+    "datasets",
     "deepface<=0.0.75",
     "googletrans==3.1.0a0",
     "google-cloud-vision",
     "grpcio",
     "importlib_metadata",
     "importlib_resources",
     "ipython",
@@ -40,30 +39,27 @@
     "Pillow",
     "pooch",
     "protobuf",
     "pytest",
     "pytest-cov",
     "Requests",
     "retina_face",
-    "salesforce-lavis",
+    "ammico-lavis",
     "setuptools",
     "spacy",
-    "tensorflow<=2.12.3",
-    "torch",
+    "tensorflow>=2.13.0",
+    "torch<2.1.0",
     "transformers",
     "google-cloud-vision",
-    "setuptools",
-    "opencv-contrib-python",
-    "dash",
-    "dash_renderjson",
     "dash_bootstrap_components",
     "colorgram.py",
     "webcolors",
     "colour-science",
-    "scikit-learn!=1.3.0",
+    "scikit-learn>1.3.0",
+    "tqdm"
 ]
 
 [project.scripts]
 ammico_prefetch_models = "ammico.utils:ammico_prefetch_models"
 
 [project.urls]
 homepage = "https://github.com/ssciwr/AMMICO"  # FIXME not shown by pip
```

