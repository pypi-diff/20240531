# Comparing `tmp/recaptcha_cracker-0.0.1.tar.gz` & `tmp/recaptcha_cracker-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recaptcha_cracker-0.0.1.tar", last modified: Fri Apr 26 01:29:05 2024, max compression
+gzip compressed data, was "recaptcha_cracker-0.1.0.tar", last modified: Fri May 31 06:05:55 2024, max compression
```

## Comparing `recaptcha_cracker-0.0.1.tar` & `recaptcha_cracker-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 01:29:05.900719 recaptcha_cracker-0.0.1/
--rw-rw-rw-   0        0        0     1138 2024-04-26 01:11:08.000000 recaptcha_cracker-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     3608 2024-04-26 01:29:05.898439 recaptcha_cracker-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2556 2024-04-26 01:15:38.000000 recaptcha_cracker-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 01:29:05.884891 recaptcha_cracker-0.0.1/recaptcha_cracker/
--rw-rw-rw-   0        0        0       78 2024-04-25 23:07:07.000000 recaptcha_cracker-0.0.1/recaptcha_cracker/__init__.py
--rw-rw-rw-   0        0        0     2422 2024-04-25 23:21:55.000000 recaptcha_cracker-0.0.1/recaptcha_cracker/audio_manager.py
--rw-rw-rw-   0        0        0     3018 2024-04-25 23:20:41.000000 recaptcha_cracker-0.0.1/recaptcha_cracker/cracker.py
-drwxrwxrwx   0        0        0        0 2024-04-26 01:29:05.895778 recaptcha_cracker-0.0.1/recaptcha_cracker.egg-info/
--rw-rw-rw-   0        0        0     3608 2024-04-26 01:29:05.000000 recaptcha_cracker-0.0.1/recaptcha_cracker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2024-04-26 01:29:05.000000 recaptcha_cracker-0.0.1/recaptcha_cracker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 01:29:05.000000 recaptcha_cracker-0.0.1/recaptcha_cracker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-04-26 01:29:05.000000 recaptcha_cracker-0.0.1/recaptcha_cracker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-26 01:29:05.000000 recaptcha_cracker-0.0.1/recaptcha_cracker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 01:29:05.900719 recaptcha_cracker-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1322 2024-04-26 01:28:51.000000 recaptcha_cracker-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 01:29:05.893777 recaptcha_cracker-0.0.1/test/
--rw-rw-rw-   0        0        0      398 2024-04-25 22:36:40.000000 recaptcha_cracker-0.0.1/test/test_cracker.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:05:55.457436 recaptcha_cracker-0.1.0/
+-rw-rw-rw-   0        0        0     1138 2024-04-26 01:11:08.000000 recaptcha_cracker-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4414 2024-05-31 06:05:55.455057 recaptcha_cracker-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3303 2024-05-31 05:20:35.000000 recaptcha_cracker-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 06:05:55.432676 recaptcha_cracker-0.1.0/recaptcha_cracker/
+-rw-rw-rw-   0        0        0       37 2024-05-31 00:20:56.000000 recaptcha_cracker-0.1.0/recaptcha_cracker/__init__.py
+-rw-rw-rw-   0        0        0     3033 2024-05-31 05:31:13.000000 recaptcha_cracker-0.1.0/recaptcha_cracker/recaptcha_v2.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:05:55.445094 recaptcha_cracker-0.1.0/recaptcha_cracker/utils/
+-rw-rw-rw-   0        0        0       39 2024-05-31 00:00:23.000000 recaptcha_cracker-0.1.0/recaptcha_cracker/utils/__init__.py
+-rw-rw-rw-   0        0        0     2305 2024-05-31 05:32:37.000000 recaptcha_cracker-0.1.0/recaptcha_cracker/utils/audio_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:05:55.453359 recaptcha_cracker-0.1.0/recaptcha_cracker.egg-info/
+-rw-rw-rw-   0        0        0     4414 2024-05-31 06:05:55.000000 recaptcha_cracker-0.1.0/recaptcha_cracker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      426 2024-05-31 06:05:55.000000 recaptcha_cracker-0.1.0/recaptcha_cracker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 06:05:55.000000 recaptcha_cracker-0.1.0/recaptcha_cracker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2024-05-31 06:05:55.000000 recaptcha_cracker-0.1.0/recaptcha_cracker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-31 06:05:55.000000 recaptcha_cracker-0.1.0/recaptcha_cracker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 06:05:55.457436 recaptcha_cracker-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1355 2024-05-31 05:36:52.000000 recaptcha_cracker-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:05:55.451354 recaptcha_cracker-0.1.0/tests/
+-rw-rw-rw-   0        0        0     2586 2024-05-31 05:25:42.000000 recaptcha_cracker-0.1.0/tests/test_audio_manager.py
+-rw-rw-rw-   0        0        0      419 2024-05-31 05:25:55.000000 recaptcha_cracker-0.1.0/tests/test_recaptcha_v2.py
```

### Comparing `recaptcha_cracker-0.0.1/LICENSE` & `recaptcha_cracker-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `recaptcha_cracker-0.0.1/PKG-INFO` & `recaptcha_cracker-0.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,86 +1,71 @@
-Metadata-Version: 2.1
-Name: recaptcha-cracker
-Version: 0.0.1
-Summary: RecaptchaCracker is a tool designed to automate reCAPTCHA v2 resolution on web pages using Selenium. Allows you to resolve audio captchas, making it easy to integrate into web automation workflows.
-Home-page: https://github.com/wipodev/Recaptcha_Cracker
-Author: Wipodev
-Author-email: ajwipo@gmail.com
-License: MIT
-Project-URL: Documentation, https://github.com/wipodev/Recaptcha_Cracker/blob/main/README.md
-Project-URL: Source, https://github.com/wipodev/Recaptcha_Cracker
-Project-URL: Bug Tracker, https://github.com/wipodev/Recaptcha_Cracker/issues
-Keywords: python,captcha,speech recognition,selenium,web automation
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: seleniumbase~=4.25.4
-Requires-Dist: pydub~=0.25.1
-Requires-Dist: SpeechRecognition~=3.10.3
+# Recaptcha Cracker
 
-# Recaptcha Cracker [![Python](https://img.shields.io/pypi/v/recaptcha-cracker.svg)](https://pypi.org/project/recaptcha-cracker/)
+[![Github release](https://img.shields.io/github/v/release/wipodev/Recaptcha_Cracker?color=0172ad&logo=github&logoColor=white)](https://github.com/wipodev/Recaptcha_Cracker/releases/latest)
+[![PyPI - Version](https://img.shields.io/pypi/v/Recaptcha_Cracker?label=pypi%20release&color=0172ad)](https://pypi.org/project/Recaptcha_Cracker/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/Recaptcha_Cracker?color=0172ad&label=pypi%20downloads)](https://pypi.org/project/Recaptcha_Cracker/)
+[![GitHub Downloads (all assets, all releases)](https://img.shields.io/github/downloads/wipodev/Recaptcha_Cracker/total?color=0172ad&label=github%20downloads)](https://github.com/wipodev/Recaptcha_Cracker)
+[![License](https://img.shields.io/badge/license-MIT-%230172ad)](https://github.com/wipodev/Recaptcha_Cracker/blob/master/LICENSE)
 
 ## Description
 
-RecaptchaCracker is a tool designed to automate reCAPTCHA v2 resolution on web pages using Selenium.
-Allows you to resolve audio captchas, making it easy to integrate into web automation workflows.
+RecaptchaCracker is a tool designed to automate the resolution of Captchas on web pages using Seleniumbase.
+It allows you to solve "reCaptcha v2" captchas using audio transcription, making it easy to integrate into web automation workflows.
 
 ## Features
 
-- Automated resolution of reCAPTCHA captchas on web pages.
-- Flexible configuration of the number of attempts for solving audio captchas.
+- Automated resolution of reCAPTCHA V2 captchas on web pages.
+- Flexible configuration of the number of attempts to solve audio captchas.
 - Easy integration into web automation workflows.
 
 ## Requirements
 
 - Python 3.10+
 - Seleniumbase
 - Pydub
 - SpeechRecognition
+- verbose-terminal
 
 If you're getting an error related to FFmpeg not being installed or in your PATH, get it here: https://ffmpeg.org/download.html
 If the error persists, make sure FFmpeg is properly installed for your OS and in your PATH.
 
 ## Installation
 
 ```bash
 pip install recaptcha-cracker
 ```
 
 ## Usage
 
-1. Import the RecaptchaCracker class into your Python script:
+1. Import the necessary class to your Python script:
 
 ```python
