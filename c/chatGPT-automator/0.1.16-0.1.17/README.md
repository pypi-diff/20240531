# Comparing `tmp/chatGPT_automator-0.1.16.tar.gz` & `tmp/chatGPT_automator-0.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatGPT_automator-0.1.16.tar", last modified: Sun Oct 22 11:57:55 2023, max compression
+gzip compressed data, was "chatGPT_automator-0.1.17.tar", last modified: Fri May 31 15:22:28 2024, max compression
```

## Comparing `chatGPT_automator-0.1.16.tar` & `chatGPT_automator-0.1.17.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kevinljw   (501) staff       (20)        0 2023-10-22 11:57:55.912780 chatGPT_automator-0.1.16/
--rw-r--r--   0 kevinljw   (501) staff       (20)     1068 2023-08-20 17:42:30.000000 chatGPT_automator-0.1.16/LICENSE
--rw-r--r--   0 kevinljw   (501) staff       (20)     2450 2023-10-22 11:57:55.912255 chatGPT_automator-0.1.16/PKG-INFO
-drwxr-xr-x   0 kevinljw   (501) staff       (20)        0 2023-10-22 11:57:55.908160 chatGPT_automator-0.1.16/chatGPT_automator/
--rw-r--r--   0 kevinljw   (501) staff       (20)       80 2023-08-21 05:15:58.000000 chatGPT_automator-0.1.16/chatGPT_automator/__init__.py
--rwxrwxrwx   0 kevinljw   (501) staff       (20)    10394 2023-10-22 11:57:00.000000 chatGPT_automator-0.1.16/chatGPT_automator/master.py
-drwxr-xr-x   0 kevinljw   (501) staff       (20)        0 2023-10-22 11:57:55.911378 chatGPT_automator-0.1.16/chatGPT_automator.egg-info/
--rw-r--r--   0 kevinljw   (501) staff       (20)     2450 2023-10-22 11:57:55.000000 chatGPT_automator-0.1.16/chatGPT_automator.egg-info/PKG-INFO
--rw-r--r--   0 kevinljw   (501) staff       (20)      278 2023-10-22 11:57:55.000000 chatGPT_automator-0.1.16/chatGPT_automator.egg-info/SOURCES.txt
--rw-r--r--   0 kevinljw   (501) staff       (20)        1 2023-10-22 11:57:55.000000 chatGPT_automator-0.1.16/chatGPT_automator.egg-info/dependency_links.txt
--rw-r--r--   0 kevinljw   (501) staff       (20)       42 2023-10-22 11:57:55.000000 chatGPT_automator-0.1.16/chatGPT_automator.egg-info/requires.txt
--rw-r--r--   0 kevinljw   (501) staff       (20)       18 2023-10-22 11:57:55.000000 chatGPT_automator-0.1.16/chatGPT_automator.egg-info/top_level.txt
--rw-r--r--   0 kevinljw   (501) staff       (20)       38 2023-10-22 11:57:55.912984 chatGPT_automator-0.1.16/setup.cfg
--rw-r--r--   0 kevinljw   (501) staff       (20)      825 2023-10-22 11:56:31.000000 chatGPT_automator-0.1.16/setup.py
+drwxr-xr-x   0 kevinljw   (501) staff       (20)        0 2024-05-31 15:22:28.901351 chatGPT_automator-0.1.17/
+-rw-r--r--   0 kevinljw   (501) staff       (20)     1068 2023-08-20 17:42:30.000000 chatGPT_automator-0.1.17/LICENSE
+-rw-r--r--   0 kevinljw   (501) staff       (20)     2450 2024-05-31 15:22:28.901018 chatGPT_automator-0.1.17/PKG-INFO
+drwxr-xr-x   0 kevinljw   (501) staff       (20)        0 2024-05-31 15:22:28.898314 chatGPT_automator-0.1.17/chatGPT_automator/
+-rw-r--r--   0 kevinljw   (501) staff       (20)       80 2023-08-21 05:15:58.000000 chatGPT_automator-0.1.17/chatGPT_automator/__init__.py
+-rwxrwxrwx   0 kevinljw   (501) staff       (20)    10963 2024-05-31 15:19:58.000000 chatGPT_automator-0.1.17/chatGPT_automator/master.py
+drwxr-xr-x   0 kevinljw   (501) staff       (20)        0 2024-05-31 15:22:28.900480 chatGPT_automator-0.1.17/chatGPT_automator.egg-info/
+-rw-r--r--   0 kevinljw   (501) staff       (20)     2450 2024-05-31 15:22:28.000000 chatGPT_automator-0.1.17/chatGPT_automator.egg-info/PKG-INFO
+-rw-r--r--   0 kevinljw   (501) staff       (20)      278 2024-05-31 15:22:28.000000 chatGPT_automator-0.1.17/chatGPT_automator.egg-info/SOURCES.txt
+-rw-r--r--   0 kevinljw   (501) staff       (20)        1 2024-05-31 15:22:28.000000 chatGPT_automator-0.1.17/chatGPT_automator.egg-info/dependency_links.txt
+-rw-r--r--   0 kevinljw   (501) staff       (20)       42 2024-05-31 15:22:28.000000 chatGPT_automator-0.1.17/chatGPT_automator.egg-info/requires.txt
+-rw-r--r--   0 kevinljw   (501) staff       (20)       18 2024-05-31 15:22:28.000000 chatGPT_automator-0.1.17/chatGPT_automator.egg-info/top_level.txt
+-rw-r--r--   0 kevinljw   (501) staff       (20)       38 2024-05-31 15:22:28.901476 chatGPT_automator-0.1.17/setup.cfg
+-rw-r--r--   0 kevinljw   (501) staff       (20)      825 2024-05-31 15:22:08.000000 chatGPT_automator-0.1.17/setup.py
```

### Comparing `chatGPT_automator-0.1.16/LICENSE` & `chatGPT_automator-0.1.17/LICENSE`

 * *Files identical despite different names*

### Comparing `chatGPT_automator-0.1.16/PKG-INFO` & `chatGPT_automator-0.1.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatGPT_automator
-Version: 0.1.16
+Version: 0.1.17
 Summary: Regarding automating ChatGPT using Selenium in Python
 Home-page: https://github.com/kevinljw/chatgpt_automator
 Author: evinljw
 Author-email: evin92@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chatGPT_automator-0.1.16/chatGPT_automator/master.py` & `chatGPT_automator-0.1.17/chatGPT_automator/master.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,15 +100,17 @@
             if (Path.cwd() / self.chrome_driver_path).exists():
                 driver = webdriver.Chrome(service=ChromeService(str(Path.cwd() / self.chrome_driver_path)), options=chrome_options)
         return driver
 
     def talk_to_chatgpt(self, prompt, to_list=False, to_csv=False, new_chat=False):
         if new_chat:
             try:
