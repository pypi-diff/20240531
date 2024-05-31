# Comparing `tmp/multi_med_image_ml-0.0.7.tar.gz` & `tmp/multi_med_image_ml-0.0.8.tar.gz`

## Comparing `multi_med_image_ml-0.0.7.tar` & `multi_med_image_ml-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/setup.py
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0   506885 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/.images/logo.png
--rw-r--r--   0        0        0  2674703 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/.images/model_diagram.png
--rw-r--r--   0        0        0   289892 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/.images/regress_figure.png
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/example/example_train.py
--rw-r--r--   0        0        0     6228 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/example/options/base_options.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/example/options/test_options.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/example/options/train_options.py
--rw-r--r--   0        0        0     9558 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/src/multi_med_image_ml/DataBaseWrapper.py
--rwxr-xr-x   0        0        0    10802 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/src/multi_med_image_ml/MedImageLoader.py
--rw-r--r--   0        0        0    19875 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/src/multi_med_image_ml/MultiInputTester.py
--rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/src/multi_med_image_ml/MultiInputTrainer.py
--rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/src/multi_med_image_ml/Records.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/src/multi_med_image_ml/__init__.py
--rw-r--r--   0        0        0    17625 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/src/multi_med_image_ml/models.py
--rw-r--r--   0        0        0    46062 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/src/multi_med_image_ml/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0    11771 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/tests/unit_tests.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/tests/weights.json
--rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/README.md
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/setup.py
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0   332414 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/.images/logo.png
+-rw-r--r--   0        0        0  2707942 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/.images/model_diagram.png
+-rw-r--r--   0        0        0   328523 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/.images/regress_figure.png
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/example/example_train.py
+-rwxr-xr-x   0        0        0      116 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/example/example_train.sh
+-rw-r--r--   0        0        0     6194 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/example/options/base_options.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/example/options/test_options.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/example/options/train_options.py
+-rw-r--r--   0        0        0     9992 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/src/multi_med_image_ml/DataBaseWrapper.py
+-rwxr-xr-x   0        0        0    10918 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/src/multi_med_image_ml/MedImageLoader.py
+-rw-r--r--   0        0        0    19875 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/src/multi_med_image_ml/MultiInputTester.py
+-rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/src/multi_med_image_ml/MultiInputTrainer.py
+-rw-r--r--   0        0        0    10139 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/src/multi_med_image_ml/Records.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/src/multi_med_image_ml/__init__.py
+-rw-r--r--   0        0        0    17645 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/src/multi_med_image_ml/models.py
+-rw-r--r--   0        0        0    46176 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/src/multi_med_image_ml/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0    11771 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/tests/unit_tests.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/tests/weights.json
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/README.md
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     5624 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/PKG-INFO
```

### Comparing `multi_med_image_ml-0.0.7/.github/workflows/publish-to-pypi.yml` & `multi_med_image_ml-0.0.8/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.7/example/example_train.py` & `multi_med_image_ml-0.0.8/example/example_train.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 from options.train_options import *
 
 import os
 import sys
-wd = os.path.dirname(os.path.dirname(os.path.realpath(__file__)))
-sys.path.insert(0,wd)
-sys.path.insert(0,os.path.join(wd,'src'))
-sys.path.insert(0,os.path.join(wd,'src','multi_med_image_ml'))
-
-from src.multi_med_image_ml.MedImageLoader import *
-from src.multi_med_image_ml.models import *
-from src.multi_med_image_ml.MultiInputTrainer import *
+wd = os.path.dirname(os.path.realpath(__file__))
+
+from multi_med_image_ml.MedImageLoader import *
+from multi_med_image_ml.models import *
+from multi_med_image_ml.MultiInputTrainer import *
 # Path function, used when switching platforms.
 
-def path_func(filename,reverse=False):
-	prefix = os.path.join(os.path.dirname(os.path.dirname(wd)),'MGH_ML_pipeline')
+def key_to_filename(key,reverse=False):
+	prefix = os.path.join(os.path.dirname(wd),'MGH_ML_pipeline')
 	suffix = '_resized_96.npy'
-	if reverse:
-		return os.path.join(prefix,filename[1:] + suffix)
+	if not reverse:
+		string = os.path.join(prefix,key[1:] + suffix)
 	else:
-		return os.sep + filename[len(prefix):-len(suffix)]
+		string = key[len(prefix):-len(suffix)]
+	return string
 
 opt = TrainOptions().parse()
 
 model = MultiInputModule(weights=opt.pretrained_model)
+model.cuda(opt.gpu_ids[0])
 
 medim_loader = MedImageLoader(opt.all_vars,
 	dim=opt.dim,
 	cache=True,
 	label=opt.label,
 	confounds=opt.confounds,
 	return_obj = True,
 	dtype="torch",
 	val_ranges=opt.val_ranges,
 	static_inputs=opt.static_inputs,
-	augment=opt.augment)
+	augment=opt.augment,
+	key_to_filename=key_to_filename,
+	gpu_ids = opt.gpu_ids
+	)
 
 trainer = MultiInputTrainer(model,
 		batch_size=opt.batch_size,
 		lr=opt.lr,
 		name=opt.name,
 		checkpoint_dir=opt.checkpoint_dir,
 		loss_image_dir=os.path.join(opt.results_dir,
 						opt.name,"loss_ims")
 	)
 
 for i in range(opt.epochs):
 	print(f"Epoch {i}")
 	for p in medim_loader:
