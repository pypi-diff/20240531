# Comparing `tmp/ALLMDEV-1.3.7-py3-none-any.whl.zip` & `tmp/ALLMDEV-1.3.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,26 @@
-Zip file size: 29609 bytes, number of entries: 23
+Zip file size: 38430 bytes, number of entries: 24
 -rw-rw-rw-  2.0 fat       39 b- defN 24-Apr-17 06:01 ALLMDEV/__init__.py
 -rw-rw-rw-  2.0 fat     3706 b- defN 24-May-04 14:17 ALLMDEV/agentapi.py
 -rw-rw-rw-  2.0 fat     3440 b- defN 24-Apr-27 08:48 ALLMDEV/agentchat.py
+-rw-rw-rw-  2.0 fat    34081 b- defN 24-May-31 09:55 ALLMDEV/api.py
 -rw-rw-rw-  2.0 fat     4986 b- defN 24-May-11 17:03 ALLMDEV/azureagentapi.py
 -rw-rw-rw-  2.0 fat     3298 b- defN 24-May-11 16:47 ALLMDEV/azureagentchat.py
 -rw-rw-rw-  2.0 fat     2435 b- defN 24-May-11 16:47 ALLMDEV/azurecli.py
--rw-rw-rw-  2.0 fat    25481 b- defN 24-May-26 10:07 ALLMDEV/backend.py
+-rw-rw-rw-  2.0 fat    32582 b- defN 24-May-31 09:56 ALLMDEV/backend.py
 -rw-rw-rw-  2.0 fat     4952 b- defN 24-May-25 12:45 ALLMDEV/chat_history.py
 -rw-rw-rw-  2.0 fat     3221 b- defN 24-May-15 11:30 ALLMDEV/cli.py
 -rw-rw-rw-  2.0 fat    12685 b- defN 24-May-15 08:32 ALLMDEV/instruct.py
 -rw-rw-rw-  2.0 fat     3096 b- defN 24-Apr-27 08:57 ALLMDEV/newagent.py
 -rw-rw-rw-  2.0 fat     2231 b- defN 24-May-22 04:35 ALLMDEV/serve.py
 -rw-rw-rw-  2.0 fat     1932 b- defN 24-May-15 12:35 ALLMDEV/studio.py
 -rw-rw-rw-  2.0 fat      683 b- defN 24-May-04 14:32 ALLMDEV/test.py
 -rw-rw-rw-  2.0 fat     3096 b- defN 24-May-05 07:54 ALLMDEV/updateagent.py
 -rw-rw-rw-  2.0 fat     4530 b- defN 24-May-11 16:47 ALLMDEV/vertexagentapi.py
 -rw-rw-rw-  2.0 fat     2826 b- defN 24-May-14 10:42 ALLMDEV/vertexagentchat.py
 -rw-rw-rw-  2.0 fat     2126 b- defN 24-May-14 10:42 ALLMDEV/vertexcli.py
--rw-rw-rw-  2.0 fat     6093 b- defN 24-May-26 10:55 ALLMDEV-1.3.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-26 10:55 ALLMDEV-1.3.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      591 b- defN 24-May-26 10:55 ALLMDEV-1.3.7.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        8 b- defN 24-May-26 10:55 ALLMDEV-1.3.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1778 b- defN 24-May-26 10:55 ALLMDEV-1.3.7.dist-info/RECORD
-23 files, 93325 bytes uncompressed, 26783 bytes compressed:  71.3%
+-rw-rw-rw-  2.0 fat     6145 b- defN 24-May-31 10:00 ALLMDEV-1.3.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-31 10:00 ALLMDEV-1.3.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      589 b- defN 24-May-31 10:00 ALLMDEV-1.3.8.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 24-May-31 10:00 ALLMDEV-1.3.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1850 b- defN 24-May-31 10:00 ALLMDEV-1.3.8.dist-info/RECORD
+24 files, 134629 bytes uncompressed, 35500 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -3,14 +3,17 @@
 
 Filename: ALLMDEV/agentapi.py
 Comment: 
 
 Filename: ALLMDEV/agentchat.py
 Comment: 
 
+Filename: ALLMDEV/api.py
+Comment: 
+
 Filename: ALLMDEV/azureagentapi.py
 Comment: 
 
 Filename: ALLMDEV/azureagentchat.py
 Comment: 
 
 Filename: ALLMDEV/azurecli.py
