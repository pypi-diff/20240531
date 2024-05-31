# Comparing `tmp/ollama_chat-0.9.8.tar.gz` & `tmp/ollama_chat-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ollama_chat-0.9.8.tar", last modified: Wed May 29 20:07:23 2024, max compression
+gzip compressed data, was "ollama_chat-0.9.9.tar", last modified: Fri May 31 18:30:33 2024, max compression
```

## Comparing `ollama_chat-0.9.8.tar` & `ollama_chat-0.9.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-29 20:07:23.071281 ollama_chat-0.9.8/
--rw-r--r--   0 craighobbs   (501) staff       (20)     1081 2024-05-29 16:38:26.000000 ollama_chat-0.9.8/LICENSE
--rw-r--r--   0 craighobbs   (501) staff       (20)     3636 2024-05-29 20:07:23.071218 ollama_chat-0.9.8/PKG-INFO
--rw-r--r--   0 craighobbs   (501) staff       (20)     2778 2024-05-29 20:06:26.000000 ollama_chat-0.9.8/README.md
--rw-r--r--   0 craighobbs   (501) staff       (20)       50 2024-05-29 16:38:26.000000 ollama_chat-0.9.8/pyproject.toml
--rw-r--r--   0 craighobbs   (501) staff       (20)     1059 2024-05-29 20:07:23.071540 ollama_chat-0.9.8/setup.cfg
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-29 20:07:23.068423 ollama_chat-0.9.8/src/
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-29 20:07:23.069610 ollama_chat-0.9.8/src/ollama_chat/
--rw-r--r--   0 craighobbs   (501) staff       (20)        0 2024-05-29 16:38:26.000000 ollama_chat-0.9.8/src/ollama_chat/__init__.py
--rw-r--r--   0 craighobbs   (501) staff       (20)      229 2024-05-29 16:38:26.000000 ollama_chat-0.9.8/src/ollama_chat/__main__.py
--rw-r--r--   0 craighobbs   (501) staff       (20)    12030 2024-05-29 17:01:39.000000 ollama_chat-0.9.8/src/ollama_chat/app.py
--rw-r--r--   0 craighobbs   (501) staff       (20)     3113 2024-05-29 16:38:26.000000 ollama_chat-0.9.8/src/ollama_chat/main.py
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-29 20:07:23.070795 ollama_chat-0.9.8/src/ollama_chat/static/
--rw-r--r--   0 craighobbs   (501) staff       (20)        0 2024-05-29 16:38:26.000000 ollama_chat-0.9.8/src/ollama_chat/static/__init__.py
--rw-r--r--   0 craighobbs   (501) staff       (20)     3774 2024-05-29 16:38:26.000000 ollama_chat-0.9.8/src/ollama_chat/static/index.html
--rw-r--r--   0 craighobbs   (501) staff       (20)    17920 2024-05-29 20:03:34.000000 ollama_chat-0.9.8/src/ollama_chat/static/ollamaChat.bare
--rw-r--r--   0 craighobbs   (501) staff       (20)     3506 2024-05-29 16:38:26.000000 ollama_chat-0.9.8/src/ollama_chat/static/ollamaChat.smd
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-29 20:07:23.070958 ollama_chat-0.9.8/src/ollama_chat.egg-info/
--rw-r--r--   0 craighobbs   (501) staff       (20)     3636 2024-05-29 20:07:23.000000 ollama_chat-0.9.8/src/ollama_chat.egg-info/PKG-INFO
--rw-r--r--   0 craighobbs   (501) staff       (20)      527 2024-05-29 20:07:23.000000 ollama_chat-0.9.8/src/ollama_chat.egg-info/SOURCES.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)        1 2024-05-29 20:07:23.000000 ollama_chat-0.9.8/src/ollama_chat.egg-info/dependency_links.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       54 2024-05-29 20:07:23.000000 ollama_chat-0.9.8/src/ollama_chat.egg-info/entry_points.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       44 2024-05-29 20:07:23.000000 ollama_chat-0.9.8/src/ollama_chat.egg-info/requires.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       12 2024-05-29 20:07:23.000000 ollama_chat-0.9.8/src/ollama_chat.egg-info/top_level.txt
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-31 18:30:33.184502 ollama_chat-0.9.9/
+-rw-r--r--   0 craighobbs   (501) staff       (20)     1081 2024-05-29 16:38:26.000000 ollama_chat-0.9.9/LICENSE
+-rw-r--r--   0 craighobbs   (501) staff       (20)     3636 2024-05-31 18:30:33.184441 ollama_chat-0.9.9/PKG-INFO
+-rw-r--r--   0 craighobbs   (501) staff       (20)     2778 2024-05-29 20:06:26.000000 ollama_chat-0.9.9/README.md
+-rw-r--r--   0 craighobbs   (501) staff       (20)       50 2024-05-29 16:38:26.000000 ollama_chat-0.9.9/pyproject.toml
+-rw-r--r--   0 craighobbs   (501) staff       (20)     1059 2024-05-31 18:30:33.184754 ollama_chat-0.9.9/setup.cfg
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-31 18:30:33.181819 ollama_chat-0.9.9/src/
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-31 18:30:33.182945 ollama_chat-0.9.9/src/ollama_chat/
+-rw-r--r--   0 craighobbs   (501) staff       (20)        0 2024-05-29 16:38:26.000000 ollama_chat-0.9.9/src/ollama_chat/__init__.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)      229 2024-05-29 16:38:26.000000 ollama_chat-0.9.9/src/ollama_chat/__main__.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)    12030 2024-05-29 17:01:39.000000 ollama_chat-0.9.9/src/ollama_chat/app.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)     3113 2024-05-29 16:38:26.000000 ollama_chat-0.9.9/src/ollama_chat/main.py
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-31 18:30:33.184051 ollama_chat-0.9.9/src/ollama_chat/static/
+-rw-r--r--   0 craighobbs   (501) staff       (20)        0 2024-05-29 16:38:26.000000 ollama_chat-0.9.9/src/ollama_chat/static/__init__.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)     3774 2024-05-29 16:38:26.000000 ollama_chat-0.9.9/src/ollama_chat/static/index.html
+-rw-r--r--   0 craighobbs   (501) staff       (20)    21165 2024-05-31 18:19:48.000000 ollama_chat-0.9.9/src/ollama_chat/static/ollamaChat.bare
+-rw-r--r--   0 craighobbs   (501) staff       (20)     3506 2024-05-29 16:38:26.000000 ollama_chat-0.9.9/src/ollama_chat/static/ollamaChat.smd
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-31 18:30:33.184207 ollama_chat-0.9.9/src/ollama_chat.egg-info/
+-rw-r--r--   0 craighobbs   (501) staff       (20)     3636 2024-05-31 18:30:33.000000 ollama_chat-0.9.9/src/ollama_chat.egg-info/PKG-INFO
+-rw-r--r--   0 craighobbs   (501) staff       (20)      527 2024-05-31 18:30:33.000000 ollama_chat-0.9.9/src/ollama_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)        1 2024-05-31 18:30:33.000000 ollama_chat-0.9.9/src/ollama_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       54 2024-05-31 18:30:33.000000 ollama_chat-0.9.9/src/ollama_chat.egg-info/entry_points.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       44 2024-05-31 18:30:33.000000 ollama_chat-0.9.9/src/ollama_chat.egg-info/requires.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       12 2024-05-31 18:30:33.000000 ollama_chat-0.9.9/src/ollama_chat.egg-info/top_level.txt
```

### Comparing `ollama_chat-0.9.8/LICENSE` & `ollama_chat-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.8/PKG-INFO` & `ollama_chat-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ollama-chat
-Version: 0.9.8
+Version: 0.9.9
 Summary: ollama-chat
 Home-page: https://github.com/craigahobbs/ollama-chat
 Author: Craig A. Hobbs
 Author-email: craigahobbs@gmail.com
 License: MIT
 Keywords: ollama-chat
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ollama_chat-0.9.8/README.md` & `ollama_chat-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.8/setup.cfg` & `ollama_chat-0.9.9/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ollama-chat
-version = 0.9.8
+version = 0.9.9
 url = https://github.com/craigahobbs/ollama-chat
 author = Craig A. Hobbs
 author_email = craigahobbs@gmail.com
 license = MIT
 description = ollama-chat
 long_description = file:README.md
 long_description_content_type = text/markdown
