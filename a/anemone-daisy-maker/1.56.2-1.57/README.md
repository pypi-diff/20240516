# Comparing `tmp/anemone_daisy_maker-1.56.2.tar.gz` & `tmp/anemone_daisy_maker-1.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anemone_daisy_maker-1.56.2.tar", last modified: Tue May 14 07:22:51 2024, max compression
+gzip compressed data, was "anemone_daisy_maker-1.57.tar", last modified: Wed May 15 06:56:27 2024, max compression
```

## Comparing `anemone_daisy_maker-1.56.2.tar` & `anemone_daisy_maker-1.57.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-14 07:22:51.620202 anemone_daisy_maker-1.56.2/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    11357 2024-05-14 07:13:31.000000 anemone_daisy_maker-1.56.2/LICENSE
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6928 2024-05-14 07:22:51.616202 anemone_daisy_maker-1.56.2/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-14 07:22:51.616202 anemone_daisy_maker-1.56.2/anemone/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)    75174 2024-05-14 07:22:51.000000 anemone_daisy_maker-1.56.2/anemone/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       33 2024-05-14 07:22:51.000000 anemone_daisy_maker-1.56.2/anemone/__main__.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-14 07:22:51.616202 anemone_daisy_maker-1.56.2/anemone_daisy_maker.egg-info/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6928 2024-05-14 07:22:51.000000 anemone_daisy_maker-1.56.2/anemone_daisy_maker.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      316 2024-05-14 07:22:51.000000 anemone_daisy_maker-1.56.2/anemone_daisy_maker.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-14 07:22:51.000000 anemone_daisy_maker-1.56.2/anemone_daisy_maker.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       54 2024-05-14 07:22:51.000000 anemone_daisy_maker-1.56.2/anemone_daisy_maker.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-14 07:22:51.000000 anemone_daisy_maker-1.56.2/anemone_daisy_maker.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-14 07:22:51.000000 anemone_daisy_maker-1.56.2/anemone_daisy_maker.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       38 2024-05-14 07:22:51.620202 anemone_daisy_maker-1.56.2/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     7078 2024-05-14 07:22:51.000000 anemone_daisy_maker-1.56.2/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-15 06:56:27.347980 anemone_daisy_maker-1.57/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    11357 2024-05-15 06:56:21.000000 anemone_daisy_maker-1.57/LICENSE
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6926 2024-05-15 06:56:27.347980 anemone_daisy_maker-1.57/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-15 06:56:27.347980 anemone_daisy_maker-1.57/anemone/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)    76206 2024-05-15 06:56:27.000000 anemone_daisy_maker-1.57/anemone/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       33 2024-05-15 06:56:27.000000 anemone_daisy_maker-1.57/anemone/__main__.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-15 06:56:27.347980 anemone_daisy_maker-1.57/anemone_daisy_maker.egg-info/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6926 2024-05-15 06:56:27.000000 anemone_daisy_maker-1.57/anemone_daisy_maker.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      316 2024-05-15 06:56:27.000000 anemone_daisy_maker-1.57/anemone_daisy_maker.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-15 06:56:27.000000 anemone_daisy_maker-1.57/anemone_daisy_maker.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       54 2024-05-15 06:56:27.000000 anemone_daisy_maker-1.57/anemone_daisy_maker.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-15 06:56:27.000000 anemone_daisy_maker-1.57/anemone_daisy_maker.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-15 06:56:27.000000 anemone_daisy_maker-1.57/anemone_daisy_maker.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       38 2024-05-15 06:56:27.347980 anemone_daisy_maker-1.57/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     7076 2024-05-15 06:56:27.000000 anemone_daisy_maker-1.57/setup.py
```

### Comparing `anemone_daisy_maker-1.56.2/LICENSE` & `anemone_daisy_maker-1.57/LICENSE`

 * *Files identical despite different names*

### Comparing `anemone_daisy_maker-1.56.2/PKG-INFO` & `anemone_daisy_maker-1.57/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anemone_daisy_maker
-Version: 1.56.2
+Version: 1.57
 Summary: Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data
 Home-page: http://ssb22.user.srcf.net/indexer/anemone.html
 Author: Silas S. Brown
 Author-email: ssb22@cam.ac.uk
 License: Apache 2
 Platform: all
 Classifier: Programming Language :: Python :: 3
```

### Comparing `anemone_daisy_maker-1.56.2/anemone/__init__.py` & `anemone_daisy_maker-1.57/anemone/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 """
-Anemone 1.56 (http://ssb22.user.srcf.net/anemone)
+Anemone 1.57 (http://ssb22.user.srcf.net/anemone)
 (c) 2023-24 Silas S. Brown.  License: Apache 2
 
 To use this module, either run it from the command
 line, or import it and use the anemone() function.
 """
 
 # Licensed under the Apache License, Version 2.0 (the "License");
@@ -33,30 +33,25 @@
     You can also specify a JSON dictionary instead
     of the name of a JSON file, and/or an HTML
     string instead of the name of an HTML file
     (this can also be done on the command line
     with careful quoting).
     If you do not give this function any arguments
     it will look at the system command line.
-    Return value is a list of warnings, if any.
-
-    Other functions below are generally for
-    internal use and are of interest only if you
-    want to maintain Anemone, although you might
-    find {fetch(), deBlank(), version} useful."""
+    Return value is a list of warnings, if any."""
     
-    R=Run(*[(json.dumps(f) if isinstance(f,dict)
-             else f) for f in files],**options)
+    R=Run(*files,**options)
+    R.check()
     if R.mp3_recode or any(f.strip().lower().
                            endswith(
                                f"{os.extsep}wav")
                            for f in files
                            if isinstance(f,str)):
         check_we_got_LAME()
-    write_all(R,get_texts(R))
+    R.write_all(R.get_texts())
     return R.warnings
 
 def populate_argument_parser(args) -> None:
     """Calls add_argument on args, with the names
     of all Anemone command-line options, which are
     also options for anemone(), and help text.
     This is also used for runtime module help."""
