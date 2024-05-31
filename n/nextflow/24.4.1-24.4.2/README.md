# Comparing `tmp/nextflow-24.4.1.tar.gz` & `tmp/nextflow-24.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextflow-24.4.1.tar", last modified: Tue May 21 16:46:42 2024, max compression
+gzip compressed data, was "nextflow-24.4.2.tar", last modified: Fri May 31 09:40:24 2024, max compression
```

## Comparing `nextflow-24.4.1.tar` & `nextflow-24.4.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-05-21 16:46:42.724222 nextflow-24.4.1/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1417 2024-05-21 16:46:42.724222 nextflow-24.4.1/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      877 2023-01-24 06:27:33.000000 nextflow-24.4.1/README.md
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-05-21 16:46:42.724222 nextflow-24.4.1/launcher/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    16053 2024-05-21 16:46:42.000000 nextflow-24.4.1/launcher/nextflow
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-05-21 16:46:42.724222 nextflow-24.4.1/nextflow.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1417 2024-05-21 16:46:42.000000 nextflow-24.4.1/nextflow.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      164 2024-05-21 16:46:42.000000 nextflow-24.4.1/nextflow.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2024-05-21 16:46:42.000000 nextflow-24.4.1/nextflow.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2024-05-21 16:46:42.000000 nextflow-24.4.1/nextflow.egg-info/top_level.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       38 2024-05-21 16:46:42.724222 nextflow-24.4.1/setup.cfg
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      805 2024-05-21 16:44:01.000000 nextflow-24.4.1/setup.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-05-31 09:40:24.392436 nextflow-24.4.2/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1417 2024-05-31 09:40:24.392436 nextflow-24.4.2/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      877 2023-01-24 06:27:33.000000 nextflow-24.4.2/README.md
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-05-31 09:40:24.392436 nextflow-24.4.2/launcher/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    16068 2024-05-31 09:40:24.000000 nextflow-24.4.2/launcher/nextflow
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-05-31 09:40:24.392436 nextflow-24.4.2/nextflow.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1417 2024-05-31 09:40:24.000000 nextflow-24.4.2/nextflow.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      164 2024-05-31 09:40:24.000000 nextflow-24.4.2/nextflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2024-05-31 09:40:24.000000 nextflow-24.4.2/nextflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2024-05-31 09:40:24.000000 nextflow-24.4.2/nextflow.egg-info/top_level.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       38 2024-05-31 09:40:24.392436 nextflow-24.4.2/setup.cfg
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      805 2024-05-31 09:37:53.000000 nextflow-24.4.2/setup.py
```

### Comparing `nextflow-24.4.1/PKG-INFO` & `nextflow-24.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextflow
-Version: 24.4.1
+Version: 24.4.2
 Summary: A Python wrapper that installs the Nextflow launcher
 Home-page: UNKNOWN
 Author: Jordi Deu-Pons
 License: Apache License 2.0
 Keywords: pipeline,workflow,nextflow
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `nextflow-24.4.1/README.md` & `nextflow-24.4.2/README.md`

 * *Files identical despite different names*