@@ -48,23 +51,23 @@
 
 Filename: ALLMDEV/vertexagentchat.py
 Comment: 
 
 Filename: ALLMDEV/vertexcli.py
 Comment: 
 
-Filename: ALLMDEV-1.3.7.dist-info/METADATA
+Filename: ALLMDEV-1.3.8.dist-info/METADATA
 Comment: 
 
-Filename: ALLMDEV-1.3.7.dist-info/WHEEL
+Filename: ALLMDEV-1.3.8.dist-info/WHEEL
 Comment: 
 
-Filename: ALLMDEV-1.3.7.dist-info/entry_points.txt
+Filename: ALLMDEV-1.3.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: ALLMDEV-1.3.7.dist-info/top_level.txt
+Filename: ALLMDEV-1.3.8.dist-info/top_level.txt
 Comment: 
 
-Filename: ALLMDEV-1.3.7.dist-info/RECORD
+Filename: ALLMDEV-1.3.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ALLMDEV/backend.py

```diff
@@ -1,8 +1,8 @@
-from fastapi import FastAPI, WebSocket, Request, File, UploadFile, Form, Request, HTTPException
+from fastapi import FastAPI, WebSocket, Request, File, UploadFile, Form, Request, HTTPException, Header
 from flask import request, jsonify
 from pydantic import BaseModel
 from llama_index.llms.llama_cpp import LlamaCPP
 from langchain.embeddings import SentenceTransformerEmbeddings
 from langchain.vectorstores import Chroma
 import asyncio
 import os
@@ -16,16 +16,19 @@
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from fastapi import FastAPI
 from fastapi.middleware.cors import CORSMiddleware
 import sqlite3
 import hashlib
 import re
 from datetime import datetime, timedelta
+from dotenv import load_dotenv
+import jwt
 
-
+load_dotenv()
+SECRET = os.getenv("SECRET")
 
 app = FastAPI()
 
 
 
 app.add_middleware(
     CORSMiddleware,
@@ -107,18 +110,28 @@
     cursor = conn.cursor()
 
     cursor.execute('''
     CREATE TABLE IF NOT EXISTS users (
         id INTEGER PRIMARY KEY AUTOINCREMENT,
         email TEXT UNIQUE NOT NULL,
         password TEXT NOT NULL,
-        fullname TEXT NOT NULL           
+        fullname TEXT NOT NULL,
+        role TEXT, 
+        profilepic TEXT,
+        designation TEXT,
+        notifications TEXT,
+        JWT TEXT
     )
     ''')
 
+    cursor.execute('''
+    CREATE TABLE IF NOT EXISTS monitoring (
+        logs TEXT
+    )''')
+
     conn.commit()
     conn.close()
 
 config = load_config()
 
 def sanitize_email(email):
     # Replace invalid characters with underscores
@@ -487,84 +500,128 @@
             await websocket.send_json(config)
 
     except Exception as e:
         print(e)
     finally:
         await websocket.close()
 
-@app.route('/signup', methods=['POST'])
+
+@app.post("/signup")
 async def signup(request: Request):
     data = await request.json()
-    print(data)
     fullname = data.get('fullname')
-    email = data['email']
+    email = data.get('email')
     password = data.get('password')
+    role = data.get('role')
+    profilepic = data.get('profilepic')
+    designation = data.get('designation')
+    notifications = data.get('notifications')
 
-    hashed_password = hashlib.sha256(password.encode()).hexdigest()
+    if not email or not password or not fullname:
+        raise HTTPException(status_code=400, detail="Required fields are missing")
 
     conn = sqlite3.connect('user_database.db')
     cursor = conn.cursor()
 
+    # Check if '@' is in the email to distinguish signup from user creation
     if '@' in email:
         try:
             cursor.execute('''
-            INSERT INTO users (email, password, fullname) VALUES (?, ?, ?)
-            ''', (email, hashed_password, fullname))
+                INSERT INTO users (email, password, fullname, role, profilepic, designation, notifications)
+                VALUES (?, ?, ?, ?, ?, ?, ?)
+            ''', (email, hashlib.sha256(password.encode()).hexdigest(), fullname, role, profilepic, designation, notifications))
+
+            token = jwt.encode({'email': email}, SECRET, algorithm='HS256')
+
+            # Store JWT token in the database
+            cursor.execute('''
+                UPDATE users SET jwt = ? WHERE email = ?
+            ''', (token, email))
 
             sanitized_table_name = sanitize_email(email)
             cursor.execute(f'''
-            CREATE TABLE IF NOT EXISTS {sanitized_table_name} (
-                chat_id INTEGER PRIMARY KEY AUTOINCREMENT,
-                timestamp TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
-                messageheader TEXT,
-                chats TEXT                   
-            )
-        ''')
+                CREATE TABLE IF NOT EXISTS {sanitized_table_name} (
+                    chat_id INTEGER PRIMARY KEY AUTOINCREMENT,
+                    timestamp TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
+                    messageheader TEXT,
+                    chats TEXT                   
+                )
+            ''')
             conn.commit()
+        
             response = {'message': 'User signed up successfully!'}
         except sqlite3.IntegrityError:
             response = {'message': 'Username already exists!'}
+        except Exception as e:
+            response = {'message': 'Error occurred while signing up'}
+            print(e)
     else:
-        response = {'message': 'Invalid email format.'}
-    
-    
+        response = {'message': 'Email format is not correct'}
+        raise HTTPException(status_code=400, detail=response)
 
     conn.close()
-    return JSONResponse(content=response)
+    return response
 
 # Route for user login
 @app.route('/login', methods=['POST'])
 async def login(request: Request):
     data = await request.json()
     email = data['email']
     password = data['password']
 
     hashed_password = hashlib.sha256(password.encode()).hexdigest()
 
     conn = sqlite3.connect('user_database.db')
     cursor = conn.cursor()
 
     cursor.execute('''
-    SELECT id, fullname FROM users WHERE email = ? AND password = ?
+    SELECT id, fullname, role FROM users WHERE email = ? AND password = ?
     ''', (email, hashed_password))
 
     user = cursor.fetchone()
 
     if user:
         print(user)
         user_id = user[0]
         fullname = user[1]
+        role = user[2]
+        token = jwt.encode({'email': email, 'role': user[2]}, SECRET, algorithm='HS256')
         print(fullname, user_id)
-        response = {'message': f"Welcome, {fullname}!","status": True, "user_id": user_id}
+        response = {'message': f"Welcome, {fullname}!","status": True, "token": token, "role": role }
     else:
         response = {'message': 'Invalid username or password.'}
 
     conn.close()
     return JSONResponse(content=response)
 
+def is_user(token):
+    try:
+        payload = jwt.decode(token, SECRET, algorithms=["HS256"])
+        user_role = payload.get("role")
+        if user_role and user_role.lower() == 'admin':
+            return True
+        else:
+            return False
+    except jwt.ExpiredSignatureError:
+        raise HTTPException(status_code=401, detail="Token has expired")
+    except jwt.InvalidTokenError:
+        raise HTTPException(status_code=401, detail="Invalid token")
+
+@app.get("/check_user")
+def check_user(authorization: str = Header(None)):
+    if authorization is None:
+        raise HTTPException(status_code=401, detail="Authorization header missing")
+    
+    token = authorization.split(" ")[1]  # Assuming the header is "Bearer <token>"
+    
+    if is_user(token):
+        return {"status": "true"}
+    else:
+        raise HTTPException(status_code=403, detail="You are not authorized to access this page")
+
 @app.post('/newchat')
 async def update_chat_history(request: Request):
     data = await request.json()
     print(data)
     user_email = data['userEmail']
     message_header = data['messageheader']
     chats = data['chats']
@@ -629,14 +686,15 @@
         if chat_history:
             # Parse the chat history from JSON
             chat_history_json = json.loads(chat_history[0])
             return JSONResponse(content={'chat': chat_history_json})
         else:
             raise HTTPException(status_code=404, detail='Chat history not found.')
     except Exception as e:
+        print(e)
         raise HTTPException(status_code=500, detail=f'Error fetching chat history: {str(e)}')
     finally:
         # Close the database connection
         conn.close()
 
 @app.post('/updatechat')
 async def update_chat_history(request: Request):
@@ -687,58 +745,216 @@
     user_email = data.get('userEmail')
 
     if not user_email:
         raise HTTPException(status_code=400, detail='userEmail is required')
 
     email_safe = user_email.replace('.', '_').replace('@', '_')
     today_start = get_start_of_day(datetime.now())
-    seven_days_ago = get_date_x_days_ago(7)
+    yesterday_start = get_date_x_days_ago(1)
 
     conn = sqlite3.connect('user_database.db')
     cursor = conn.cursor()
 
     try:
         cursor.execute(f'''
             SELECT chat_id, messageheader, timestamp
             FROM {email_safe}
         ''')
 
         chats = cursor.fetchall()
 
         today_chats = []
-        past_seven_days_chats = []
+        yesterday_chats = []
+        previous_chats = []
+
 
         for chat in chats:
             chat_id, message_header, timestamp = chat
             chat_date = datetime.fromisoformat(timestamp)
 
             if chat_date >= today_start:
                 today_chats.append({
                     'chat_id': chat_id,
                     'message_header': message_header,
                     'timestamp': timestamp
                 })
-            elif chat_date >= seven_days_ago:
-                past_seven_days_chats.append({
+            elif chat_date >= yesterday_start and chat_date < today_start:
+                yesterday_chats.append({
+                    'chat_id': chat_id,
+                    'message_header': message_header,
+                    'timestamp': timestamp
+                })
+            else:
+                previous_chats.append({
                     'chat_id': chat_id,
                     'message_header': message_header,
                     'timestamp': timestamp
                 })
 
-        print(today_chats, past_seven_days_chats)
         return JSONResponse(content={
             'today': today_chats,
-            'past_seven': past_seven_days_chats
+            'yesterday': yesterday_chats,
+            'previous': previous_chats
         })
 
     except Exception as e:
         raise HTTPException(status_code=500, detail=f'Error fetching chat sidebar: {str(e)}')
     finally:
         conn.close()
 
+@app.route('/fetch_user_details', methods=['POST'])
+async def fetch_user_details(request: Request):
+    data = await request.json()
+    email = data['email']
+
+    conn = sqlite3.connect('user_database.db')
+    cursor = conn.cursor()
+
+    cursor.execute('''
+    SELECT email, fullname, role, profilepic, designation, notifications, JWT FROM users WHERE email = ?
+    ''', (email,))
+
+    user = cursor.fetchone()
+
+    if user:
+        email, fullname, role, profilepic, designation, notifications, JWT = user
+        response = {
+            'status': True,
+            'email': email,
+            'fullname': fullname,
+            'role': role,
+            'profilepic': profilepic,
+            'designation': designation,
+            'notifications': notifications,
+            "JWT":JWT
+        }
+    else:
+        response = {'status': False, 'message': 'User not found'}
+
+    conn.close()
+    return JSONResponse(content=response)
+
+
+@app.get("/fetch_users")
+async def fetch_non_admin_users():
+    conn = sqlite3.connect('user_database.db')
+    cursor = conn.cursor()
+
+    cursor.execute('''
+    SELECT email, fullname, role, profilepic, designation, notifications 
+    FROM users 
+    WHERE role != "admin" AND role != "Admin"
+    ''')
+
+    users = cursor.fetchall()
+
+    user_list = [
+        {
+            "email": user[0],
+            "fullname": user[1],
+            "role": user[2],
+            "profilepic": user[3],
+            "designation": user[4],
+            "notifications": user[5]
+        }
+        for user in users
+    ]
+
+    conn.close()
+    return JSONResponse(content={"status": True, "users": user_list})
+
+
+class UpdateUserRequest(BaseModel):
+    email: str
+    password: str
+    fullname: str
+    role: str
+    profilepic: str
+    designation: str
+    notifications: str
+
+@app.post('/update_user')
+async def update_user(request: Request):
+    data = await request.json()
+    print(data)
+    email = data.get('email')
+
+    # Validate that email is provided
+    if not email:
+        raise HTTPException(status_code=400, detail="Email is required to update user information.")
+    
+    update_fields = {
+        'password': data.get('password'),
+        'fullname': data.get('fullname'),
+        'role': data.get('role'),
+        'profilepic': data.get('profilepic'),
+        'designation': data.get('designation'),
+        'notifications': data.get('notifications')
+    }
+    
+    # Filter out None values from the update_fields dictionary
+    update_fields = {k: v for k, v in update_fields.items() if v is not None}
+    
+    # Validate that at least one field to update is provided
+    if not update_fields:
+        raise HTTPException(status_code=400, detail="At least one field is required to update user information.")
+    
+    set_clause = ', '.join([f"{k} = ?" for k in update_fields.keys()])
+    values = list(update_fields.values())
+    values.append(email)  # Add email to the end of the values list for the WHERE clause
+    
+    conn = sqlite3.connect('user_database.db')
+    cursor = conn.cursor()
+    
+    try:
+        cursor.execute(f"UPDATE users SET {set_clause} WHERE email = ?", values)
+        conn.commit()
+        
+        if cursor.rowcount == 0:
+            raise HTTPException(status_code=404, detail="User not found.")
+        
+        response = {'message': 'User information updated successfully.', 'status': True}
+    except sqlite3.Error as e:
+        conn.rollback()
+        raise HTTPException(status_code=500, detail=f"Database error: {e}")
+    finally:
+        conn.close()
+    
+    return JSONResponse(content=response)
+
+@app.post("/delete_user")
+async def delete_user(request: Request):
+    data = await request.json()
+    email = data.get('email')
+
+    if not email:
+        raise HTTPException(status_code=400, detail="Email not provided")
+
+    conn = sqlite3.connect('user_database.db')
+    cursor = conn.cursor()
+
+    # Check if the user exists
+    cursor.execute('SELECT 1 FROM users WHERE email = ?', (email,))
+    user_exists = cursor.fetchone()
+
+    if not user_exists:
+        conn.close()
+        raise HTTPException(status_code=404, detail="User not found")
+
+    # Delete the user
+    cursor.execute('DELETE FROM users WHERE email = ?', (email,))
+    sanitized_table_name = sanitize_email(email)
+    cursor.execute(f'DROP TABLE IF EXISTS {sanitized_table_name}')
+    conn.commit()
+    conn.close()
+
+    return {"message": "User deleted successfully"}
+
+
+
 def main():
     import uvicorn
     setup_database()
     uvicorn.run(app, host="0.0.0.0", port=8000)
 
 if __name__ == "__main__":
     main()
```