@@ -176,14 +171,15 @@
 language of the book (this can help for
 search-based navigation).  If passing this option
 into the anemone module, you may use a list
 instead of a comma-separated string, which might
 be useful if there are commas in some chapter
 titles.""")
     args.add_argument("--chapter-heading-level",default=1,help="Heading level to use for chapters that don't have titles")
+    args.add_argument("--warnings-are-errors",action="store_true",help="Treat warnings as errors")
     args.add_argument("--dry-run",action="store_true",help="Don't actually output DAISY, just check the input and parameters")
 
 generator=__doc__.strip().split('\n')[0] # string we use to identify ourselves in HTTP requests and in Daisy files
 
 def get_argument_parser():
     "populates an ArgumentParser for Anemone"
     
@@ -228,93 +224,107 @@
     else: raise AnemoneError(str(m))
 class AnemoneError(Exception): pass
 
 try: import mutagen
 except ImportError: error("Anemone needs the Mutagen library to determine play lengths.\nPlease do: pip install mutagen")
 from io import BytesIO
 
+# These must be defined before Run for type hints:
+PageInfo = NT('PageInfo',['duringId','pageNo'])
+TagAndText = NT('TagAndText',['tag','text'])
+TextsAndTimesWithPages = NT('TextsAndTimesWithPages',['textsAndTimes','pageInfos'])
+ChapterTOCInfo = NT('ChapterTOCInfo',['hTag','hLine','itemNo'])
+BookTOCInfo = NT('BookTOCInfo',['hTag','hLine','recNo','itemNo'])
+del NT
+
 class Run():
   """The parameters we need for an Anemone run.
   Constructor can either parse args from the
   command line, or from anemone() caller."""
   def __init__(self,*inFiles,**kwargs):
     R = self
     R.audioData,R.filenameTitles = [],[]
     R.jsonData = []
     R.textData,R.htmlData = [],[]
     R.imageFiles,R.outputFile = [],None
     R.warnings = []
     if inFiles: # being called as a module
+        inFiles2 = [f for f in inFiles if isinstance(f,str)]
         R.__dict__.update(
             get_argument_parser().parse_args(
-                list(inFiles)+
+                (inFiles2 if inFiles2 else ["placeholder"]) +
                 [a for k,v in kwargs.items()
                  for a in
                  ['--'+k.replace('_','-'),str(v)]
                  if type(v) in [str,int]])
             .__dict__)
+        if not inFiles2: del R.files[0] # placeholder
+        R.files += [f for f in inFiles if not isinstance(f,str)] # in case passing bytes or JSON directly
     else: # being called from the command line
         R.__dict__.update(get_argument_parser().parse_args().__dict__)
     R.__dict__.update((k,v)
                       for k,v in kwargs.items()
                       if type(v) not in [str,int,type(None)]) # (None means keep the default from parse_args; boolean and bytes we might as well handle directly; list e.g. merge_books should bypass parser; ditto session object for cache, a type we can't even name here if requests_cache is not installed)
     for k in ['merge_books','chapter_titles']:
-        if not isinstance(R.__dict__[k],list): R.__dict__[k]=R.__dict__[k].split(',') # comma-separate if coming from the command line, but allow lists to be passed in to the module
+        if not isinstance(R.__dict__[k],list):
+            R.__dict__[k]=R.__dict__[k].split(',') # comma-separate if coming from the command line, but allow lists to be passed in to the module
+            if R.__dict__[k]==['']:
+                R.__dict__[k] = []
     for f in R.files:
         fOrig = f
-        if f.lower().endswith(f"{os.extsep}zip"):
+        if isinstance(f,dict):
+            # support direct JSON pass-in as dict
+            R.jsonData.append(f)
+            R.check_for_JSON_transcript()
+            continue
+        if isinstance(f,str) and f.lower().endswith(f"{os.extsep}zip"):
             if R.outputFile: error(f"Only one {os.extsep}zip output file may be specified")
             R.outputFile = f ; continue
-        if re.match("https?://",f):
+        elif isinstance(f,str) and re.match("https?://",f):
             f=fetch(f,R.cache,R.refresh,R.refetch,R.delay,R.user_agent)
         elif delimited(f,'{','}'): pass
         elif delimited(f,'<','>'): pass
         elif not os.path.isfile(f): error(f"File not found: {f}")
         else: f = open(f,"rb").read()
         if delimited(f,'{','}'):
             R.jsonData.append(json.loads(f))
-            check_for_JSON_transcript(R)
+            R.check_for_JSON_transcript()
         elif delimited(f,'<','>'):
             R.htmlData.append(f)
         elif fOrig.lower().endswith(f"{os.extsep}mp3") or fOrig.lower().endswith(f"{os.extsep}wav"):
             R.audioData.append(f)
             R.filenameTitles.append(fOrig[:fOrig.rindex(os.extsep)])
         elif fOrig.lower().endswith(f"{os.extsep}txt"):
             R.textData.append(f.decode('utf-8').strip())
         else: error(f"Format of '{fOrig}' has not been recognised")
+  def check(self) -> None:
+    "Checks we've got everything"
+    # You may omit calling this if you're creating
+    # a temporary Run just to call something like
+    # check_for_JSON_transcript and get its HTML
+    R = self
     if not R.audioData: error("Creating DAISY files without audio is not yet implemented")
     if R.htmlData and not R.jsonData: error("Full text without time markers is not yet implemented")
     if R.jsonData and not R.htmlData: error("Time markers without full text is not implemented")
     if R.htmlData and R.textData: error("Combining full text with title-only text files is not yet implemented.  Please specify full text for everything or just titles for everything, not both.")
     if R.jsonData and not len(R.audioData)==len(R.jsonData): error(f"If JSON marker files are specified, there must be exactly one JSON file for each recording file.  We got f{len(R.jsonData)} JSON files and f{len(R.audioData)} recording files.")
     if R.textData and not len(R.audioData)==len(R.textData): error(f"If text files are specified, there must be exactly one text file for each recording file.  We got f{len(R.textData)} text files and f{len(R.audioData)} recording files.")
     if R.htmlData and not len(R.audioData)==len(R.htmlData): error(f"If HTML documents are specified, there must be exactly one HTML document for each recording.  We got f{len(R.htmlData)} HTML documents and f{len(R.audioData)} recordings.")
     if not R.outputFile:
         R.outputFile=f"output_daisy{os.extsep}zip"
     if not R.title: R.title=R.outputFile.replace(f"{os.extsep}zip","").replace("_daisy","")
-  def warning(self,warningText):
+  def warning(self,warningText) -> None:
+    if self.warnings_are_errors:error(warningText)
     self.warnings.append(warningText)
     sys.stderr.write(f"WARNING: {warningText}\n")
-
-def delimited(s,start:int,end:int) -> bool:
-    """Checks to see if a string or binary data
-    is delimited by start and end, converting as
-    needed, after stripping"""
-    if isinstance(s,bytes):
-        s = s.replace(b"\xEF\xBB\xBF",b"").strip() # just in case somebody's using UTF-8 BOMs
-        return s.startswith(start.encode('latin1')) and s.endswith(end.encode('latin1'))
-    else: # string; assume no BOM to skip
-        s = s.strip()
-        return s.startswith(start) and s.endswith(end)
-
-def check_for_JSON_transcript(R) -> None:
+  def check_for_JSON_transcript(self) -> None:
     """Checks to see if the last thing added to
     the Run object is a JSON podcast transcript,
     and converts it to HTML + time markers"""
-    
+    R = self
     if isinstance(R.jsonData[-1].get(
             "segments",None),list) and all(
                 isinstance(s,dict) and
                 "startTime" in s and "body" in s
                 for s in R.jsonData[-1]["segments"]): # looks like JSON transcript format instead of markers format
         curSpeaker=None ; bodyList = []
         for s in R.jsonData[-1]["segments"]:
@@ -327,38 +337,19 @@
         R.htmlData.append(' '.join(
             f'<span {R.marker_attribute}="{i}">{c}</span>' for i,c in enumerate(bodyList) if c))
         R.jsonData[-1]={"markers":[
             {"id":f"{i}","time":t}
             for i,t in enumerate(
                     s["startTime"] for s in R.jsonData[-1]["segments"])
             if bodyList[i]]}
-
-def check_we_got_LAME() -> None:
-    """Complains if a LAME binary is not
-    available on this system.  Makes a little
-    extra effort to find one on Windows."""
-    
-    if which('lame'): return
-    if sys.platform=='win32':
-        os.environ["PATH"] += r";C:\Program Files (x86)\Lame for Audacity;C:\Program Files\Lame for Audacity"
-        if which('lame'): return
-    error(f"Anemone requires the LAME program to encode/recode MP3s.\nPlease {'run the exe installer from lame.buanzo.org' if sys.platform=='win32' else 'install lame'} and try again.")
-
-PageInfo = NT('PageInfo',['duringId','pageNo'])
-TagAndText = NT('TagAndText',['tag','text'])
-TextsAndTimesWithPages = NT('TextsAndTimesWithPages',['textsAndTimes','pageInfos'])
-ChapterTOCInfo = NT('ChapterTOCInfo',['hTag','hLine','itemNo'])
-BookTOCInfo = NT('BookTOCInfo',['hTag','hLine','recNo','itemNo'])
-del NT
-
-def get_texts(R) -> list:
+  def get_texts(self) -> list:
     """Gets the text markup required for the run,
     extracting it from HTML (guided by JSON IDs)
     if we need to do that."""
-    
+    R = self
     if R.textData: return R.textData # section titles only, from text files
     elif not R.htmlData: return R.filenameTitles # section titles only, from sound filenames
     recordingTexts = []
     for h,j in zip(R.htmlData,R.jsonData):
         markers = j['markers']
         want_pids = [jsonAttr(m,"id") for m in markers]
         id_to_content = {}
@@ -433,78 +424,23 @@
                 rTxt.append(TagAndText(tag,content_fixes(content)))
             else:
                 R.warning(f"JSON {len(recordingTexts)+1} marker {i+1} marks paragraph ID {want_pids[i]} which is not present in HTML {len(recordingTexts)+1}.  Anemone will make this a blank paragraph.")
                 rTxt.append(TagAndText('p',''))
         recordingTexts.append(
             TextsAndTimesWithPages(rTxt,pageNos))
     return recordingTexts
-
-tagRewrite = { # used by get_texts
-    'legend':'h3', # used in fieldset
-}
-
-def content_fixes(content:str) -> str:
-    """Miscellaneous fixes for final XML/XHTML
-    to work around some issues with readers"""
-    content = easyReader_em_fix(content)
-    content = re.sub('( *</?br> *)+',' <br />',content) # allow line breaks inside paragraphs, in case any in mid-"sentence", but collapse them because readers typically add extra space to each, plus add a space beforehand in case any reader doesn't render the linebreak (e.g. EasyReader 10 in a sentence span)
-    return content
-
-def easyReader_em_fix(content:str) -> str:
-    """EasyReader 10 workaround: it does not show
-    strong or em, which is OK but it puts space
-    around it: no good if it happened after a "("
-    or similar, so delete those occurrences"""
-    while True:
-        c2 = re.sub(
-            r"<(?P<tag>(strong|em))>(.*?)</(?P=tag)>",
-            lambda m:easyReader_em_fix(m.group(3))
-            if m.start() and
-            content[m.start()-1] not in ' >'
-            or m.end()<len(content) and
-            content[m.end()] not in ' <'
-            else f"<{m.group(1)}>{easyReader_em_fix(m.group(3))}</{m.group(1)}>",
-            string = content)
-        if c2==content: break
-        content = c2 # and re-check
-    return content
-
-def jsonAttr(d:dict,suffix:str) -> str:
-    """Returns the value of a dictionary key whose
-    name ends with the given lower-case suffix
-    (after converting names to lower case), after
-    checking exactly one key does this.  Used for
-    checking JSON for things like paragraphId if
-    you know only that it ends with 'Id'"""
-    
-    keys = [k for k in d.keys() if k.lower().endswith(suffix)]
-    if not keys: error(f"No *{suffix} in {repr(keys)}")
-    if len(keys)>1: error(f"More than one *{suffix} in {repr(keys)}")
-    return str(d[keys[0]])
-
-def parseTime(t:str) -> float:
-    """Parses a string containing seconds,
-    minutes:seconds or hours:minutes:seconds
-    (decimal fractions of seconds allowed),
-    and returns floating-point seconds"""
-    
-    tot = 0.0 ; mul = 1
-    for u in reversed(t.split(':')):
-        tot += float(u)*mul ; mul *= 60
-    return tot
-
-def write_all(R:Run,recordingTexts) -> None:
+  def write_all(self,recordingTexts) -> None:
     """Writes the DAISY zip and everything in it.
     Each item of recordingTexts is either 1 text
     for section title of whole recording, or a
     TextsAndTimesWithPages i.e. ([TagAndText,time,
     TagAndText,time,TagAndText],[PageInfo,...])"""
-    
+    R = self
     assert len(R.audioData) == len(recordingTexts)
-    headings = getHeadings(R,recordingTexts)
+    headings = R.getHeadings(recordingTexts)
     if R.dry_run: return sys.stderr.write(f"Dry run: {len(R.warnings) if R.warnings else 'no'} warning{'' if len(R.warnings)==1 else 's'} for {R.outputFile}\n")
     merge0lenSpans(recordingTexts,headings)
     if R.mp3_recode or any(
             'audio/mp3' not in mutagen.File(BytesIO(dat)).mime for dat in R.audioData): # parallelise lame if possible
         if not __name__=="__main__":
             sys.stderr.write(f"Making {R.outputFile}...\n"),sys.stderr.flush() # especially if repeatedly called, print which outputFile we're working on BEFORE the mp3s also
         executor = ThreadPoolExecutor(
@@ -512,23 +448,24 @@
         recordingTasks=[executor.submit(
             (recodeMP3 if
              R.mp3_recode or
              'audio/mp3' not in mutagen.File(BytesIO(dat)).mime
              else lambda x:x),
             dat) for dat in R.audioData]
     else: executor,recordingTasks = None,None
-    try: write_all0(R,recordingTexts,headings,recordingTasks)
+    try: R.write_all0(recordingTexts,headings,recordingTasks)
     except: # unhandled exception: clean up
         try: executor.shutdown(wait=False,cancel_futures=False) # (cancel_futures is Python 3.9+)
         except: pass # (no executor / can't do it) # noqa: E722
         try: os.remove(R.outputFile) # incomplete
         except: pass # noqa: E722
         raise
-def write_all0(R:Run,recordingTexts,headings,recordingTasks) -> None:
-    "Service function for write_all"
+  def write_all0(self,recordingTexts,headings,recordingTasks) -> None:
+    "Service method for write_all"
+    R = self
     if os.sep in R.outputFile:
         Path(R.outputFile[:R.outputFile.rindex(os.sep)]).mkdir(parents=True,exist_ok=True)
     z = ZipFile(R.outputFile,"w",ZIP_DEFLATED,True)
     R.dataSectors = R.catalogueEntries = 0
     def writestr(n,s):
         if isinstance(s,bytes): L = len(s)
         else: L = len(s.encode('utf-8'))
@@ -575,58 +512,56 @@
         writestr(f"{recNo:04d}.mp3",
                  R.audioData[recNo-1]
                  if recordingTasks is None
                  else recordingTasks[recNo-1].result())
         if recordingTasks is not None:
             sys.stderr.write(" done\n")
         writestr(f'{recNo:04d}.smil',D(
-            section_smil(R,recNo,secsSoFar,
+            R.section_smil(recNo,secsSoFar,
                          secsThisRecording,curP,
                          rTxt.textsAndTimes if isinstance(rTxt,TextsAndTimesWithPages) else rTxt)))
         writestr(f'{recNo:04d}.{"xml" if R.daisy3 else "htm"}',
-                 D(text_htm(
-                     R,
+                 D(R.text_htm(
                      (rTxt.textsAndTimes[
                          (1 if isinstance(rTxt.textsAndTimes[0],float) else 0)
                          ::2]
                       if isinstance(rTxt,TextsAndTimesWithPages)
                       else [TagAndText('h1',rTxt)]),
                      curP)))
         secsSoFar += secsThisRecording
         curP += (1+len(rTxt.textsAndTimes)//2 if isinstance(rTxt,TextsAndTimesWithPages) else 1)
     for n,u in enumerate(R.imageFiles):
         writestr(f'{n+1}{u[u.rindex("."):]}',
                  fetch(u,R.cache,R.refresh,R.refetch,R.delay,R.user_agent) if re.match("https?://",u) else open(u,'rb').read())
     if not R.date: R.date = "%d-%02d-%02d" % time.localtime()[:3]
     if R.daisy3:
         writestr('dtbook.2005.basic.css',D(d3css))
-        writestr('package.opf',D(package_opf(
-            R, hasFullText, len(recordingTexts),
+        writestr('package.opf',D(R.package_opf(
+            hasFullText, len(recordingTexts),
             secsSoFar)))
         writestr('text.res',D(textres))
-    else: writestr('master.smil',D(master_smil(R,headings,secsSoFar)))
+    else: writestr('master.smil',D(R.master_smil(headings,secsSoFar)))
     writestr(
         'navigation.ncx' if R.daisy3
         else 'ncc.html',
-        D(ncc_html(
-            R,headings,hasFullText,secsSoFar,
+        D(R.ncc_html(
+            headings,hasFullText,secsSoFar,
             [timeAdjust(
                 t.textsAndTimes if isinstance(t,TextsAndTimesWithPages) else t,
                 durations[i])
              for i,t in enumerate(recordingTexts)],
             [(t.pageInfos if isinstance(t,TextsAndTimesWithPages) else [])
              for t in recordingTexts])))
     if not R.daisy3: writestr('er_book_info.xml',D(er_book_info(durations))) # not DAISY standard but EasyReader can use this
     z.close()
     sys.stderr.write(f"Wrote {R.outputFile}\n")
-
-def getHeadings(R:Run,recordingTexts) -> list:
+  def getHeadings(self,recordingTexts) -> list:
     """Gets headings from recordingTexts for the
     DAISY's NCC / OPF data"""