### Comparing `nextflow-24.4.1/launcher/nextflow` & `nextflow-24.4.2/launcher/nextflow`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 [[ "$NXF_DEBUG" == 'x' ]] && set -x
-NXF_VER=${NXF_VER:-'24.04.1'}
+NXF_VER=${NXF_VER:-'24.04.2'}
 NXF_ORG=${NXF_ORG:-'nextflow-io'}
 NXF_HOME=${NXF_HOME:-$HOME/.nextflow}
 NXF_PROT=${NXF_PROT:-'https'}
 NXF_BASE=${NXF_BASE:-$NXF_PROT://www.nextflow.io/releases}
 NXF_TEMP=${NXF_TEMP:-$TMPDIR}
 NXF_DIST=${NXF_DIST:-$NXF_HOME/framework}
 NXF_CLI="$0 $@"
@@ -307,28 +307,28 @@
   major=${BASH_REMATCH[1]}
   minor=${BASH_REMATCH[2]}
   # legacy version - Java 7/8 only
   if [ $major -eq 0 ] && [ $minor -lt 26 ]; then
     version_check="^(1.7|1.8)"
     version_message="Java 7 or 8"
   else
-    version_check="^(1.8|9|10|11|12|13|14|15|16|17|18|19|20|21)"
+    version_check="^(1.8|9|10|11|12|13|14|15|16|17|18|19|20|21|22)"
     version_message="Java 8 or later (up to 21)"
   fi
   if [[ ! $JAVA_VER =~ $version_check ]]; then
       echo_red "ERROR: Cannot find Java or it's a wrong version -- please make sure that $version_message is installed"
       if [[ "$NXF_JAVA_HOME" ]]; then
       echo_yellow "NOTE: Nextflow is trying to use the Java VM defined by the following environment variables:\n JAVA_CMD: $JAVA_CMD\n NXF_JAVA_HOME: $NXF_JAVA_HOME\n"
       else
       echo_yellow "NOTE: Nextflow is trying to use the Java VM defined by the following environment variables:\n JAVA_CMD: $JAVA_CMD\n JAVA_HOME: $JAVA_HOME\n"
       fi
       exit 1
   fi
-  if [[ ! $JAVA_VER =~ ^(11|12|13|14|15|16|17|18|19|20|21) ]]; then
-      echo_yellow "NOTE: Nextflow is not tested with Java $JAVA_VER -- It's recommended the use of version 11 up to 21\n"
+  if [[ ! $JAVA_VER =~ ^(11|12|13|14|15|16|17|18|19|20|21|22) ]]; then
+      echo_yellow "NOTE: Nextflow is not tested with Java $JAVA_VER -- It's recommended the use of version 11 up to 22\n"
   fi
   mkdir -p "$(dirname "$JAVA_KEY")"
   [[ -f $JAVA_VER ]] && echo $JAVA_VER > "$JAVA_KEY"
 fi
 
 # Verify nextflow jar is available
 if [ ! -f "$NXF_BIN" ]; then
@@ -342,15 +342,15 @@
 COLUMNS=${COLUMNS:-`tty -s && tput cols 2>/dev/null || true`}
 declare -a JAVA_OPTS=()
 JAVA_OPTS+=(-Dfile.encoding=UTF-8 -Dcapsule.trampoline -Dcapsule.java.cmd="$JAVA_CMD" -Dcom.sun.security.enableAIAcaIssuers=true)
 if [[ $cmd == console ]]; then bg=1;
 else JAVA_OPTS+=(-Djava.awt.headless=true)
 fi
 
-[[ "$JAVA_VER" =~ ^(21) ]] && [[ ! "$NXF_ENABLE_VIRTUAL_THREADS" ]] && NXF_ENABLE_VIRTUAL_THREADS=true
+[[ "$JAVA_VER" =~ ^(21|22) ]] && [[ ! "$NXF_ENABLE_VIRTUAL_THREADS" ]] && NXF_ENABLE_VIRTUAL_THREADS=true
 [[ "$JAVA_HOME" ]] && JAVA_OPTS+=(-Dcapsule.java.home="$JAVA_HOME")
 [[ "$CAPSULE_LOG" ]] && JAVA_OPTS+=(-Dcapsule.log=$CAPSULE_LOG)
 [[ "$CAPSULE_RESET" ]] && JAVA_OPTS+=(-Dcapsule.reset=true)
 [[ "$cmd" != "run" && "$cmd" != "node" ]] && JAVA_OPTS+=(-XX:+TieredCompilation -XX:TieredStopAtLevel=1)
 [[ "$NXF_OPTS" ]] && JAVA_OPTS+=($NXF_OPTS)
 [[ "$NXF_CLASSPATH" ]] && export NXF_CLASSPATH
 [[ "$NXF_GRAB" ]] && export NXF_GRAB
@@ -413,15 +413,15 @@
     declare -a cmd_base="(${BASH_REMATCH[1]})"
     declare -a cmd_tail="(${BASH_REMATCH[2]})"
 
     launcher="${cmd_base[@]}"
     [[ "$NXF_JVM_ARGS" ]] && launcher+=($NXF_JVM_ARGS)
     [[ "$remote_debug" ]] && launcher+=(-agentlib:jdwp=transport=dt_socket,server=y,suspend=y,address=$NXF_REMOTE_DEBUG_PORT)
 
-    if [[ "$JAVA_VER" =~ ^(9|10|11|12|13|14|15|16|17|18|19|20|21) ]]; then
+    if [[ "$JAVA_VER" =~ ^(9|10|11|12|13|14|15|16|17|18|19|20|21|22) ]]; then
       launcher+=(--add-opens=java.base/java.lang=ALL-UNNAMED)
       launcher+=(--add-opens=java.base/java.io=ALL-UNNAMED)
       launcher+=(--add-opens=java.base/java.nio=ALL-UNNAMED)
       launcher+=(--add-opens=java.base/java.net=ALL-UNNAMED)
       launcher+=(--add-opens=java.base/java.util=ALL-UNNAMED)
       launcher+=(--add-opens=java.base/java.util.concurrent.locks=ALL-UNNAMED)
       launcher+=(--add-opens=java.base/java.util.concurrent.atomic=ALL-UNNAMED)
@@ -433,15 +433,15 @@
       launcher+=(--add-opens=java.base/sun.net.www.protocol.ftp=ALL-UNNAMED)
       launcher+=(--add-opens=java.base/sun.net.www.protocol.file=ALL-UNNAMED)
       launcher+=(--add-opens=java.base/jdk.internal.misc=ALL-UNNAMED)
       launcher+=(--add-opens=java.base/jdk.internal.vm=ALL-UNNAMED)
       launcher+=(--add-opens=java.base/java.util.regex=ALL-UNNAMED)
       if [[ "$NXF_ENABLE_VIRTUAL_THREADS" == 'true' ]]; then
         if [[ "$JAVA_VER" =~ ^(19|20) ]]; then launcher+=(--enable-preview)
-        elif [[ ! "$JAVA_VER" =~ ^(21) ]]; then die "Virtual threads require Java 19 or later - current version $JAVA_VER"
+        elif [[ ! "$JAVA_VER" =~ ^(21|22) ]]; then die "Virtual threads require Java 19 or later - current version $JAVA_VER"
         fi
       fi
       launcher+=("${cmd_tail[@]}")
     else
       launcher+=("${cmd_tail[@]}")
     fi
```

### Comparing `nextflow-24.4.1/nextflow.egg-info/PKG-INFO` & `nextflow-24.4.2/nextflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextflow
-Version: 24.4.1
+Version: 24.4.2
 Summary: A Python wrapper that installs the Nextflow launcher
 Home-page: UNKNOWN
 Author: Jordi Deu-Pons
 License: Apache License 2.0
 Keywords: pipeline,workflow,nextflow
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `nextflow-24.4.1/setup.py` & `nextflow-24.4.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-__version__ = '24.04.1'
+__version__ = '24.04.2'
 
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 setup(
```