```

### Comparing `ollama_chat-0.9.8/src/ollama_chat/app.py` & `ollama_chat-0.9.9/src/ollama_chat/app.py`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.8/src/ollama_chat/main.py` & `ollama_chat-0.9.9/src/ollama_chat/main.py`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.8/src/ollama_chat/static/index.html` & `ollama_chat-0.9.9/src/ollama_chat/static/index.html`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.8/src/ollama_chat/static/ollamaChat.bare` & `ollama_chat-0.9.9/src/ollama_chat/static/ollamaChat.bare`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 endfunction
 
 
 # The Ollama Chat application URL arguments
 ollamaChatArguments = argsValidate(arrayNew( \
     objectNew('name', 'view'), \
     objectNew('name', 'id'), \
+    objectNew('name', 'multiline', 'type', 'bool'), \
     objectNew('name', 'action', 'explicit', true), \
     objectNew('name', 'actionId', 'explicit', true), \
     objectNew('name', 'message', 'explicit', true) \
 ))
 
 
 # The application title
@@ -194,15 +195,15 @@
             ollamaChatErrorPage('Failed to get current model')
             return
         endif
         model = objectGet(modelResponse, 'model')
     endif
 
     # Render the floating controls
-    elementModelRender(ollamaChatPageFloatingElements(id, generating))
+    elementModelRender(ollamaChatPageFloatingElements(args, generating))
     documentSetFocus(ollamaChatPromptInputID)
 
     # Render the chat title
     documentSetTitle(title)
     markdownPrint( \
         '# ' + title, \
         '', \
@@ -238,14 +239,15 @@
     ollamaChatConversationPageBottom(args, conversation, generating)
 endfunction
 
 
 # Helper to render the bottom of Ollama Chat conversation page
 async function ollamaChatConversationPageBottom(args, conversation, generating):
     id = objectGet(args, 'id')
+    multiline = objectGet(args, 'multiline')
 
     # Render the model reply
     exchanges = objectGet(conversation, 'exchanges')
     markdownPrint(objectGet(arrayGet(exchanges, arrayLength(exchanges) - 1), 'model'))
 
     # Render the regenerate and delete links
     if !generating:
@@ -259,18 +261,18 @@
                 formsLinkButtonElements('Regenerate', systemPartial(ollamaChatOnConversationClick, id, 'regenerateConversationExchange')) \
             )) \
         )
     endif
 
     # Render the bottom space
     fontSizePx = documentFontSize()
