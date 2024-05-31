# Comparing `tmp/cli_for_tools-0.1.1.tar.gz` & `tmp/cli_for_tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli_for_tools-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cli_for_tools-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cli_for_tools-0.1.1.tar` & `cli_for_tools-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2041 2023-08-30 21:32:03.777174 cli_for_tools-0.1.1/README.md
--rw-r--r--   0        0        0       86 2023-08-30 21:32:03.777174 cli_for_tools-0.1.1/cli_for_tools/__init__.py
--rw-r--r--   0        0        0     2585 2023-08-30 21:32:03.777174 cli_for_tools-0.1.1/cli_for_tools/paco_cli.py
--rw-r--r--   0        0        0      515 2023-08-30 21:32:03.777174 cli_for_tools-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2444 1970-01-01 00:00:00.000000 cli_for_tools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2773 2024-05-31 20:26:06.239655 cli_for_tools-0.2.0/README.md
+-rw-r--r--   0        0        0       86 2024-05-31 20:26:06.239655 cli_for_tools-0.2.0/cli_for_tools/__init__.py
+-rw-r--r--   0        0        0     2748 2024-05-31 20:26:06.239655 cli_for_tools-0.2.0/cli_for_tools/paco_cli.py
+-rw-r--r--   0        0        0      515 2024-05-31 20:26:06.239655 cli_for_tools-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3176 1970-01-01 00:00:00.000000 cli_for_tools-0.2.0/PKG-INFO
```

### Comparing `cli_for_tools-0.1.1/cli_for_tools/paco_cli.py` & `cli_for_tools-0.2.0/cli_for_tools/paco_cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,26 +5,32 @@
 app = typer.Typer(
     help="Paco el chato es el asistente para las tareas de gabinete en el proyecto de erradicación de gato feral en Isla Guadalupe"
 )
 
 
 def clean_data_when_use_yolo():
     os.system("sudo chown --recursive $USER:$USER .")
-    os.system("rm --force --recursive raw")
-    os.system("rm --force --recursive resized")
+    os.system("rm --force cat_detected/*.txt")
+    os.system("rm --force --recursive camera_trap_photos/")
+
+
+def setup_classifier():
+    os.system("mkdir camera_trap_photos")
+    os.system("cp *.* camera_trap_photos/")
+    os.system("rm --recursive cat_detected/")
 
 
 def clean_data_when_after_made_little_map():
     os.system("sudo chown --recursive $USER .")
     os.system("sudo chmod g+w --recursive .")
     os.system("echo ¿Qué borraremos?")
 
 
 def analyze_photo():
-    command = "docker run -itv $PWD:/workdir/data/raw/photos -v $PWD:/workdir/data islasgeci/cat_recognition:latest make detection_with_yolo"
+    command = "docker run --volume $PWD:/workdir islasgeci/cetys_cat_recognition:latest make classification"
     os.system(command)
 
 
 def make_data_map_of_traps_jpg():
     command = "docker run -v $PWD:/workdir/data islasgeci/ig_position_traps_map make data/map_of_traps.jpg"
     os.system(command)
 