## Comparing `ALLMDEV-1.3.7.dist-info/METADATA` & `ALLMDEV-1.3.8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ALLMDEV
-Version: 1.3.7
+Version: 1.3.8
 Summary: A simple and efficient python library for fast inference of GGUF Large Language Models.
 Author: All Advance AI
 Author-email: allmdev@allaai.com
 Maintainer: Soham Ghadge
 Maintainer-email: soham.ghadge@allaai.com
 Keywords: GGUF,GGUF Large Language Model,GGUF Large Language Models,GGUF Large Language Modeling,GGUF Large Language Modeling Library
 Description-Content-Type: text/markdown
@@ -20,14 +20,16 @@
 Requires-Dist: pdfminer.six
 Requires-Dist: pydantic ==1.10.13
 Requires-Dist: sentence-transformers
 Requires-Dist: vertexai
 Requires-Dist: google-cloud-aiplatform
 Requires-Dist: openai
 Requires-Dist: python-multipart
+Requires-Dist: pyjwt
+Requires-Dist: python-dotenv
 
 # ALLM
 
 ALLM is a Python library designed for fast inference of GGUF (Generic Global Unsupervised Features) Large Language Models (LLMs) on both CPU and GPU. It provides a convenient interface for loading pre-trained GGUF models and performing inference using them. This library is ideal for applications where quick response times are crucial, such as chatbots, text generation, and more.
 
 ## Features