-    bottomSpacePx = mathFloor(4.5 * fontSizePx)
+    bottomSpacePx = if(multiline, 12, 4) * fontSizePx
     bottomElementId = stringSlice(argsURL(ollamaChatArguments, null, false, ollamaChatBottomID), 1)
     elementModelRender(arrayNew( \
-        objectNew('html', 'div', 'attr', objectNew('style', 'height: ' + bottomSpacePx + 'px')), \
+        objectNew('html', 'div', 'attr', objectNew('style', 'height: ' + numberToFixed(bottomSpacePx, ollamaChatPrecision) + 'px')), \
         objectNew('html', 'div', 'attr', objectNew('id', bottomElementId)) \
     ))
 
     # Set the conversation update timeout
     if generating:
         windowSetTimeout(systemPartial(ollamaChatOnConversationTimeout, args), ollamaChatTimeoutMs)
     endif
@@ -299,41 +301,63 @@
 
     # Render the page bottom
     documentSetReset(ollamaChatDocumentResetID)
     ollamaChatConversationPageBottom(args, conversation, generating)
 endfunction
 
 
-# The chat refresh period, in milliseconds
+# The conversation refresh period, in milliseconds
 ollamaChatTimeoutMs = 500
 
 
-# The Ollama Chat prompt input ID
+# The conversation prompt input ID
 ollamaChatPromptInputID = 'ollama-chat-prompt'
 
 
-# The Ollama Chat document reset ID
+# The conversation prompt session storage key
+ollamaChatSessionKey = 'ollama-chat-conversation-message'
+
+
+# The conversation document reset ID
 ollamaChatDocumentResetID = 'ollama-chat-document-reset-id'
 
 
-# The Ollama Chat scroll-to bottom ID
+# The conversation bottom element ID (for scroll to bottom)
 ollamaChatBottomID = 'ollama-chat-bottom-id'
 
 
