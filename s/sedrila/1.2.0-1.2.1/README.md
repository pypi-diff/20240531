# Comparing `tmp/sedrila-1.2.0.tar.gz` & `tmp/sedrila-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sedrila-1.2.0.tar", max compression
+gzip compressed data, was "sedrila-1.2.1.tar", max compression
```

## Comparing `sedrila-1.2.0.tar` & `sedrila-1.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1108 2022-11-04 08:14:04.746613 sedrila-1.2.0/LICENSE
--rwxr-xr-x   0        0        0     4087 2024-03-25 11:31:56.923322 sedrila-1.2.0/README.md
--rwxr-xr-x   0        0        0      622 2024-01-16 08:42:09.535422 sedrila-1.2.0/baseresources/favicon-32x32.png
--rwxr-xr-x   0        0        0       79 2024-01-06 12:00:53.054430 sedrila-1.2.0/baseresources/local.css
--rwxr-xr-x   0        0        0     7882 2024-04-04 09:44:27.185644 sedrila-1.2.0/baseresources/sedrila.css
--rwxr-xr-x   0        0        0     1929 2023-12-21 08:14:44.888758 sedrila-1.2.0/baseresources/sidebar.js
--rwxr-xr-x   0        0        0     6616 2024-05-17 11:08:38.901920 sedrila-1.2.0/py/base.py
--rwxr-xr-x   0        0        0     3501 2024-04-09 14:20:20.887078 sedrila-1.2.0/py/git.py
--rwxr-xr-x   0        0        0       34 2022-11-17 11:17:31.396262 sedrila-1.2.0/py/sdrl/__init__.py
--rwxr-xr-x   0        0        0    23644 2024-04-22 15:45:50.407435 sedrila-1.2.0/py/sdrl/course.py
--rwxr-xr-x   0        0        0     9777 2024-03-14 17:40:26.435091 sedrila-1.2.0/py/sdrl/glossary.py
--rwxr-xr-x   0        0        0     1209 2024-03-28 09:55:55.453116 sedrila-1.2.0/py/sdrl/html.py
--rwxr-xr-x   0        0        0     3902 2024-05-14 17:35:24.775544 sedrila-1.2.0/py/sdrl/interactive.py
--rwxr-xr-x   0        0        0     8393 2024-05-14 17:35:25.529976 sedrila-1.2.0/py/sdrl/macros.py
--rwxr-xr-x   0        0        0     4154 2024-05-14 17:35:25.184525 sedrila-1.2.0/py/sdrl/markdown.py
--rwxr-xr-x   0        0        0     6222 2024-04-09 14:20:22.676239 sedrila-1.2.0/py/sdrl/part.py
--rwxr-xr-x   0        0        0     1504 2024-02-23 11:01:27.759372 sedrila-1.2.0/py/sdrl/participant.py
--rwxr-xr-x   0        0        0     1334 2023-11-22 14:11:46.025037 sedrila-1.2.0/py/sdrl/replacements.py
--rwxr-xr-x   0        0        0     8344 2024-04-02 17:08:18.901707 sedrila-1.2.0/py/sdrl/repo.py
--rwxr-xr-x   0        0        0       31 2024-01-24 12:48:05.392624 sedrila-1.2.0/py/sdrl/subcmd/__init__.py
--rwxr-xr-x   0        0        0    28479 2024-05-01 09:55:22.353458 sedrila-1.2.0/py/sdrl/subcmd/author.py
--rwxr-xr-x   0        0        0     9005 2024-04-22 15:45:50.721474 sedrila-1.2.0/py/sdrl/subcmd/instructor.py
--rwxr-xr-x   0        0        0     5915 2024-05-14 18:01:22.555644 sedrila-1.2.0/py/sdrl/subcmd/student.py
--rwxr-xr-x   0        0        0      975 2024-02-24 16:55:02.006852 sedrila-1.2.0/py/sedrila.py
--rwxr-xr-x   0        0        0     2329 2024-05-17 11:08:38.891917 sedrila-1.2.0/pyproject.toml
--rwxr-xr-x   0        0        0     1546 2024-03-20 16:45:46.286389 sedrila-1.2.0/templates/base.html
--rwxr-xr-x   0        0        0      198 2023-12-21 08:24:47.653800 sedrila-1.2.0/templates/chapter.html
--rwxr-xr-x   0        0        0      154 2024-01-05 15:47:36.097811 sedrila-1.2.0/templates/glossary.html
--rwxr-xr-x   0        0        0      158 2023-12-21 08:24:47.628801 sedrila-1.2.0/templates/homepage.html
--rwxr-xr-x   0        0        0      312 2024-03-20 16:41:25.421337 sedrila-1.2.0/templates/task.html
--rwxr-xr-x   0        0        0      159 2023-12-21 08:24:47.660799 sedrila-1.2.0/templates/taskgroup.html
--rw-r--r--   0        0        0    11173 1970-01-01 00:00:00.000000 sedrila-1.2.0/setup.py
--rw-r--r--   0        0        0     5519 1970-01-01 00:00:00.000000 sedrila-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1108 2022-11-04 08:14:04.746613 sedrila-1.2.1/LICENSE
+-rwxr-xr-x   0        0        0     4087 2024-03-25 11:31:56.923322 sedrila-1.2.1/README.md
+-rwxr-xr-x   0        0        0      622 2024-01-16 08:42:09.535422 sedrila-1.2.1/baseresources/favicon-32x32.png
+-rwxr-xr-x   0        0        0       79 2024-01-06 12:00:53.054430 sedrila-1.2.1/baseresources/local.css
+-rwxr-xr-x   0        0        0     7882 2024-04-04 09:44:27.185644 sedrila-1.2.1/baseresources/sedrila.css
+-rwxr-xr-x   0        0        0     1929 2023-12-21 08:14:44.888758 sedrila-1.2.1/baseresources/sidebar.js
+-rwxr-xr-x   0        0        0     6616 2024-05-31 11:06:56.667135 sedrila-1.2.1/py/base.py
+-rwxr-xr-x   0        0        0     3501 2024-04-09 14:20:20.887078 sedrila-1.2.1/py/git.py
+-rwxr-xr-x   0        0        0       34 2022-11-17 11:17:31.396262 sedrila-1.2.1/py/sdrl/__init__.py
+-rwxr-xr-x   0        0        0    23686 2024-05-31 10:51:06.427633 sedrila-1.2.1/py/sdrl/course.py
+-rwxr-xr-x   0        0        0     9777 2024-03-14 17:40:26.435091 sedrila-1.2.1/py/sdrl/glossary.py
+-rwxr-xr-x   0        0        0     1209 2024-03-28 09:55:55.453116 sedrila-1.2.1/py/sdrl/html.py
+-rwxr-xr-x   0        0        0     3990 2024-05-29 16:50:08.943081 sedrila-1.2.1/py/sdrl/interactive.py
+-rwxr-xr-x   0        0        0     8393 2024-05-14 17:35:25.529976 sedrila-1.2.1/py/sdrl/macros.py
+-rwxr-xr-x   0        0        0     4154 2024-05-14 17:35:25.184525 sedrila-1.2.1/py/sdrl/markdown.py
+-rwxr-xr-x   0        0        0     6222 2024-04-09 14:20:22.676239 sedrila-1.2.1/py/sdrl/part.py
+-rwxr-xr-x   0        0        0     1504 2024-02-23 11:01:27.759372 sedrila-1.2.1/py/sdrl/participant.py
+-rwxr-xr-x   0        0        0     1334 2023-11-22 14:11:46.025037 sedrila-1.2.1/py/sdrl/replacements.py
+-rwxr-xr-x   0        0        0     8344 2024-04-02 17:08:18.901707 sedrila-1.2.1/py/sdrl/repo.py
+-rwxr-xr-x   0        0        0       31 2024-01-24 12:48:05.392624 sedrila-1.2.1/py/sdrl/subcmd/__init__.py
+-rwxr-xr-x   0        0        0    28479 2024-05-01 09:55:22.353458 sedrila-1.2.1/py/sdrl/subcmd/author.py
+-rwxr-xr-x   0        0        0     9005 2024-04-22 15:45:50.721474 sedrila-1.2.1/py/sdrl/subcmd/instructor.py
+-rwxr-xr-x   0        0        0     5915 2024-05-14 18:01:22.555644 sedrila-1.2.1/py/sdrl/subcmd/student.py
+-rwxr-xr-x   0        0        0      975 2024-02-24 16:55:02.006852 sedrila-1.2.1/py/sedrila.py
+-rwxr-xr-x   0        0        0     2329 2024-05-31 11:06:56.678101 sedrila-1.2.1/pyproject.toml
+-rwxr-xr-x   0        0        0     1546 2024-03-20 16:45:46.286389 sedrila-1.2.1/templates/base.html
+-rwxr-xr-x   0        0        0      198 2023-12-21 08:24:47.653800 sedrila-1.2.1/templates/chapter.html
+-rwxr-xr-x   0        0        0      154 2024-01-05 15:47:36.097811 sedrila-1.2.1/templates/glossary.html
+-rwxr-xr-x   0        0        0      158 2023-12-21 08:24:47.628801 sedrila-1.2.1/templates/homepage.html
+-rwxr-xr-x   0        0        0      312 2024-03-20 16:41:25.421337 sedrila-1.2.1/templates/task.html
+-rwxr-xr-x   0        0        0      159 2023-12-21 08:24:47.660799 sedrila-1.2.1/templates/taskgroup.html
+-rw-r--r--   0        0        0    11173 1970-01-01 00:00:00.000000 sedrila-1.2.1/setup.py
+-rw-r--r--   0        0        0     5519 1970-01-01 00:00:00.000000 sedrila-1.2.1/PKG-INFO
```

### Comparing `sedrila-1.2.0/LICENSE` & `sedrila-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.0/README.md` & `sedrila-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.0/baseresources/favicon-32x32.png` & `sedrila-1.2.1/baseresources/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.0/baseresources/sedrila.css` & `sedrila-1.2.1/baseresources/sedrila.css`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.0/baseresources/sidebar.js` & `sedrila-1.2.1/baseresources/sidebar.js`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.0/py/base.py` & `sedrila-1.2.1/py/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import requests
 import rich
 import rich.table
 import yaml
 
 