-    
+    R = self
     ret = [] ; cvChaps = [] ; chapNo = 0
     try: bookTitlesAndNumChaps = [
             (n,int(v))
             for n,v in [
                     (b if isinstance(b,tuple)
                      else b.split('/'))
                     for b in R.merge_books if b]]
@@ -737,170 +672,32 @@
                         bookTitlesAndNumChaps[0][0], # the book title (must point to a real heading for similar reason as above, TODO: if there's substantial text before 1st heading, we'll need to insert a heading in the text with 0.001s audio or something instead of doing this; may also need to in-place change recordingTexts adding 1 to all headings: don't do this unless inserting h1)
                         chapHeadings[0].itemNo))
         ret.append(chapHeadings)
     if len(bookTitlesAndNumChaps)>1 or bookTitlesAndNumChaps and not chapNo==bookTitlesAndNumChaps[0][1]: R.warning("merge-books specified more files than given")
     if len(cvChaps) not in [0,len(ret)]: R.warning(f"Verse-indexed only {len(cvChaps)} of {len(ret)} chapters.  Missing: {', '.join(str(i) for i in range(1,len(ret)+1) if i not in cvChaps)}")
     if cvChaps and not R.daisy3 and not R.strict_ncc_divs: R.warning("Verse-indexing in Daisy 2 can prevent EasyReader 10 from displaying the text: try Daisy 3 instead") # (and with strict_ncc_divs, verses are not shown in Book navigation in Daisy 2)
     return ret