-# Conversation action on-click event handler
+# The numeric attribute precision
+ollamaChatPrecision = 3
+
+
+# Generic conversation button on-click event handler
 async function ollamaChatOnConversationClick(id, url):
     # Perform the conversation acgtion
     actionRequest = jsonStringify(objectNew('id', id))
     systemFetch(objectNew('url', url, 'body', actionRequest))
 
     # Render the page
     ollamaChatMain()
 endfunction
 
 
+# Conversation multiline button on-click event handler
+async function ollamaChatOnConversationMultiline(args):
+    # If there is prompt text save it in session storage
+    prompt = stringTrim(documentInputValue(ollamaChatPromptInputID))
+    if prompt != '':
+        sessionStorageSet(ollamaChatSessionKey, prompt)
+    endif
+
+    # Toggle multiline prompt mode
+    multiline = objectGet(args, 'multiline')
+    windowSetLocation(argsURL(ollamaChatArguments, objectNew('multiline', !multiline)))
+endfunction
+
+
 # Prompt on-enter/on-click event handler
 async function ollamaChatOnPrompt(id, message):
     # Get the prompt text
     prompt = if(message != null, message, stringTrim(documentInputValue(ollamaChatPromptInputID)))
     if prompt == '':
         return
     endif
@@ -360,124 +384,174 @@
 
     # Render the conversation page
     ollamaChatMain()
 endfunction
 
 
 # The Ollama chat pages floating controls element model
-function ollamaChatPageFloatingElements(id, generating):
+function ollamaChatPageFloatingElements(args, generating):
+    id = objectGet(args, 'id')
+    multiline = objectGet(args, 'multiline')
     elements = arrayNew()
 
     # Compute spacing
     fontSizePx = documentFontSize()
-    topSpacePx = mathFloor(1.5 * fontSizePx)
-    borderRadiusPx = mathFloor(0.5 * fontSizePx)
-    menuPadPx = mathFloor(0.75 * fontSizePx)
-    inputPadPx = fontSizePx
-    textPadPx = mathFloor(0.5 * fontSizePx)
-    buttonLeftRightPx = mathFloor(0.5 * fontSizePx)
-    buttonTopBottomPx = fontSizePx
+    topSpacePx = 1.5 * fontSizePx
+    borderRadiusPx = 0.5 * fontSizePx
+    menuPadPx = 0.65 * fontSizePx
+    inputPadPx = 0.75 * fontSizePx
+    textPadPx = 0.5 * fontSizePx
+    buttonSize = 2 * fontSizePx
     topBottomPx = fontSizePx
     leftRightPx = 2 * fontSizePx
 
     # The top space
-    arrayPush(elements, objectNew('html', 'div', 'attr', objectNew('style', 'height: ' + topSpacePx + 'px')))
+    arrayPush(elements, objectNew( \
+        'html', 'div', \
+        'attr', objectNew('style', 'height: ' + numberToFixed(topSpacePx, ollamaChatPrecision) + 'px')) \
+    )
 
     # The menu controls
     separator = stringFromCharCode(160) + '|' + stringFromCharCode(160)
     arrayPush(elements, objectNew( \
         'html', 'div', \
         'attr', objectNew( \
             'style', arrayJoin(arrayNew( \
                 'align-items: left', \
                 'background-color: #e0e0e0', \
-                'border-radius: ' + borderRadiusPx + 'px', \
+                'border-radius: ' + numberToFixed(borderRadiusPx, ollamaChatPrecision) + 'px', \
                 'color: black', \
                 'display: flex', \
-                'left: ' + topBottomPx + 'px', \
-                'padding: ' + menuPadPx + 'px', \
+                'left: ' + numberToFixed(topBottomPx, ollamaChatPrecision) + 'px', \
+                'padding: ' + numberToFixed(menuPadPx, ollamaChatPrecision) + 'px', \
                 'position: fixed', \
-                'top: ' + topBottomPx + 'px' \
+                'top: ' + numberToFixed(topBottomPx, ollamaChatPrecision) + 'px' \
             ), '; ') \
         ), \
         'elem', arrayNew( \
             formsLinkElements('Back', argsURL(ollamaChatArguments, null, true)), \
-            if(!generating, arrayNew( \
+            arrayNew( \
                 objectNew('text', separator), \
                 formsLinkElements('Top', argsURL(ollamaChatArguments, null, false, '_top')), \
                 objectNew('text', separator), \
                 formsLinkElements('Bottom', argsURL(ollamaChatArguments, null, false, ollamaChatBottomID)) \
-            )) \
+            ) \
         ) \
     ))
 
