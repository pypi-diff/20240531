# Comparing `tmp/cliexercises-2.1.2.tar.gz` & `tmp/cliexercises-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, from Unix
```

## Comparing `cliexercises-2.1.2.tar` & `cliexercises-2.2.0.tar`

### file list

```diff
@@ -1,45 +1,52 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/__init__.py
--rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/app_guide.md
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/cli_exercises.css
--rw-r--r--   0        0        0     9336 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/cli_exercises.py
--rw-r--r--   0        0        0    27383 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/questions.json
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/user_progress.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/.hidden
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/anchors.txt
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/blocks.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/c1.txt
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/c2.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/code.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/colors.txt
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/duplicates.txt
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/file_size.txt
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/fruits.txt
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/fun.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/greeting.txt
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/hex.txt
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/ip.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/lines.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/multi_empty_lines.txt
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/names.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/nums_1.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/nums_2.txt
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/patterns.txt
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/purchases.txt
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/range.txt
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/replace.txt
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/sample.txt
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/scores.csv
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/shopping_feb.txt
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/shopping_jan.txt
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/table.txt
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/timings.txt
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/twos.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/varying_fields.csv
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/backups/color list.txt
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/backups/dot_files/.bash_aliases
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/backups/dot_files/.inputrc
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cliexercises-2.1.2/src/cliexercises/sample_input/backups/text/ip.txt
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 cliexercises-2.1.2/LICENSE
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 cliexercises-2.1.2/README.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 cliexercises-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 cliexercises-2.1.2/PKG-INFO
+drwxrwxr-x   0 sundeep   (1000) sundeep   (1000)        0 2024-05-31 05:42:12.000000 cliexercises-2.2.0/
+drwxrwxr-x   0 sundeep   (1000) sundeep   (1000)        0 2024-05-31 05:40:29.000000 cliexercises-2.2.0/src/
+drwxrwxr-x   0 sundeep   (1000) sundeep   (1000)        0 2024-05-31 05:40:29.000000 cliexercises-2.2.0/src/cliexercises/
+drwxrwxr-x   0 sundeep   (1000) sundeep   (1000)        0 2024-05-31 05:40:29.000000 cliexercises-2.2.0/src/cliexercises/sample_input/
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       21 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/.hidden
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       40 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/c1.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)      100 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/anchors.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)      634 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/patterns.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       25 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/greeting.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       61 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/blocks.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       87 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/fruits.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       39 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/c2.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)      183 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/sample.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       43 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/shopping_feb.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       84 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/file_size.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       41 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/nums_2.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)      119 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/range.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       22 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/lines.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       40 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/colors.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       57 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/purchases.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       48 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/replace.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       39 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/fun.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       70 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/scores.csv
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       98 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/twos.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       69 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/varying_fields.csv
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       13 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/nums_1.txt
+drwxrwxr-x   0 sundeep   (1000) sundeep   (1000)        0 2024-05-31 05:40:29.000000 cliexercises-2.2.0/src/cliexercises/sample_input/backups/
+drwxrwxr-x   0 sundeep   (1000) sundeep   (1000)        0 2024-05-31 05:40:29.000000 cliexercises-2.2.0/src/cliexercises/sample_input/backups/dot_files/
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       26 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/backups/dot_files/.bash_aliases
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       30 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/backups/dot_files/.inputrc
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       15 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/backups/color list.txt
+drwxrwxr-x   0 sundeep   (1000) sundeep   (1000)        0 2024-05-31 05:40:29.000000 cliexercises-2.2.0/src/cliexercises/sample_input/backups/text/
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       23 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/backups/text/ip.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       77 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/hex.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       42 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/shopping_jan.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       79 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/table.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       63 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/code.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       49 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/timings.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)        8 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/names.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       60 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/multi_empty_lines.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)      151 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/duplicates.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       76 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/sample_input/ip.txt
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)      703 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/cli_exercises.css
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)       19 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/user_progress.json
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)        0 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/__init__.py
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)     9371 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/cli_exercises.py
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)    27383 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/questions.json
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)     3868 2020-02-02 00:00:00.000000 cliexercises-2.2.0/src/cliexercises/app_guide.md
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)      760 2020-02-02 00:00:00.000000 cliexercises-2.2.0/pyproject.toml
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)      991 2020-02-02 00:00:00.000000 cliexercises-2.2.0/README.md
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)     1072 2020-02-02 00:00:00.000000 cliexercises-2.2.0/LICENSE
+-rw-r--r--   0 sundeep   (1000) sundeep   (1000)     1613 2024-05-31 05:42:12.000000 cliexercises-2.2.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `cliexercises-2.1.2/src/cliexercises/app_guide.md` & `cliexercises-2.2.0/src/cliexercises/app_guide.md`

 * *Files identical despite different names*

### Comparing `cliexercises-2.1.2/src/cliexercises/cli_exercises.css` & `cliexercises-2.2.0/src/cliexercises/cli_exercises.css`

 * *Files identical despite different names*

