# Comparing `tmp/simpleai_base-0.2.1-cp312-none-win_amd64.whl.zip` & `tmp/simpleai_base-0.3.1-pp310-pypy310_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 2254421 bytes, number of entries: 12
--rw-r--r--  4.6 unx      343 b- defN 24-May-16 11:05 simpleai_base-0.2.1.dist-info/METADATA
--rw-r--r--  4.6 unx       95 b- defN 24-May-16 11:05 simpleai_base-0.2.1.dist-info/WHEEL
--rw-r--r--  4.6 unx     5017 b- defN 24-May-16 11:05 simpleai_base/comfyclient_pipeline.py
--rw-r--r--  4.6 unx      630 b- defN 24-May-16 11:05 simpleai_base/config.py
--rw-r--r--  4.6 unx      156 b- defN 24-May-16 11:05 simpleai_base/models_hub_host.py
--rw-r--r--  4.6 unx     9216 b- defN 24-May-16 11:05 simpleai_base/models_info.py
--rw-r--r--  4.6 unx     2446 b- defN 24-May-16 11:05 simpleai_base/params_mapper.py
--rw-r--r--  4.6 unx     2682 b- defN 24-May-16 11:05 simpleai_base/utils.py
--rw-r--r--  4.6 unx     1220 b- defN 24-May-16 11:05 simpleai_base/version.py
--rw-r--r--  4.6 unx     1524 b- defN 24-May-16 11:05 simpleai_base/__init__.py
--rwxr-xr-x  4.6 unx  5118464 b- defN 24-May-16 11:05 simpleai_base/simpleai_base.cp312-win_amd64.pyd
--rw-r--r--  4.6 unx     1005 b- defN 24-May-16 11:05 simpleai_base-0.2.1.dist-info/RECORD
-12 files, 5142798 bytes uncompressed, 2252733 bytes compressed:  56.2%
+Zip file size: 4084841 bytes, number of entries: 12
+-rw-r--r--  4.6 unx      357 b- defN 24-May-16 18:42 simpleai_base-0.3.1.dist-info/METADATA
+-rw-r--r--  4.6 unx      136 b- defN 24-May-16 18:42 simpleai_base-0.3.1.dist-info/WHEEL
+-rw-r--r--  4.6 unx     1443 b- defN 24-May-16 18:42 simpleai_base/__init__.py
+-rw-r--r--  4.6 unx      609 b- defN 24-May-16 18:42 simpleai_base/config.py
+-rw-r--r--  4.6 unx     4892 b- defN 24-May-16 18:42 simpleai_base/comfyclient_pipeline.py
+-rw-r--r--  4.6 unx      152 b- defN 24-May-16 18:42 simpleai_base/models_hub_host.py
+-rw-r--r--  4.6 unx     2388 b- defN 24-May-16 18:42 simpleai_base/params_mapper.py
+-rw-r--r--  4.6 unx     2610 b- defN 24-May-16 18:42 simpleai_base/utils.py
+-rw-r--r--  4.6 unx     1182 b- defN 24-May-16 18:42 simpleai_base/version.py
+-rw-r--r--  4.6 unx     9009 b- defN 24-May-16 18:42 simpleai_base/models_info.py
+-rwxr-xr-x  4.6 unx 12579776 b- defN 24-May-16 18:42 simpleai_base/simpleai_base.pypy310-pp73-x86_64-linux-gnu.so
+-rw-r--r--  4.6 unx     1020 b- defN 24-May-16 18:42 simpleai_base-0.3.1.dist-info/RECORD
+12 files, 12603574 bytes uncompressed, 4083127 bytes compressed:  67.6%
```

## zipnote {}

```diff
@@ -1,37 +1,37 @@
-Filename: simpleai_base-0.2.1.dist-info/METADATA
+Filename: simpleai_base-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: simpleai_base-0.2.1.dist-info/WHEEL
+Filename: simpleai_base-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: simpleai_base/comfyclient_pipeline.py
+Filename: simpleai_base/__init__.py
 Comment: 
 
 Filename: simpleai_base/config.py
 Comment: 
 
-Filename: simpleai_base/models_hub_host.py
+Filename: simpleai_base/comfyclient_pipeline.py
 Comment: 
 
-Filename: simpleai_base/models_info.py
+Filename: simpleai_base/models_hub_host.py
 Comment: 
 
 Filename: simpleai_base/params_mapper.py
 Comment: 
 
 Filename: simpleai_base/utils.py
 Comment: 
 
 Filename: simpleai_base/version.py
 Comment: 
 
-Filename: simpleai_base/__init__.py
+Filename: simpleai_base/models_info.py
 Comment: 
 
-Filename: simpleai_base/simpleai_base.cp312-win_amd64.pyd
+Filename: simpleai_base/simpleai_base.pypy310-pp73-x86_64-linux-gnu.so
 Comment: 
 
-Filename: simpleai_base-0.2.1.dist-info/RECORD
+Filename: simpleai_base-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simpleai_base/comfyclient_pipeline.py

 * *Ordering differences only*