+    # Get the saved session prompt, if any
+    prompt = sessionStorageGet(ollamaChatSessionKey)
+    if prompt != null:
+        sessionStorageRemove(ollamaChatSessionKey)
+    endif
+
     # The prompt controls
     arrayPush(elements, objectNew( \
         'html', 'div', \
         'attr', objectNew( \
             'style', arrayJoin(arrayNew( \
-                'align-items: center', \
+                'align-items: flex-end', \
                 'background-color: #c0c0c0', \
-                'border-radius: ' + borderRadiusPx + 'px', \
-                'bottom: ' + topBottomPx + 'px', \
+                'border-radius: ' + numberToFixed(borderRadiusPx, ollamaChatPrecision) + 'px', \
+                'bottom: ' + numberToFixed(topBottomPx, ollamaChatPrecision) + 'px', \
                 'display: flex', \
-                'left: ' + leftRightPx + 'px', \
-                'padding: ' + inputPadPx + 'px', \
+                'left: ' + numberToFixed(leftRightPx, ollamaChatPrecision) + 'px', \
+                'padding: ' + numberToFixed(inputPadPx, ollamaChatPrecision) + 'px', \
                 'position: fixed', \
-                'right: ' + leftRightPx + 'px' \
+                'right: ' + numberToFixed(leftRightPx, ollamaChatPrecision) + 'px' \
             ), '; ') \
         ), \
         'elem', arrayNew( \
+            ollamaChatSVGButton(0.75 * buttonSize, buttonSize, 24, 'M4,6 H20 M4,12 H20 M4,18 H20', 'none', 'none', \
+                systemPartial(ollamaChatOnConversationMultiline, args)), \
             objectNew( \
-                'html', 'input', \
+                'html', if(multiline, 'textarea', 'input'), \
                 'attr', objectNew( \
-                    'type', 'text', \
+                    'type', if(!multiline, 'text'), \
                     'id', ollamaChatPromptInputID, \
                     'placeholder', 'Type your message...', \
+                    'rows', if(multiline, 8), \
                     'style', arrayJoin(arrayNew( \
                         'background-color: white', \
                         'border: none', \
                         'flex: 1', \
                         'font-size: inherit', \
-                        'margin-right: ' + textPadPx + 'px', \
+                        'font-family: inherit', \
+                        'margin-left: ' + numberToFixed(textPadPx, ollamaChatPrecision) + 'px', \
+                        'margin-right: ' + numberToFixed(textPadPx, ollamaChatPrecision) + 'px', \
                         'min-width: 0', \
                         'outline: none', \
-                        'padding: ' + textPadPx + 'px' \
-                    ), '; ') \
+                        'padding: ' + numberToFixed(textPadPx, ollamaChatPrecision) + 'px', \
+                        'resize: none' \
+                    ), '; '), \
+                    'value', if(!multiline, prompt) \
                 ), \
-                'callback', if(!generating, objectNew('keyup', systemPartial(formsTextOnKeyup, systemPartial(ollamaChatOnPrompt, id)))) \
+                'elem', if(multiline && prompt != null, objectNew('text', prompt)), \
+                'callback', if(!multiline && !generating, \
+                    objectNew('keyup', systemPartial(formsTextOnKeyup, systemPartial(ollamaChatOnPrompt, id))) \
+                ) \
             ), \
-            if(!generating, objectNew( \
-                'html', 'button', \
-                'attr', objectNew( \
-                    'style', arrayJoin(arrayNew( \
-                        'background-color: #4dff4d', \
-                        'border-radius: ' + borderRadiusPx + 'px', \
-                        'border: none', \
-                        'color: black', \
-                        'font-size: inherit', \
-                        'padding: ' + buttonLeftRightPx + 'px ' + buttonTopBottomPx + 'px' \
-                    ), '; ') \
-                ), \
-                'elem', objectNew('text', 'Go'), \
-                'callback', objectNew('click', systemPartial(ollamaChatOnPrompt, id)) \
-            )), \
-            if(generating, objectNew( \
-                'html', 'button', \
-                'attr', objectNew( \
-                    'style', arrayJoin(arrayNew( \
-                        'background-color: #ff4d4d', \
-                        'border-radius: ' + borderRadiusPx + 'px', \
-                        'border: none', \
-                        'color: white', \
-                        'font-size: inherit', \
-                        'padding: ' + buttonLeftRightPx + 'px ' + buttonTopBottomPx + 'px' \
-                    ), '; ') \
-                ), \
-                'elem', objectNew('text', 'Stop'), \
-                'callback', objectNew('click', systemPartial(ollamaChatOnConversationClick, id, 'stopConversation')) \
-            )) \
+            if(!generating, \
+                ollamaChatSVGButton(buttonSize, buttonSize, 24, 'M12,18 V7 M7,12 L12,7 L17,12', 'none', 'white', \
+                    systemPartial(ollamaChatOnPrompt, id)) \
+            ), \
+            if(generating, \
+                ollamaChatSVGButton(buttonSize, buttonSize, 24, 'M8,8 H16 V16 H8 Z', 'black', 'white', \
+                    systemPartial(ollamaChatOnConversationClick, id, 'stopConversation')) \
+            ) \
         ) \
     ))
 
     return elements
 endfunction