-
-def merge0lenSpans(recordingTexts,headings)->None:
-    """Finds spans in the text that are marked as
-    zero length in the audio, and merges them into
-    their neighbours if possible.  This is so that
-    the resulting DAISY file can still be
-    navigable if some of the time markers are
-    somehow missing in the input JSON, i.e. we
-    don't know when item 1 becomes item 2, but we
-    do know where item 1 starts and where item 2
-    ends, so can we set the navigation to create
-    a combined item for both 1 and 2."""
-    
-    for cT,cH in zip(recordingTexts,headings):
-        if not isinstance(cT,TextsAndTimesWithPages): continue
-        textsAndTimes,pages = cT
-        i=0
-        while i < len(textsAndTimes)-2:
-            while i < len(textsAndTimes)-2 and \
-                  isinstance(textsAndTimes[i],TagAndText) and \
-            (0 if i==0 else textsAndTimes[i-1])==\
-            textsAndTimes[i+1] and \
-            textsAndTimes[i].tag==textsAndTimes[i+2].tag: # tag identical and 0-length
-                textsAndTimes[i] = TagAndText(textsAndTimes[i].tag, f"{textsAndTimes[i].text}{' ' if textsAndTimes[i].tag=='span' else '<br>'}{textsAndTimes[i+2].text}") # new combined item
-                del textsAndTimes[i+1:i+3] # old
-                for hI,hV in enumerate(cH):
-                    if hV.itemNo > i//2: cH[hI]=ChapterTOCInfo(hV.hTag,hV.hLine,hV.itemNo-1)
-                for pI,pInfo in enumerate(pages):
-                    if pInfo.duringId > i//2: pages[pI]=PageInfo(pInfo.duringId-1,pInfo.pageNo)
-            i += 1
-
-def recodeMP3(dat:bytes) -> bytes:
-    """Takes MP3 or WAV data, re-codes it
-    as suitable for DAISY, and returns the bytes
-    of new MP3 data for putting into DAISY ZIP"""
-
-    # It seems broken players like FSReader can get timing wrong if mp3 contains
-    # too many tags at the start (e.g. images).
-    # eyed3 clear() won't help: it zeros out bytes without changing indices.
-    # To ensure everything is removed, better decode to raw PCM and re-encode :-(
-    decodeJob = run(["lame","-t","--decode"]+(["--mp3input"] if 'audio/mp3' in mutagen.File(BytesIO(dat)).mime else [])+["-","-o","-"],input=dat,check=True,stdout=PIPE,stderr=PIPE)
-    # (On some LAME versions, the above might work
-    # with AIFF files too, but we say MP3 or WAV.
-    # Some LAME versions can't take WAV from stdin
-    # only raw when encoding, but ok if --decode)
-    m = re.search(b'(?s)([0-9.]+) kHz, ([0-9]+).*?([0-9]+) bit',decodeJob.stderr) # hope nobody disabled --decode when building LAME (is OK on lame.buanzo.org EXEs)
-    if not m: error("lame did not give expected format for frequency, channels and bits output")
-    return run(["lame","--quiet","-r","-s",m.group(1).decode('latin1')]+(['-a'] if m.group(2)==b'2' else [])+['-m','m','--bitwidth',m.group(3).decode('latin1'),"-","--resample","44.1","-b","64","-q","0","-o","-"],input=decodeJob.stdout,check=True,stdout=PIPE).stdout
-
-def fetch(url:str,
-          cache = "cache", # not necessarily str
-          refresh:bool = False,
-          refetch:bool = False,
-          delay:int = 0,
-          user_agent = None) -> bytes:
-    """Fetches a URL, with delay and/or cache.
-    
-    cache: the cache directory (None = don't save)
-    or a requests_cache session object to do it
-    (delay option is ignored when using session)
-
-    refresh: if True, send an If-Modified-Since
-    request if we have a cached item (the date of
-    modification will be the timestamp of the file
-    in the cache, not necessarily the actual last
-    modified time as given by the server)
-
-    refetch: if True, reload unconditionally
-    without first checking the cache
-
-    delay: number of seconds between fetches
-    (tracked globally from last fetch)
-
-    user_agent: the User-Agent string to use, if
-    not using Python's default User-Agent"""
-    
-    ifModSince = None
-    if hasattr(cache,"get"):
-        # if we're given a requests_cache session,
-        # use that instead of our own caching code
-        r = cache.request('GET',url,
-                          headers = {
-                              "User-Agent":
-                              user_agent}
-                          if user_agent else {},
-                          refresh=refresh,
-                          force_refresh=refetch)
-        if r.status_code == 200: return r.content
-        else: raise HTTPError("",r.status_code,"unexpected HTTP code",{},None)
-
-    # Fallback to our own filesystem-based code
-    # for quick command-line use if you want to
-    # manually manage the cache (delete parts of
-    # it by directory etc) :
-    if cache:
-      fn = re.sub('[%&?@*#{}<>!:+`=|$]', # these characters need to be removed on Windows's filesystem
-                  '', # TODO: store original URL somewhere just in case some misguided webmaster puts two identical URLs modulo those characters??
-                  cache+os.sep+unquote(re.sub('.*?://','',url))
-                  .replace('/',os.sep))
-      if fn.endswith(os.sep): fn += "index.html"
-      fn = os.sep.join(f.replace('.',os.extsep)
-                       for f in fn.split(os.sep)) # just in case we're on RISC OS (not tested)
-      fnExc = fn+os.extsep+"exception"
-      if os.path.exists(fn):
-        if refetch: pass # ignore already dl'd
-        elif refresh:
-            ifModSince=os.stat(fn).st_mtime
-        else: return open(fn,'rb').read()
-      elif os.path.exists(fnExc) and not refetch and not refresh: raise HTTPError("",int(open(fnExc).read()),"HTTP error on last fetch",{},None) # useful especially if a wrapper script is using our fetch() for multiple chapters and stopping on a 404
-      Path(fn[:fn.rindex(os.sep)]).mkdir(parents=True,exist_ok=True)
-    sys.stderr.write("Fetching "+url+"...")
-    sys.stderr.flush()
-    global _last_urlopen_time
-    try: _last_urlopen_time
-    except NameError: _last_urlopen_time = 0
-    if delay: time.sleep(min(0,_last_urlopen_time+delay-time.time()))
-    headers = {"User-Agent":user_agent} if user_agent else {}
-    if ifModSince:
-        t = time.gmtime(ifModSince)
-        headers["If-Modified-Since"]=f"{'Mon Tue Wed Thu Fri Sat Sun'.split()[t.tm_wday]}, {t.tm_mday} {'Jan Feb Mar Apr May Jun Jul Aug Sep Oct Nov Dec'.split()[t.tm_mon-1]} {t.tm_year} {t.tm_hour:02d}:{t.tm_min:02d}:{t.tm_sec:02d} GMT"
-    try: dat = urlopen(Request(url,headers=headers)).read()
-    except HTTPError as e:
-        _last_urlopen_time = time.time()
-        if e.getcode()==304 and cache:
-            sys.stderr.write(" no new data\n")
-            return open(fn,'rb').read()
-        else:
-            sys.stderr.write(f"error {e.getcode()}\n")
-            if cache: open(fnExc,"w").write(
-                    str(e.getcode()))
-            raise
-    _last_urlopen_time = time.time()
-    if cache:
-        open(fn,'wb').write(dat)
-        sys.stderr.write(" saved\n")
-    else: sys.stderr.write(" fetched\n")
-    return dat
-
-def ncc_html(R:Run, headings = [],
+  def ncc_html(self, headings = [],
              hasFullText:bool = False,
              totalSecs = 0,
              recTimeTxts = [],
              pageNos=[]) -> str:
     """Returns the Navigation Control Centre (NCC)
     recTimeTxts includes 0 and total
     pageNos is [[PageInfo,...],...]"""
-    
+    R = self
     numPages = sum(len(L) for L in pageNos)
     maxPageNo = max((
         max(
             (int(i.pageNo) for i in PNs),
             default=0)
         for PNs in pageNos),default=0)
     # TODO: we assume all pages are 'normal' pages
     # (not 'front' pages in Roman letters etc)
-    headingsR = normaliseDepth(R,hReduce(headings)) # (hType,hText,recNo,textNo)
+    headingsR = R.normaliseDepth(hReduce(headings)) # (hType,hText,recNo,textNo)
     return deBlank(f"""<?xml version="1.0" encoding="utf-8"?>
 {'<!DOCTYPE ncx PUBLIC "-//NISO//DTD ncx 2005-1//EN" "http://www.daisy.org/z3986/2005/ncx-2005-1.dtd">' if R.daisy3 else '<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">'}
 <{'ncx xmlns="http://www.daisy.org/z3986/2005/ncx/" version="2005-1"'
     if R.daisy3
     else f'html lang="{R.lang}" xmlns="http://www.w3.org/1999/xhtml"'} xml:lang="{R.lang}">
   <head>
     {'<meta name="dtb:uid" content=""/>' if R.daisy3 else '<meta content="text/html; charset=utf-8" http-equiv="Content-type" />'}
@@ -946,38 +743,21 @@
       <navLabel><text>{N}</text></navLabel>
       <content src="{r+1:04d}.smil#pr{r+1}.{after}"/>
     </pageTarget>""" for r,PNs in enumerate(pageNos) for (PO,(after,N)) in enumerate(PNs))+"""
   </pageList>
 </ncx>""" if R.daisy3 else """
   </body>
 </html>"""))
