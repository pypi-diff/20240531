# Comparing `tmp/pyphonic-1.0.2.tar.gz` & `tmp/pyphonic-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyphonic-1.0.2.tar", last modified: Fri May 17 03:03:09 2024, max compression
+gzip compressed data, was "pyphonic-1.1.0.tar", last modified: Fri May 31 03:24:21 2024, max compression
```

## Comparing `pyphonic-1.0.2.tar` & `pyphonic-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:03:09.166270 pyphonic-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-17 03:03:09.166270 pyphonic-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-17 03:03:04.000000 pyphonic-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-17 03:03:04.000000 pyphonic-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 03:03:09.166270 pyphonic-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:03:09.162270 pyphonic-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:03:09.166270 pyphonic-1.0.2/src/pyphonic/
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/10_fftramp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/11_polysynth.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/12_syncdnoise.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/13_sccompressor.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/4_butterworth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/5_midiarp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/6_wavetable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/7_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/8_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/9_saturator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/circular_buffer_overlap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/flipper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/midi_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/midirando.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-17 03:03:04.000000 pyphonic-1.0.2/src/pyphonic/multithreaded_noise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:03:09.166270 pyphonic-1.0.2/src/pyphonic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-17 03:03:09.000000 pyphonic-1.0.2/src/pyphonic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-17 03:03:09.000000 pyphonic-1.0.2/src/pyphonic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 03:03:09.000000 pyphonic-1.0.2/src/pyphonic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 03:03:09.000000 pyphonic-1.0.2/src/pyphonic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:24:21.397197 pyphonic-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-31 03:24:10.000000 pyphonic-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-05-31 03:24:21.397197 pyphonic-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-31 03:24:10.000000 pyphonic-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-31 03:24:10.000000 pyphonic-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 03:24:21.397197 pyphonic-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:24:21.393197 pyphonic-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:24:21.397197 pyphonic-1.1.0/src/pyphonic/
+-rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-05-31 03:24:10.000000 pyphonic-1.1.0/src/pyphonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-31 03:24:10.000000 pyphonic-1.1.0/src/pyphonic/circular_buffer_overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-31 03:24:10.000000 pyphonic-1.1.0/src/pyphonic/flipper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-31 03:24:10.000000 pyphonic-1.1.0/src/pyphonic/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-31 03:24:10.000000 pyphonic-1.1.0/src/pyphonic/midi_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-31 03:24:10.000000 pyphonic-1.1.0/src/pyphonic/multithreaded_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-31 03:24:10.000000 pyphonic-1.1.0/src/pyphonic/preset_10_fftramp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-31 03:24:10.000000 pyphonic-1.1.0/src/pyphonic/preset_11_polysynth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-31 03:24:10.000000 pyphonic-1.1.0/src/pyphonic/preset_12_syncdnoise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-31 03:24:10.000000 pyphonic-1.1.0/src/pyphonic/preset_13_sccompressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-31 03:24:10.000000 pyphonic-1.1.0/src/pyphonic/preset_14_nn_voice_change.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-31 03:24:10.000000 pyphonic-1.1.0/src/pyphonic/preset_15_gen_midi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-31 03:24:10.000000 pyphonic-1.1.0/src/pyphonic/preset_4_butterworth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-31 03:24:10.000000 pyphonic-1.1.0/src/pyphonic/preset_5_midiarp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-31 03:24:10.000000 pyphonic-1.1.0/src/pyphonic/preset_6_wavetable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-31 03:24:10.000000 pyphonic-1.1.0/src/pyphonic/preset_7_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-31 03:24:10.000000 pyphonic-1.1.0/src/pyphonic/preset_8_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-31 03:24:10.000000 pyphonic-1.1.0/src/pyphonic/preset_9_saturator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:24:21.397197 pyphonic-1.1.0/src/pyphonic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-05-31 03:24:21.000000 pyphonic-1.1.0/src/pyphonic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-31 03:24:21.000000 pyphonic-1.1.0/src/pyphonic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 03:24:21.000000 pyphonic-1.1.0/src/pyphonic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 03:24:21.000000 pyphonic-1.1.0/src/pyphonic.egg-info/top_level.txt
```

### Comparing `pyphonic-1.0.2/PKG-INFO` & `pyphonic-1.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,64 +1,65 @@
 Metadata-Version: 2.1
 Name: pyphonic
-Version: 1.0.2
+Version: 1.1.0
 Summary: Make a VST plugin for your DAW using Python
 Author-email: AudioFluff <tom@audiofluff.com>, Tom Grek <tom.grek@gmail.com>
 Project-URL: Homepage, https://github.com/audiofluff/pyphonic
 Project-URL: Issues, https://github.com/audiofluff/pyphonic/issues
