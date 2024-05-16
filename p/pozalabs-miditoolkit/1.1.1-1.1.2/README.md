# Comparing `tmp/pozalabs-miditoolkit-1.1.1.tar.gz` & `tmp/pozalabs-miditoolkit-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pozalabs-miditoolkit-1.1.1.tar", max compression
+gzip compressed data, was "pozalabs-miditoolkit-1.1.2.tar", max compression
```

## Comparing `pozalabs-miditoolkit-1.1.1.tar` & `pozalabs-miditoolkit-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1101 2024-04-12 07:25:11.576871 pozalabs-miditoolkit-1.1.1/LICENSE
--rw-r--r--   0        0        0     3859 2024-04-12 07:25:11.576871 pozalabs-miditoolkit-1.1.1/README.md
--rwxr-xr-x   0        0        0      547 2024-04-12 07:25:11.576871 pozalabs-miditoolkit-1.1.1/miditoolkit/__init__.py
--rw-r--r--   0        0        0      344 2024-04-12 07:25:11.576871 pozalabs-miditoolkit-1.1.1/miditoolkit/constants.py
--rwxr-xr-x   0        0        0        0 2024-04-12 07:25:11.576871 pozalabs-miditoolkit-1.1.1/miditoolkit/midi/__init__.py
--rwxr-xr-x   0        0        0     9805 2024-04-12 07:25:11.576871 pozalabs-miditoolkit-1.1.1/miditoolkit/midi/containers.py
--rwxr-xr-x   0        0        0    28871 2024-04-12 07:25:11.576871 pozalabs-miditoolkit-1.1.1/miditoolkit/midi/parser.py
--rwxr-xr-x   0        0        0      140 2024-04-12 07:25:11.576871 pozalabs-miditoolkit-1.1.1/miditoolkit/pianoroll/__init__.py
--rwxr-xr-x   0        0        0     6838 2024-04-12 07:25:11.576871 pozalabs-miditoolkit-1.1.1/miditoolkit/pianoroll/parser.py
--rwxr-xr-x   0        0        0      704 2024-04-12 07:25:11.576871 pozalabs-miditoolkit-1.1.1/miditoolkit/pianoroll/utils.py
--rw-r--r--   0        0        0    12688 2024-04-12 07:25:11.576871 pozalabs-miditoolkit-1.1.1/miditoolkit/pianoroll/vis.py
--rw-r--r--   0        0        0     1439 2024-04-12 07:25:11.580870 pozalabs-miditoolkit-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     4714 1970-01-01 00:00:00.000000 pozalabs-miditoolkit-1.1.1/setup.py
--rw-r--r--   0        0        0     4821 1970-01-01 00:00:00.000000 pozalabs-miditoolkit-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1101 2024-04-15 10:38:25.901056 pozalabs-miditoolkit-1.1.2/LICENSE
+-rw-r--r--   0        0        0     3859 2024-04-15 10:38:25.901056 pozalabs-miditoolkit-1.1.2/README.md
+-rwxr-xr-x   0        0        0      547 2024-04-15 10:38:25.901056 pozalabs-miditoolkit-1.1.2/miditoolkit/__init__.py
+-rw-r--r--   0        0        0      344 2024-04-15 10:38:25.901056 pozalabs-miditoolkit-1.1.2/miditoolkit/constants.py
+-rwxr-xr-x   0        0        0        0 2024-04-15 10:38:25.901056 pozalabs-miditoolkit-1.1.2/miditoolkit/midi/__init__.py
+-rwxr-xr-x   0        0        0     9805 2024-04-15 10:38:25.901056 pozalabs-miditoolkit-1.1.2/miditoolkit/midi/containers.py
+-rwxr-xr-x   0        0        0    28883 2024-04-15 10:38:25.901056 pozalabs-miditoolkit-1.1.2/miditoolkit/midi/parser.py
+-rwxr-xr-x   0        0        0      140 2024-04-15 10:38:25.901056 pozalabs-miditoolkit-1.1.2/miditoolkit/pianoroll/__init__.py
+-rwxr-xr-x   0        0        0     6838 2024-04-15 10:38:25.901056 pozalabs-miditoolkit-1.1.2/miditoolkit/pianoroll/parser.py
+-rwxr-xr-x   0        0        0      704 2024-04-15 10:38:25.901056 pozalabs-miditoolkit-1.1.2/miditoolkit/pianoroll/utils.py
+-rw-r--r--   0        0        0    12688 2024-04-15 10:38:25.901056 pozalabs-miditoolkit-1.1.2/miditoolkit/pianoroll/vis.py
+-rw-r--r--   0        0        0     1439 2024-04-15 10:38:25.901056 pozalabs-miditoolkit-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4714 1970-01-01 00:00:00.000000 pozalabs-miditoolkit-1.1.2/setup.py
+-rw-r--r--   0        0        0     4821 1970-01-01 00:00:00.000000 pozalabs-miditoolkit-1.1.2/PKG-INFO
```

### Comparing `pozalabs-miditoolkit-1.1.1/LICENSE` & `pozalabs-miditoolkit-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pozalabs-miditoolkit-1.1.1/README.md` & `pozalabs-miditoolkit-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pozalabs-miditoolkit-1.1.1/miditoolkit/__init__.py` & `pozalabs-miditoolkit-1.1.2/miditoolkit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Author: Wen-Yi Hsiao, Taiwan
 """
 
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 
 # Convenience exports for commonly used classes.
 
 from miditoolkit.midi.containers import (
     ControlChange,
     Instrument,
     KeySignature,
```

### Comparing `pozalabs-miditoolkit-1.1.1/miditoolkit/midi/containers.py` & `pozalabs-miditoolkit-1.1.2/miditoolkit/midi/containers.py`

 * *Files identical despite different names*

### Comparing `pozalabs-miditoolkit-1.1.1/miditoolkit/midi/parser.py` & `pozalabs-miditoolkit-1.1.2/miditoolkit/midi/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -510,15 +510,15 @@
             track = mido.MidiTrack()
             # segment-free
             # track name
             if instrument.name:
                 track.append(mido.MetaMessage("track_name", time=0, name=instrument.name))
 
             # Set the program number
-            if instrument.program:
+            if instrument.program is not None:
                 track.append(
                     mido.Message(
                         "program_change",
                         time=0,
                         program=instrument.program,
                     )
                 )
```

### Comparing `pozalabs-miditoolkit-1.1.1/miditoolkit/pianoroll/parser.py` & `pozalabs-miditoolkit-1.1.2/miditoolkit/pianoroll/parser.py`

 * *Files identical despite different names*

### Comparing `pozalabs-miditoolkit-1.1.1/miditoolkit/pianoroll/utils.py` & `pozalabs-miditoolkit-1.1.2/miditoolkit/pianoroll/utils.py`

 * *Files identical despite different names*

### Comparing `pozalabs-miditoolkit-1.1.1/miditoolkit/pianoroll/vis.py` & `pozalabs-miditoolkit-1.1.2/miditoolkit/pianoroll/vis.py`

 * *Files identical despite different names*

### Comparing `pozalabs-miditoolkit-1.1.1/pyproject.toml` & `pozalabs-miditoolkit-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pozalabs-miditoolkit"
 packages = [{ include = "miditoolkit"}]
-version = "1.1.1"
+version = "1.1.2"
 description = "A python package for working with MIDI data files. (POZAlabs forked)"
 authors = ["pozalabs <contact@pozalabs.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = [
     "midi",
     "mir",
```

### Comparing `pozalabs-miditoolkit-1.1.1/setup.py` & `pozalabs-miditoolkit-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.5,<4.0', 'mido>=1.1.16,<2.0.0', 'numpy>=1.19,<2.0']
 
 setup_kwargs = {
     'name': 'pozalabs-miditoolkit',
-    'version': '1.1.1',
+    'version': '1.1.2',
     'description': 'A python package for working with MIDI data files. (POZAlabs forked)',
     'long_description': "# Miditoolkit\n\nA Python package for working with MIDI files.\n\n[![PyPI version fury.io](https://badge.fury.io/py/miditoolkit.svg)](https://pypi.python.org/pypi/miditoolkit/)\n[![Python 3.7](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/)\n[![GitHub CI](https://github.com/YatingMusic/miditoolkit/actions/workflows/pytest.yml/badge.svg)](https://github.com/YatingMusic/miditoolkit/actions/workflows/pytest.yml)\n[![GitHub license](https://img.shields.io/github/license/YatingMusic/miditoolkit.svg)](https://github.com/YatingMusic/miditoolkit/blob/main/LICENSE)\n[![Downloads](https://static.pepy.tech/badge/miditoolkit)](https://pepy.tech/project/miditoolkit)\n[![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\nMiditoolkit works by loading/writing MIDIs with [mido](https://github.com/mido/mido) in a user-friendly way. It is inspired from [pretty_midi](https://github.com/craffel/pretty-midi), with similar usage and core features, but handles the MIDI events in native **[ticks](https://www.recordingblogs.com/wiki/midi-tick)** time unit instead of seconds. It also comes with a few optimizations and speed-ups, and can parse MIDI tracks into **piano-rolls** for computation or visualization purposes.\nIf you are working with seconds time units (for e.g. music transcription), you'll be likely better with pretty_midi. Otherwise, if you are working solely on MIDI and symbolic music, miditoolkit should provide slightly faster performances.\n\n## Main Features\n\n* MIDI\n    * Global\n        * ticks per beat\n        * tempo changes\n        * key signatures\n        * time signatures\n        * lyrics\n        * markers\n    * Instruments\n        * control changes\n        * pitch bend\n    * Editing\n        * chunk/cropping\n    * IO\n        * BytesIO\n* Piano-rolls\n    * Tools\n        * notes to piano-rolls\n        * piano-rolls to notes\n        * chromagram\n    * Visualization\n* External Library\n   * [structure analysis](https://github.com/wayne391/sf_segmenter)\n\n## TODO\n\n* better documentation;\n* finish the code cleaning of the pianoroll methods (vis);\n* a way to switch the time in seconds across the whole MidiFile object;\n* cropping Control Changes and bars;\n* symbolic features\n* new structural analysis\n\n## Installation\n\nYou can install miditoolkit via [PYPI](https://pypi.org/project/miditoolkit/):\n\n```bash\npip install miditoolkit\n```\n\n... or directly from git if you want to get the latest features or fixes (only recommended if you need it):\n\n```bash\npip install git+https://github.com/YatingMusic/miditoolkit\n```\n\n## Example Usage\n\n```python\nfrom miditoolkit import MidiFile\nfrom miditoolkit.midi.utils import example_midi_file\n\npath_midi = example_midi_file()\nmidi_obj = MidiFile(path_midi)\n\nprint(midi_obj)\n```\n\nOutput:\n\n```\nticks per beat: 480\nmax tick: 72002\ntempo changes: 68\ntime sig: 2\nkey sig: 0\nmarkers: 71\nlyrics: False\ninstruments: 2\n```\n\nA. [Parse and create MIDI files](examples/parse_and_create_MIDI_files.ipynb)\nB. [Piano-roll Manipulation](examples/pinoroll_manipulation.ipynb)\n\n## Philosophy\n\n* [mido](https://github.com/mido/mido) processes MIDI files in the lower level such as messages and ports, and is the backend pretty_midi and miditoolkit;\n* [pretty_midi](https://github.com/craffel/pretty-midi) parses MIDI files and pianorolls in seconds time unit, plus has audio related features;\n* [pypianoroll](https://github.com/salu133445/pypianoroll) parses MIDI files into pianorolls in ticks time unit.\n\n**Miditoolkit** is designed for handling MIDI in **[ticks](https://www.recordingblogs.com/wiki/midi-tick)**, the native time unit of the MIDI protocol. We keep the midi parser as simple as possible, and offer several important functions to complete the versatility. For example, piano-rolls, tick-to-second, chromagram, etc.\n",
     'author': 'pozalabs',
     'author_email': 'contact@pozalabs.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pozalabs-miditoolkit-1.1.1/PKG-INFO` & `pozalabs-miditoolkit-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pozalabs-miditoolkit
-Version: 1.1.1
+Version: 1.1.2
 Summary: A python package for working with MIDI data files. (POZAlabs forked)
 License: MIT
 Keywords: midi,mir,music
 Author: pozalabs
 Author-email: contact@pozalabs.com
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
```