```

## Comparing `ALLMDEV-1.3.7.dist-info/entry_points.txt` & `ALLMDEV-1.3.8.dist-info/entry_points.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,10 +6,10 @@
 allm-agentchat-azure = ALLMDEV.azureagentchat:main
 allm-agentchat-vertex = ALLMDEV.vertexagentchat:main
 allm-launch = ALLMDEV.backend:main
 allm-newagent = ALLMDEV.newagent:main
 allm-run = ALLMDEV.cli:main
 allm-run-azure = ALLMDEV.azurecli:main
 allm-run-vertex = ALLMDEV.vertexcli:main
-allm-serve = ALLMDEV.serve:main
+allm-serve = ALLMDEV.api:main
 allm-studio = ALLMDEV.studio:main
 allm-updateagent = ALLMDEV.updateagent:main
```

## Comparing `ALLMDEV-1.3.7.dist-info/RECORD` & `ALLMDEV-1.3.8.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 ALLMDEV/__init__.py,sha256=8XSO2SVH9cZ_Iut8rNwcDxtEaBp4LIdXP6hAKGRgeaI,39
 ALLMDEV/agentapi.py,sha256=vnkpCaviW0w5EQTE99els4Nb8QABv0TgNoP2FdFsWVQ,3706
 ALLMDEV/agentchat.py,sha256=UHLn4mVEBz6C77G8aaf3DWrzuVPfA-PCEp6uFZpcGyM,3440