-Classifier: License :: Free for non-commercial use
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Artistic Software
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: MIDI
 Classifier: Topic :: Multimedia :: Sound/Audio :: Sound Synthesis
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Pyphonic
 
-![Publish workflow](https://github.com/tomgrek/pyphonic/actions/workflows/python-publish.yml/badge.svg) ![Docs workflow](https://github.com/tomgrek/pyphonic/actions/workflows/pages-publish.yml/badge.svg) 
+![Publish workflow](https://github.com/AudioFluff/PyPhonic/actions/workflows/python-publish.yml/badge.svg) ![Docs workflow](https://github.com/AudioFluff/PyPhonic/actions/workflows/pages-publish.yml/badge.svg) 
 
 This is the Python library for the Pyphonic VST plugin.
 
 ![Plugin screenshot](docs/plugin_standalone.png)
 
-Docs: https://tomgrek.github.io/pyphonic/
+Docs: https://audiofluff.github.io/PyPhonic/
 
 The VST streams audio and midi to some server; the server responds with some processed audio.
 
 This library is (one implementation of) the server component.
 
 ## Where do I get the VST?
 
-The VST is not yet released. It's in the final stages of development with release expected in May 2024; you can sign up at https://audiofluff.com to get notified when it's released.
+The VST is not yet released. It's in the final stages of development with release _definitely happening_ in June 2024; you can sign up at https://audiofluff.com to get notified when it's released.
 
 ## Quickstart
 
 ##### Super Quick Demo
 
 ```bash
-python -c "import pyphonic; from pyphonic.demo import process;  pyphonic.start(process, 8020)"
+python -c "import pyphonic; from pyphonic.preset_11_polysynth import process;  pyphonic.start(process, 8020)"
 ```
 
 An example using NumPy (recommended over basic Python):
 
 ```bash
-python -c "import pyphonic; from pyphonic.sampler import process_npy;  pyphonic.start(process_npy, 8020)"
+python -c "import pyphonic; from pyphonic.preset_7_sampler import process_npy;  pyphonic.start(process_npy, 8020)"
 ```
 
 An example using PyTorch:
 
 ```bash
-python -c "import pyphonic; from pyphonic.torch_saturator import process_torch;  pyphonic.start(process_torch, 8020)"
+python -c "import pyphonic; from pyphonic.preset_9_saturator import process_torch;  pyphonic.start(process_torch, 8020)"
 
 ```
 
-Enter `127.0.0.1:8020` in the VST and you'll hear synthesized tones for each MIDI note you press.
+Enter `127.0.0.1:8020` in the VST. Preset 11 sends notes in response to MIDI; preset 7 plays a sample in response to MIDI; preset 9 adds saturation to incoming audio.
 
 ##### Here's an example that simply echoes back the audio received from the server:
 
 ```python
 import pyphonic
 
 def process(midi, audio):
@@ -81,51 +82,74 @@
         return midi, [[x * 1.1 for x in left], [x * 1.1 for x in right]]
     return midi, [[0.0 for _ in left], [0.0 for _ in right]]
 
 PORT = 8020
 pyphonic.start(process, PORT)
 ```
 
+##### Here's an example of NumPy
+
+```python
+import pyphonic
+
+def process_npy(midi, audio):
+    return [], audio * 0.5
+
+PORT = 8020
+pyphonic.start(process_npy, PORT)
+```
+
 ## Next Steps
 
 YMMV with network audio, particularly if you're running this server on a different computer than the VST.
 
 That's why the Pyphonic VST also provides the ability to then take the **exact same Python code** and run it _within the VST_. In other words, the remote setup is great for POC and debugging, the next step is to run it in the VST itself. (Optional third step is then to translate the Python code to C++ but that's on you).
 
 Remotely, you can use any third party Python lib installed in your environment (e.g. `PyTorch`). In the VST, currently, `numpy`, `scipy`, `torch` and `librosa` (which includes `numba` and `scikit-learn`) are offered.
 
 ## Docs
 
 ## Included Demos
 
-1. `pyphonic.demo` - a simple polyphonic sine wave synth
-2. `pyphonic.arp` - a beat sync'd minor triad MIDI arpeggiator
-3. `pyphonic.butterworth` - a configurable high/low/bandpass filter
-4. `pyphonic.sampler` - a wavetable synth or "ROMpler", demonstrating pitch shifting
-5. `pyphonic.stretcher` - a time stretching wavetable synth
-6. `pyphonic.torch_noise` - to be charitable, it adds a vinyl crackle or tape hiss to the audio
-7. `pyphonic.torch_saturator` - a saturator/distortion effect, nice warmth on EDM drums
-8. (TODO) `pyphonic.reverb` - a reverb effect
-9. (TODO) `pyphonic.delay` - a beat sync'd delay effect
-10. (TODO) `pyphonic.pitcher` - a realtime pitch shift and time stretch effect for audio
-11. (TODO) `pyphonic.deverb` - A deep learning model trained to remove reverb
-12. (TODO) `pyphonic.source_separation` - A [deep learning model](https://pytorch.org/audio/stable/tutorials/hybrid_demucs_tutorial.html#sphx-glr-tutorials-hybrid-demucs-tutorial-py) trained to separate music into drums, bass, vocals and other
+Note: You will need to look at these files to see if they have a `process`, `process_npy` or `process_torch` function and use it accordingly.
+
+4. `pyphonic.preset_4_butterworth` - a configurable high/low/bandpass filter
+5. `pyphonic.preset_5_midiarp` - a beat sync'd minor triad MIDI arpeggiator
+6. `pyphonic.preset_6_wavetable` - a wavetable synth or "ROMpler", demonstrating pitch shifting
+7. `pyphonic.preset_7_sampler` - a time stretching wavetable synth
+8. `pyphonic.preset_8_noise` - to be charitable, it adds a vinyl crackle or tape hiss to the audio
+9. `pyphonic.preset_9_saturator` - a saturator/distortion effect, nice warmth on EDM drums; also has an electric guitar setting
+10. `pyphonic.preset_10_fftramp` - Ramped FFT-based filtering, interesting effect.
+11. `pyphonic.preset_11_polysynth` - a simple polyphonic sine wave synth
+12. `pyphonic.preset_12_syncdnoise` - beat sync'd noise showing how to get transport info. Can add fizz after a kick.
+13. `pyphonic.preset_13_sccompressor` - fake sidechain compressor, ducking the audio on the kick
+14. `pyphonic.preset_14_nn_voice_change` - uses the SpeechT5 model and HifiGAN vocoder to transform one voice (vocal) to sound like a different speaker. Needs Huggingface and CUDA.
+15. `pyphonic.preset_15_gen_midi` - generates a new MIDI chord every 2 bars with a configurable root note but based on the familiar C, G, Am, F progression. Markovian. DAW must be playing/recording for it to work.
+16. (TODO) `pyphonic.reverb` - a reverb effect
+17. (TODO) `pyphonic.delay` - a beat sync'd delay effect
+18. (TODO) `pyphonic.pitcher` - a realtime pitch shift and time stretch effect for audio
+19. (TODO) `pyphonic.deverb` - A deep learning model trained to remove reverb
+20. (TODO) `pyphonic.source_separation` - A [deep learning model](https://pytorch.org/audio/stable/tutorials/hybrid_demucs_tutorial.html#sphx-glr-tutorials-hybrid-demucs-tutorial-py) trained to separate music into drums, bass, vocals and other
 
 ## Status
 
-The VST is fully functional, rarely crashes, and stays quite performant even under heavy load. Before releasing it (hopefully to the KVR community), I need to 1. make a few more presets that push performance boundaries and check edge cases - dogfooding, basically - 2. write more docs and 3. make a Windows installer. A Mac installer will follow (and Linux if there's interest).
+The VST is fully functional, hardly ever crashes the DAW, and stays quite performant even under heavy load.
 
-As at early May 2024 I reckon this should be this month.
+As at late May 2024 the release will firmly be in June 2024. Just a few scary things to do like forming an LLC.
 
 ## Development
 
 Contributions welcome!
 
 In particular, the VST plugin automatically pulls `presets.json` and uses that to populate the presets dropdown. If you come up with a great preset and want to share it, please consider making a pull request.
 
+## License
+
+This Python package is licensed under the MIT license. The VST plugin is under separate license.
+
 ### How to add to presets.json
 
 ```
 import json
 f = open('my_python_file.py').read()
 json.dump(f, open("ready_to_copy_paste_into_presets.json", "w"))
 ```
```

### Comparing `pyphonic-1.0.2/README.md` & `pyphonic-1.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 # Pyphonic
 
-![Publish workflow](https://github.com/tomgrek/pyphonic/actions/workflows/python-publish.yml/badge.svg) ![Docs workflow](https://github.com/tomgrek/pyphonic/actions/workflows/pages-publish.yml/badge.svg) 
+![Publish workflow](https://github.com/AudioFluff/PyPhonic/actions/workflows/python-publish.yml/badge.svg) ![Docs workflow](https://github.com/AudioFluff/PyPhonic/actions/workflows/pages-publish.yml/badge.svg) 
 
 This is the Python library for the Pyphonic VST plugin.
 
 ![Plugin screenshot](docs/plugin_standalone.png)
 
-Docs: https://tomgrek.github.io/pyphonic/
+Docs: https://audiofluff.github.io/PyPhonic/
 
 The VST streams audio and midi to some server; the server responds with some processed audio.
 
 This library is (one implementation of) the server component.
 
 ## Where do I get the VST?
 
-The VST is not yet released. It's in the final stages of development with release expected in May 2024; you can sign up at https://audiofluff.com to get notified when it's released.
+The VST is not yet released. It's in the final stages of development with release _definitely happening_ in June 2024; you can sign up at https://audiofluff.com to get notified when it's released.
 
 ## Quickstart
 
 ##### Super Quick Demo
 
 ```bash
-python -c "import pyphonic; from pyphonic.demo import process;  pyphonic.start(process, 8020)"
+python -c "import pyphonic; from pyphonic.preset_11_polysynth import process;  pyphonic.start(process, 8020)"
 ```
 
 An example using NumPy (recommended over basic Python):
 
 ```bash
-python -c "import pyphonic; from pyphonic.sampler import process_npy;  pyphonic.start(process_npy, 8020)"
+python -c "import pyphonic; from pyphonic.preset_7_sampler import process_npy;  pyphonic.start(process_npy, 8020)"
 ```
 
 An example using PyTorch:
 
 ```bash
-python -c "import pyphonic; from pyphonic.torch_saturator import process_torch;  pyphonic.start(process_torch, 8020)"
+python -c "import pyphonic; from pyphonic.preset_9_saturator import process_torch;  pyphonic.start(process_torch, 8020)"
 
 ```
 
-Enter `127.0.0.1:8020` in the VST and you'll hear synthesized tones for each MIDI note you press.
+Enter `127.0.0.1:8020` in the VST. Preset 11 sends notes in response to MIDI; preset 7 plays a sample in response to MIDI; preset 9 adds saturation to incoming audio.
 
 ##### Here's an example that simply echoes back the audio received from the server:
 
 ```python
 import pyphonic
 
 def process(midi, audio):
@@ -64,51 +64,74 @@
         return midi, [[x * 1.1 for x in left], [x * 1.1 for x in right]]
     return midi, [[0.0 for _ in left], [0.0 for _ in right]]
 
 PORT = 8020
 pyphonic.start(process, PORT)
 ```
 
+##### Here's an example of NumPy
+
+```python
+import pyphonic
+
+def process_npy(midi, audio):
+    return [], audio * 0.5
+
+PORT = 8020
+pyphonic.start(process_npy, PORT)
+```
+
 ## Next Steps
 
 YMMV with network audio, particularly if you're running this server on a different computer than the VST.
 
 That's why the Pyphonic VST also provides the ability to then take the **exact same Python code** and run it _within the VST_. In other words, the remote setup is great for POC and debugging, the next step is to run it in the VST itself. (Optional third step is then to translate the Python code to C++ but that's on you).
 
 Remotely, you can use any third party Python lib installed in your environment (e.g. `PyTorch`). In the VST, currently, `numpy`, `scipy`, `torch` and `librosa` (which includes `numba` and `scikit-learn`) are offered.
 
 ## Docs
 
 ## Included Demos
 
-1. `pyphonic.demo` - a simple polyphonic sine wave synth
-2. `pyphonic.arp` - a beat sync'd minor triad MIDI arpeggiator
-3. `pyphonic.butterworth` - a configurable high/low/bandpass filter
-4. `pyphonic.sampler` - a wavetable synth or "ROMpler", demonstrating pitch shifting
-5. `pyphonic.stretcher` - a time stretching wavetable synth
-6. `pyphonic.torch_noise` - to be charitable, it adds a vinyl crackle or tape hiss to the audio
-7. `pyphonic.torch_saturator` - a saturator/distortion effect, nice warmth on EDM drums
-8. (TODO) `pyphonic.reverb` - a reverb effect
-9. (TODO) `pyphonic.delay` - a beat sync'd delay effect
-10. (TODO) `pyphonic.pitcher` - a realtime pitch shift and time stretch effect for audio
-11. (TODO) `pyphonic.deverb` - A deep learning model trained to remove reverb
-12. (TODO) `pyphonic.source_separation` - A [deep learning model](https://pytorch.org/audio/stable/tutorials/hybrid_demucs_tutorial.html#sphx-glr-tutorials-hybrid-demucs-tutorial-py) trained to separate music into drums, bass, vocals and other
+Note: You will need to look at these files to see if they have a `process`, `process_npy` or `process_torch` function and use it accordingly.
+
+4. `pyphonic.preset_4_butterworth` - a configurable high/low/bandpass filter
+5. `pyphonic.preset_5_midiarp` - a beat sync'd minor triad MIDI arpeggiator
+6. `pyphonic.preset_6_wavetable` - a wavetable synth or "ROMpler", demonstrating pitch shifting
+7. `pyphonic.preset_7_sampler` - a time stretching wavetable synth
+8. `pyphonic.preset_8_noise` - to be charitable, it adds a vinyl crackle or tape hiss to the audio
+9. `pyphonic.preset_9_saturator` - a saturator/distortion effect, nice warmth on EDM drums; also has an electric guitar setting
+10. `pyphonic.preset_10_fftramp` - Ramped FFT-based filtering, interesting effect.
+11. `pyphonic.preset_11_polysynth` - a simple polyphonic sine wave synth
+12. `pyphonic.preset_12_syncdnoise` - beat sync'd noise showing how to get transport info. Can add fizz after a kick.
+13. `pyphonic.preset_13_sccompressor` - fake sidechain compressor, ducking the audio on the kick
+14. `pyphonic.preset_14_nn_voice_change` - uses the SpeechT5 model and HifiGAN vocoder to transform one voice (vocal) to sound like a different speaker. Needs Huggingface and CUDA.
+15. `pyphonic.preset_15_gen_midi` - generates a new MIDI chord every 2 bars with a configurable root note but based on the familiar C, G, Am, F progression. Markovian. DAW must be playing/recording for it to work.
+16. (TODO) `pyphonic.reverb` - a reverb effect
+17. (TODO) `pyphonic.delay` - a beat sync'd delay effect
+18. (TODO) `pyphonic.pitcher` - a realtime pitch shift and time stretch effect for audio
+19. (TODO) `pyphonic.deverb` - A deep learning model trained to remove reverb
+20. (TODO) `pyphonic.source_separation` - A [deep learning model](https://pytorch.org/audio/stable/tutorials/hybrid_demucs_tutorial.html#sphx-glr-tutorials-hybrid-demucs-tutorial-py) trained to separate music into drums, bass, vocals and other
 
 ## Status
 
-The VST is fully functional, rarely crashes, and stays quite performant even under heavy load. Before releasing it (hopefully to the KVR community), I need to 1. make a few more presets that push performance boundaries and check edge cases - dogfooding, basically - 2. write more docs and 3. make a Windows installer. A Mac installer will follow (and Linux if there's interest).
+The VST is fully functional, hardly ever crashes the DAW, and stays quite performant even under heavy load.
 
-As at early May 2024 I reckon this should be this month.
+As at late May 2024 the release will firmly be in June 2024. Just a few scary things to do like forming an LLC.
 
 ## Development
 
 Contributions welcome!
 
 In particular, the VST plugin automatically pulls `presets.json` and uses that to populate the presets dropdown. If you come up with a great preset and want to share it, please consider making a pull request.
 
+## License
+
+This Python package is licensed under the MIT license. The VST plugin is under separate license.
+
 ### How to add to presets.json
 
 ```
 import json
 f = open('my_python_file.py').read()
 json.dump(f, open("ready_to_copy_paste_into_presets.json", "w"))
 ```
```

### Comparing `pyphonic-1.0.2/pyproject.toml` & `pyphonic-1.1.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -3,24 +3,24 @@
     "setuptools>=61.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyphonic"
-version = "1.0.2"
+version = "1.1.0"
 authors = [
   { name="AudioFluff", email="tom@audiofluff.com" },
   { name="Tom Grek", email="tom.grek@gmail.com" },
 ]
 description = "Make a VST plugin for your DAW using Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
-    'License :: Free for non-commercial use',
+    'License :: OSI Approved :: MIT License',
     'Topic :: Artistic Software',
     'Topic :: Multimedia :: Sound/Audio',
     'Topic :: Multimedia :: Sound/Audio :: MIDI',
     'Topic :: Multimedia :: Sound/Audio :: Sound Synthesis',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'Programming Language :: Python :: 3'
 ]
```

### Comparing `pyphonic-1.0.2/src/pyphonic/10_fftramp.py` & `pyphonic-1.1.0/src/pyphonic/preset_10_fftramp.py`

 * *Files identical despite different names*

### Comparing `pyphonic-1.0.2/src/pyphonic/11_polysynth.py` & `pyphonic-1.1.0/src/pyphonic/preset_11_polysynth.py`

 * *Files identical despite different names*

### Comparing `pyphonic-1.0.2/src/pyphonic/4_butterworth.py` & `pyphonic-1.1.0/src/pyphonic/preset_4_butterworth.py`

 * *Files identical despite different names*

### Comparing `pyphonic-1.0.2/src/pyphonic/5_midiarp.py` & `pyphonic-1.1.0/src/pyphonic/preset_5_midiarp.py`

 * *Files identical despite different names*

### Comparing `pyphonic-1.0.2/src/pyphonic/6_wavetable.py` & `pyphonic-1.1.0/src/pyphonic/preset_6_wavetable.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                 voices[msg.note]["playing"] = True
             voices[msg.note]["velocity"] = msg.velocity
         elif msg.type == "note_off":
             voices[msg.note]["position"] = 0
             voices[msg.note]["playing"] = False
             # Could add some tail off instead of dead stop
     
-    new_audio = np.zeros((num_channels, num_samples))
+    new_audio = np.zeros((num_channels, num_samples), dtype=np.float32)
 
     for voice, data in voices.items():
         if not data["playing"]:
             continue
         start_pos = data["position"] % data["wave"].shape[1]
         end_pos = (start_pos + num_samples)
         if end_pos >= data["wave"].shape[1]:
```

### Comparing `pyphonic-1.0.2/src/pyphonic/7_sampler.py` & `pyphonic-1.1.0/src/pyphonic/preset_7_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             else:
                 voices[msg.note]["playing"] = True
             voices[msg.note]["velocity"] = msg.velocity
         elif msg.type == "note_off":
             voices[msg.note]["position"] = 0
             voices[msg.note]["playing"] = False
     
-    new_audio = np.zeros((num_samples, num_channels))
+    new_audio = np.zeros((num_samples, num_channels), dtype=np.float32)
 
     for voice, data in voices.items():
         if not data["playing"]:
             continue
         start_pos = data["position"] % data["wave"].shape[1]
         end_pos = (start_pos + num_samples)
         if end_pos >= data["wave"].shape[1]:
```

### Comparing `pyphonic-1.0.2/src/pyphonic/9_saturator.py` & `pyphonic-1.1.0/src/pyphonic/preset_9_saturator.py`

 * *Files identical despite different names*

### Comparing `pyphonic-1.0.2/src/pyphonic/__init__.py` & `pyphonic-1.1.0/src/pyphonic/__init__.py`

 * *Files identical despite different names*

### Comparing `pyphonic-1.0.2/src/pyphonic/circular_buffer_overlap.py` & `pyphonic-1.1.0/src/pyphonic/circular_buffer_overlap.py`

 * *Files identical despite different names*

### Comparing `pyphonic-1.0.2/src/pyphonic/flipper.py` & `pyphonic-1.1.0/src/pyphonic/flipper.py`

 * *Files identical despite different names*

### Comparing `pyphonic-1.0.2/src/pyphonic/functions.py` & `pyphonic-1.1.0/src/pyphonic/functions.py`

 * *Files identical despite different names*

### Comparing `pyphonic-1.0.2/src/pyphonic/midi_parser.py` & `pyphonic-1.1.0/src/pyphonic/midi_parser.py`

 * *Files identical despite different names*

### Comparing `pyphonic-1.0.2/src/pyphonic.egg-info/PKG-INFO` & `pyphonic-1.1.0/src/pyphonic.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,64 +1,65 @@
 Metadata-Version: 2.1
 Name: pyphonic
-Version: 1.0.2
+Version: 1.1.0
 Summary: Make a VST plugin for your DAW using Python
 Author-email: AudioFluff <tom@audiofluff.com>, Tom Grek <tom.grek@gmail.com>
 Project-URL: Homepage, https://github.com/audiofluff/pyphonic
 Project-URL: Issues, https://github.com/audiofluff/pyphonic/issues
-Classifier: License :: Free for non-commercial use
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Artistic Software
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: MIDI
 Classifier: Topic :: Multimedia :: Sound/Audio :: Sound Synthesis
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Pyphonic
 
-![Publish workflow](https://github.com/tomgrek/pyphonic/actions/workflows/python-publish.yml/badge.svg) ![Docs workflow](https://github.com/tomgrek/pyphonic/actions/workflows/pages-publish.yml/badge.svg) 
+![Publish workflow](https://github.com/AudioFluff/PyPhonic/actions/workflows/python-publish.yml/badge.svg) ![Docs workflow](https://github.com/AudioFluff/PyPhonic/actions/workflows/pages-publish.yml/badge.svg) 
 
 This is the Python library for the Pyphonic VST plugin.
 
 ![Plugin screenshot](docs/plugin_standalone.png)
 
-Docs: https://tomgrek.github.io/pyphonic/
+Docs: https://audiofluff.github.io/PyPhonic/
 
 The VST streams audio and midi to some server; the server responds with some processed audio.
 
 This library is (one implementation of) the server component.
 
 ## Where do I get the VST?
 
-The VST is not yet released. It's in the final stages of development with release expected in May 2024; you can sign up at https://audiofluff.com to get notified when it's released.
+The VST is not yet released. It's in the final stages of development with release _definitely happening_ in June 2024; you can sign up at https://audiofluff.com to get notified when it's released.
 
 ## Quickstart
 
 ##### Super Quick Demo
 
 ```bash
-python -c "import pyphonic; from pyphonic.demo import process;  pyphonic.start(process, 8020)"
+python -c "import pyphonic; from pyphonic.preset_11_polysynth import process;  pyphonic.start(process, 8020)"
 ```
 
 An example using NumPy (recommended over basic Python):
 
 ```bash
-python -c "import pyphonic; from pyphonic.sampler import process_npy;  pyphonic.start(process_npy, 8020)"
+python -c "import pyphonic; from pyphonic.preset_7_sampler import process_npy;  pyphonic.start(process_npy, 8020)"
 ```
 
 An example using PyTorch:
 
 ```bash
-python -c "import pyphonic; from pyphonic.torch_saturator import process_torch;  pyphonic.start(process_torch, 8020)"
+python -c "import pyphonic; from pyphonic.preset_9_saturator import process_torch;  pyphonic.start(process_torch, 8020)"
 
 ```
 
-Enter `127.0.0.1:8020` in the VST and you'll hear synthesized tones for each MIDI note you press.
+Enter `127.0.0.1:8020` in the VST. Preset 11 sends notes in response to MIDI; preset 7 plays a sample in response to MIDI; preset 9 adds saturation to incoming audio.
 
 ##### Here's an example that simply echoes back the audio received from the server:
 
 ```python
 import pyphonic
 
 def process(midi, audio):
@@ -81,51 +82,74 @@
         return midi, [[x * 1.1 for x in left], [x * 1.1 for x in right]]
     return midi, [[0.0 for _ in left], [0.0 for _ in right]]
 
 PORT = 8020
 pyphonic.start(process, PORT)
 ```
 
+##### Here's an example of NumPy
+
+```python
+import pyphonic
+
+def process_npy(midi, audio):
+    return [], audio * 0.5
+
+PORT = 8020
+pyphonic.start(process_npy, PORT)
+```
+
 ## Next Steps
 
 YMMV with network audio, particularly if you're running this server on a different computer than the VST.
 
 That's why the Pyphonic VST also provides the ability to then take the **exact same Python code** and run it _within the VST_. In other words, the remote setup is great for POC and debugging, the next step is to run it in the VST itself. (Optional third step is then to translate the Python code to C++ but that's on you).
 
 Remotely, you can use any third party Python lib installed in your environment (e.g. `PyTorch`). In the VST, currently, `numpy`, `scipy`, `torch` and `librosa` (which includes `numba` and `scikit-learn`) are offered.
 
 ## Docs
 
 ## Included Demos
 
-1. `pyphonic.demo` - a simple polyphonic sine wave synth
-2. `pyphonic.arp` - a beat sync'd minor triad MIDI arpeggiator
-3. `pyphonic.butterworth` - a configurable high/low/bandpass filter
-4. `pyphonic.sampler` - a wavetable synth or "ROMpler", demonstrating pitch shifting
-5. `pyphonic.stretcher` - a time stretching wavetable synth
-6. `pyphonic.torch_noise` - to be charitable, it adds a vinyl crackle or tape hiss to the audio
-7. `pyphonic.torch_saturator` - a saturator/distortion effect, nice warmth on EDM drums
-8. (TODO) `pyphonic.reverb` - a reverb effect
-9. (TODO) `pyphonic.delay` - a beat sync'd delay effect
-10. (TODO) `pyphonic.pitcher` - a realtime pitch shift and time stretch effect for audio
-11. (TODO) `pyphonic.deverb` - A deep learning model trained to remove reverb
-12. (TODO) `pyphonic.source_separation` - A [deep learning model](https://pytorch.org/audio/stable/tutorials/hybrid_demucs_tutorial.html#sphx-glr-tutorials-hybrid-demucs-tutorial-py) trained to separate music into drums, bass, vocals and other
+Note: You will need to look at these files to see if they have a `process`, `process_npy` or `process_torch` function and use it accordingly.
+
+4. `pyphonic.preset_4_butterworth` - a configurable high/low/bandpass filter
+5. `pyphonic.preset_5_midiarp` - a beat sync'd minor triad MIDI arpeggiator
+6. `pyphonic.preset_6_wavetable` - a wavetable synth or "ROMpler", demonstrating pitch shifting
+7. `pyphonic.preset_7_sampler` - a time stretching wavetable synth
+8. `pyphonic.preset_8_noise` - to be charitable, it adds a vinyl crackle or tape hiss to the audio
+9. `pyphonic.preset_9_saturator` - a saturator/distortion effect, nice warmth on EDM drums; also has an electric guitar setting
+10. `pyphonic.preset_10_fftramp` - Ramped FFT-based filtering, interesting effect.
+11. `pyphonic.preset_11_polysynth` - a simple polyphonic sine wave synth
+12. `pyphonic.preset_12_syncdnoise` - beat sync'd noise showing how to get transport info. Can add fizz after a kick.
+13. `pyphonic.preset_13_sccompressor` - fake sidechain compressor, ducking the audio on the kick
+14. `pyphonic.preset_14_nn_voice_change` - uses the SpeechT5 model and HifiGAN vocoder to transform one voice (vocal) to sound like a different speaker. Needs Huggingface and CUDA.
+15. `pyphonic.preset_15_gen_midi` - generates a new MIDI chord every 2 bars with a configurable root note but based on the familiar C, G, Am, F progression. Markovian. DAW must be playing/recording for it to work.
+16. (TODO) `pyphonic.reverb` - a reverb effect
+17. (TODO) `pyphonic.delay` - a beat sync'd delay effect
+18. (TODO) `pyphonic.pitcher` - a realtime pitch shift and time stretch effect for audio
+19. (TODO) `pyphonic.deverb` - A deep learning model trained to remove reverb
+20. (TODO) `pyphonic.source_separation` - A [deep learning model](https://pytorch.org/audio/stable/tutorials/hybrid_demucs_tutorial.html#sphx-glr-tutorials-hybrid-demucs-tutorial-py) trained to separate music into drums, bass, vocals and other
 
 ## Status
 
-The VST is fully functional, rarely crashes, and stays quite performant even under heavy load. Before releasing it (hopefully to the KVR community), I need to 1. make a few more presets that push performance boundaries and check edge cases - dogfooding, basically - 2. write more docs and 3. make a Windows installer. A Mac installer will follow (and Linux if there's interest).
+The VST is fully functional, hardly ever crashes the DAW, and stays quite performant even under heavy load.
 
-As at early May 2024 I reckon this should be this month.
+As at late May 2024 the release will firmly be in June 2024. Just a few scary things to do like forming an LLC.
 
 ## Development
 
 Contributions welcome!
 
 In particular, the VST plugin automatically pulls `presets.json` and uses that to populate the presets dropdown. If you come up with a great preset and want to share it, please consider making a pull request.
 
+## License
+
+This Python package is licensed under the MIT license. The VST plugin is under separate license.
+
 ### How to add to presets.json
 
 ```
 import json
 f = open('my_python_file.py').read()
 json.dump(f, open("ready_to_copy_paste_into_presets.json", "w"))
 ```
```

### Comparing `pyphonic-1.0.2/src/pyphonic.egg-info/SOURCES.txt` & `pyphonic-1.1.0/src/pyphonic.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+LICENSE
 README.md
 pyproject.toml
-src/pyphonic/10_fftramp.py
-src/pyphonic/11_polysynth.py
-src/pyphonic/12_syncdnoise.py
-src/pyphonic/13_sccompressor.py
-src/pyphonic/4_butterworth.py
-src/pyphonic/5_midiarp.py
-src/pyphonic/6_wavetable.py
-src/pyphonic/7_sampler.py
-src/pyphonic/8_noise.py
-src/pyphonic/9_saturator.py
 src/pyphonic/__init__.py
 src/pyphonic/circular_buffer_overlap.py
 src/pyphonic/flipper.py
 src/pyphonic/functions.py
 src/pyphonic/midi_parser.py
-src/pyphonic/midirando.py
 src/pyphonic/multithreaded_noise.py
+src/pyphonic/preset_10_fftramp.py
+src/pyphonic/preset_11_polysynth.py
+src/pyphonic/preset_12_syncdnoise.py
+src/pyphonic/preset_13_sccompressor.py
+src/pyphonic/preset_14_nn_voice_change.py
+src/pyphonic/preset_15_gen_midi.py
+src/pyphonic/preset_4_butterworth.py
+src/pyphonic/preset_5_midiarp.py
+src/pyphonic/preset_6_wavetable.py
+src/pyphonic/preset_7_sampler.py
+src/pyphonic/preset_8_noise.py
+src/pyphonic/preset_9_saturator.py
 src/pyphonic.egg-info/PKG-INFO
 src/pyphonic.egg-info/SOURCES.txt
 src/pyphonic.egg-info/dependency_links.txt
 src/pyphonic.egg-info/top_level.txt
```