```diff
@@ -1,125 +1,125 @@
-import os
-import json
-import websocket 
-import uuid
-import random
-import httpx
-import numpy as np
-from io import BytesIO
-from PIL import Image
-
-def upload_mask(mask):
-    with BytesIO() as output:
-        mask.save(output)
-        output.seek(0)
-        files = {'mask': ('mask.jpg', output)}
-        data = {'overwrite': 'true', 'type': 'example_type'}
-        response = httpx.post("http://{}/upload/mask".format(server_address), files=files, data=data)
-    return response.json()
-
-def queue_prompt(prompt):
-    p = {"prompt": prompt, "client_id": client_id}
-    data = json.dumps(p).encode('utf-8')
-    with httpx.Client() as client:
-        response = client.post("http://{}/prompt".format(server_address), data=data)
-        return json.loads(response.read())
-
-def get_image(filename, subfolder, folder_type):
-    params = httpx.QueryParams({
-        "filename": filename,
-        "subfolder": subfolder,
-        "type": folder_type
-    })
-    with httpx.Client() as client:
-        response = client.get(f"http://{server_address}/view", params=params)
-        return response.read()
-
-def get_history(prompt_id):
-    with httpx.Client() as client:
-        response = client.get("http://{}/history/{}".format(server_address, prompt_id))
-        return json.loads(response.read())
-
-def get_images(ws, prompt, callback=None):
-    prompt_id = queue_prompt(prompt)['prompt_id']
-    print('[ComfyClient] Request and get ComfyTask_id:{}'.format(prompt_id))
-    output_images = {}
-    current_node = ''
-    last_node = None
-    preview_image = []
-    last_step = None
-    current_step = None
-    current_total_steps = None
-    while True:
-        out = ws.recv()
-        if isinstance(out, str):
-            message = json.loads(out)
-            current_type = message['type']
-            #print(f'current_message={message}')
-            if message['type'] == 'executing':
-                data = message['data']
-                if data['node'] is None and data['prompt_id'] == prompt_id:
-                    break
-                else:
-                    current_node = data['node']
-            elif message['type'] == 'progress':
-                current_step = message["data"]["value"]
-                current_total_steps = message["data"]["max"]
-        else:
-            if current_type == 'progress':
-                if 'KSampler' in prompt[current_node]['class_type'] and callback is not None:
-                    if current_step == last_step:
-                        preview_image.append(out[8:])
-                    else:
-                        if last_step is not None:
-                            callback(last_step, current_total_steps, Image.open(BytesIO(preview_image[0])))
-                        preview_image = []
-                        preview_image.append(out[8:])
-                        last_step = current_step
-                if prompt[current_node]['class_type'] == 'SaveImageWebsocket':
-                    images_output = output_images.get(prompt[current_node]['_meta']['title'], [])
-                    images_output.append(out[8:])
-                    output_images[prompt[current_node]['_meta']['title']] = images_output[0]
-            continue  
-
-    output_images = {k: np.array(Image.open(BytesIO(v))) for k, v in output_images.items()}
-    print(f'[ComfyClient] The ComfyTask:{prompt_id} has finished: {len(output_images)}')
-    return output_images
-
-def images_upload(images):
-    result = {}
-    if images is None:
-        return result
-    for k,np_image in images.items():
-        pil_image = Image.fromarray(np_image)
-        with BytesIO() as output:
-            pil_image.save(output, format="PNG")
-            output.seek(0)
-            files = {'image': (f'image_{client_id}_{random.randint(1000, 9999)}.png', output)}
-            data = {'overwrite': 'true', 'type': 'input'}
-            response = httpx.post("http://{}/upload/image".format(server_address), files=files, data=data)
-        result.update({k: response.json()["name"]})
-    print(f'[ComfyClient] The ComfyTask:upload_input_images has finished: {len(result)}')
-    return result
-
-
-def process_flow(flow_name, params, images, callback=None):
-    global ws
-
-    flow_file = os.path.join(WORKFLOW_DIR, f'{flow_name}_api.json')
-    if ws is None:
-        ws = websocket.WebSocket()
-        ws.connect("ws://{}/ws?clientId={}".format(server_address, client_id))
-    images_map = images_upload(images)
-    params.add_params(images_map)
-    with open(flow_file, 'r', encoding="utf-8") as workflow_api_file:
-        flowdata = json.load(workflow_api_file)
-    print(f'[ComfyClient] Ready ComfyTask to process: workflow={flow_name}, params={params.params}')
-    images = get_images(ws, params.convert2comfy(flowdata), callback=callback)
-
-    return images
-
-WORKFLOW_DIR = 'workflows'
-COMFYUI_ENDPOINT = '127.0.0.1:8188'
-server_address = COMFYUI_ENDPOINT
-client_id = str(uuid.uuid4())  
-ws = None
+import os
+import json
+import websocket 
+import uuid
+import random
+import httpx
+import numpy as np
+from io import BytesIO
+from PIL import Image
+
+def upload_mask(mask):
+    with BytesIO() as output:
+        mask.save(output)
+        output.seek(0)
+        files = {'mask': ('mask.jpg', output)}
+        data = {'overwrite': 'true', 'type': 'example_type'}
+        response = httpx.post("http://{}/upload/mask".format(server_address), files=files, data=data)
+    return response.json()
+
+def queue_prompt(prompt):
+    p = {"prompt": prompt, "client_id": client_id}
+    data = json.dumps(p).encode('utf-8')
+    with httpx.Client() as client:
+        response = client.post("http://{}/prompt".format(server_address), data=data)
+        return json.loads(response.read())
+
+def get_image(filename, subfolder, folder_type):
+    params = httpx.QueryParams({
+        "filename": filename,
+        "subfolder": subfolder,
+        "type": folder_type
+    })
+    with httpx.Client() as client:
+        response = client.get(f"http://{server_address}/view", params=params)
+        return response.read()
+
+def get_history(prompt_id):
+    with httpx.Client() as client:
+        response = client.get("http://{}/history/{}".format(server_address, prompt_id))
+        return json.loads(response.read())
+
+def get_images(ws, prompt, callback=None):
+    prompt_id = queue_prompt(prompt)['prompt_id']
+    print('[ComfyClient] Request and get ComfyTask_id:{}'.format(prompt_id))
+    output_images = {}
+    current_node = ''
+    last_node = None
+    preview_image = []
+    last_step = None
+    current_step = None
+    current_total_steps = None
+    while True:
+        out = ws.recv()
+        if isinstance(out, str):
+            message = json.loads(out)
+            current_type = message['type']
+            #print(f'current_message={message}')
+            if message['type'] == 'executing':
+                data = message['data']
+                if data['node'] is None and data['prompt_id'] == prompt_id:
+                    break
+                else:
+                    current_node = data['node']
+            elif message['type'] == 'progress':
+                current_step = message["data"]["value"]
+                current_total_steps = message["data"]["max"]
+        else:
+            if current_type == 'progress':
+                if 'KSampler' in prompt[current_node]['class_type'] and callback is not None:
+                    if current_step == last_step:
+                        preview_image.append(out[8:])
+                    else:
+                        if last_step is not None:
+                            callback(last_step, current_total_steps, Image.open(BytesIO(preview_image[0])))
+                        preview_image = []
+                        preview_image.append(out[8:])
+                        last_step = current_step
+                if prompt[current_node]['class_type'] == 'SaveImageWebsocket':
+                    images_output = output_images.get(prompt[current_node]['_meta']['title'], [])
+                    images_output.append(out[8:])
+                    output_images[prompt[current_node]['_meta']['title']] = images_output[0]
+            continue  
+
+    output_images = {k: np.array(Image.open(BytesIO(v))) for k, v in output_images.items()}
+    print(f'[ComfyClient] The ComfyTask:{prompt_id} has finished: {len(output_images)}')
+    return output_images
+
+def images_upload(images):
+    result = {}
+    if images is None:
+        return result
+    for k,np_image in images.items():
+        pil_image = Image.fromarray(np_image)
+        with BytesIO() as output:
+            pil_image.save(output, format="PNG")
+            output.seek(0)
+            files = {'image': (f'image_{client_id}_{random.randint(1000, 9999)}.png', output)}
+            data = {'overwrite': 'true', 'type': 'input'}
+            response = httpx.post("http://{}/upload/image".format(server_address), files=files, data=data)
+        result.update({k: response.json()["name"]})
+    print(f'[ComfyClient] The ComfyTask:upload_input_images has finished: {len(result)}')
+    return result
+
+
+def process_flow(flow_name, params, images, callback=None):
+    global ws
+
+    flow_file = os.path.join(WORKFLOW_DIR, f'{flow_name}_api.json')
+    if ws is None:
+        ws = websocket.WebSocket()
+        ws.connect("ws://{}/ws?clientId={}".format(server_address, client_id))
+    images_map = images_upload(images)
+    params.add_params(images_map)
+    with open(flow_file, 'r', encoding="utf-8") as workflow_api_file:
+        flowdata = json.load(workflow_api_file)
+    print(f'[ComfyClient] Ready ComfyTask to process: workflow={flow_name}, params={params.params}')
+    images = get_images(ws, params.convert2comfy(flowdata), callback=callback)
+
+    return images
+
+WORKFLOW_DIR = 'workflows'
+COMFYUI_ENDPOINT = '127.0.0.1:8188'
+server_address = COMFYUI_ENDPOINT
+client_id = str(uuid.uuid4())  
+ws = None
```