-from recaptcha_cracker import RecaptchaCracker
+from recaptcha_cracker import RecaptchaV2
 ```
 
-2. Initialize a RecaptchaCracker object with a SeleniumBase Driver object:
+2. Initialize a RecaptchaV2 object with a SeleniumBase Driver object:
 
 ```python
 from seleniumbase import Driver
 
 # Inicializa el objeto Driver
 driver = Driver()
 
-# Carga la pÃ¡gina web
+# Carga la página web
 driver.get("https://www.google.com/recaptcha/api2/demo")
 
-# Inicializa el objeto RecaptchaCracker
-cracker = RecaptchaCracker(driver)
+# Inicializa el objeto RecaptchaV2
+recaptcha = RecaptchaV2(driver)
 
 ```
 
-3. Use the click_recaptcha() method to resolve a reCAPTCHA on a web page:
+3. Use the cracker() method to resolve a reCAPTCHA on a web page:
 
 ```python
-checked_status = cracker.click_recaptcha(selector='//*[@id="recaptcha-demo"]/div/div/iframe')
+checked_status = recaptcha.cracker(selector='//*[@id="recaptcha-demo"]/div/div/iframe')
 ```
 
 4. If the reCAPTCHA is successfully resolved, the method will return True. Otherwise, it will return False.
 
 ## Contributions
 
 If you'd like to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.
```