-SEDRILA_VERSION = "1.2.0"  # keep in sync with pyproject.toml
+SEDRILA_VERSION = "1.2.1"  # keep in sync with pyproject.toml
 CONFIG_FILENAME = "sedrila.yaml"  # at top-level of source dir
 GLOSSARY_BASENAME = "glossary"  # .md at top-level of chapterdir, .html in build directory
 METADATA_FILE = "course.json"  # at top-level of build directory
 CACHE_FILE = "course.pickle"  # at top-level of instructor build directory
 TEMPLATES_DIR = "templates"
 SEDRILA_COMMAND_ENV = "SEDRILA_COMMAND"
```

### Comparing `sedrila-1.2.0/py/git.py` & `sedrila-1.2.1/py/git.py`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.0/py/sdrl/course.py` & `sedrila-1.2.1/py/sdrl/course.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,17 +78,18 @@
                     title=self.title, timevalue=self.timevalue, difficulty=self.difficulty,
                     assumes=self.assumes, requires=self.requires)
 
     def from_file(self, file: str, taskgroup: 'Taskgroup') -> 'Task':
         """Initializer used in author mode"""
         self.read_partsfile(file)
         # ----- get taskdata from file:
-        nameparts = os.path.basename(self.sourcefile).split('.')
-        assert len(nameparts) == 2  # taskname, suffix 'md'
-        self.slug = nameparts[0]  # must be globally unique
+        filename = os.path.basename(self.sourcefile)
+        mm = re.fullmatch(r"(.+)\.md", filename)
+        assert mm, filename  # we only get handed .md files here 
+        self.slug = mm.group(1)  # must be globally unique
         self.outputfile = f"{self.slug}.html"
         b.copyattrs(file,
                     self.metadata, self,
                     mustcopy_attrs='title, timevalue, difficulty',
                     cancopy_attrs='stage, explains, assumes, requires',
                     mustexist_attrs='',
                     typecheck=dict(timevalue=numbers.Number, difficulty=int))
```