## simpleai_base/config.py

 * *Ordering differences only*

```diff
@@ -1,21 +1,21 @@
-from . import utils
-
-paths_checkpoints = ''
-paths_loras = ''
-path_embeddings = ''
-
-def set_paths(checkpoints, loras, embeddings):
-    global paths_checkpoints, paths_loras, path_embeddings
-
-    paths_checkpoints = checkpoints
-    paths_loras = loras
-    path_embeddings = embeddings
-
-
-def get_model_filenames(folder_paths, extensions=None, name_filter=None):
-    if extensions is None:
-        extensions = ['.pth', '.ckpt', '.bin', '.safetensors', '.fooocus.patch']
-    files = []
-    for folder in folder_paths:
-        files += utils.get_files_from_folder(folder, extensions, name_filter)
-    return files
+from . import utils
+
+paths_checkpoints = ''
+paths_loras = ''
+path_embeddings = ''
+
+def set_paths(checkpoints, loras, embeddings):
+    global paths_checkpoints, paths_loras, path_embeddings
+
+    paths_checkpoints = checkpoints
+    paths_loras = loras
+    path_embeddings = embeddings
+
+
+def get_model_filenames(folder_paths, extensions=None, name_filter=None):
+    if extensions is None:
+        extensions = ['.pth', '.ckpt', '.bin', '.safetensors', '.fooocus.patch']
+    files = []
+    for folder in folder_paths:
+        files += utils.get_files_from_folder(folder, extensions, name_filter)
+    return files
```