+
+
+# Create an SVG button element model
+function ollamaChatSVGButton(width, height, viewSize, symbolPath, symbolFill, backgroundColor, callback):
+    return objectNew( \
+        'html', 'button', \
+        'attr', objectNew( \
+            'type', 'button', \
+            'style', arrayJoin(arrayNew( \
+                'background: transparent', \
+                'border: none', \
+                'padding: 0', \
+                'cursor: pointer' \
+            ), '; '), \
+            'onmouseover', "this.children[0].style.opacity='0.75';", \
+            'onmouseout', "this.children[0].style.opacity='1';" \
+        ), \
+        'elem', objectNew( \
+            'svg', 'svg', \
+            'attr', objectNew( \
+                'width', numberToFixed(width, ollamaChatPrecision), \
+                'height', numberToFixed(height, ollamaChatPrecision), \
+                'viewBox', '0 0 ' + viewSize + ' ' + viewSize, \
+                'fill', 'none', \
+                'style', 'vertical-align: middle', \
+                'preserveAspectRatio', 'none' \
+            ), \
+            'elem', arrayNew( \
+                if(backgroundColor != null, objectNew( \
+                    'svg', 'circle', \
+                    'attr', objectNew( \
+                        'cx', numberToFixed(0.5 * viewSize, ollamaChatPrecision), \
+                        'cy', numberToFixed(0.5 * viewSize, ollamaChatPrecision), \
+                        'r', numberToFixed(0.5 * viewSize, ollamaChatPrecision), \
+                        'stroke', 'none', \
+                        'fill', backgroundColor \
+                    ) \
+                )), \
+                objectNew( \
+                    'svg', 'path', \
+                    'attr', objectNew( \
+                        'd', symbolPath, \
+                        'stroke', if(symbolFill == 'none', 'black', 'none'), \
+                        'fill', symbolFill, \
+                        'stroke-width', numberToFixed(0.1 * viewSize) \
+                    ) \
+                ) \
+            ) \
+        ), \
+        'callback', objectNew('click', callback) \
+    )
+endfunction
```

### Comparing `ollama_chat-0.9.8/src/ollama_chat/static/ollamaChat.smd` & `ollama_chat-0.9.9/src/ollama_chat/static/ollamaChat.smd`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.8/src/ollama_chat.egg-info/PKG-INFO` & `ollama_chat-0.9.9/src/ollama_chat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ollama-chat
-Version: 0.9.8
+Version: 0.9.9
 Summary: ollama-chat
 Home-page: https://github.com/craigahobbs/ollama-chat
 Author: Craig A. Hobbs
 Author-email: craigahobbs@gmail.com
 License: MIT
 Keywords: ollama-chat
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ollama_chat-0.9.8/src/ollama_chat.egg-info/SOURCES.txt` & `ollama_chat-0.9.9/src/ollama_chat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