### Comparing `recaptcha_cracker-0.0.1/recaptcha_cracker/audio_manager.py` & `recaptcha_cracker-0.1.0/recaptcha_cracker/recaptcha_v2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,75 @@
-import requests
-from pydub import AudioSegment
-from io import BytesIO
-import speech_recognition as sr
-
-class AudioManager:
-    def __init__(self, url):
-        self.url = url
-
-    def download_audio(self):
-        response = requests.get(self.url)
-        if response.status_code == 200:
-            return BytesIO(response.content)
+from selenium.common.exceptions import TimeoutException, NoSuchElementException
+from seleniumbase import Driver
+from .utils import AudioManager
+import time
+from verbose_terminal import console
+
+class RecaptchaV2:
+  def __init__(self, driver: Driver, attempts: int = 3):
+    self.driver = driver
+    self.attempts = attempts
+
+  def cracker(self, selector: str):
+    try:
+      iframe_captcha = self.driver.wait_for_element('xpath', selector)
+      self.driver.switch_to.frame(iframe_captcha)
+      self.driver.click('#recaptcha-anchor-label')
+      if self._check_recaptcha():
+        return True
+      if not self._handle_audio_recaptcha():
+        return False
+      self.driver.switch_to.frame(iframe_captcha)
+      return self._check_recaptcha()
+    except (TimeoutException, NoSuchElementException) as e:
+      console.error(f"Error solving captcha: {e}")
+      return False
+
+  def _handle_audio_recaptcha(self):
+        try:
+            iframe_captcha_audio = self.driver.wait_for_element('xpath', '//iframe[contains(@src, "recaptcha") and contains(@src, "bframe")]')
+            self.driver.switch_to.frame(iframe_captcha_audio)
+            self.driver.click('#recaptcha-audio-button')
+            return self._solve_audio_recaptcha()
+        except (TimeoutException, NoSuchElementException) as e:
+            console.error(f"Error when handling the audio captcha: {e}")
+            return False
+        finally:
+            self.driver.switch_to.parent_frame()
+
+  def _solve_audio_recaptcha(self):
+    for _ in range(self.attempts):
+      try:
+        url = self._get_attribute('.rc-audiochallenge-tdownload-link', 'href')
+        if url is None:
+          return False
+        recognized_text = AudioManager(url).get_audio_transcript()
+        self.driver.press_keys('#audio-response', f'{recognized_text}\n')
+        if self.driver.is_element_visible('.rc-audiochallenge-error-message'):
+          console.error("Error detected, trying again...")
         else:
-            return None
-
-    def convert_to_wav(self, audio_bytes):
-        audio = AudioSegment.from_file(audio_bytes)
-        if audio:
-            wav_audio = audio.set_frame_rate(44100).set_channels(1)
-            return wav_audio
-        else:
-            return None
-
-    def save_audio(self, audio, output_file):
-        audio.export(output_file, format="wav")
-
-    def recognize_speech(self, audio_file):
-        recognizer = sr.Recognizer()
-        with sr.AudioFile(audio_file) as source:
-            audio_data = recognizer.record(source)
-            try:
-                text = recognizer.recognize_google(audio_data, language="en-US")
-                return text
-            except sr.UnknownValueError:
-                return None
-            except sr.RequestError:
-                return None
-
-    def get_audio_transcript(self, output_file="output.wav"):
-        audio_bytes = self.download_audio()
-        if audio_bytes:
-            wav_audio = self.convert_to_wav(audio_bytes)
-            if wav_audio:
-                self.save_audio(wav_audio, output_file)
-                print(f"Archivo WAV guardado: {output_file}")
-
-                recognized_text = None
-                while not recognized_text:
-                    try:
-                        recognized_text = self.recognize_speech(output_file)
-                        if recognized_text:
-                            print(f"Texto reconocido: {recognized_text}")
-                        else:
-                            print("No se pudo entender el audio. Intentando de nuevo...")
-                    except Exception as e:
-                        print(f"Error: {str(e)}. Intentando de nuevo...")
-                return recognized_text
-            else:
-                print("No se pudo convertir el archivo a WAV.")
-        else:
-            print("Error al descargar el archivo de audio.")
-
-# Ejemplo de uso
-if __name__ == "__main__":
-    url = "URL_DEL_AUDIO_AQUÍ"
-
-    print(AudioManager(url).get_audio_transcript())
+          return True
+      except Exception as e:
+        console.error(f"Error solving audio captcha: {e}")
+        return False
+    console.error(f"Could not resolve audio captcha after {self.attempts} attempts.")
+    return False
+
+  def _check_recaptcha(self):
+    try:
+      time.sleep(1)
+      return self._get_attribute('#recaptcha-anchor', 'aria-checked') == 'true'
+    except (TimeoutException, NoSuchElementException) as e:
+      console.error(f"Error checking the captcha: {e}")
+      return False
+    finally:
+      self.driver.switch_to.parent_frame()
+
+  def _get_attribute(self, selector: str, attribute: str, type: str = None) -> str:
+    try:
+      if type is None:
+        return self.driver.wait_for_element(selector).get_attribute(attribute)
+      else:
+        return self.driver.wait_for_element(type, selector).get_attribute(attribute)
+    except (TimeoutException, NoSuchElementException) as e:
+      console.error(f"Error getting attribute: {e}")
+      return None
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `recaptcha_cracker-0.0.1/recaptcha_cracker.egg-info/PKG-INFO` & `recaptcha_cracker-0.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,86 +1,94 @@
 Metadata-Version: 2.1
 Name: recaptcha-cracker
-Version: 0.0.1
-Summary: RecaptchaCracker is a tool designed to automate reCAPTCHA v2 resolution on web pages using Selenium. Allows you to resolve audio captchas, making it easy to integrate into web automation workflows.
+Version: 0.1.0
+Summary: captcha_cracker - A complete Python package for solving various types of CAPTCHAs, including text CAPTCHAs, reCAPTCHAs, and more. Enhance your automation scripts with robust CAPTCHA resolution capabilities.
 Home-page: https://github.com/wipodev/Recaptcha_Cracker
 Author: Wipodev
 Author-email: ajwipo@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/wipodev/Recaptcha_Cracker/blob/main/README.md
 Project-URL: Source, https://github.com/wipodev/Recaptcha_Cracker
 Project-URL: Bug Tracker, https://github.com/wipodev/Recaptcha_Cracker/issues
-Keywords: python,captcha,speech recognition,selenium,web automation
+Keywords: python,captcha,speech recognition,selenium,web automation,recaptcha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: seleniumbase~=4.25.4
 Requires-Dist: pydub~=0.25.1
 Requires-Dist: SpeechRecognition~=3.10.3
+Requires-Dist: verbose-terminal~=1.0.1
 
-# Recaptcha Cracker [![Python](https://img.shields.io/pypi/v/recaptcha-cracker.svg)](https://pypi.org/project/recaptcha-cracker/)
+# Recaptcha Cracker
+
+[![Github release](https://img.shields.io/github/v/release/wipodev/Recaptcha_Cracker?color=0172ad&logo=github&logoColor=white)](https://github.com/wipodev/Recaptcha_Cracker/releases/latest)
+[![PyPI - Version](https://img.shields.io/pypi/v/Recaptcha_Cracker?label=pypi%20release&color=0172ad)](https://pypi.org/project/Recaptcha_Cracker/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/Recaptcha_Cracker?color=0172ad&label=pypi%20downloads)](https://pypi.org/project/Recaptcha_Cracker/)
+[![GitHub Downloads (all assets, all releases)](https://img.shields.io/github/downloads/wipodev/Recaptcha_Cracker/total?color=0172ad&label=github%20downloads)](https://github.com/wipodev/Recaptcha_Cracker)
+[![License](https://img.shields.io/badge/license-MIT-%230172ad)](https://github.com/wipodev/Recaptcha_Cracker/blob/master/LICENSE)
 
 ## Description
 
-RecaptchaCracker is a tool designed to automate reCAPTCHA v2 resolution on web pages using Selenium.
-Allows you to resolve audio captchas, making it easy to integrate into web automation workflows.
+RecaptchaCracker is a tool designed to automate the resolution of Captchas on web pages using Seleniumbase.
+It allows you to solve "reCaptcha v2" captchas using audio transcription, making it easy to integrate into web automation workflows.
 
 ## Features
 
-- Automated resolution of reCAPTCHA captchas on web pages.
-- Flexible configuration of the number of attempts for solving audio captchas.
+- Automated resolution of reCAPTCHA V2 captchas on web pages.
+- Flexible configuration of the number of attempts to solve audio captchas.
 - Easy integration into web automation workflows.
 
 ## Requirements
 
 - Python 3.10+
 - Seleniumbase
 - Pydub
 - SpeechRecognition
+- verbose-terminal
 
 If you're getting an error related to FFmpeg not being installed or in your PATH, get it here: https://ffmpeg.org/download.html
 If the error persists, make sure FFmpeg is properly installed for your OS and in your PATH.
 
 ## Installation
 
 ```bash
 pip install recaptcha-cracker
 ```
 
 ## Usage
 
-1. Import the RecaptchaCracker class into your Python script:
+1. Import the necessary class to your Python script:
 
 ```python
