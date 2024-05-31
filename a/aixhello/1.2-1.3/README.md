# Comparing `tmp/aixhello-1.2.tar.gz` & `tmp/aixhello-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixhello-1.2.tar", last modified: Fri May 31 09:07:41 2024, max compression
+gzip compressed data, was "aixhello-1.3.tar", last modified: Fri May 31 09:22:48 2024, max compression
```

## Comparing `aixhello-1.2.tar` & `aixhello-1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 09:07:41.212841 aixhello-1.2/
--rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-1.2/LICENSE
--rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      573 2024-05-31 09:07:41.212841 aixhello-1.2/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-05-31 08:12:32.000000 aixhello-1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 09:07:41.195843 aixhello-1.2/aixhello/
--rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-1.2/aixhello/__init__.py
--rw-rw-rw-   0        0        0   259945 2024-05-31 08:57:18.000000 aixhello-1.2/aixhello/xyello.c
-drwxrwxrwx   0        0        0        0 2024-05-31 09:07:41.211850 aixhello-1.2/aixhello.egg-info/
--rw-rw-rw-   0        0        0      573 2024-05-31 09:07:41.000000 aixhello-1.2/aixhello.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2024-05-31 09:07:41.000000 aixhello-1.2/aixhello.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 09:07:41.000000 aixhello-1.2/aixhello.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-31 09:07:41.000000 aixhello-1.2/aixhello.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-31 09:07:41.218842 aixhello-1.2/setup.cfg
--rw-rw-rw-   0        0        0      648 2024-05-31 09:04:48.000000 aixhello-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:22:48.048009 aixhello-1.3/
+-rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-1.3/LICENSE
+-rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      573 2024-05-31 09:22:48.048009 aixhello-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2024-05-31 08:12:32.000000 aixhello-1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 09:22:48.038739 aixhello-1.3/aixhello/
+-rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-1.3/aixhello/__init__.py
+-rw-rw-rw-   0        0        0   258883 2024-05-31 09:22:31.000000 aixhello-1.3/aixhello/xyello.c
+drwxrwxrwx   0        0        0        0 2024-05-31 09:22:48.047008 aixhello-1.3/aixhello.egg-info/
+-rw-rw-rw-   0        0        0      573 2024-05-31 09:22:47.000000 aixhello-1.3/aixhello.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2024-05-31 09:22:47.000000 aixhello-1.3/aixhello.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 09:22:47.000000 aixhello-1.3/aixhello.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-31 09:22:47.000000 aixhello-1.3/aixhello.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-31 09:22:48.050009 aixhello-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      968 2024-05-31 09:21:45.000000 aixhello-1.3/setup.py
```

### Comparing `aixhello-1.2/LICENSE` & `aixhello-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aixhello-1.2/PKG-INFO` & `aixhello-1.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 1.2
+Version: 1.3
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-1.2/aixhello/xyello.c` & `aixhello-1.3/aixhello/xyello.c`

 * *Files 1% similar despite different names*

```diff
@@ -2114,15 +2114,15 @@
   PyTypeObject *__pyx_CoroutineAwaitType;
   #endif
   #ifdef __Pyx_Coroutine_USED
   PyTypeObject *__pyx_CoroutineType;
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
-  PyObject *__pyx_kp_s_Please_insert_your_message;
+  PyObject *__pyx_kp_u_Please_insert_your_message;
   PyObject *__pyx_n_s__3;
   PyObject *__pyx_n_s_aixhello_xyello;
   PyObject *__pyx_kp_s_aixhello_xyello_pyx;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_cline_in_traceback;
   PyObject *__pyx_n_s_dict;
   PyObject *__pyx_n_s_doc;
@@ -2181,15 +2181,15 @@
   Py_CLEAR(clear_module_state->__pyx_empty_unicode);
   #ifdef __Pyx_CyFunction_USED
   Py_CLEAR(clear_module_state->__pyx_CyFunctionType);
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
   #endif