-
-def addPbeforeTag(tag:str, num:int, paras:list) -> bool:
-    "Decides whether a <p> should be added before the current tag"
-    return tag=='span' and (
-        num==0
-        or not paras[num-1].tag=="span"
-        or paras[num-1].text.endswith("<br />"))
-def closePafterTag(tag:str, text:str, num:int, paras:list) -> bool:
-    "Decides whether a </p> should be added after closing the current tag"
-    return tag=='span' and (
-        text.endswith("<br />")
-        or num+1==len(paras)
-        or not paras[num+1].tag=='span')
-
-def removeImages(text:str) -> str:
-    "Removes our normalised <img> markup from text"
-    return re.sub('<img src="[^"]*" [^/]*/>','',text)
-def imageParagraph(R:Run,text:str) -> str:
+  def imageParagraph(self,text:str) -> str:
     "Pulls out our normalised <img> markup for use after the paragraph"
+    R = self
     return f"""{'<p><imggroup>' if R.daisy3 and re.search('<img src="',text) else ''}{''.join(re.findall('<img src="[^"]*" [^/]*/>',text))}{'</imggroup></p>' if R.daisy3 and re.search('<img src="',text) else ''}"""
-
-def daisy3OpenLevelTags(R:Run, tag:str, num:int, paras:list[TagAndText]) -> str:
+  def daisy3OpenLevelTags(self, tag:str, num:int, paras:list[TagAndText]) -> str:
     "Gives the <levelN> tags that should be placed before the current point in the DAISY 3 format"
-    if not R.daisy3: return ''
+    if not self.daisy3: return ''
     elif not tag.startswith('h'):
         if num: return '' # will have been started
         else: return '<level1>'
     return ''.join(
         f'<level{n}>'
         for n in range(
                 min(
@@ -991,17 +771,17 @@
                 if any(
                         paras[p].tag
                         .startswith('h')
                         for p in range(
                                 num-1,-1,-1))
                 else 1,
                 int(tag[1:])+1))
-def daisy3CloseLevelTags(R:Run, tag:str, num:int, paras:list[TagAndText]) -> str:
+  def daisy3CloseLevelTags(self, tag:str, num:int, paras:list[TagAndText]) -> str:
     "Gives the </levelN> tags that should be placed before the current point in the DAISY 3 format"
-    if not R.daisy3 or not num+1==len(paras) \
+    if not self.daisy3 or not num+1==len(paras) \
        and not paras[num+1].tag.startswith('h'):
         return ''
     return ''.join(
         f'</level{n}>'
         for n in range(
                 next(
                     int(paras[p].tag[1:])
@@ -1011,60 +791,19 @@
                 ) if any(
                     paras[p].tag.startswith('h')
                     for p in range(num,-1,-1)
                 ) else 1,
                 0 if num+1==len(paras)
                 else int(paras[num+1].tag[1:])-1,
                 -1))
-
-def numDaisy3NavpointsToClose(s:int, headingsR:list[BookTOCInfo]) -> int:
-    """Calculates the number of DAISY 3 navigation
-    points that need closing after index s"""
-    
-    thisTag = headingsR[s]
-    if thisTag.hTag.startswith('h'):
-        thisDepth = int(thisTag.hTag[1])
-    else: thisDepth = None # a div navpoint
-    if s+1==len(headingsR): nextDepth = 1
-    else:
-        nextTag = headingsR[s+1]
-        if nextTag.hTag.startswith('h'):
-            nextDepth = int(nextTag.hTag[1])
-        else: nextDepth = None # another div
-    if thisDepth == nextDepth: return 1 # e.g. this is div and next is div, or same heading level
-    elif nextDepth is None: return 0 # never close if it's heading followed by div
-    headingNums_closed = ''.join(
-        ('' if not i.hTag.startswith('h')
-         else i.hTag[1]
-         if int(i.hTag[1])>=nextDepth
-         else '0')
-        for i in reversed(headingsR[:s+1])
-    ).split('0',1)[0]
-    if thisDepth: D=thisDepth
-    else: D=int(headingNums_closed[0]) # the heading before this div (TODO: this code assumes there will be one, which is currently true as these divs are generated only by verse numbering)
-    N = sum(1 for j in range(nextDepth,D+1)
-            if str(j) in headingNums_closed)
-    return N+(1 if thisDepth is None else 0)
-
-def hReduce(headings:list) -> list[BookTOCInfo]:
-    """convert a list of ChapterTOCInfo lists (or
-    text strings for unstructured chapters) into a
-    single BookTOCInfo list"""
-    return reduce(lambda a,b:a+b,[
-        ([BookTOCInfo(hType,hText,recNo,textNo)
-          for (hType,hText,textNo) in i]
-         if isinstance(i,list) else
-         [BookTOCInfo('h1',i,recNo,0)])
-        for recNo,i in enumerate(headings)],[])
-
-def normaliseDepth(R:Run, items:list) -> list:
+  def normaliseDepth(self, items:list) -> list:
     """Ensure that heading items' depth conforms
     to DAISY standard, in a BookTOCInfo list"""
     
-    if R.allow_jumps: return items
+    if self.allow_jumps: return items
     curDepth = 0
     for i in range(len(items)):
       ii = items[i] # TagAndText or BookTOCInfo
       if ii[0].lower().startswith('h'):
         depth = int(ii[0][1:])
         if depth > curDepth+1:
             if isinstance(ii,BookTOCInfo):
@@ -1072,18 +811,18 @@
                     f'h{curDepth+1}',ii.hLine,
                     ii.recNo,ii.itemNo)
             else: items[i]=TagAndText(
                     f'h{curDepth+1}',ii.text)
             curDepth += 1
         else: curDepth = depth
     return items
-
-def master_smil(R:Run,headings = [],
+  def master_smil(self,headings = [],
                 totalSecs = 0):
     "Compile the master smil for a DAISY file"
+    R = self
     headings = hReduce(headings)
     return f"""<?xml version="1.0"?>
 <!DOCTYPE smil PUBLIC "-//W3C//DTD SMIL 1.0//EN" "http://www.w3.org/TR/REC-smil/SMIL10.dtd">
 <smil>
   <head>
     <meta name="dc:title" content="{deHTML(R.title)}" />
     <meta name="dc:format" content="Daisy 2.02" />
@@ -1098,35 +837,21 @@
   t.recNo+1:04d}.smil#t{t.recNo+1}.{t.itemNo
   }" id="ms_{s+1:04d}" />"""
                     for s,t in
                     enumerate(headings))+"""
   </body>
 </smil>
 """