-from recaptcha_cracker import RecaptchaCracker
+from recaptcha_cracker import RecaptchaV2
 ```
 
-2. Initialize a RecaptchaCracker object with a SeleniumBase Driver object:
+2. Initialize a RecaptchaV2 object with a SeleniumBase Driver object:
 
 ```python
 from seleniumbase import Driver
 
 # Inicializa el objeto Driver
 driver = Driver()
 
 # Carga la pÃ¡gina web
 driver.get("https://www.google.com/recaptcha/api2/demo")
 
-# Inicializa el objeto RecaptchaCracker
-cracker = RecaptchaCracker(driver)
+# Inicializa el objeto RecaptchaV2
+recaptcha = RecaptchaV2(driver)
 
 ```
 
-3. Use the click_recaptcha() method to resolve a reCAPTCHA on a web page:
+3. Use the cracker() method to resolve a reCAPTCHA on a web page:
 
 ```python
-checked_status = cracker.click_recaptcha(selector='//*[@id="recaptcha-demo"]/div/div/iframe')
+checked_status = recaptcha.cracker(selector='//*[@id="recaptcha-demo"]/div/div/iframe')
 ```
 
 4. If the reCAPTCHA is successfully resolved, the method will return True. Otherwise, it will return False.
 
 ## Contributions
 
 If you'd like to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.
```

### Comparing `recaptcha_cracker-0.0.1/setup.py` & `recaptcha_cracker-0.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='recaptcha-cracker',
-    version='0.0.1',
+    version='0.1.0',
     author='Wipodev',
     author_email='ajwipo@gmail.com',
-    description='RecaptchaCracker is a tool designed to automate reCAPTCHA v2 resolution on web pages using Selenium. Allows you to resolve audio captchas, making it easy to integrate into web automation workflows.',
+    description='captcha_cracker - A complete Python package for solving various types of CAPTCHAs, including text CAPTCHAs, reCAPTCHAs, and more. Enhance your automation scripts with robust CAPTCHA resolution capabilities.',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/wipodev/Recaptcha_Cracker',
     project_urls={
         'Documentation': 'https://github.com/wipodev/Recaptcha_Cracker/blob/main/README.md',
         'Source': 'https://github.com/wipodev/Recaptcha_Cracker',
         'Bug Tracker': 'https://github.com/wipodev/Recaptcha_Cracker/issues',
@@ -18,15 +18,16 @@
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.10',
     license='MIT',
-    keywords='python, captcha, speech recognition, selenium, web automation',
-    packages=find_packages(exclude=('tests*', 'testing*', 'test*')),
+    keywords='python, captcha, speech recognition, selenium, web automation, recaptcha',
+    packages=find_packages(exclude=['tests']),
     install_requires=[
         'seleniumbase~=4.25.4',
         'pydub~=0.25.1',
         'SpeechRecognition~=3.10.3',
+        'verbose-terminal~=1.0.1'
     ],
 )
```