-                self.driver.find_element(by=By.CSS_SELECTOR, value="nav>div:nth-child(1)>a").click()
+                self.driver.find_element(by=By.CSS_SELECTOR, value="nav>div:nth-child(1)>span:last-child>button").click()
+                time.sleep(0.5)
+                WebDriverWait(self.driver, 15).until(EC.visibility_of_element_located((By.XPATH, "(//form//button[@disabled])[last()]")))
                 WebDriverWait(self.driver, 15).until(EC.visibility_of_element_located((By.CSS_SELECTOR, "form textarea")))
             except:
                 pass
         self.send_prompt_to_chatgpt(prompt)
         if to_list or to_csv:
             return self.return_last_table(to_csv)
         else:
@@ -118,27 +120,29 @@
         input_box = self.driver.find_element(by=By.CSS_SELECTOR, value="form textarea")
         # prompt = prompt.replace("\n","\\n").replace("\'","\\\'")
         prompt_escaped = json.dumps(prompt).strip("\"").replace("'", "\\'").replace('"', '\\"')
         self.driver.execute_script(f"arguments[0].value = '{prompt_escaped}';", input_box)
         time.sleep(0.3)
         input_box.send_keys(Keys.ENTER)
         try:
-            input_btn = self.driver.find_element(by=By.CSS_SELECTOR, value="form textarea+button")
+            # input_btn = self.driver.find_element(by=By.CSS_SELECTOR, value="form div+button")
+            input_btn = input_box.find_element(By.XPATH, '../following-sibling::button')
             time.sleep(0.1)
             input_btn.click()
         except:
             pass
         # time.sleep(self.wait_sec)
         try:
-            WebDriverWait(self.driver, self.wait_sec).until(EC.visibility_of_element_located((By.CSS_SELECTOR, "form button>[data-state=\"closed\"]")))
+            # WebDriverWait(self.driver, self.wait_sec).until(EC.visibility_of_element_located((By.CSS_SELECTOR, "form button>[data-state=\"closed\"]")))
+            WebDriverWait(self.driver, self.wait_sec).until(EC.visibility_of_element_located((By.XPATH, "(//form//button[@disabled])[last()]")))
         except:
             time.sleep(self.wait_sec)
             return
     def return_chatgpt_conversation(self):