-		print(medim_loader.mode)
-		print(medim_loader.tl())
 		trainer.loop(p,dataloader=medim_loader)
```

### Comparing `multi_med_image_ml-0.0.7/example/options/base_options.py` & `multi_med_image_ml-0.0.8/example/options/base_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 	def __init__(self):
 		"""Reset the class; indicates the class hasn't been initailized"""
 		self.initialized = False
 
 	def initialize(self, parser):
 		"""Define the common options that are used in both training and test."""
 		# basic parameters
-		self.wd = os.path.dirname(os.path.dirname(os.path.dirname(os.path.realpath(__file__))))
+		self.wd = os.path.dirname(os.path.realpath(__file__))
 		#parser.add_argument('--dataroot', required=True, help='path to images (should have subfolders trainA, trainB, valA, valB, etc)')
 		parser.add_argument('--name', type=str, default='experiment_name', help='name of the experiment. It decides where to store samples and models')
 		parser.add_argument('--dim',nargs=3,help='Dimensions of images',default=[96,96,96])
 		parser.add_argument('--gpu_ids', type=str, default='0', help='gpu ids: e.g. 0  0,1,2, 0,2. use -1 for CPU')
 		parser.add_argument('--checkpoint_dir', type=str, default=os.path.join(self.wd,'checkpoint'), help='models are saved here')
 		parser.add_argument('--label',default=['AlzStage'],nargs='+',help='Which labels to read in')
 		parser.add_argument('--y_weight', type=int, default=6, help='Amount of weight to give to label when training it')
```

### Comparing `multi_med_image_ml-0.0.7/example/options/test_options.py` & `multi_med_image_ml-0.0.8/example/options/test_options.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.7/example/options/train_options.py` & `multi_med_image_ml-0.0.8/example/options/train_options.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.7/src/multi_med_image_ml/DataBaseWrapper.py` & `multi_med_image_ml-0.0.8/src/multi_med_image_ml/DataBaseWrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import pandas as pd
 import os
 import numpy as np
 from .utils import *
+from .Records import ImageRecord
 import dateutil
 
 class DataBaseWrapper():
 	"""
 	Wrapper for Pandas table to cache some common and repeated functions
 	"""
 	def __init__(self,
 					all_vars = None,
 					filename=None,
 					labels=[],
 					confounds=[],
 					dim=None,
 					cdim=None,
-					path_func = path_func_default):
-		self.path_func = path_func
-		check_path_func(self.path_func)
+					key_to_filename = key_to_filename_default):
+		self.key_to_filename = key_to_filename
+		check_key_to_filename(self.key_to_filename)
 
 		self.filename = filename
 		self.dim = dim
 		self.labels = [] if labels is None else labels
 		self.confounds = [] if confounds is None else confounds
 		if all_vars is not None:
 			self.all_vars = all_vars
@@ -36,20 +37,22 @@
 		else:
 			raise Exception("DatabaseWrapper cannot have no inputs")
 		self.jdict = []
 		
 		if isinstance(self.all_vars,str) and os.path.isfile(self.all_vars)\
 			 and os.path.splitext(self.all_vars)[1] == ".pkl":
 			self.all_vars = pd.read_pickle(self.all_vars)
-	
+	def has_im(self,im: ImageRecord):
+		fkey = self.key_to_filename(im.npy_file,reverse=True)
+		return fkey in self.all_vars.index
 	def build_metadata(self):
 		for l in self.labels:
 			if l not in self.all_vars.columns:
-				print("%s was dead the whole time" % l)
-				print(self.all_vars)
+				print("%s not in all_vars.columns" % l)
+				print(self.all_vars.columns)
 			assert(l in self.all_vars.columns)
 		for c in self.confounds:
 			assert(c in self.all_vars.columns)
 		assert(len(set(self.labels).intersection(set(self.confounds)))==0)
 		self.uniques = {}
 		self.n_buckets=10
 		for c in self.confounds + self.labels:
@@ -113,16 +116,17 @@
 					[(rd[i] + \
 					self.uniques[c]["nonnan_list"][i])/2 \
 					for i in range(self.n_buckets_cont)]
 				self.uniques[c]["nonnan_list"][-1] = max_
 				self.uniques[c]["nonnan_list"][0] = min_
 				assert(len(self.uniques[c]["nonnan_list"]) == \
 					self.n_buckets_cont)
-	def get_confound_encode(self,filename: str):
-		confound_strs = [self.loc_val(filename,c) for c in self.confounds]
+	def get_confound_encode(self,npy_file: str):
+		assert(os.path.splitext(npy_file)[1] == ".npy")
+		confound_strs = [self.loc_val(npy_file,c) for c in self.confounds]
 		cnum_list = []
 		for j,c in enumerate(self.confounds):
 			if self.uniques[c]["discrete"]:
 				c_uniques = self.uniques[c]["unique"]
 				if is_nan(confound_strs[j]):
 					cnum_list.append(-1)
 				else:
@@ -137,16 +141,17 @@
 					for kk in range(len(unnl)-1):
 						if unnl[kk] <= confound_strs[j] and \
 							unnl[kk+1] >= confound_strs[j]:
 							cnum_list.append(kk)
 							break
 		assert(len(cnum_list) == len(self.confounds))
 		return cnum_list
-	def get_label_encode(self,filename: str):
-		label_strs = [self.loc_val(filename,c) for c in self.labels]
+	def get_label_encode(self,npy_file: str):
+		assert(os.path.splitext(npy_file)[1] == ".npy")
+		label_strs = [self.loc_val(npy_file,c) for c in self.labels]
 		cnum_list = []
 		for j,c in enumerate(self.labels):
 			if self.uniques[c]["discrete"]:
 				c_uniques = self.uniques[c]["unique"]
 				if is_nan(label_strs[j]):
 					cnum_list.append(-1)
 				else:
@@ -161,61 +166,57 @@
 					for kk in range(len(unnl)-1):
 						if unnl[kk] <= label_strs[j] and \
 							unnl[kk+1] >= label_strs[j]:
 							cnum_list.append(kk)
 							break
 		assert(len(cnum_list) == len(self.labels))
 		return cnum_list
-	def _get_val(self,fkey: str,potential_columns):
+	def _get_val(self,npy_file: str,potential_columns):
 		assert(np.all([isinstance(_,str) for _ in potential_columns]))
 		val = None
 		#fkey = get_dim_str(filename,dim=self.dim)
 		for c in potential_columns:
 			if c in self.columns:
-				val = self.loc_val(fkey,c)
-				assert(fkey in self.all_vars.index)
-				#if not isinstance(val,str):
-				#	print("fffffffffffff")
-				#	print(val)
-				#	print(type(val))
-				#	print("ddddddddddddd")
+				val = self.loc_val(npy_file,c)
 				if not(is_nan(val) or isinstance(val,str)):
 					print(val)
 				assert(is_nan(val) or isinstance(val,str))
-				#val = str(val)
-				#print("-----")
-				#print(c)
-				#print(fkey)
-				#print("******")
-				#print(val)
-				#print("AAAAAAAA")
 				if not is_nan(val):
 					break
 		
 		return val
-	def get_ID(self,fkey):
-		id = self._get_val(fkey,["PatientID","Patient ID"])
+	def get_ID(self,npy_file):
+		id = self._get_val(npy_file,["PatientID","Patient ID"])
 		return id
-	def parse_date(self,d):
+	def parse_date(self,d,date_format="%Y-%m-%d %H:%M:%S"):
 		if is_nan(d):
 			return datetime.datetime(year=1970,month=1,day=1)
 		elif is_float(d):
 			return dateutil.parser.parse(str(d))
 		else:
-			return dateutil.parser.parse(d)
-	def get_exam_date(self,fkey: str) -> datetime.date:
-		d = self._get_val(fkey,["ExamEndDTS","Acquisition Date"])
+			try:
+				return datetime.datetime.strptime(
+					d.replace("_"," ").split(".")[0],
+					date_format)
+			except ValueError:
+				return dateutil.parser.parse(d.replace("_"," "))
+	def get_exam_date(self,npy_file: str) -> datetime.date:
+		d = self._get_val(npy_file,["ExamEndDTS","Acquisition Date"])
 		return self.parse_date(d)
-	def get_birth_date(self,fkey):
-		d = self._get_val(fkey,["BirthDTS"])
+	def get_birth_date(self,npy_file: str) -> datetime.date:
+		d = self._get_val(npy_file,["BirthDTS"])
 		return self.parse_date(d)
 	
-	def loc_val(self,fkey,c):
-		fkey = self.path_func(fkey)
+	def loc_val(self,npy_file,c):
+		fkey = self.key_to_filename(npy_file,reverse=True)
 		try:
+			if fkey not in self.all_vars.index:
+				print("Error - %s not present in index. Adding..." % fkey)
+			#assert(fkey in self.all_vars.index)
+			
 			return self.all_vars.loc[fkey,c]
 		except KeyError:
 			nifti_file = get_dim_str(fkey,dim=self.dim,outtype=".nii.gz")
 			
 			if not os.path.isfile(nifti_file):
 				nifti_file = get_dim_str(fkey,dim=self.dim,outtype=".nii")
 			if not os.path.isfile(nifti_file):
@@ -234,32 +235,33 @@
 			if not (os.path.isfile(json_file)):
 				json_file = os.path.join(
 					os.path.dirname(nifti_file),
 					"metadata.json")
 				if not os.path.isfile(json_file):
 					return
 		npy_file = get_dim_str(nifti_file,self.dim)
-		
-		if npy_file not in self.jdict and npy_file not in self.all_vars.index:
+		fkey = self.key_to_filename(npy_file,reverse=True)
+		if fkey not in self.jdict and fkey not in self.all_vars.index:
 			with open(json_file,'r') as fileobj:
 				json_dict = json.load(fileobj)