### Comparing `sedrila-1.2.0/py/sdrl/glossary.py` & `sedrila-1.2.1/py/sdrl/glossary.py`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.0/py/sdrl/html.py` & `sedrila-1.2.1/py/sdrl/html.py`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.0/py/sdrl/interactive.py` & `sedrila-1.2.1/py/sdrl/interactive.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,16 @@
             elif str(inp) == "j" or str(inp.name) == "KEY_DOWN":
                 if rowindex < len(entries) - 1:
                     rowindex += 1
             elif str(inp) == "k" or str(inp.name) == "KEY_UP":
                 if rowindex > 0:
                     rowindex -= 1
             elif not(course_url is None) and (str(inp) == "o" or str(inp) == "O"):
-                webbrowser.open(f"{course_url}/{entries[rowindex][0]}.html")
+                webbrowser.open(f"{course_url}/{entries[rowindex][0]}.html")  # TODO 2 on WSL, see 
+                # https://github.com/python/cpython/issues/89752
 
 
 def select_entries(entries: tg.Sequence[r.ReportEntry]):
     selected = {entry[0]: True for entry in entries}
     filter_entries(entries, selected, None, None)
     return list(filter(lambda entry: selected[entry[0]], entries))
```

### Comparing `sedrila-1.2.0/py/sdrl/macros.py` & `sedrila-1.2.1/py/sdrl/macros.py`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.0/py/sdrl/markdown.py` & `sedrila-1.2.1/py/sdrl/markdown.py`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.0/py/sdrl/part.py` & `sedrila-1.2.1/py/sdrl/part.py`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.0/py/sdrl/participant.py` & `sedrila-1.2.1/py/sdrl/participant.py`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.0/py/sdrl/replacements.py` & `sedrila-1.2.1/py/sdrl/replacements.py`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.0/py/sdrl/repo.py` & `sedrila-1.2.1/py/sdrl/repo.py`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.0/py/sdrl/subcmd/author.py` & `sedrila-1.2.1/py/sdrl/subcmd/author.py`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.0/py/sdrl/subcmd/instructor.py` & `sedrila-1.2.1/py/sdrl/subcmd/instructor.py`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.0/py/sdrl/subcmd/student.py` & `sedrila-1.2.1/py/sdrl/subcmd/student.py`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.0/py/sedrila.py` & `sedrila-1.2.1/py/sedrila.py`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.0/pyproject.toml` & `sedrila-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # https://packaging.python.org/en/latest/
 # https://packaging.python.org/en/latest/specifications/pyproject-toml/
 # https://packaging.python.org/en/latest/guides/writing-pyproject-toml/
 # https://python-poetry.org/docs/pyproject/
 [tool.poetry]
 name = "sedrila"