## simpleai_base/models_hub_host.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-models_hub_host = "http://124.222.60.66:1120"
-models_hub_host_2 =  "http://91.229.91.74:1120"
-accelerate_DID = "FWRfVFKLSrmmnrggmuCTATSqYpjGSPgu3"
-    
+models_hub_host = "http://124.222.60.66:1120"
+models_hub_host_2 =  "http://91.229.91.74:1120"
+accelerate_DID = "FWRfVFKLSrmmnrggmuCTATSqYpjGSPgu3"
+
```

## simpleai_base/models_info.py

 * *Ordering differences only*

```diff
@@ -1,207 +1,207 @@
-import os
-import json
-import base64
-import hashlib
-import requests
-import time
-from . import models_hub_host
-from . import config
-
-
-models_info = {}
-models_info_muid = {}
-models_info_rsync = {}
-models_info_file = ['models_info', 0]
-models_info_path = os.path.abspath(f'./models/{models_info_file[0]}.json')
-
-default_models_info = {
-    "checkpoints/juggernautXL_version6Rundiffusion.safetensors": {
-        "size": 7105348560,
-        "hash": "H+bH7FTHhgQM2rx7TolyAGnZcJaSLiDQHxPndkQStH8=" },
-    "checkpoints/sd_xl_base_1.0_0.9vae.safetensors": {
-        "size": 6938078334,
-        "hash": "5rueqFu/e/ZHinxtGLcSRvIuldQbzdgO1AqiEsM8/v8=" },
-    "checkpoints/bluePencilXL_v050.safetensors": {
-        "size": 6938040682,
-        "hash": "jEYqgPS1KRsk/rYk1nJIvQn3H5B01wFNiteQGxIL3Mc=" },
-    "checkpoints/sd_xl_refiner_1.0_0.9vae.safetensors": {
-        "size": 6075981930,
-        "hash": "jQzmwBYATL2s1Q+Tfa04HYw5ZijWIaf5cZFHBTJ4AWQ=" },
-    "checkpoints/realisticStockPhoto_v10.safetensors": {
-        "size": 6938053346,
-        "hash": "LUTON43cySJ2nfTv/nTa4zcKiH6piXCT4fX73FC2egI=" },
-    "checkpoints/DreamShaper_8_pruned.safetensors": {
-        "size": 2132625894,
-        "hash": "h521I8MNO5AXFD1WcFAV4VostWKHYsEdCG/tlTir1/0=" },
-    "checkpoints/juggernautXL_v7Rundiffusion.safetensors": {
-        "size": 7105352832,
-        "hash": "ByRRjGtahV4XYEMvvwPIBblb0voHJy8PNq33rtlaAeM=" },
-    "checkpoints/bluePencilXLV200.cXoH.safetensors": {
-        "size": 6938040682,
-        "hash": "1ZYnt0lbBYHe0rBIismPneuGtS1D6dkCkU8Pnc/9sWw=" },
-    "checkpoints/dreamshaperXL_turboDpmppSDE.safetensors": {
-        "size": 6939220250,
-        "hash": "Z28NYMjoYBRtXooNgCWZyt0E58rfhcKD8Yn0HwHJ41k=" }
-     }
-    
-
-def init_models_info():
-    global models_info, models_info_file, models_info_path
-
-    if os.path.exists(models_info_path):
-        file_mtime = time.localtime(os.path.getmtime(models_info_path)) 
-        if (models_info is None or file_mtime != models_info_file[1]):
-            try:
-                with open(models_info_path, "r", encoding="utf-8") as json_file:
-                    models_info.update(json.load(json_file))
-                models_info_file[1] = file_mtime
-            except Exception as e:
-                print(f'[ModelInfo] Load model info file [{models_info_path}] failed!')
-                print(e)
-    refresh_models_info_from_path()
-    return
-    
-def refresh_models_info_from_path():
-    global models_info, models_info_file, models_info_path
-
-    model_filenames = config.get_model_filenames(config.paths_checkpoints)
-    lora_filenames = config.get_model_filenames(config.paths_loras)
-    embedding_filenames = config.get_model_filenames([config.path_embeddings])
-    models_info_muid = {}
-    new_filenames = []
-    new_models_info = {}
-    for k in model_filenames:
-        filename = 'checkpoints/'+k
-        if filename not in models_info.keys():
-            new_filenames.append(filename)
-        else:
-            new_models_info.update({filename: models_info[filename]})
-            if models_info[filename]['muid']:
-                models_info_muid.update({models_info[filename]['muid']: filename})
-    for k in lora_filenames:
-        filename = 'loras/'+k
-        if filename not in models_info.keys():
-            new_filenames.append(filename)
-        else:
-            new_models_info.update({filename: models_info[filename]})
-            if models_info[filename]['muid']:
-                models_info_muid.update({models_info[filename]['muid']: filename})
-    for k in embedding_filenames:
-        filename = 'embeddings/'+k
-        if filename not in models_info.keys():
-            new_filenames.append(filename)
-        else:
-            new_models_info.update({filename: models_info[filename]})
-            if models_info[filename]['muid']:
-                models_info_muid.update({models_info[filename]['muid']: filename})
-    models_info = new_models_info
-
-    if len(new_filenames)>0:
-        try:
-            for f in new_filenames:
-                if f.startswith("checkpoints/"):
-                    file_path = os.path.join(config.paths_checkpoints[0], f[12:])
-                elif f.startswith("loras/"):
-                    file_path = os.path.join(config.paths_loras[0], f[6:])
-                elif f.startswith("embeddings/"):
-                    file_path = os.path.join(config.path_embeddings, f[11:])
-                else:
-                    file_path = os.path.abspath(f'./models/{f}')
-                size = os.path.getsize(file_path)
-                if f in default_models_info.keys() and size == default_models_info[f]["size"]:
-                    hash = default_models_info[f]["hash"]
-                else:
-                    hash = ''
-                models_info.update({f:{'size': size, 'hash': hash, 'url': None, 'muid': None}})
-            with open(models_info_path, "w", encoding="utf-8") as json_file:
-                json.dump(models_info, json_file, indent=4)
-            models_info_file[1] = time.localtime(os.path.getmtime(models_info_path))
-        except Exception as e:
-            print(f'[ModelInfo] Update model info file [{models_info_path}] failed!')
-            print(e)
-    
-    return
-
-                
-def get_file_sha256(file_path):
-    sha256obj = hashlib.sha256()
-    with open(file_path, 'rb') as f:
-        while True:
-            b = f.read(4*1024*1024)
-            if not b:
-                break
-            sha256obj.update(b)
-    return base64.b64encode(sha256obj.digest()).decode('utf-8')
-                
-
-
-
-def sync_model_info(downurls):
-    global models_info, models_info_rsync, models_info_file, models_info_path
-
-    keys = sorted(models_info.keys())
-    # file hash completion
-    for f in keys:
-        if not models_info[f]['hash']:
-            print(f'[ModelInfo] Computing file hash for {f}')
-            if f.startswith("checkpoints/"):
-                file_path = os.path.join(config.paths_checkpoints[0], f[12:])
-            elif f.startswith("loras/"):
-                file_path = os.path.join(config.paths_loras[0], f[6:])
-            elif f.startswith("embeddings/"):
-                file_path = os.path.join(config.path_embeddings, f[11:])
-            else:
-                file_path = os.path.abspath(f'./models/{f}')
-            models_info[f].update({'hash':get_file_sha256(file_path)})
-    keylist = []
-    for i in range(len(keys)):
-        if keys[i].startswith('checkpoints'):
-            keylist.append(keys[i])
-        if keys[i].startswith('loras'):
-            keylist.append(keys[i])
-    for i in range(len(keys)):
-        if not keys[i].startswith('checkpoints') and not keys[i].startswith('loras'):
-            keylist.append(keys[i])
-
-    models_info_rsync = {}
-    models_info_update_flag = False
-    for i in range(len(keylist)):
-        #print(f'downurls: i={i}, k={keylist[i]}, {downurls[i]}')
-        durl = '' if i >= len(downurls) else downurls[i]
-        if durl and models_info[keylist[i]]['url'] != durl:
-            models_info_rsync.update({keylist[i]: {"hash": models_info[keylist[i]]['hash'], "url": durl}})
-            models_info[keylist[i]]['url'] = durl
-            models_info_update_flag = True
-
-    file_mtime = time.localtime(os.path.getmtime(models_info_path))
-    for k in models_info.keys():
-        if not models_info[k]['muid'] and k not in models_info_rsync.keys():
-            models_info_rsync.update({k: {"hash": models_info[k]['hash'], "url": ""}})
-    try:
-        #response = requests.post(f'{models_hub_host}/register_claim/', data = token_did.get_register_claim('SimpleSDXLHub'))
-        #rsync_muid_msg = { "files": token_did.encrypt_default(json.dumps(models_info_rsync)) }
-        #headers = { "DID": token_did.DID}
-        #response = requests.post(f'{models_hub_host}/rsync_muid/', data = json.dumps(rsync_muid_msg), headers = headers)
-        #results = json.loads(response.text)
-        #if (results["message"] == "it's ok!" and results["results"]):
-        #    for k in results["results"].keys():
-        #        models_info[k]['muid'] = results["results"][k]['muid']
-        #        models_info_muid[results["results"][k]['muid']] = k
-        #        models_info[k]['url'] = results["results"][k]['url']
-        #    print(f'[ModelInfo] Rsync {len(results["results"].keys())} MUIDs info from model hub.')
-        #    with open(models_info_path, "w", encoding="utf-8") as json_file:
-        #        json.dump(models_info, json_file, indent=4)
-            models_info_file[1] = time.localtime(os.path.getmtime(models_info_path))
-    except Exception as e:
-            print(f'[ModelInfo] Connect the models hub site failed!')
-            print(e)
-
-    file_mtime2 = time.localtime(os.path.getmtime(models_info_path))
-    if (models_info_update_flag and file_mtime == file_mtime2):
-        with open(models_info_path, "w", encoding="utf-8") as json_file:
-            json.dump(models_info, json_file, indent=4)
-        models_info_file[1] = time.localtime(os.path.getmtime(models_info_path))
-    return keylist
-
-
-
+import os
+import json
+import base64
+import hashlib
+import requests
+import time
+from . import models_hub_host
+from . import config
+
+
+models_info = {}
+models_info_muid = {}
+models_info_rsync = {}
+models_info_file = ['models_info', 0]
+models_info_path = os.path.abspath(f'./models/{models_info_file[0]}.json')
+
+default_models_info = {
+    "checkpoints/juggernautXL_version6Rundiffusion.safetensors": {
+        "size": 7105348560,
+        "hash": "H+bH7FTHhgQM2rx7TolyAGnZcJaSLiDQHxPndkQStH8=" },
+    "checkpoints/sd_xl_base_1.0_0.9vae.safetensors": {
+        "size": 6938078334,
+        "hash": "5rueqFu/e/ZHinxtGLcSRvIuldQbzdgO1AqiEsM8/v8=" },
+    "checkpoints/bluePencilXL_v050.safetensors": {
+        "size": 6938040682,
+        "hash": "jEYqgPS1KRsk/rYk1nJIvQn3H5B01wFNiteQGxIL3Mc=" },
+    "checkpoints/sd_xl_refiner_1.0_0.9vae.safetensors": {
+        "size": 6075981930,
+        "hash": "jQzmwBYATL2s1Q+Tfa04HYw5ZijWIaf5cZFHBTJ4AWQ=" },
+    "checkpoints/realisticStockPhoto_v10.safetensors": {
+        "size": 6938053346,
+        "hash": "LUTON43cySJ2nfTv/nTa4zcKiH6piXCT4fX73FC2egI=" },
+    "checkpoints/DreamShaper_8_pruned.safetensors": {
+        "size": 2132625894,
+        "hash": "h521I8MNO5AXFD1WcFAV4VostWKHYsEdCG/tlTir1/0=" },
+    "checkpoints/juggernautXL_v7Rundiffusion.safetensors": {
+        "size": 7105352832,
+        "hash": "ByRRjGtahV4XYEMvvwPIBblb0voHJy8PNq33rtlaAeM=" },
+    "checkpoints/bluePencilXLV200.cXoH.safetensors": {
+        "size": 6938040682,
+        "hash": "1ZYnt0lbBYHe0rBIismPneuGtS1D6dkCkU8Pnc/9sWw=" },
+    "checkpoints/dreamshaperXL_turboDpmppSDE.safetensors": {
+        "size": 6939220250,
+        "hash": "Z28NYMjoYBRtXooNgCWZyt0E58rfhcKD8Yn0HwHJ41k=" }
+     }
+    
+
+def init_models_info():
+    global models_info, models_info_file, models_info_path
+
+    if os.path.exists(models_info_path):
+        file_mtime = time.localtime(os.path.getmtime(models_info_path)) 
+        if (models_info is None or file_mtime != models_info_file[1]):
+            try:
+                with open(models_info_path, "r", encoding="utf-8") as json_file:
+                    models_info.update(json.load(json_file))
+                models_info_file[1] = file_mtime
+            except Exception as e:
+                print(f'[ModelInfo] Load model info file [{models_info_path}] failed!')
+                print(e)
+    refresh_models_info_from_path()
+    return
+    
+def refresh_models_info_from_path():
+    global models_info, models_info_file, models_info_path
+
+    model_filenames = config.get_model_filenames(config.paths_checkpoints)
+    lora_filenames = config.get_model_filenames(config.paths_loras)
+    embedding_filenames = config.get_model_filenames([config.path_embeddings])
+    models_info_muid = {}
+    new_filenames = []
+    new_models_info = {}
+    for k in model_filenames:
+        filename = 'checkpoints/'+k
+        if filename not in models_info.keys():
+            new_filenames.append(filename)
+        else:
+            new_models_info.update({filename: models_info[filename]})
+            if models_info[filename]['muid']:
+                models_info_muid.update({models_info[filename]['muid']: filename})
+    for k in lora_filenames:
+        filename = 'loras/'+k
+        if filename not in models_info.keys():
+            new_filenames.append(filename)
+        else:
+            new_models_info.update({filename: models_info[filename]})
+            if models_info[filename]['muid']:
+                models_info_muid.update({models_info[filename]['muid']: filename})
+    for k in embedding_filenames:
+        filename = 'embeddings/'+k
+        if filename not in models_info.keys():
+            new_filenames.append(filename)
+        else:
+            new_models_info.update({filename: models_info[filename]})
+            if models_info[filename]['muid']:
+                models_info_muid.update({models_info[filename]['muid']: filename})
+    models_info = new_models_info
+
+    if len(new_filenames)>0:
+        try:
+            for f in new_filenames:
+                if f.startswith("checkpoints/"):
+                    file_path = os.path.join(config.paths_checkpoints[0], f[12:])
+                elif f.startswith("loras/"):
+                    file_path = os.path.join(config.paths_loras[0], f[6:])
+                elif f.startswith("embeddings/"):
+                    file_path = os.path.join(config.path_embeddings, f[11:])
+                else:
+                    file_path = os.path.abspath(f'./models/{f}')
+                size = os.path.getsize(file_path)
+                if f in default_models_info.keys() and size == default_models_info[f]["size"]:
+                    hash = default_models_info[f]["hash"]
+                else:
+                    hash = ''
+                models_info.update({f:{'size': size, 'hash': hash, 'url': None, 'muid': None}})
+            with open(models_info_path, "w", encoding="utf-8") as json_file:
+                json.dump(models_info, json_file, indent=4)
+            models_info_file[1] = time.localtime(os.path.getmtime(models_info_path))
+        except Exception as e:
+            print(f'[ModelInfo] Update model info file [{models_info_path}] failed!')
+            print(e)
+    
+    return
+
+                
+def get_file_sha256(file_path):
+    sha256obj = hashlib.sha256()
+    with open(file_path, 'rb') as f:
+        while True:
+            b = f.read(4*1024*1024)
+            if not b:
+                break
+            sha256obj.update(b)
+    return base64.b64encode(sha256obj.digest()).decode('utf-8')
+                
+
+
+
+def sync_model_info(downurls):
+    global models_info, models_info_rsync, models_info_file, models_info_path
+
+    keys = sorted(models_info.keys())
+    # file hash completion
+    for f in keys:
+        if not models_info[f]['hash']:
+            print(f'[ModelInfo] Computing file hash for {f}')
+            if f.startswith("checkpoints/"):
+                file_path = os.path.join(config.paths_checkpoints[0], f[12:])
+            elif f.startswith("loras/"):
+                file_path = os.path.join(config.paths_loras[0], f[6:])
+            elif f.startswith("embeddings/"):
+                file_path = os.path.join(config.path_embeddings, f[11:])
+            else:
+                file_path = os.path.abspath(f'./models/{f}')
+            models_info[f].update({'hash':get_file_sha256(file_path)})
+    keylist = []
+    for i in range(len(keys)):
+        if keys[i].startswith('checkpoints'):
+            keylist.append(keys[i])
+        if keys[i].startswith('loras'):
+            keylist.append(keys[i])
+    for i in range(len(keys)):
+        if not keys[i].startswith('checkpoints') and not keys[i].startswith('loras'):
+            keylist.append(keys[i])
+
+    models_info_rsync = {}
+    models_info_update_flag = False
+    for i in range(len(keylist)):
+        #print(f'downurls: i={i}, k={keylist[i]}, {downurls[i]}')
+        durl = '' if i >= len(downurls) else downurls[i]
+        if durl and models_info[keylist[i]]['url'] != durl:
+            models_info_rsync.update({keylist[i]: {"hash": models_info[keylist[i]]['hash'], "url": durl}})
+            models_info[keylist[i]]['url'] = durl
+            models_info_update_flag = True
+
+    file_mtime = time.localtime(os.path.getmtime(models_info_path))
+    for k in models_info.keys():
+        if not models_info[k]['muid'] and k not in models_info_rsync.keys():
+            models_info_rsync.update({k: {"hash": models_info[k]['hash'], "url": ""}})
+    try:
+        #response = requests.post(f'{models_hub_host}/register_claim/', data = token_did.get_register_claim('SimpleSDXLHub'))
+        #rsync_muid_msg = { "files": token_did.encrypt_default(json.dumps(models_info_rsync)) }
+        #headers = { "DID": token_did.DID}
+        #response = requests.post(f'{models_hub_host}/rsync_muid/', data = json.dumps(rsync_muid_msg), headers = headers)
+        #results = json.loads(response.text)
+        #if (results["message"] == "it's ok!" and results["results"]):
+        #    for k in results["results"].keys():
+        #        models_info[k]['muid'] = results["results"][k]['muid']
+        #        models_info_muid[results["results"][k]['muid']] = k
+        #        models_info[k]['url'] = results["results"][k]['url']
+        #    print(f'[ModelInfo] Rsync {len(results["results"].keys())} MUIDs info from model hub.')
+        #    with open(models_info_path, "w", encoding="utf-8") as json_file:
+        #        json.dump(models_info, json_file, indent=4)
+            models_info_file[1] = time.localtime(os.path.getmtime(models_info_path))
+    except Exception as e:
+            print(f'[ModelInfo] Connect the models hub site failed!')
+            print(e)
+
+    file_mtime2 = time.localtime(os.path.getmtime(models_info_path))
+    if (models_info_update_flag and file_mtime == file_mtime2):
+        with open(models_info_path, "w", encoding="utf-8") as json_file:
+            json.dump(models_info, json_file, indent=4)
+        models_info_file[1] = time.localtime(os.path.getmtime(models_info_path))
+    return keylist
+
+
+
```

## simpleai_base/params_mapper.py

 * *Ordering differences only*

```diff
@@ -1,58 +1,58 @@
-
-class ComfyTaskParams:
-    def __init__(self, params):
-        self.params = params
-        self.workflow = ''
-
-    fooo2node = {
-        'seed': 'KSampler:main_sampler:seed',
-        'steps': 'KSampler:main_sampler:steps',
-        'cfg_scale': 'KSampler:main_sampler:cfg',
-        'sampler': 'KSampler:main_sampler:sampler_name',
-        'scheduler': 'KSampler:main_sampler:scheduler',
-        'denoise': 'KSampler:main_sampler:denoise',
-        'base_model': 'CheckpointLoaderSimple:base_model:ckpt_name',
-        'width': 'EmptyLatentImage:aspect_ratios_size:width;ImageResize:resize_input_image:width',
-        'height': 'EmptyLatentImage:aspect_ratios_size:height;ImageResize:resize_input_image:height',
-        'prompt': 'CLIPTextEncode:prompt:text',
-        'negative_prompt': 'CLIPTextEncode:negative_prompt:text',
-        'input_image': 'LoadImage:input_image:image',
-        'layer_diffuse_injection': 'LayeredDiffusionApply:layer_diffuse_apply:config',
-        'sd_version': 'LayeredDiffusionDecode:layer_diffuse_decode:sd_version;LayeredDiffusionDecodeRGBA:layer_diffuse_decode_rgba:sd_version',
-        'layer_diffuse_cond': 'LayeredDiffusionCondApply:layer_diffuse_cond_apply:config'
-        }
-
-    def set_mapping_rule(self, maps):
-        self.fooo2node.update(maps)
-
-    def add_params(self, new_parms):
-        self.params.update(new_parms)
-
-    def convert2comfy(self, workflow):
-        #print(f'params:{self.params}')
-        self.workflow = workflow
-        for (pk1,v) in self.params.items():
-            nk = self.fooo2node[pk1]
-            self.replace_key(nk,v)
-        return self.workflow
-
-
-    def replace_key(self,nk,v):
-        lines = nk.split(';')
-        for line in lines:
-            parts = line.strip().split(':')
-            class_type = parts[0].strip()
-            meta_title = parts[1].strip()
-            inputs = parts[2].strip()
-            for n in self.workflow.keys():
-                if self.workflow[n]["class_type"]==class_type and self.workflow[n]["_meta"]["title"]==meta_title:
-                    if '|' in inputs:
-                        keys = inputs.split('|')
-                        vs = v.strip().split('|')
-                        for i in range(len(keys)):
-                            self.workflow[n]["inputs"][keys[i]] = vs[i]
-                    else:
-                        self.workflow[n]["inputs"][inputs] = v
-    
-
-
+
+class ComfyTaskParams:
+    def __init__(self, params):
+        self.params = params
+        self.workflow = ''
+
+    fooo2node = {
+        'seed': 'KSampler:main_sampler:seed',
+        'steps': 'KSampler:main_sampler:steps',
+        'cfg_scale': 'KSampler:main_sampler:cfg',
+        'sampler': 'KSampler:main_sampler:sampler_name',
+        'scheduler': 'KSampler:main_sampler:scheduler',
+        'denoise': 'KSampler:main_sampler:denoise',
+        'base_model': 'CheckpointLoaderSimple:base_model:ckpt_name',
+        'width': 'EmptyLatentImage:aspect_ratios_size:width;ImageResize:resize_input_image:width',
+        'height': 'EmptyLatentImage:aspect_ratios_size:height;ImageResize:resize_input_image:height',
+        'prompt': 'CLIPTextEncode:prompt:text',
+        'negative_prompt': 'CLIPTextEncode:negative_prompt:text',
+        'input_image': 'LoadImage:input_image:image',
+        'layer_diffuse_injection': 'LayeredDiffusionApply:layer_diffuse_apply:config',
+        'sd_version': 'LayeredDiffusionDecode:layer_diffuse_decode:sd_version;LayeredDiffusionDecodeRGBA:layer_diffuse_decode_rgba:sd_version',
+        'layer_diffuse_cond': 'LayeredDiffusionCondApply:layer_diffuse_cond_apply:config'
+        }
+
+    def set_mapping_rule(self, maps):
+        self.fooo2node.update(maps)
+
+    def add_params(self, new_parms):
+        self.params.update(new_parms)
+
+    def convert2comfy(self, workflow):
+        #print(f'params:{self.params}')
+        self.workflow = workflow
+        for (pk1,v) in self.params.items():
+            nk = self.fooo2node[pk1]
+            self.replace_key(nk,v)
+        return self.workflow
+
+
+    def replace_key(self,nk,v):
+        lines = nk.split(';')
+        for line in lines:
+            parts = line.strip().split(':')
+            class_type = parts[0].strip()
+            meta_title = parts[1].strip()
+            inputs = parts[2].strip()
+            for n in self.workflow.keys():
+                if self.workflow[n]["class_type"]==class_type and self.workflow[n]["_meta"]["title"]==meta_title:
+                    if '|' in inputs:
+                        keys = inputs.split('|')
+                        vs = v.strip().split('|')
+                        for i in range(len(keys)):
+                            self.workflow[n]["inputs"][keys[i]] = vs[i]
+                    else:
+                        self.workflow[n]["inputs"][inputs] = v
+    
+
+
```

## simpleai_base/utils.py

 * *Ordering differences only*

```diff
@@ -1,72 +1,72 @@
-import os
-import hashlib
-
-folder_variation = {}
-def get_files_from_folder(folder_path, extensions=None, name_filter=None, variation=False):
-    global folder_variation
-
-    if not os.path.isdir(folder_path):
-        raise ValueError("Folder path is not a valid directory.")
-
-    filenames = []
-    for root, dirs, files in os.walk(folder_path, topdown=False):
-        relative_path = os.path.relpath(root, folder_path)
-        if relative_path == ".":
-            relative_path = ""
-        for filename in sorted(files, key=lambda s: s.casefold()):
-            _, file_extension = os.path.splitext(filename)
-            if (extensions is None or file_extension.lower() in extensions) and (name_filter is None or name_filter in _):
-                path = os.path.join(relative_path, filename)
-                if variation:
-                    mtime = int(os.path.getmtime(os.path.join(root, filename)))
-                    if folder_path not in folder_variation or path not in folder_variation[folder_path] or mtime > folder_variation[folder_path][path]:
-                        if folder_path not in folder_variation:
-                            folder_variation.update({folder_path: {path: mtime}})
-                        else:
-                            folder_variation[folder_path].update({path: mtime})
-                        filenames.append(path)
-                else:
-                    filenames.append(path)
-
-
-    return filenames
-
-HASH_SHA256_LENGTH = 10
-def sha256(filename, use_addnet_hash=False, length=HASH_SHA256_LENGTH):
-    print(f"Calculating sha256 for {filename}: ", end='')
-    if use_addnet_hash:
-        with open(filename, "rb") as file:
-            sha256_value = addnet_hash_safetensors(file)
-    else:
-        sha256_value = calculate_sha256(filename)
-    print(f"{sha256_value}")
-
-    return sha256_value[:length] if length is not None else sha256_value
-
-
-def addnet_hash_safetensors(b):
-    """kohya-ss hash for safetensors from https://github.com/kohya-ss/sd-scripts/blob/main/library/train_util.py"""
-    hash_sha256 = hashlib.sha256()
-    blksize = 1024 * 1024
-
-    b.seek(0)
-    header = b.read(8)
-    n = int.from_bytes(header, "little")
-
-    offset = n + 8
-    b.seek(offset)
-    for chunk in iter(lambda: b.read(blksize), b""):
-        hash_sha256.update(chunk)
-
-    return hash_sha256.hexdigest()
-
-
-def calculate_sha256(filename) -> str:
-    hash_sha256 = hashlib.sha256()
-    blksize = 1024 * 1024
-
-    with open(filename, "rb") as f:
-        for chunk in iter(lambda: f.read(blksize), b""):
-            hash_sha256.update(chunk)
-
-    return hash_sha256.hexdigest()
+import os
+import hashlib
+
+folder_variation = {}
+def get_files_from_folder(folder_path, extensions=None, name_filter=None, variation=False):
+    global folder_variation
+
+    if not os.path.isdir(folder_path):
+        raise ValueError("Folder path is not a valid directory.")
+
+    filenames = []
+    for root, dirs, files in os.walk(folder_path, topdown=False):
+        relative_path = os.path.relpath(root, folder_path)
+        if relative_path == ".":
+            relative_path = ""
+        for filename in sorted(files, key=lambda s: s.casefold()):
+            _, file_extension = os.path.splitext(filename)
+            if (extensions is None or file_extension.lower() in extensions) and (name_filter is None or name_filter in _):
+                path = os.path.join(relative_path, filename)
+                if variation:
+                    mtime = int(os.path.getmtime(os.path.join(root, filename)))
+                    if folder_path not in folder_variation or path not in folder_variation[folder_path] or mtime > folder_variation[folder_path][path]:
+                        if folder_path not in folder_variation:
+                            folder_variation.update({folder_path: {path: mtime}})
+                        else:
+                            folder_variation[folder_path].update({path: mtime})
+                        filenames.append(path)
+                else:
+                    filenames.append(path)
+
+
+    return filenames
+
+HASH_SHA256_LENGTH = 10
+def sha256(filename, use_addnet_hash=False, length=HASH_SHA256_LENGTH):
+    print(f"Calculating sha256 for {filename}: ", end='')
+    if use_addnet_hash:
+        with open(filename, "rb") as file:
+            sha256_value = addnet_hash_safetensors(file)
+    else:
+        sha256_value = calculate_sha256(filename)
+    print(f"{sha256_value}")
+
+    return sha256_value[:length] if length is not None else sha256_value
+
+
+def addnet_hash_safetensors(b):
+    """kohya-ss hash for safetensors from https://github.com/kohya-ss/sd-scripts/blob/main/library/train_util.py"""
+    hash_sha256 = hashlib.sha256()
+    blksize = 1024 * 1024
+
+    b.seek(0)
+    header = b.read(8)
+    n = int.from_bytes(header, "little")
+
+    offset = n + 8
+    b.seek(offset)
+    for chunk in iter(lambda: b.read(blksize), b""):
+        hash_sha256.update(chunk)
+
+    return hash_sha256.hexdigest()
+
+
+def calculate_sha256(filename) -> str:
+    hash_sha256 = hashlib.sha256()
+    blksize = 1024 * 1024
+
+    with open(filename, "rb") as f:
+        for chunk in iter(lambda: f.read(blksize), b""):
+            hash_sha256.update(chunk)
+
+    return hash_sha256.hexdigest()
```

## simpleai_base/version.py

 * *Ordering differences only*

```diff
@@ -1,38 +1,38 @@
-import os
-import pygit2
-
-branch = ''
-commit_id = ''
-simplesdxl_ver = ''
-
-def get_simplesdxl_ver():
-    global simplesdxl_ver, commit_id
-    if not simplesdxl_ver:
-        simplesdxl_log = os.path.abspath(f'./simplesdxl_log.md')
-        line = ''
-        if os.path.exists(simplesdxl_log):
-            with open(simplesdxl_log, "r", encoding="utf-8") as log_file:
-                line = log_file.readline().strip()
-                while line:
-                    if line.startswith("# "):
-                        break
-                    line = log_file.readline().strip()
-        else:
-            line = '# 2023-12-20'
-        date = line.split(' ')[1].split('-')
-        simplesdxl_ver = f'v{date[0]}{date[1]}{date[2]}'
-        if commit_id:
-            simplesdxl_ver += f'.{commit_id}'
-    return simplesdxl_ver
-
-def get_branch():
-    global branch, commit_id
-    if not branch:
-        pygit2.option(pygit2.GIT_OPT_SET_OWNER_VALIDATION, 0)
-        repo = pygit2.Repository(os.path.abspath(os.path.dirname(__file__)))
-        branch = repo.head.shorthand
-        if branch=="main":
-            branch = "Fooocus"
-        commit_id = repo.head.target.hex[:7]
-    return branch
-
+import os
+import pygit2
+
+branch = ''
+commit_id = ''
+simplesdxl_ver = ''
+
+def get_simplesdxl_ver():
+    global simplesdxl_ver, commit_id
+    if not simplesdxl_ver:
+        simplesdxl_log = os.path.abspath(f'./simplesdxl_log.md')
+        line = ''
+        if os.path.exists(simplesdxl_log):
+            with open(simplesdxl_log, "r", encoding="utf-8") as log_file:
+                line = log_file.readline().strip()
+                while line:
+                    if line.startswith("# "):
+                        break
+                    line = log_file.readline().strip()
+        else:
+            line = '# 2023-12-20'
+        date = line.split(' ')[1].split('-')
+        simplesdxl_ver = f'v{date[0]}{date[1]}{date[2]}'
+        if commit_id:
+            simplesdxl_ver += f'.{commit_id}'
+    return simplesdxl_ver
+
+def get_branch():
+    global branch, commit_id
+    if not branch:
+        pygit2.option(pygit2.GIT_OPT_SET_OWNER_VALIDATION, 0)
+        repo = pygit2.Repository(os.path.abspath(os.path.dirname(__file__)))
+        branch = repo.head.shorthand
+        if branch=="main":
+            branch = "Fooocus"
+        commit_id = repo.head.target.hex[:7]
+    return branch
+
```

## simpleai_base/__init__.py

```diff
@@ -1,35 +1,36 @@
-import os
-import importlib.util
-
-#from simpleai_base import simpleai_base
-
-__all__ = ['models_info', 'models_hub_host', 'comfyclient_pipeline', 'params_mapper', 'config']
-
-def get_torch_xformers_cuda_version():
-    try:
-        torch_version = ""
-        cuda_version = ""
-        torch_spec = importlib.util.find_spec("torch")
-        for folder in torch_spec.submodule_search_locations:
-            ver_file = os.path.join(folder, "version.py")
-            if os.path.isfile(ver_file):
-                spec = importlib.util.spec_from_file_location("torch_version_import", ver_file)
-                module = importlib.util.module_from_spec(spec)
-                spec.loader.exec_module(module)
-                torch_version = module.__version__
-                cuda_version = getattr(module, 'cuda', "")
-        xformers_version = ""
-        xformers_spec = importlib.util.find_spec("xformers")
-        for folder in xformers_spec.submodule_search_locations:
-            ver_file = os.path.join(folder, "version.py")
-            if os.path.isfile(ver_file):
-                spec = importlib.util.spec_from_file_location("xformers_version_import", ver_file)
-                module = importlib.util.module_from_spec(spec)
-                spec.loader.exec_module(module)
-                xformers_version = module.__version__
-    except:
-        pass
-    return torch_version, xformers_version, cuda_version
-
-torch_version, xformers_version, cuda_version = get_torch_xformers_cuda_version()
-
+import os
+import importlib.util
+
+# from simpleai_base import simpleai_base
+
+__all__ = ['models_info', 'models_hub_host', 'comfyclient_pipeline', 'params_mapper', 'config']
+
+
+def get_torch_xformers_cuda_version():
+    torch_ver = ""
+    cuda_ver = ""
+    xformers_ver = ""
+    try:
+        torch_spec = importlib.util.find_spec("torch")
+        for folder in torch_spec.submodule_search_locations:
+            ver_file = os.path.join(folder, "version.py")
+            if os.path.isfile(ver_file):
+                spec = importlib.util.spec_from_file_location("torch_version_import", ver_file)
+                module = importlib.util.module_from_spec(spec)
+                spec.loader.exec_module(module)
+                torch_ver = module.__version__
+                cuda_ver = getattr(module, 'cuda', "")
+        xformers_spec = importlib.util.find_spec("xformers")
+        for folder in xformers_spec.submodule_search_locations:
+            ver_file = os.path.join(folder, "version.py")
+            if os.path.isfile(ver_file):
+                spec = importlib.util.spec_from_file_location("xformers_version_import", ver_file)
+                module = importlib.util.module_from_spec(spec)
+                spec.loader.exec_module(module)
+                xformers_ver = module.__version__
+    except:
+        pass
+    return torch_ver, xformers_ver, cuda_ver
+
+
+torch_version, xformers_version, cuda_version = get_torch_xformers_cuda_version()
```