-			json_dict["fkey"] = npy_file
-			json_dict["filename"] = npy_file
+			json_dict["fkey"] = fkey
+			json_dict["filename"] = fkey
 			for item in json_dict:
 				if isinstance(json_dict[item],list):
 					json_dict[item] = "_".join(
 							[str(_) for _ in sorted(json_dict[item])]
 						)
 			self.columns = self.columns.union(set(json_dict))
 			self.jdict.append(json_dict)
 			assert(len(self.jdict) > 0)
 	def get_file_list(self):
-		return [self.path_func(str(_),reverse=True) \
+		return [self.key_to_filename(str(_)) \
 			for _ in self.all_vars.index]
 	def out_dataframe(self,fkey_ass = None):
+		
 		if len(self.jdict) > 0:
 			out = pd.DataFrame(self.jdict,columns = list(self.columns))
 			out.set_index("fkey",inplace=True)
 			if len(self.all_vars) > 0:
 				self.all_vars = pd.concat([self.all_vars,out],
 						ignore_index=False,
 						join='inner')
```

### Comparing `multi_med_image_ml-0.0.7/src/multi_med_image_ml/MedImageLoader.py` & `multi_med_image_ml-0.0.8/src/multi_med_image_ml/MedImageLoader.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 
 from .Records import BatchRecord,ImageRecord
 from .DataBaseWrapper import DataBaseWrapper
 
 # Translates a filename to a key and back, for storing files as keys in the
 # pandas dataframe. By default, the keys are the full filepaths. This function
 # may need to be changed when switching to different systems
-def path_func_default(fkey,reverse=False):
+def key_to_filename_default(fkey,reverse=False):
 	return fkey
 
 class MedImageLoader():
 	def __init__(self,*image_folders,
 			pandas_cache = '../pandas/',
 			cache = True,
-			path_func = path_func_default,
+			key_to_filename = key_to_filename_default,
 			batch_by_pid=True,
 			file_record_name=None,
 			all_vars = None,
 			batch_size = 14,
 			dim = (96,96,96),
 			get_encoded = False,
 			static_inputs = None,
@@ -41,15 +41,16 @@
 			augment = True,
 			val_ranges = {},
 			dtype="torch",
 			Y_dim = (1,32),
 			C_dim = (16,32),
 			return_obj = False,
 			channels_first = True,
-			recycle=True):
+			recycle=True,
+			gpu_ids = ""):
 		self.channels_first = channels_first
 		self.image_folders = image_folders
 		self.augment = augment
 		self.dim=dim
 		self.dtype=dtype
 		self.cache = cache
 		self.pandas_cache = pandas_cache
@@ -60,21 +61,21 @@
 		self.static_inputs = static_inputs
 		self.label = label
 		self.confounds = confounds
 		self.group_by = group_by
 		self.Y_dim = Y_dim
 		self.C_dim = C_dim
 		self.mode = None
+		self.gpu_ids = gpu_ids
 		
 		# If set to true, restacks images every time via the data 
 		# matching function. Best for very large and imbalanced datasets
 		self.recycle=recycle
 		
-		self.path_func = path_func
-		check_path_func(self.path_func)
+		check_key_to_filename(key_to_filename)
 
 		# Stores images so that they aren't repeated in different stacks
 		self.image_dict = {}
 		# If true, this uses one match confound at a time and cycles through
 		# them
 		self.zero_data_list = []
 		self.match_confounds = match_confounds
@@ -96,15 +97,15 @@
 				"all_vars_%s.pkl" % get_dim_str(dim=self.dim))
 		
 		self.all_vars = DataBaseWrapper(
 					filename=self.all_vars_file,
 					labels=self.label,
 					confounds=self.confounds,
 					dim=self.dim,
-					path_func=self.path_func)
+					key_to_filename=key_to_filename)
 		if not self.pickle_input():
 			self.build_pandas_database()
 		self.all_vars.build_metadata()
 		
 		# Determine which mode the scheduler is in
 		if (self.label is not None and len(self.label) > 0):
 			self.mode = "match"
@@ -143,15 +144,15 @@
 		assert(not self.pickle_input())
 		old_mode = self.mode
 		self.mode = "iterate"
 		self._load_list_stack()
 		
 		for i,filename in enumerate(self.image_dict):
 			im = self.image_dict[filename]
-			if im.fkey not in self.all_vars.all_vars.index:
+			if not self.all_vars.has_im(im):
 				try:
 					im.get_image()
 					im.clear_image()
 				except ImageFileError:
 					continue
 			if i % 100 == 0:
 				self.all_vars.out_dataframe()
@@ -193,30 +194,29 @@
 		elif self.mode == "match":
 			[fname_list],_ = get_balanced_filename_list(self.tl(),
 				self.match_confounds,
 				selection_ratios=[1], total_size_limit=np.inf,
 				non_confound_value_ranges = self.val_ranges,verbose=False,
 				all_vars=self.all_vars.all_vars)
 			fname_list = list(fname_list)
+			fname_list = [self.all_vars.key_to_filename(_) for _ in fname_list]
 			if len(fname_list) == 0:
-				
 				print(self.all_vars.all_vars.loc[:,self.tl()])
 				raise Exception("No valid files from %s" % self.tl())
 			assert(isinstance(fname_list,list))
 			return self.all_vars.stack_list_by_label(fname_list,self.tl())
 		else:
 			raise Exception("Invalid mode: %s" % self.mode)
 	def _load_list_stack(self):
 		X_files = self.get_file_list() 
 		for i,filename_list in enumerate(X_files):
 			for j,filename in enumerate(filename_list):
 				if filename in self.image_dict:
 					X_files[i][j] = self.image_dict[filename]
 				else:
-					
 					X_files[i][j] = ImageRecord(filename,
 								dim=self.dim,
 								y_nums=[i] if len(X_files) == 1 else None,
 								Y_dim = self.Y_dim,
 								C_dim = self.C_dim,
 								dtype=self.dtype,
 								all_vars = self.all_vars,
@@ -317,15 +317,16 @@
 		if self.batch_by_pid:
 			p = temp[0]
 		else:
 			p = BatchRecord(temp,
 				dtype = self.dtype,
 				sort=False,
 				batch_by_pid=False,
-				channels_first=self.channels_first)
+				channels_first=self.channels_first,
+				gpu_ids=self.gpu_ids)
 		if self.return_obj:
 			return p
 		elif self.return_labels():
 			return p.get_image(),p.get_Y()
 		else:
 			return p.get_image()
```

### Comparing `multi_med_image_ml-0.0.7/src/multi_med_image_ml/MultiInputTester.py` & `multi_med_image_ml-0.0.8/src/multi_med_image_ml/MultiInputTester.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.7/src/multi_med_image_ml/MultiInputTrainer.py` & `multi_med_image_ml-0.0.8/src/multi_med_image_ml/MultiInputTrainer.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.7/src/multi_med_image_ml/Records.py` & `multi_med_image_ml-0.0.8/src/multi_med_image_ml/Records.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,23 +19,23 @@
 		all_vars = None,
 		dim=(96,96,96),
 		dtype="torch",
 		ID = None,
 		extra_info_list = None,
 		y_on_c = True,
 		cache = True,
-		Y_dim = (16,32),
+		Y_dim = (1,32),
 		C_dim = (16,32),
 		y_nums = None,
 		c_nums = None,
 		static_inputs=[]):
 		
 		self.dim=dim
 		self.filename = filename
-		self.fkey = get_dim_str(self.filename,self.dim)
+		self.npy_file = get_dim_str(self.filename,self.dim)
 		self.image_type = None
 		self.dtype = dtype
 		self.all_vars = all_vars
 		self.Y_dim = Y_dim
 		self.C_dim = C_dim
 		self.y_on_c = y_on_c # Adds the Y value to the C array as well
 		
@@ -54,15 +54,15 @@
 		self.c_nums = c_nums
 		
 		self.static_inputs = []
 		self.static_input_res = None
 		
 		self.loaded = False
 		if self.all_vars is not None:
-			if self.fkey in self.all_vars.all_vars:
+			if self.npy_file in self.all_vars.all_vars:
 				self.load_extra_info()
 		
 		self.cache = cache
 		self.cached_record = None
 	def get_exam_date(self):
 		if not self.loaded:
 			self.load_extra_info()
@@ -71,26 +71,26 @@
 		if not self.loaded:
 			self.load_extra_info()
 		return self.bdate
 	def load_extra_info(self):
 		if self.loaded: return
 		if self.all_vars is None:
 			return
-		if self.fkey not in self.all_vars.all_vars.index:
+		if not self.all_vars.has_im(self):
 			return
-		self.bdate = self.all_vars.get_birth_date(self.fkey)
-		self.exam_date = self.all_vars.get_exam_date(self.fkey)
-		self.group_by = self.all_vars.get_ID(self.fkey)
+		self.bdate = self.all_vars.get_birth_date(self.npy_file)
+		self.exam_date = self.all_vars.get_exam_date(self.npy_file)
+		self.group_by = self.all_vars.get_ID(self.npy_file)
 		self.loaded = True
 	def get_static_inputs(self):
 		if self.static_input_res is None:
 			self.static_input_res = []
 			for key in self.static_inputs:
 				static_inputs.append(
-					self.all_vars.loc_val(self.fkey,key)
+					self.all_vars.loc_val(self.npy_file,key)
 				)
 		return self.static_input_res
 	def _is_valid_operand(self, other):
 		return hasattr(other, "exam_date") and hasattr(other,"group_by")
 	def __eq__(self, other):
 		if not self._is_valid_operand(other):
 			return NotImplemented
@@ -191,21 +191,21 @@
 		if augment and self.dtype == "torch":
 			return generate_transforms(self.image)
 		else: return self.image
 	def _get_Y(self):
 		"""Returns label"""
 		if self.y_nums is not None:
 			return self.y_nums
-		self.y_nums = self.all_vars.get_label_encode(self.fkey)
+		self.y_nums = self.all_vars.get_label_encode(self.npy_file)
 		return self.y_nums
 	def _get_C(self):
 		"""Returns confound array"""
 		if self.c_nums is not None:
 			return self.c_nums
-		self.c_nums = self.all_vars.get_confound_encode(self.fkey)
+		self.c_nums = self.all_vars.get_confound_encode(self.npy_file)
 		return self.c_nums
 	def get_Y(self):
 		if self.Y is not None:
 			return self.Y
 		y_nums = self._get_Y()
 		if self.dtype == "numpy":
 			self.Y = np.zeros(self.Y_dim)