+ALLMDEV/api.py,sha256=7aq8I0bv2uTTSOkVNYiV_N4usigXIrJuWHMaMEY9NNw,34081
 ALLMDEV/azureagentapi.py,sha256=dzMwkJHfRBqRxYAwpe_aQRgASqnsNBaEzT9jsc791QQ,4986
 ALLMDEV/azureagentchat.py,sha256=6L9m2B6dfe9LUWdd_Vj6_TT1n1GBXxVvqOeA-yTuV_Q,3298
 ALLMDEV/azurecli.py,sha256=nLoSVPpxWwIJWhiddB0_qzNw53hrAE6ijK0diDlaGYs,2435
-ALLMDEV/backend.py,sha256=owOM8c2NBz2Z4sxzqBCd0hbNJq79nQ1aZrlETzco0Jc,25481
+ALLMDEV/backend.py,sha256=qcGM2euc5iIG0z8BpzG6G5fq2WiPGNEZUfCtF8cFGAo,32582
 ALLMDEV/chat_history.py,sha256=Et8kDK4RKdIr-v4CoYdvd5yb37GxTHpu4U1gHw5C2GY,4952
 ALLMDEV/cli.py,sha256=13o2i7g_DtOyP8N8x7QdMr8iUGr4raJX26NJ9oqpgNw,3221
 ALLMDEV/instruct.py,sha256=-3ybhrmAwgLy_MptpJHhFnbQq1NcT4DHeMV2-46Tzl8,12685
 ALLMDEV/newagent.py,sha256=BzdKTA6gutbZbJS3nL1aWZqmTxe7QABkrLz9zpxlQZc,3096
 ALLMDEV/serve.py,sha256=RUKwji_795izII7XlYku1KUK6bvgR_SYBB9N34GwqUA,2231
 ALLMDEV/studio.py,sha256=LlrIEWcs-o8cIjnprJVijR8cNxrOsnFvl9AgTrk43iw,1932
 ALLMDEV/test.py,sha256=CxP_WW9ZXEiLCJh_9MLdieFU-yfNMwWlXrcrs7gtXx8,683
 ALLMDEV/updateagent.py,sha256=BzdKTA6gutbZbJS3nL1aWZqmTxe7QABkrLz9zpxlQZc,3096
 ALLMDEV/vertexagentapi.py,sha256=fPbLJoy8Wirh7wPc31EzlgLSqfF2e4PkEwYCO9h4yqk,4530
 ALLMDEV/vertexagentchat.py,sha256=dYvJ2_teBGeEN3TTrXq4pSulYJW5kmNPKFa9xg9ec9s,2826
 ALLMDEV/vertexcli.py,sha256=-5BgOKO7oMsjcsJRluAM0ivWllzpBpWmVQIzHbq_Xrk,2126