-version = "1.2.0"  # keep in sync with base.py
+version = "1.2.1"  # keep in sync with base.py
 description = "Tool infrastructure for building and running \"self-driven lab\" courses"
 license = "MIT"
 authors = ["Lutz Prechelt <prechelt@inf.fu-berlin.de>"]
 readme = "README.md"
 homepage = "https://github.com/fubinf/sedrila"
 repository = "https://github.com/fubinf/sedrila"
 keywords = ["static site generator"]
```

### Comparing `sedrila-1.2.0/templates/base.html` & `sedrila-1.2.1/templates/base.html`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.0/setup.py` & `sedrila-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
  'rich>=13.7,<14.0']
 
 entry_points = \
 {'console_scripts': ['sedrila = sedrila:main']}
 
 setup_kwargs = {
     'name': 'sedrila',
-    'version': '1.2.0',
+    'version': '1.2.1',
     'description': 'Tool infrastructure for building and running "self-driven lab" courses',
     'long_description': '[![Documentation Status](https://readthedocs.org/projects/sedrila/badge/?version=latest)](https://sedrila.readthedocs.io/en/latest/?badge=latest)\n\n# `sedrila`: Tool infrastructure for building and running "self-driven lab" courses\n\nA "self-driven lab" (SeDriLa) course is one where students select freely \na subset from a large set of tasks.\nThe tasks are described with sufficient detail that no guidance from an instructor\nis needed most of the time.\n\nsedrila is a command-line tool supporting course authors for authoring a course\nand then course instructors and students for executing it.\n\nFind the [documentation at readthedocs](https://sedrila.readthedocs.io).\n\n\n## Ideas for future versions\n\n- Process `SEDRILA_INSTRUCTOR_COURSE_URLS` as described in the instructor documentation.\n- `sedrila instructor` should keep a JSON file `student_course_urls.json` that maps student usernames\n  to the course URL first seen for that student, because if a student ever changed\n  the URL in the `student.yaml`, prior signed commits of instructors might become \n  invalid semantically if the new course has a different set of tasks.  \n  The map is added to when a `student.yaml` is first seen\n  and checked against at each later time.  \n  Note that a student taking part a second time, with a fresh repo,\n  might require manual editing of that JSON file to remove that entry.\n- Better yet, there could be an option `sedrial instructor --allow-repo2` that \n  performs that editing automatically\n  and also checks that the new repo contains no instructor-signed commits.\n- Command `sedrila instructor --clean-up-repos-home`\n  to clean up instructor work directory trees-of-trees\n  by deleting all level-1 subtrees in which the `student.yaml`\n  has a `course_url` that is not mentioned in the \n  `SEDRILA_INSTRUCTOR_COURSE_URLS`environment variable.\n  This option should ask a safety question before starting to work.\n\n\n## Development process: TODO-handling during development\n\nWe use this convention for the development of `sedrila`.\nIt may also be helpful for course authors if the team is small enough.\n\nIf something is incomplete, add a TODO marker with a priorization digit:\n- `TODO 1`: to be completed soon (within a few days)\n- `TODO 2`: to be completed once the prio 1 things are done (within days or a few weeks)\n- `TODO 3`: to be completed at some later time (usually several weeks or more into the future,\n  because it is big) or never (because it is not-so-important: "nice-to-have features")\n\nAdd a short description of what needs to be done. Examples:\n- `TODO 1: find proper formulation`\n- `TODO 2: restructure to use ACME lib`\n- `TODO 3: add automatic grammar correction`\n\nIf you intend to do it yourself, add your name in parens:  \n`TODO 1: find proper formulation (Lutz)`\n\nThen use the IDE global search to work through these layer-by-layer.\nDemote items to a lower priority when they become stale or remove them.\nKick out prio 3 items when they become unlikely.\n\n\n## A currently needed refactoring: Target directory structure\n\nThe current layout of the source tree is wrong.\nCurrently, the `templates` and `baseresources` directories will end up \nas top-level directories when the package is installed,\nwhich means they will clash with any top-level modules of that name\nanywhere in our dependencies.\n\nWe need to perform the following refactorings to arrive at a proper structure:\n\n- `py` --> `sedrila`: This will be the top level directory that gets installed.\n- `sedrila/sdrl/*` --> `sedrila/*`: We remove the now-intermediate namespace.\n  This implies joining the current `sdrl/tests` into `sedrila/tests`.\n- `templates` --> `sedrila/templates`: The HTML templates simply become part of the\n  tree to be installed.\n- `baseresources` --> `sedrila/baseresources`: Ditto.\n\nThese changes require a lot of changes of import statements.\nFor instance, the current module `base` will become `sedrila.base`\nand `sdrl.course` will become `sedrila.course`.\nThe logic for computing `sedrila_libdir` in `courses.py` must be adapted.\nThe files lists in `pyproject.toml` must be corrected.\n',
     'author': 'Lutz Prechelt',
     'author_email': 'prechelt@inf.fu-berlin.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fubinf/sedrila',
```

### Comparing `sedrila-1.2.0/PKG-INFO` & `sedrila-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sedrila
-Version: 1.2.0
+Version: 1.2.1
 Summary: Tool infrastructure for building and running "self-driven lab" courses
 Home-page: https://github.com/fubinf/sedrila
 License: MIT
 Keywords: static site generator
 Author: Lutz Prechelt
 Author-email: prechelt@inf.fu-berlin.de
 Requires-Python: >=3.11,<4.0
```