-        return self.driver.find_elements(by=By.CSS_SELECTOR, value='div.text-base')
+        return self.driver.find_elements(by=By.CSS_SELECTOR, value='main div[data-message-author-role="assistant"]')
 
     def save_conversation(self, file_name):
         directory_name = "conversations"
         if not os.path.exists(directory_name):
             os.makedirs(directory_name)
 
         delimiter = "|＠|"
@@ -147,16 +151,16 @@
             for i in range(0, len(chatgpt_conversation), 2):
                 file.write(
                     f"prompt: {chatgpt_conversation[i].text}\nresponse: {chatgpt_conversation[i + 1].text}\n\n{delimiter}\n\n")
 
     def return_last_response(self):
         """ :return: the text of the last chatgpt response """
         try:
-            WebDriverWait(self.driver, 20).until(EC.visibility_of_element_located((By.CSS_SELECTOR, "div.text-base")))
-            response_elements = self.driver.find_elements(by=By.CSS_SELECTOR, value='div.text-base')
+            WebDriverWait(self.driver, 20).until(EC.visibility_of_element_located((By.CSS_SELECTOR, 'main div[data-message-author-role="assistant"]')))
+            response_elements = self.driver.find_elements(by=By.CSS_SELECTOR, value='main div[data-message-author-role="assistant"]')
             if response_elements:
                 return response_elements[-1].text
             else:
                 return ""
         except:
             return ""
     def return_last_table(self, to_csv):
@@ -169,25 +173,25 @@
             table_data = []
             for row in rows:
                 columns = row.find_elements(by=By.CSS_SELECTOR, value='th,td')
                 row_data = [col.text for col in columns]
                 table_data.append(row_data)
             return table_data
         try:
-            WebDriverWait(self.driver, 20).until(EC.visibility_of_element_located((By.CSS_SELECTOR, "div.text-base")))
-            response_elements = self.driver.find_elements(by=By.CSS_SELECTOR, value='div.text-base')
-            table_element = response_elements[-1].find_element(by=By.CSS_SELECTOR, value='div.text-base table')
+            WebDriverWait(self.driver, 20).until(EC.visibility_of_element_located((By.CSS_SELECTOR, 'main div[data-message-author-role="assistant"]')))
+            response_elements = self.driver.find_elements(by=By.CSS_SELECTOR, value='main div[data-message-author-role="assistant"]')
+            table_element = response_elements[-1].find_element(by=By.CSS_SELECTOR, value='div>table')
             if table_element:
                 table_data = table_to_list(table_element)
                 return StringIO("\n".join([",".join([quote_field(cell) for cell in row]) for row in table_data])) if to_csv else table_data
             else:
                 return self.return_last_response()
         except:
             try:
-                code_content = response_elements[-1].find_element(by=By.CSS_SELECTOR, value='div.text-base code').text
+                code_content = response_elements[-1].find_element(by=By.CSS_SELECTOR, value='div>code').text
                 rows = code_content.split("\n")
                 table = []
                 for row in rows:
                     # Split by '|' to get the cells
                     cells = [cell.strip() for cell in row.split("|") if cell.strip()]
                 # Skip rows that don't have data
                 if len(cells) > 1:
```

### Comparing `chatGPT_automator-0.1.16/chatGPT_automator.egg-info/PKG-INFO` & `chatGPT_automator-0.1.17/chatGPT_automator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatGPT-automator
-Version: 0.1.16
+Version: 0.1.17
 Summary: Regarding automating ChatGPT using Selenium in Python
 Home-page: https://github.com/kevinljw/chatgpt_automator
 Author: evinljw
 Author-email: evin92@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chatGPT_automator-0.1.16/setup.py` & `chatGPT_automator-0.1.17/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("Discription.md", "r",encoding="utf-8") as f:
     long_description = f.read()
     
 setuptools.setup(
     name = "chatGPT_automator",
-    version = "0.1.16",
+    version = "0.1.17",
     author = "evinljw",
     author_email="evin92@gmail.com",
     description="Regarding automating ChatGPT using Selenium in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
     url="https://github.com/kevinljw/chatgpt_automator",
```