-ALLMDEV-1.3.7.dist-info/METADATA,sha256=rNUB4sPvqmJt5ZVgK3pTXFbl0xIubg3FDBLKAyU0c7w,6093
-ALLMDEV-1.3.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ALLMDEV-1.3.7.dist-info/entry_points.txt,sha256=u71vTXywZkZgH8fa1luPKfAsQCbItzqCHI6DgWpJGH4,591
-ALLMDEV-1.3.7.dist-info/top_level.txt,sha256=zQYMpzphh7BJt_BseuV6ImX-bYvNZcuXsmNLbIr57Ts,8
-ALLMDEV-1.3.7.dist-info/RECORD,,
+ALLMDEV-1.3.8.dist-info/METADATA,sha256=6TOj9a9y0x0f7aOtV99GN1K5N9UgVKdVDLT0lt2x9vk,6145
+ALLMDEV-1.3.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ALLMDEV-1.3.8.dist-info/entry_points.txt,sha256=pjURSzuC4nj_kFl775kwqXRV2icVzPLAt9uTPNSUwig,589
+ALLMDEV-1.3.8.dist-info/top_level.txt,sha256=zQYMpzphh7BJt_BseuV6ImX-bYvNZcuXsmNLbIr57Ts,8
+ALLMDEV-1.3.8.dist-info/RECORD,,
```