-  Py_CLEAR(clear_module_state->__pyx_kp_s_Please_insert_your_message);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_Please_insert_your_message);
   Py_CLEAR(clear_module_state->__pyx_n_s__3);
   Py_CLEAR(clear_module_state->__pyx_n_s_aixhello_xyello);
   Py_CLEAR(clear_module_state->__pyx_kp_s_aixhello_xyello_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
   Py_CLEAR(clear_module_state->__pyx_n_s_dict);
   Py_CLEAR(clear_module_state->__pyx_n_s_doc);
@@ -2226,15 +2226,15 @@
   Py_VISIT(traverse_module_state->__pyx_empty_unicode);
   #ifdef __Pyx_CyFunction_USED
   Py_VISIT(traverse_module_state->__pyx_CyFunctionType);
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
   #endif
-  Py_VISIT(traverse_module_state->__pyx_kp_s_Please_insert_your_message);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_Please_insert_your_message);
   Py_VISIT(traverse_module_state->__pyx_n_s__3);
   Py_VISIT(traverse_module_state->__pyx_n_s_aixhello_xyello);
   Py_VISIT(traverse_module_state->__pyx_kp_s_aixhello_xyello_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
   Py_VISIT(traverse_module_state->__pyx_n_s_dict);
   Py_VISIT(traverse_module_state->__pyx_n_s_doc);
@@ -2281,15 +2281,15 @@
 #define __pyx_CoroutineAwaitType __pyx_mstate_global->__pyx_CoroutineAwaitType
 #endif
 #ifdef __Pyx_Coroutine_USED
 #define __pyx_CoroutineType __pyx_mstate_global->__pyx_CoroutineType
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
-#define __pyx_kp_s_Please_insert_your_message __pyx_mstate_global->__pyx_kp_s_Please_insert_your_message
+#define __pyx_kp_u_Please_insert_your_message __pyx_mstate_global->__pyx_kp_u_Please_insert_your_message
 #define __pyx_n_s__3 __pyx_mstate_global->__pyx_n_s__3
 #define __pyx_n_s_aixhello_xyello __pyx_mstate_global->__pyx_n_s_aixhello_xyello
 #define __pyx_kp_s_aixhello_xyello_pyx __pyx_mstate_global->__pyx_kp_s_aixhello_xyello_pyx
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
 #define __pyx_n_s_dict __pyx_mstate_global->__pyx_n_s_dict
 #define __pyx_n_s_doc __pyx_mstate_global->__pyx_n_s_doc
@@ -2308,19 +2308,14 @@
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
 #define __pyx_n_s_xyellw __pyx_mstate_global->__pyx_n_s_xyellw
 #define __pyx_n_s_xyellw_say_msg __pyx_mstate_global->__pyx_n_s_xyellw_say_msg
 #define __pyx_tuple_ __pyx_mstate_global->__pyx_tuple_
 #define __pyx_codeobj__2 __pyx_mstate_global->__pyx_codeobj__2
 /* #### Code section: module_code ### */
 
-/* "aixhello/xyello.pyx":2
- * class xyellw:
- *     def say_msg(self):             # <<<<<<<<<<<<<<
- *         return "Please insert your message"
- */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_1say_msg(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
@@ -2415,29 +2410,19 @@
 }
 
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_say_msg(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("say_msg", 1);
 
-  /* "aixhello/xyello.pyx":3
- * class xyellw:
- *     def say_msg(self):
- *         return "Please insert your message"             # <<<<<<<<<<<<<<
- */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(__pyx_kp_s_Please_insert_your_message);
-  __pyx_r = __pyx_kp_s_Please_insert_your_message;
+  __Pyx_INCREF(__pyx_kp_u_Please_insert_your_message);
+  __pyx_r = __pyx_kp_u_Please_insert_your_message;
   goto __pyx_L0;
 
-  /* "aixhello/xyello.pyx":2
- * class xyellw:
- *     def say_msg(self):             # <<<<<<<<<<<<<<
- *         return "Please insert your message"
- */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -2454,15 +2439,15 @@
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 /* #### Code section: pystring_table ### */
 
 static int __Pyx_CreateStringTabAndInitStrings(void) {
   __Pyx_StringTabEntry __pyx_string_tab[] = {
-    {&__pyx_kp_s_Please_insert_your_message, __pyx_k_Please_insert_your_message, sizeof(__pyx_k_Please_insert_your_message), 0, 0, 1, 0},
+    {&__pyx_kp_u_Please_insert_your_message, __pyx_k_Please_insert_your_message, sizeof(__pyx_k_Please_insert_your_message), 0, 1, 0, 0},
     {&__pyx_n_s__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 0, 1, 1},
     {&__pyx_n_s_aixhello_xyello, __pyx_k_aixhello_xyello, sizeof(__pyx_k_aixhello_xyello), 0, 0, 1, 1},
     {&__pyx_kp_s_aixhello_xyello_pyx, __pyx_k_aixhello_xyello_pyx, sizeof(__pyx_k_aixhello_xyello_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
     {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
     {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
@@ -2491,19 +2476,14 @@
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "aixhello/xyello.pyx":2
- * class xyellw:
- *     def say_msg(self):             # <<<<<<<<<<<<<<
- *         return "Please insert your message"
- */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
   __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple_, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_say_msg, 2, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
@@ -2864,37 +2844,22 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "aixhello/xyello.pyx":1
- * class xyellw:             # <<<<<<<<<<<<<<
- *     def say_msg(self):
- *         return "Please insert your message"
- */
   __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_xyellw, __pyx_n_s_xyellw, (PyObject *) NULL, __pyx_n_s_aixhello_xyello, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "aixhello/xyello.pyx":2
- * class xyellw:
- *     def say_msg(self):             # <<<<<<<<<<<<<<
- *         return "Please insert your message"
- */
   __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_1say_msg, 0, __pyx_n_s_xyellw_say_msg, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__2)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_say_msg, __pyx_t_3) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "aixhello/xyello.pyx":1
- * class xyellw:             # <<<<<<<<<<<<<<
- *     def say_msg(self):
- *         return "Please insert your message"
- */
   __pyx_t_3 = __Pyx_Py3ClassCreate(((PyObject*)&PyType_Type), __pyx_n_s_xyellw, __pyx_empty_tuple, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_xyellw, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
```

### Comparing `aixhello-1.2/aixhello.egg-info/PKG-INFO` & `aixhello-1.3/aixhello.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 1.2
+Version: 1.3
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-1.2/setup.py` & `aixhello-1.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,34 @@
 from setuptools import setup, Extension
 from Cython.Build import cythonize
 
+extensions = [
+    Extension(
+        "aixhello.xyello",
+        ["aixhello/xyello.pyx"],
+    )
+]
+
+cythonize_options = {
+    'compiler_directives': {
+        'language_level': 3,          # Use Python 3 syntax
+        'emit_code_comments': False,  # Suppress the generation of code comments
+    }
+}
+
 setup(
     name='aixhello',
-    version='1.2',
+    version='1.3',  # Increment the version number
     description='AI HRM Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='SecureAI',
     author_email='package@xerocai.com',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
-    ext_modules=cythonize([Extension("aixhello.xyello", ["aixhello/xyello.pyx"])]),
+    ext_modules=cythonize(extensions, **cythonize_options),
     packages=['aixhello'],
-)
+)
```