@@ -245,25 +245,26 @@
 class BatchRecord():
 	def __init__(self,
 			image_records,
 			dtype="torch",
 			device=None,
 			sort=True,
 			batch_by_pid=False,
-			channels_first = True):
+			channels_first = True,
+			gpu_ids=""):
 		self.image_records = image_records
 		assert(
 			np.all(
 				[isinstance(image_record,ImageRecord) \
 					for image_record in image_records
 				]
 				)
 			)
+		self.gpu_ids = gpu_ids
 		self.channels_first = channels_first
-
 		self.batch_by_pid=batch_by_pid
 		if sort: self.image_records = sorted(image_records)
 		#assert(
 		#	np.all(
 		#		[_.group_by == self.image_records[0].group_by \
 		#			for _ in self.image_records]
 		#	)
@@ -329,15 +330,18 @@
 				Xs.append(np.expand_dims(X,axis=0))
 			else:
 				raise Exception("Invalid dtype")
 		if no_arr:
 			return Xs
 		elif self.dtype == "torch":
 			Xs = torch.concatenate(Xs,0)
-			return Xs.float()
+			if self.gpu_ids == "":
+				return Xs.float()
+			else:
+				return Xs.float().cuda(self.gpu_ids[0])
 		elif self.dtype == "numpy":
 			Xs = np.concatenate(Xs,axis=0)
 			return Xs #.astype(np.float32)
 		else:
 			raise Exception("Invalid dtype: %s" % self.dtype)
 	def get_image(self,augment=False):
 		return self._get("X",augment=augment)
```

### Comparing `multi_med_image_ml-0.0.7/src/multi_med_image_ml/models.py` & `multi_med_image_ml-0.0.8/src/multi_med_image_ml/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -392,22 +392,28 @@
 		use_regression = hasattr(self,'regressor') and \
 			(self.regressor is not None) and \
 			(self.training or return_regress)
 		if not encoded_input:
 			if isinstance(x,BatchRecord):
 				assert(x.dtype == "torch")
 				if len(x.get_static_inputs()[0]) > 0:
-					print(x.get_static_inputs())
 					static_inputs = [_[0] for _ in x.get_static_inputs()]
 					if self.n_stat_inputs != len(static_inputs):
 						raise Exception(
 					"Number of static inputs not equal to input: %d != %d"\
 						 % (len(static_inputs),self.n_stat_inputs))
 				dates1 = x.get_exam_dates()