@@ -71,14 +77,15 @@
     Clasifica las fotos que vienen de las trampas cámara. \n
     Requerimiento: En la carpeta de trabajo debe estar una carpeta (varias carpetas) con las fotos. \n
     El nombre de la carpeta principal debe ser sin espacios. Por ejemplo: \n
     - `FOTOS GATOS`: es un nombre incorrecto, \n
     - `FOTOS_GATOS`: es un nombre correcto. \n
     Al final generará la carpeta `cat_detected` con las fotos en las que detectó gato.
     """
+    setup_classifier()
     analyze_photo()
     clean_data_when_use_yolo()
 
 
 @app.command()
 def version():
     print(ct.__version__)
```

### Comparing `cli_for_tools-0.1.1/pyproject.toml` & `cli_for_tools-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cli_for_tools-0.1.1/PKG-INFO` & `cli_for_tools-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,72 @@
-Metadata-Version: 2.1
-Name: cli_for_tools
-Version: 0.1.1
-Summary: Cli for traps team tools
-Home-page: https://github.com/IslasGECI/cli_guadalupe_data
-Author: Ciencia de Datos • GECI
-Author-email: ciencia.datos@islas.org.mx
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Dist: typer[all]
-
 <a href="https://www.islas.org.mx/"><img src="https://www.islas.org.mx/img/logo.svg" align="right" width="256" /></a>
 # Cli Guadalupe Data
 
+
+![demo](https://github.com/IslasGECI/kanban/assets/53709062/faed1c14-9a41-4125-8140-fa58c3910cd2)
+
 ## `paco_el_chato`
 Paco el chato es el asistente para las tareas de gabinete en el proyecto de erradicación de gato
 feral en Isla Guadalupe.
 
 Tiene tres habilidades:
 - clasificar fotos con gatos
 - generar un esbozo del mapa con trampas activas y desactivas de Isla Guadalupe
 - actualizar la paquetería para hacer las tareas anteriores
 
 ## Instalación 🏗️
 Podemos instalar esta aplicación usando `pip`:
 ```shell
-pip uninstall cli_for_tools
-pip install git+https://github.com/IslasGECI/cli_guadalupe_data@latest
+pip uninstall cli-for-tools
+pip install cli-for-tools
 ```
 
 ## Modo de uso
 Para utilizar `haz-mapa` o `clasifica-fotos` debemos abrir la terminal desde la carpeta de trabajo:
 1. damos doble _click_ a la carpeta de trabajo
 1. damos _click_ derecho al ratón y escogemos la opción **Open Terminal**
 1. escribimos el comando `paco_el_chato --help` y tendremos la ayuda general
 1. escribimos el comando `paco_el_chato haz-mapa --help` y tendremos la ayuda del comando `haz-mapa`
 1. escribimos el comando `paco_el_chato clasifica-fotos --help` y tendremos la ayuda del comando `clasifica-fotos`
 
 ## `haz-mapa`
 Hace un esbozo del mapa de Isla Guadalupe con las trampas activas e inactivas.
 
-**Requerimiento**: En la carpeta de trabajo debe estar:
-- IG_POSICION_{fecha}.txt         : Archivo que obtenemos de mapsource
+``` sh
+paco_el_chato haz-mapa
+```
+
+### Requerimientos
+En la carpeta de trabajo deben existir los archivos:
+- IG_MAPSOURCE_TRAMPAS_{fecha}.txt: Archivo que obtenemos de MapSource
 - IG_POSICION_TRAMPAS_{fecha}.xlsx: Archivos con los esfuerzos de la semana
 
 Al final generará el archivo `map_of_traps.jpg`.
 
+### Posibles fuentes de error
+Si las fechas no coinciden es posible que el mapa que generamos sea incorrecto.
+Si la fecha del archivo de MapSource está una semana atrás al de posición todas las trampas aparecerán desactivas.
+Por ejemplo, con los archivos `IG_POSICION_TRAMPAS_19NOV2023` e `IG_MAPSOURCE_TRAMPAS_12NOV2023.txt` obtendremos un mapa con todas las trampas desactivadas. 
+Esto se debe a que a partir del archivo de MapSource generamos un nuevo archivo csv con fecha de una semana después.
+Este archivo reescribe el original poniendo todas las trampas desactivas.
+
+
 ## `clasifica-fotos`
 Clasifica las fotos que vienen de las trampas cámara.
 
-**Requerimiento**: En la carpeta de trabajo debe estar una carpeta (varias carpetas) con las fotos.
+``` sh
+paco_el_chato clasifica-fotos
+```
+
+### Requerimientos
+En la carpeta de trabajo debe estar una carpeta (o varias carpetas) con las fotos.
 El nombre de la carpeta principal debe ser sin espacios. Por ejemplo:
 - `FOTOS GATOS`: es un nombre incorrecto,
 - `FOTOS_GATOS`: es un nombre correcto.
 
+
 Al final generará la carpeta `cat_detected` con las fotos en las que detectó gato.
 
 ## `actualiza-comandos`
 Actualiza los comandos:
 - `haz-mapa`
 - `clasifica-fotos`
-
```

#### html2text {}

```diff
@@ -1,31 +1,36 @@
-Metadata-Version: 2.1 Name: cli_for_tools Version: 0.1.1 Summary: Cli for traps
-team tools Home-page: https://github.com/IslasGECI/cli_guadalupe_data Author:
-Ciencia de Datos â¢ GECI Author-email: ciencia.datos@islas.org.mx Requires-
-Python: >=3.9 Description-Content-Type: text/markdown Classifier: License ::
-OSI Approved :: GNU General Public License v3 or later (GPLv3+) Requires-Dist:
-typer[all] _[_h_t_t_p_s_:_/_/_w_w_w_._i_s_l_a_s_._o_r_g_._m_x_/_i_m_g_/_l_o_g_o_._s_v_g_]# Cli Guadalupe Data ##
-`paco_el_chato` Paco el chato es el asistente para las tareas de gabinete en el
-proyecto de erradicaciÃ³n de gato feral en Isla Guadalupe. Tiene tres
-habilidades: - clasificar fotos con gatos - generar un esbozo del mapa con
-trampas activas y desactivas de Isla Guadalupe - actualizar la paqueterÃ­a para
-hacer las tareas anteriores ## InstalaciÃ³n ðï¸ Podemos instalar esta
-aplicaciÃ³n usando `pip`: ```shell pip uninstall cli_for_tools pip install
-git+https://github.com/IslasGECI/cli_guadalupe_data@latest ``` ## Modo de uso
-Para utilizar `haz-mapa` o `clasifica-fotos` debemos abrir la terminal desde la
-carpeta de trabajo: 1. damos doble _click_ a la carpeta de trabajo 1. damos
-_click_ derecho al ratÃ³n y escogemos la opciÃ³n **Open Terminal** 1.
-escribimos el comando `paco_el_chato --help` y tendremos la ayuda general 1.
-escribimos el comando `paco_el_chato haz-mapa --help` y tendremos la ayuda del
-comando `haz-mapa` 1. escribimos el comando `paco_el_chato clasifica-fotos --
-help` y tendremos la ayuda del comando `clasifica-fotos` ## `haz-mapa` Hace un
-esbozo del mapa de Isla Guadalupe con las trampas activas e inactivas.
-**Requerimiento**: En la carpeta de trabajo debe estar: - IG_POSICION_
-{fecha}.txt : Archivo que obtenemos de mapsource - IG_POSICION_TRAMPAS_
-{fecha}.xlsx: Archivos con los esfuerzos de la semana Al final generarÃ¡ el
-archivo `map_of_traps.jpg`. ## `clasifica-fotos` Clasifica las fotos que vienen
-de las trampas cÃ¡mara. **Requerimiento**: En la carpeta de trabajo debe estar
-una carpeta (varias carpetas) con las fotos. El nombre de la carpeta principal
-debe ser sin espacios. Por ejemplo: - `FOTOS GATOS`: es un nombre incorrecto, -
-`FOTOS_GATOS`: es un nombre correcto. Al final generarÃ¡ la carpeta
-`cat_detected` con las fotos en las que detectÃ³ gato. ## `actualiza-comandos`
-Actualiza los comandos: - `haz-mapa` - `clasifica-fotos`
+_[_h_t_t_p_s_:_/_/_w_w_w_._i_s_l_a_s_._o_r_g_._m_x_/_i_m_g_/_l_o_g_o_._s_v_g_]# Cli Guadalupe Data ![demo](https://
+github.com/IslasGECI/kanban/assets/53709062/faed1c14-9a41-4125-8140-
+fa58c3910cd2) ## `paco_el_chato` Paco el chato es el asistente para las tareas
+de gabinete en el proyecto de erradicaciÃ³n de gato feral en Isla Guadalupe.
+Tiene tres habilidades: - clasificar fotos con gatos - generar un esbozo del
+mapa con trampas activas y desactivas de Isla Guadalupe - actualizar la
+paqueterÃ­a para hacer las tareas anteriores ## InstalaciÃ³n ðï¸ Podemos
+instalar esta aplicaciÃ³n usando `pip`: ```shell pip uninstall cli-for-tools
+pip install cli-for-tools ``` ## Modo de uso Para utilizar `haz-mapa` o
+`clasifica-fotos` debemos abrir la terminal desde la carpeta de trabajo: 1.
+damos doble _click_ a la carpeta de trabajo 1. damos _click_ derecho al ratÃ³n
+y escogemos la opciÃ³n **Open Terminal** 1. escribimos el comando
+`paco_el_chato --help` y tendremos la ayuda general 1. escribimos el comando
+`paco_el_chato haz-mapa --help` y tendremos la ayuda del comando `haz-mapa` 1.
+escribimos el comando `paco_el_chato clasifica-fotos --help` y tendremos la
+ayuda del comando `clasifica-fotos` ## `haz-mapa` Hace un esbozo del mapa de
+Isla Guadalupe con las trampas activas e inactivas. ``` sh paco_el_chato haz-
+mapa ``` ### Requerimientos En la carpeta de trabajo deben existir los
+archivos: - IG_MAPSOURCE_TRAMPAS_{fecha}.txt: Archivo que obtenemos de
+MapSource - IG_POSICION_TRAMPAS_{fecha}.xlsx: Archivos con los esfuerzos de la
+semana Al final generarÃ¡ el archivo `map_of_traps.jpg`. ### Posibles fuentes
+de error Si las fechas no coinciden es posible que el mapa que generamos sea
+incorrecto. Si la fecha del archivo de MapSource estÃ¡ una semana atrÃ¡s al de
+posiciÃ³n todas las trampas aparecerÃ¡n desactivas. Por ejemplo, con los
+archivos `IG_POSICION_TRAMPAS_19NOV2023` e `IG_MAPSOURCE_TRAMPAS_12NOV2023.txt`
+obtendremos un mapa con todas las trampas desactivadas. Esto se debe a que a
+partir del archivo de MapSource generamos un nuevo archivo csv con fecha de una
+semana despuÃ©s. Este archivo reescribe el original poniendo todas las trampas
+desactivas. ## `clasifica-fotos` Clasifica las fotos que vienen de las trampas
+cÃ¡mara. ``` sh paco_el_chato clasifica-fotos ``` ### Requerimientos En la
+carpeta de trabajo debe estar una carpeta (o varias carpetas) con las fotos. El
+nombre de la carpeta principal debe ser sin espacios. Por ejemplo: - `FOTOS
+GATOS`: es un nombre incorrecto, - `FOTOS_GATOS`: es un nombre correcto. Al
+final generarÃ¡ la carpeta `cat_detected` con las fotos en las que detectÃ³
+gato. ## `actualiza-comandos` Actualiza los comandos: - `haz-mapa` -
+`clasifica-fotos`
```