-
-def timeAdjust(textsAndTimes,secsThisRecording:float) -> None:
-    """Ensure textsAndTimes starts at the
-    beginning of the recording, and ends at the
-    end.  Necessary for some players to play all
-    of the audio."""
-    if not isinstance(textsAndTimes,list):
-        textsAndTimes=[textsAndTimes]
-    return [0.0]+textsAndTimes[
-        (1 if isinstance(textsAndTimes[0],float)
-         else 0) :
-        (-1 if isinstance(textsAndTimes[-1],float)
-         else len(textsAndTimes))
-    ] + [secsThisRecording]
-
-def section_smil(R:Run, recNo:int = 1,
+  def section_smil(self, recNo:int = 1,
                  totalSecsSoFar:float = 0,
                  secsThisRecording:float = 0,
                  startP:int = 0,
                  textsAndTimes = []) -> str:
     "Compile a section SMIL for a DAISY file"
+    R = self
     textsAndTimes = timeAdjust(textsAndTimes,
                                secsThisRecording)
     return deBlank(f"""<?xml version="1.0" encoding="utf-8"?>
 {'<!DOCTYPE smil PUBLIC "-//NISO//DTD dtbsmil 2005-2//EN" "http://www.daisy.org/z3986/2005/dtbsmil-2005-2.dtd">'
     if R.daisy3
     else '<!DOCTYPE smil PUBLIC "-//W3C//DTD SMIL 1.0//EN" "http://www.w3.org/TR/REC-smil/SMIL10.dtd">'}
 {'<smil xmlns="http://www.w3.org/2001/SMIL20/">'
@@ -1181,46 +906,20 @@
     for j,imageID in enumerate(re.findall(
     '<img src="[^"]*" id="[^"]*',
     textsAndTimes[i][1]))) if R.daisy3 else ''
     }""" for i in range(1,len(textsAndTimes),2))+"""
     </seq>
   </body>
 </smil>
-""")
-# (do not omit text with 0-length audio altogether, even in Daisy 2: unlike image tags after paragraphs, it might end up not being displayed by EasyReader etc.  Omitting audio does NOT save being stopped at the beginning of the chapter when rewinding by paragraph: is this a bug or a feature?)
-
-def deBlank(s:str) -> str:
-    """Remove blank lines from s
-    (does not currently remove the first line if
-    blank).  Used so that optional items can be
-    placed on their own lines in our format-string
-    templates for DAISY markup.
-    """
-    return re.sub("\n( *\n)+","\n",s)
-
-def hmsTime(secs:float) -> str:
-    """Formats a floating-point number of seconds
-    into the DAISY standard hours:minutes:seconds
-    with fractions to 3 decimal places.  (Some
-    old DAISY readers can crash if more than 3
-    decimals are used, so we must stick to 3)"""
-    
-    return f"{int(secs/3600)}:{int(secs/60)%60:02d}:{secs%60:06.3f}"
-
-def deHTML(t:str) -> str:
-    """Remove HTML tags from t, collapse
-    whitespace and escape quotes so it can be
-    included in an XML attribute"""
-    
-    return re.sub(r'\s+',' ',re.sub('<[^>]*>','',t)).replace('"','&quot;').strip()
-
-def package_opf(R:Run, hasFullText:bool,
+""") # (do not omit text with 0-length audio altogether, even in Daisy 2: unlike image tags after paragraphs, it might end up not being displayed by EasyReader etc.  Omitting audio does NOT save being stopped at the beginning of the chapter when rewinding by paragraph: is this a bug or a feature?)
+  def package_opf(self, hasFullText:bool,
                 numRecs:int,
                 totalSecs:float) -> str:
     "Make the package OPF for a DAISY 3 file"
+    R = self
     return f"""<?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE package
   PUBLIC "+//ISBN 0-9673008-1-9//DTD OEB 1.2 Package//EN" "http://openebook.org/dtds/oeb-1.2/oebpkg12.dtd">
 <package xmlns="http://openebook.org/namespaces/oeb-package/1.0/" unique-identifier="{R.url}">
    <metadata>
       <dc-metadata xmlns:dc="http://purl.org/dc/elements/1.1/">
          <dc:Format>ANSI/NISO Z39.86-2005</dc:Format>
@@ -1258,20 +957,19 @@
       <item href="text.res" id="resource" media-type="application/x-dtbresource+xml"/>
    </manifest>
    <spine>"""+"".join(f"""
       <itemref idref="{i:04d}"/>""" for i in range(1,numRecs+1))+"""
    </spine>
 </package>
 """
-
-def text_htm(R:Run, paras:list[TagAndText], offset:int=0) -> str:
+  def text_htm(self, paras:list[TagAndText], offset:int=0) -> str:
     """Format the text, as htm for DAISY 2 or xml
     for DAISY 3.
     paras = TagAndText list, text is xhtml i.e. & use &amp; etc."""
-    
+    R = self
     return deBlank(f"""<?xml version="1.0"{
     ' encoding="utf-8"' if R.daisy3 else ''
     }?>{'<?xml-stylesheet type="text/css" href="dtbook.2005.basic.css"?>' if R.daisy3 else ''}
 {'<!DOCTYPE dtbook PUBLIC "-//NISO//DTD dtbook 2005-3//EN" "http://www.daisy.org/z3986/2005/dtbook-2005-3.dtd">'
     if R.daisy3
     else '<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">'}
 <{'dtbook xmlns="http://www.daisy.org/z3986/2005/dtbook/" version="2005-2"'
@@ -1288,27 +986,340 @@
         {f'<meta name="dc:identifier" content="{R.url}" />' if R.daisy3 else ''}
         {f'<meta name="dtb:uid" content="{R.url}"/>' if R.daisy3 else '<meta content="text/html; charset=utf-8" http-equiv="content-type"/>'}
         <meta name="generator" content="{generator}"/>
     </head>
     <{'book' if R.daisy3 else 'body'}>
         {f'<frontmatter><doctitle>{R.title}</doctitle><docauthor>{R.creator}</docauthor></frontmatter><bodymatter>' if R.daisy3 else ''}
 """+"\n".join(f"""{
-daisy3OpenLevelTags(R,tag,num,paras)}{
+R.daisy3OpenLevelTags(tag,num,paras)}{
 '<p>' if addPbeforeTag(tag,num,paras) else ''
 }<{tag} id=\"p{num+offset}\"{
 (' class="word"' if len(text.split())==1 else
 ' class="sentence"') if tag=='span' else ''}>{
 re.sub(" *<br />$","",removeImages(text))}</{tag
 }>{'</p>' if closePafterTag(tag,text,num,paras)
-else ''}{imageParagraph(R,text)}{
-daisy3CloseLevelTags(R,tag,num,paras)}""" for num,(tag,text) in enumerate(normaliseDepth(R,paras)))+f"""
+else ''}{R.imageParagraph(text)}{
+R.daisy3CloseLevelTags(tag,num,paras)}""" for num,(tag,text) in enumerate(R.normaliseDepth(paras)))+f"""
     </{'bodymatter></book' if R.daisy3 else 'body'}>
 </{'dtbook' if R.daisy3 else 'html'}>
 """)
 
+# -----------------------------------------------
+# Supporting functions that don't have to be in the Run class
+# -----------------------------------------------
+
+def delimited(s,start:int,end:int) -> bool:
+    """Checks to see if a string or binary data
+    is delimited by start and end, converting as
+    needed, after stripping"""
+    if isinstance(s,bytes):
+        s = s.replace(b"\xEF\xBB\xBF",b"").strip() # just in case somebody's using UTF-8 BOMs
+        return s.startswith(start.encode('latin1')) and s.endswith(end.encode('latin1'))
+    else: # string; assume no BOM to skip
+        s = s.strip()
+        return s.startswith(start) and s.endswith(end)
+
+def check_we_got_LAME() -> None:
+    """Complains if a LAME binary is not
+    available on this system.  Makes a little
+    extra effort to find one on Windows."""
+    
+    if which('lame'): return
+    if sys.platform=='win32':
+        os.environ["PATH"] += r";C:\Program Files (x86)\Lame for Audacity;C:\Program Files\Lame for Audacity"
+        if which('lame'): return
+    error(f"Anemone requires the LAME program to encode/recode MP3s.\nPlease {'run the exe installer from lame.buanzo.org' if sys.platform=='win32' else 'install lame'} and try again.")
+
+tagRewrite = { # used by get_texts
+    'legend':'h3', # used in fieldset
+}
+
+def content_fixes(content:str) -> str:
+    """Miscellaneous fixes for final XML/XHTML
+    to work around some issues with readers"""
+    content = easyReader_em_fix(content)
+    content = re.sub('( *</?br> *)+',' <br />',content) # allow line breaks inside paragraphs, in case any in mid-"sentence", but collapse them because readers typically add extra space to each, plus add a space beforehand in case any reader doesn't render the linebreak (e.g. EasyReader 10 in a sentence span)
+    return content
+
+def easyReader_em_fix(content:str) -> str:
+    """EasyReader 10 workaround: it does not show
+    strong or em, which is OK but it puts space
+    around it: no good if it happened after a "("
+    or similar, so delete those occurrences"""
+    while True:
+        c2 = re.sub(
+            r"<(?P<tag>(strong|em))>(.*?)</(?P=tag)>",
+            lambda m:easyReader_em_fix(m.group(3))
+            if m.start() and
+            content[m.start()-1] not in ' >'
+            or m.end()<len(content) and
+            content[m.end()] not in ' <'
+            else f"<{m.group(1)}>{easyReader_em_fix(m.group(3))}</{m.group(1)}>",
+            string = content)
+        if c2==content: break
+        content = c2 # and re-check
+    return content
+
+def jsonAttr(d:dict,suffix:str) -> str:
+    """Returns the value of a dictionary key whose
+    name ends with the given lower-case suffix
+    (after converting names to lower case), after
+    checking exactly one key does this.  Used for
+    checking JSON for things like paragraphId if
+    you know only that it ends with 'Id'"""
+    
+    keys = [k for k in d.keys() if k.lower().endswith(suffix)]
+    if not keys: error(f"No *{suffix} in {repr(keys)}")
+    if len(keys)>1: error(f"More than one *{suffix} in {repr(keys)}")
+    return str(d[keys[0]])
+
+def parseTime(t:str) -> float:
+    """Parses a string containing seconds,
+    minutes:seconds or hours:minutes:seconds
+    (decimal fractions of seconds allowed),
+    and returns floating-point seconds"""
+    
+    tot = 0.0 ; mul = 1
+    for u in reversed(t.split(':')):
+        tot += float(u)*mul ; mul *= 60
+    return tot
+
+def merge0lenSpans(recordingTexts:list, headings:list) -> None:
+    """Finds spans in the text that are marked as
+    zero length in the audio, and merges them into
+    their neighbours if possible.  This is so that
+    the resulting DAISY file can still be
+    navigable if some of the time markers are
+    somehow missing in the input JSON, i.e. we
+    don't know when item 1 becomes item 2, but we
+    do know where item 1 starts and where item 2
+    ends, so can we set the navigation to create
+    a combined item for both 1 and 2."""
+    
+    for cT,cH in zip(recordingTexts,headings):
+        if not isinstance(cT,TextsAndTimesWithPages): continue
+        textsAndTimes,pages = cT
+        i=0
+        while i < len(textsAndTimes)-2:
+            while i < len(textsAndTimes)-2 and \
+                  isinstance(textsAndTimes[i],TagAndText) and \
+            (0 if i==0 else textsAndTimes[i-1])==\
+            textsAndTimes[i+1] and \
+            textsAndTimes[i].tag==textsAndTimes[i+2].tag: # tag identical and 0-length
+                textsAndTimes[i] = TagAndText(textsAndTimes[i].tag, f"{textsAndTimes[i].text}{' ' if textsAndTimes[i].tag=='span' else '<br>'}{textsAndTimes[i+2].text}") # new combined item
+                del textsAndTimes[i+1:i+3] # old
+                for hI,hV in enumerate(cH):
+                    if hV.itemNo > i//2: cH[hI]=ChapterTOCInfo(hV.hTag,hV.hLine,hV.itemNo-1)
+                for pI,pInfo in enumerate(pages):
+                    if pInfo.duringId > i//2: pages[pI]=PageInfo(pInfo.duringId-1,pInfo.pageNo)
+            i += 1
+
+def recodeMP3(dat:bytes) -> bytes:
+    """Takes MP3 or WAV data, re-codes it
+    as suitable for DAISY, and returns the bytes
+    of new MP3 data for putting into DAISY ZIP"""
+
+    # It seems broken players like FSReader can get timing wrong if mp3 contains
+    # too many tags at the start (e.g. images).
+    # eyed3 clear() won't help: it zeros out bytes without changing indices.
+    # To ensure everything is removed, better decode to raw PCM and re-encode :-(
+    decodeJob = run(["lame","-t","--decode"]+(["--mp3input"] if 'audio/mp3' in mutagen.File(BytesIO(dat)).mime else [])+["-","-o","-"],input=dat,check=True,stdout=PIPE,stderr=PIPE)
+    # (On some LAME versions, the above might work
+    # with AIFF files too, but we say MP3 or WAV.
+    # Some LAME versions can't take WAV from stdin
+    # only raw when encoding, but ok if --decode)
+    m = re.search(b'(?s)([0-9.]+) kHz, ([0-9]+).*?([0-9]+) bit',decodeJob.stderr) # hope nobody disabled --decode when building LAME (is OK on lame.buanzo.org EXEs)
+    if not m: error("lame did not give expected format for frequency, channels and bits output")
+    return run(["lame","--quiet","-r","-s",m.group(1).decode('latin1')]+(['-a'] if m.group(2)==b'2' else [])+['-m','m','--bitwidth',m.group(3).decode('latin1'),"-","--resample","44.1","-b","64","-q","0","-o","-"],input=decodeJob.stdout,check=True,stdout=PIPE).stdout
+
+def fetch(url:str,
+          cache = "cache", # not necessarily str
+          refresh:bool = False,
+          refetch:bool = False,
+          delay:int = 0,
+          user_agent = None) -> bytes:
+    """Fetches a URL, with delay and/or cache.
+    
+    cache: the cache directory (None = don't save)
+    or a requests_cache session object to do it
+    (delay option is ignored when using session)
+
+    refresh: if True, send an If-Modified-Since
+    request if we have a cached item (the date of
+    modification will be the timestamp of the file
+    in the cache, not necessarily the actual last
+    modified time as given by the server)
+
+    refetch: if True, reload unconditionally
+    without first checking the cache
+
+    delay: number of seconds between fetches
+    (tracked globally from last fetch)
+
+    user_agent: the User-Agent string to use, if
+    not using Python's default User-Agent"""
+    
+    ifModSince = None
+    if hasattr(cache,"get"):
+        # if we're given a requests_cache session,
+        # use that instead of our own caching code
+        r = cache.request('GET',url,
+                          headers = {
+                              "User-Agent":
+                              user_agent}
+                          if user_agent else {},
+                          refresh=refresh,
+                          force_refresh=refetch)
+        if r.status_code == 200: return r.content
+        else: raise HTTPError("",r.status_code,"unexpected HTTP code",{},None)
+
+    # Fallback to our own filesystem-based code
+    # for quick command-line use if you want to
+    # manually manage the cache (delete parts of
+    # it by directory etc) :
+    if cache:
+      fn = re.sub('[%&?@*#{}<>!:+`=|$]', # these characters need to be removed on Windows's filesystem
+                  '', # TODO: store original URL somewhere just in case some misguided webmaster puts two identical URLs modulo those characters??
+                  cache+os.sep+unquote(re.sub('.*?://','',url))
+                  .replace('/',os.sep))
+      if fn.endswith(os.sep): fn += "index.html"
+      fn = os.sep.join(f.replace('.',os.extsep)
+                       for f in fn.split(os.sep)) # just in case we're on RISC OS (not tested)
+      fnExc = fn+os.extsep+"exception"
+      if os.path.exists(fn):
+        if refetch: pass # ignore already dl'd
+        elif refresh:
+            ifModSince=os.stat(fn).st_mtime
+        else: return open(fn,'rb').read()
+      elif os.path.exists(fnExc) and not refetch and not refresh: raise HTTPError("",int(open(fnExc).read()),"HTTP error on last fetch",{},None) # useful especially if a wrapper script is using our fetch() for multiple chapters and stopping on a 404
+      Path(fn[:fn.rindex(os.sep)]).mkdir(parents=True,exist_ok=True)
+    sys.stderr.write("Fetching "+url+"...")
+    sys.stderr.flush()
+    global _last_urlopen_time
+    try: _last_urlopen_time
+    except NameError: _last_urlopen_time = 0
+    if delay: time.sleep(min(0,_last_urlopen_time+delay-time.time()))
+    headers = {"User-Agent":user_agent} if user_agent else {}
+    if ifModSince:
+        t = time.gmtime(ifModSince)
+        headers["If-Modified-Since"]=f"{'Mon Tue Wed Thu Fri Sat Sun'.split()[t.tm_wday]}, {t.tm_mday} {'Jan Feb Mar Apr May Jun Jul Aug Sep Oct Nov Dec'.split()[t.tm_mon-1]} {t.tm_year} {t.tm_hour:02d}:{t.tm_min:02d}:{t.tm_sec:02d} GMT"
+    try: dat = urlopen(Request(url,headers=headers)).read()
+    except HTTPError as e:
+        _last_urlopen_time = time.time()
+        if e.getcode()==304 and cache:
+            sys.stderr.write(" no new data\n")
+            return open(fn,'rb').read()
+        else:
+            sys.stderr.write(f"error {e.getcode()}\n")
+            if cache: open(fnExc,"w").write(
+                    str(e.getcode()))
+            raise
+    _last_urlopen_time = time.time()
+    if cache:
+        open(fn,'wb').write(dat)
+        sys.stderr.write(" saved\n")
+    else: sys.stderr.write(" fetched\n")
+    return dat
+
+def addPbeforeTag(tag:str, num:int, paras:list) -> bool:
+    "Decides whether a <p> should be added before the current tag"
+    return tag=='span' and (
+        num==0
+        or not paras[num-1].tag=="span"
+        or paras[num-1].text.endswith("<br />"))
+def closePafterTag(tag:str, text:str, num:int, paras:list) -> bool:
+    "Decides whether a </p> should be added after closing the current tag"
+    return tag=='span' and (
+        text.endswith("<br />")
+        or num+1==len(paras)
+        or not paras[num+1].tag=='span')
+
+def removeImages(text:str) -> str:
+    "Removes our normalised <img> markup from text"
+    return re.sub('<img src="[^"]*" [^/]*/>','',text)
+
+def numDaisy3NavpointsToClose(s:int, headingsR:list[BookTOCInfo]) -> int:
+    """Calculates the number of DAISY 3 navigation
+    points that need closing after index s"""
+    
+    thisTag = headingsR[s]
+    if thisTag.hTag.startswith('h'):
+        thisDepth = int(thisTag.hTag[1])
+    else: thisDepth = None # a div navpoint
+    if s+1==len(headingsR): nextDepth = 1
+    else:
+        nextTag = headingsR[s+1]
+        if nextTag.hTag.startswith('h'):
+            nextDepth = int(nextTag.hTag[1])
+        else: nextDepth = None # another div
+    if thisDepth == nextDepth: return 1 # e.g. this is div and next is div, or same heading level
+    elif nextDepth is None: return 0 # never close if it's heading followed by div
+    headingNums_closed = ''.join(
+        ('' if not i.hTag.startswith('h')
+         else i.hTag[1]
+         if int(i.hTag[1])>=nextDepth
+         else '0')
+        for i in reversed(headingsR[:s+1])
+    ).split('0',1)[0]
+    if thisDepth: D=thisDepth
+    else: D=int(headingNums_closed[0]) # the heading before this div (TODO: this code assumes there will be one, which is currently true as these divs are generated only by verse numbering)
+    N = sum(1 for j in range(nextDepth,D+1)
+            if str(j) in headingNums_closed)
+    return N+(1 if thisDepth is None else 0)
+
+def hReduce(headings:list) -> list[BookTOCInfo]:
+    """convert a list of ChapterTOCInfo lists (or
+    text strings for unstructured chapters) into a
+    single BookTOCInfo list"""
+    return reduce(lambda a,b:a+b,[
+        ([BookTOCInfo(hType,hText,recNo,textNo)
+          for (hType,hText,textNo) in i]
+         if isinstance(i,list) else
+         [BookTOCInfo('h1',i,recNo,0)])
+        for recNo,i in enumerate(headings)],[])
+
+def timeAdjust(textsAndTimes,secsThisRecording:float) -> None:
+    """Ensure textsAndTimes starts at the
+    beginning of the recording, and ends at the
+    end.  Necessary for some players to play all
+    of the audio."""
+    if not isinstance(textsAndTimes,list):
+        textsAndTimes=[textsAndTimes]
+    return [0.0]+textsAndTimes[
+        (1 if isinstance(textsAndTimes[0],float)
+         else 0) :
+        (-1 if isinstance(textsAndTimes[-1],float)
+         else len(textsAndTimes))
+    ] + [secsThisRecording]
+
+def deBlank(s:str) -> str:
+    """Remove blank lines from s
+    (does not currently remove the first line if
+    blank).  Used so that optional items can be
+    placed on their own lines in our format-string
+    templates for DAISY markup.
+    """
+    return re.sub("\n( *\n)+","\n",s)
+
+def hmsTime(secs:float) -> str:
+    """Formats a floating-point number of seconds
+    into the DAISY standard hours:minutes:seconds
+    with fractions to 3 decimal places.  (Some
+    old DAISY readers can crash if more than 3
+    decimals are used, so we must stick to 3)"""
+    
+    return f"{int(secs/3600)}:{int(secs/60)%60:02d}:{secs%60:06.3f}"
+
+def deHTML(t:str) -> str:
+    """Remove HTML tags from t, collapse
+    whitespace and escape quotes so it can be
+    included in an XML attribute"""
+    
+    return re.sub(r'\s+',' ',re.sub('<[^>]*>','',t)).replace('"','&quot;').strip()
+
 def er_book_info(durations:list[float]) -> str:
     """Return the EasyReader book info.
     durations = list of secsThisRecording"""
     
     return """<?xml version="1.0" encoding="utf-8"?>
 <book_info>
     <smil_info>"""+"".join(f"""
```

### Comparing `anemone_daisy_maker-1.56.2/anemone_daisy_maker.egg-info/PKG-INFO` & `anemone_daisy_maker-1.57/anemone_daisy_maker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anemone-daisy-maker
-Version: 1.56.2
+Version: 1.57
 Summary: Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data
 Home-page: http://ssb22.user.srcf.net/indexer/anemone.html
 Author: Silas S. Brown
 Author-email: ssb22@cam.ac.uk
 License: Apache 2
 Platform: all
 Classifier: Programming Language :: Python :: 3
```

### Comparing `anemone_daisy_maker-1.56.2/setup.py` & `anemone_daisy_maker-1.57/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from setuptools import setup, find_packages;setup(name='anemone_daisy_maker',version='1.56.2',entry_points={'console_scripts':['anemone=anemone.__init__:anemone']},license='Apache 2',platforms='all',url='http://ssb22.user.srcf.net/indexer/anemone.html',author='Silas S. Brown',author_email='ssb22@cam.ac.uk',description='Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data',long_description='''Anemone DAISY maker
+from setuptools import setup, find_packages;setup(name='anemone_daisy_maker',version='1.57',entry_points={'console_scripts':['anemone=anemone.__init__:anemone']},license='Apache 2',platforms='all',url='http://ssb22.user.srcf.net/indexer/anemone.html',author='Silas S. Brown',author_email='ssb22@cam.ac.uk',description='Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data',long_description='''Anemone DAISY maker
 -----------------
 from http://ssb22.user.srcf.net/indexer/anemone.html
 
 `anemone.py` is a module to put together a DAISY digital talking book, from HTML text, MP3 audio recordings and time index data.  It produces DAISY 2.02 files by default, or DAISY 3 (i.e. ANSI/NISO Z39.86) if an option is set.  It currently can produce one of two different types of digital talking book:
 
 1. Full audio with basic Navigation Control Centre only: this requires a list of MP3 or WAV files for the audio, one per section, and the title of each section can be placed either in a separate text file or in the filename of the audio file.
```