-				bdate1 = x.get_birth_dates()[0]
+				for d in dates1:
+					if d is None:
+						raise Exception("Dates cannot be none")
+				bdates = x.get_birth_dates()
+				for b in bdates:
+					if b is None:
+						raise Exception("Birth dates cannot be none")
+				bdate1 = bdates[0]
 				x = x.get_image()
 				assert(torch.is_tensor(x))
 				
 			if (self.encode_age and (dates is None or bdate is None)):
 				raise Exception("Need dates as input to encode age")
 			if x.size(0) > self.n_dyn_inputs:
 				raise Exception(
@@ -544,18 +550,15 @@
 		self.models = [torch.load(_) for _ in model_list]
 		for model in self.models: model.eval()
 	def forward(self,input,hidden):
 		new_output = []
 		new_hidden = []
 		for i in range(hidden.size()[3]):
 			model = self.models[i]
-			#print("input.size(): %s" % str(input.size()))
 			x = model.Encoder(input)
 			x = torch.unsqueeze(x,1).float()
 			output,h = model.RNN(x,hidden[...,i])
 			new_output.append(torch.unsqueeze(output,3))
 			new_hidden.append(torch.unsqueeze(h,3))
-			#print("output.size(): %s" % str(output.size()))
-			#print("h.size(): %s" % str(h.size()))
 		new_output = torch.cat(new_output,dim=3)
 		new_hidden = torch.cat(new_hidden,dim=3)
 		return new_output,new_hidden
```

### Comparing `multi_med_image_ml-0.0.7/src/multi_med_image_ml/utils.py` & `multi_med_image_ml-0.0.8/src/multi_med_image_ml/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,22 +31,22 @@
 def compile_dicom_py(dicom_folder):
 	dicom2nifti.convert_directory(dicom_folder,"conv.nii.gz")
 	dicom_files = (glob.glob(os.path.join("*.dcm")))
 
 import platform
 platform_system = platform.system()
 
-def path_func_default(filename,reverse=False):
+def key_to_filename_default(filename,reverse=False):
 	return filename
 
-def check_path_func(path_func):
-	if path_func(path_func(os.path.realpath(__file__)),reverse=True) \
+def check_key_to_filename(key_to_filename):
+	if key_to_filename(key_to_filename(os.path.realpath(__file__),reverse=False),reverse=True) \
 		!= os.path.realpath(__file__):
 		raise Exception("""
-			path_func must be a function that translates
+			key_to_filename must be a function that translates
 			a filename to an index key and back with the
 			'reverse' option input""")
 
 """
 Uses dcm2niix, since that's had the best results overall when converting dicom
 to nifti, even though it's a UNIX command
 """
@@ -333,15 +333,17 @@
 	if nifti_data.dtype != np.float32:
 		nifti_data = nifti_data.astype(np.float32)
 	if len(nifti_data.shape) != len(dim):
 		nifti_data = np.squeeze(nifti_data)
 		if len(nifti_data.shape) != len(dim):
 			nifti_data = np.squeeze(np.mean(nifti_data,axis=-1))
 		assert(len(nifti_data.shape) == len(dim))
-	if nifti_data.shape != dim:
+	if nifti_data.shape != tuple(dim):
+		print(nifti_data.shape)
+		print(dim)
 		zp = [dim[i]/nifti_data.shape[i] for i in range(len(dim))]
 		nifti_data = ndimage.zoom(nifti_data,zp)
 	return nifti_data
 
 # Prime number functions used in the data matching schemes
 def prime(i, primes):
 	for prime in primes:
@@ -798,23 +800,23 @@
 
 # Given the filenames (or, rather, filestubs), returns encoded input and output
 # labels, as well as encoded confounds, if specified, as either a set of strings
 # or binary arrays
 def get_data_from_filenames(filename_list,test_variable=None,confounds=None,
 		return_as_strs = False,unique_test_vals = None,all_vars=None,
 		return_choice_arr = False,dict_obj=None,return_as_dict=False,
-		path_func = None,X_encoder=None,vae_encoder=False,uniques=None,
+		key_to_filename = None,X_encoder=None,vae_encoder=False,uniques=None,
 		density_confound_sort=True,n_buckets=3):
 	if dict_obj is not None:
 		if "uniques" in dict_obj:
 			uniques = dict_obj["uniques"]
 	if all_vars is None and test_variable is not None:
 		all_vars = pd.read_pickle(pandas_output)
-	if path_func is not None:
-		X_filenames_list = [path_func(_) for _ in filename_list]
+	if key_to_filename is not None:
+		X_filenames_list = [key_to_filename(_) for _ in filename_list]
 	else:
 		X_filenames_list = filename_list
 	selection = np.array([os.path.isfile(_) for _ in X_filenames_list],
 			dtype=bool)
 	if confounds is not None:
 		confound_strs = [[None for _ in confounds] \
 					for __ in filename_list]
```

### Comparing `multi_med_image_ml-0.0.7/tests/unit_tests.py` & `multi_med_image_ml-0.0.8/tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.7/README.md` & `multi_med_image_ml-0.0.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![ze logo](.images/logo.png)
+![ze logo](https://raw.githubusercontent.com/mleming/MultiMedImageML/main/.images/logo.png)
 
 Multi-Input Medical Image Machine Learning Toolkit
 ==================================================
 
 The Multi-Input Medical Image Machine Learning Toolkit (MultiMedImageML) is a library of Pytorch functions that can encode multiple 3D images (designed specifically for brain images) and offer a single- or multi-label output, such as a disease detection.
 
 Thus, with a dataset of brain images and labels, you can train a model to predict dementia or multiple sclerosis from multiple input brain images.
@@ -11,29 +11,29 @@
 
     pip install multi-med-image-ml
 
 
 Overview
 ========
 
-![ze figure](.images/model_diagram.png)
+![ze figure](https://raw.githubusercontent.com/mleming/MultiMedImageML/main/.images/model_diagram.png)
 
 The core deep learning architecture is a Pytorch model that can take in variable numbers of 3D images (between one and 14 by default), then encodes them into a numerical vector and, through an adversarial training process, creates an intermediate representation that contains information about disease biomarkers but not confounds, like patient age and scanning site.
 
-![ze regress figure](.images/regress_figure.png)
+![ze regress figure](https://raw.githubusercontent.com/mleming/MultiMedImageML/main/.images/regress_figure.png)
 
 The confound regression process essentially disguises the intermediary representation to have disease biomarker features while imitating the confounding features of other groups.
 
 Getting Started
 ===============
 
 Datasets
 ========
 
-This may be used with either public benchmark datasets of brain images or internal hospital records, so long as they're represented as DICOM or NIFTI images. It was largely tested on [https://adni.loni.usc.edu/data-samples/access-data/](ADNI) and data internal to MGH. If they're represented as DICOM images, they are converted to NIFTI with metadata represented as a JSON file using [https://github.com/rordenlab/dcm2niix](dcm2niix). They may be further converted to NPY files, which are resized to a specific dimension, with the metadata represented in a pandas dataframe.
+This may be used with either public benchmark datasets of brain images or internal hospital records, so long as they're represented as DICOM or NIFTI images. It was largely tested on [ADNI](https://adni.loni.usc.edu/data-samples/access-data/) and data internal to MGH. If they're represented as DICOM images, they are converted to NIFTI with metadata represented as a JSON file using [dcm2niix](https://github.com/rordenlab/dcm2niix). They may be further converted to NPY files, which are resized to a specific dimension, with the metadata represented in a pandas dataframe.
 
 The MedImageLoader builds up this representation automatically, but it is space-intensive to do so.
 
 Data may be represented with a folder structure.
 
 ```
 .
@@ -69,11 +69,11 @@
                     ├── I1591323_Axial_3D_PASL_(Eyes_Open)_20220615143803_7.json
                     └── I1591323_Axial_3D_PASL_(Eyes_Open)_20220615143803_7.nii.gz
 
 ```
 
 In the case of the above folder structure, "/path/to/control" may simply be input into the MedImageLoader function. For multiple labels, "/path/to/test", "/path/to/test2", and so on, may also be input.
 
-Confound representation
-=======================
-
+Labels and Confounds
+====================
 
+MIMIM enables for the representation of labels to classify by and confounds to regress. Confounds are represented as strings and labels can be represented as either strings or the input folder structure to MedImageLoader.
```

### Comparing `multi_med_image_ml-0.0.7/pyproject.toml` & `multi_med_image_ml-0.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 
 name = "multi_med_image_ml"
 
-version = "0.0.7"
+version = "0.0.8"
 
 dependencies = [
   "numpy",
   "scipy",
   "torch",
   "torchvision",
   "opencv-python>=4.5.4",
```

### Comparing `multi_med_image_ml-0.0.7/PKG-INFO` & `multi_med_image_ml-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: multi_med_image_ml
-Version: 0.0.7
+Version: 0.0.8
 Summary: Deep learning library to encode multiple brain images and other electronic health record data in disease detection.
 Project-URL: Homepage, https://github.com/mleming/MultiMedImageML
 Author-email: Matt Leming <mleming@mgh.harvard.edu>
 Maintainer-email: Matt Leming <mleming@mgh.harvard.edu>
 License: MIT License
 Keywords: biomedical,deep learning,ehr,machine learning,mri,pytorch
 Requires-Python: >=3.8
@@ -26,15 +26,15 @@
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: slideio==2.4.1
 Requires-Dist: torch
 Requires-Dist: torchvision
 Description-Content-Type: text/markdown
 
-![ze logo](.images/logo.png)
+![ze logo](https://raw.githubusercontent.com/mleming/MultiMedImageML/main/.images/logo.png)
 
 Multi-Input Medical Image Machine Learning Toolkit
 ==================================================
 
 The Multi-Input Medical Image Machine Learning Toolkit (MultiMedImageML) is a library of Pytorch functions that can encode multiple 3D images (designed specifically for brain images) and offer a single- or multi-label output, such as a disease detection.
 
 Thus, with a dataset of brain images and labels, you can train a model to predict dementia or multiple sclerosis from multiple input brain images.
@@ -43,29 +43,29 @@
 
     pip install multi-med-image-ml
 
 
 Overview
 ========
 
-![ze figure](.images/model_diagram.png)
+![ze figure](https://raw.githubusercontent.com/mleming/MultiMedImageML/main/.images/model_diagram.png)
 
 The core deep learning architecture is a Pytorch model that can take in variable numbers of 3D images (between one and 14 by default), then encodes them into a numerical vector and, through an adversarial training process, creates an intermediate representation that contains information about disease biomarkers but not confounds, like patient age and scanning site.
 
-![ze regress figure](.images/regress_figure.png)
+![ze regress figure](https://raw.githubusercontent.com/mleming/MultiMedImageML/main/.images/regress_figure.png)
 
 The confound regression process essentially disguises the intermediary representation to have disease biomarker features while imitating the confounding features of other groups.
 
 Getting Started
 ===============
 
 Datasets
 ========
 
-This may be used with either public benchmark datasets of brain images or internal hospital records, so long as they're represented as DICOM or NIFTI images. It was largely tested on [https://adni.loni.usc.edu/data-samples/access-data/](ADNI) and data internal to MGH. If they're represented as DICOM images, they are converted to NIFTI with metadata represented as a JSON file using [https://github.com/rordenlab/dcm2niix](dcm2niix). They may be further converted to NPY files, which are resized to a specific dimension, with the metadata represented in a pandas dataframe.
+This may be used with either public benchmark datasets of brain images or internal hospital records, so long as they're represented as DICOM or NIFTI images. It was largely tested on [ADNI](https://adni.loni.usc.edu/data-samples/access-data/) and data internal to MGH. If they're represented as DICOM images, they are converted to NIFTI with metadata represented as a JSON file using [dcm2niix](https://github.com/rordenlab/dcm2niix). They may be further converted to NPY files, which are resized to a specific dimension, with the metadata represented in a pandas dataframe.
 
 The MedImageLoader builds up this representation automatically, but it is space-intensive to do so.
 
 Data may be represented with a folder structure.
 
 ```
 .
@@ -101,11 +101,11 @@
                     ├── I1591323_Axial_3D_PASL_(Eyes_Open)_20220615143803_7.json
                     └── I1591323_Axial_3D_PASL_(Eyes_Open)_20220615143803_7.nii.gz
 
 ```
 
 In the case of the above folder structure, "/path/to/control" may simply be input into the MedImageLoader function. For multiple labels, "/path/to/test", "/path/to/test2", and so on, may also be input.
 
-Confound representation
-=======================
-
+Labels and Confounds
+====================
 
+MIMIM enables for the representation of labels to classify by and confounds to regress. Confounds are represented as strings and labels can be represented as either strings or the input folder structure to MedImageLoader.
```