### Comparing `cliexercises-2.1.2/src/cliexercises/cli_exercises.py` & `cliexercises-2.2.0/src/cliexercises/cli_exercises.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 SCRIPT_DIR = Path(__file__).parent.resolve()
 
 class CLIExercisesApp(App):
     CSS_PATH = SCRIPT_DIR.joinpath('cli_exercises.css')
     BINDINGS = [
         Binding('ctrl+s', 'show_solution', 'Solution', show=True),
-        Binding('ctrl+p', 'previous', 'Prev', show=True),
+        Binding('ctrl+p', 'previous', 'Previous', show=True),
         Binding('ctrl+n', 'next', 'Next', show=True),
         Binding('f1', 'app_guide', 'App Guide', show=False),
         Binding('f2', 'cli_exercises', 'CLI Exercises', show=False),
         Binding('f3', 'directory', 'Directory', show=False),
         ('ctrl+t', 'toggle_theme', 'Theme'),
         ('ctrl+q', 'app.quit', 'Quit'),
     ]
@@ -132,34 +132,34 @@
         self.solved = False
         self.l_question.update(
                 Markdown(f'(Q:{self.q_idx+1}/{self.q_max_idx+1}) ' +
                          self.questions[self.q_idx]['question']))
         self.ref_solution = self.questions[self.q_idx]['ref_solution']
 
         self.h_ip_op.remove()
-        v_ip = Vertical(classes='ip_op_container')
-        v_op = Vertical(classes='ip_op_container')
         ip_files = self.questions[self.q_idx]['ip_file']
-        if ip_files:
-            self.h_ip_op = Horizontal(v_ip, v_op, classes='container')
-        else:
-            self.h_ip_op = v_op
-        self.v_exercises.mount(self.h_ip_op)
-
+        v_ip_widgets = []
         for ip_file in ip_files:
             with open(ip_file, encoding='ascii') as f:
                 ip_txt = self.trim(f.read())
             l_ip = Label(ip_txt, classes='ip_op', markup=False)
             l_ip.border_title = ip_file
-            v_ip.mount(l_ip)
+            v_ip_widgets.append(l_ip)
 
         self.op_txt = self.trim(self.questions[self.q_idx]['op_file'])
         l_op = Label(self.op_txt, classes='ip_op', markup=False)
         l_op.border_title = 'Expected output'
-        v_op.mount(l_op)
+
+        v_ip = Vertical(*v_ip_widgets, classes='ip_op_container')
+        v_op = Vertical(l_op, classes='ip_op_container')
+        if ip_files:
+            self.h_ip_op = Horizontal(v_ip, v_op, classes='container')
+        else:
+            self.h_ip_op = v_op
+        self.v_exercises.mount(self.h_ip_op)
 
         if self.q_idx in self.user_progress:
             self.set_cmd(self.user_progress[self.q_idx][0])
         else:
             self.i_cmd.value = ''
             self.i_cmd.styles.background = 'lightgray'
             self.l_cmd_output.update('')
```

### Comparing `cliexercises-2.1.2/src/cliexercises/questions.json` & `cliexercises-2.2.0/src/cliexercises/questions.json`

 * *Files identical despite different names*

### Comparing `cliexercises-2.1.2/src/cliexercises/sample_input/patterns.txt` & `cliexercises-2.2.0/src/cliexercises/sample_input/patterns.txt`

 * *Files identical despite different names*

### Comparing `cliexercises-2.1.2/LICENSE` & `cliexercises-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cliexercises-2.1.2/README.md` & `cliexercises-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cliexercises-2.1.2/pyproject.toml` & `cliexercises-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 name = "cliexercises"
-version = "2.1.2"
+version = "2.2.0"
 authors = [
   { name="Sundeep Agarwal", email="learnbyexample.net@gmail.com" },
 ]
 description = "60+ beginner to intermediate level questions on CLI text processing tasks"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "textual>=0.46.0",
+  "textual>=0.63.6",
 ]
 
 [project.scripts]
 cliexercises = "cliexercises.cli_exercises:main"
 
 [project.urls]
 "Source" = "https://github.com/learnbyexample/TUI-apps/tree/main/CLI-Exercises"
```

### Comparing `cliexercises-2.1.2/PKG-INFO` & `cliexercises-2.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: cliexercises
-Version: 2.1.2
+Version: 2.2.0
 Summary: 60+ beginner to intermediate level questions on CLI text processing tasks
 Project-URL: Source, https://github.com/learnbyexample/TUI-apps/tree/main/CLI-Exercises
 Project-URL: Issues, https://github.com/learnbyexample/TUI-apps/issues
 Author-email: Sundeep Agarwal <learnbyexample.net@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
-Requires-Dist: textual>=0.46.0
+Requires-Dist: textual>=0.63.6
 Description-Content-Type: text/markdown
 
 # Linux CLI Text Processing Exercises
 
 This TUI application includes 60+ questions to test your CLI text processing skills.
 
 > **Note:** This application is intended for exercises based on Linux CLI tools. You might still be able to solve the exercises on other platforms, but I'm not sure if it works.
```

