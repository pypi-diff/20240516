# Comparing `tmp/broken_source-0.1.3-py3-none-any.whl.zip` & `tmp/broken_source-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,89 +1,98 @@
-Zip file size: 642647 bytes, number of entries: 108
--rw-r--r--  2.0 unx    61304 b- defN 20-Feb-02 00:00 Broken/Base.py
--rw-r--r--  2.0 unx     8139 b- defN 20-Feb-02 00:00 Broken/Dotmap.py
--rw-r--r--  2.0 unx     6363 b- defN 20-Feb-02 00:00 Broken/Logging.py
--rw-r--r--  2.0 unx    14839 b- defN 20-Feb-02 00:00 Broken/Project.py
--rw-r--r--  2.0 unx     2221 b- defN 20-Feb-02 00:00 Broken/Spinner.py
--rw-r--r--  2.0 unx     1395 b- defN 20-Feb-02 00:00 Broken/Types.py
--rw-r--r--  2.0 unx     3983 b- defN 20-Feb-02 00:00 Broken/__init__.py
--rw-r--r--  2.0 unx    29393 b- defN 20-Feb-02 00:00 Broken/__main__.py
--rw-r--r--  2.0 unx     1983 b- defN 20-Feb-02 00:00 Broken/BrokenEnum/Readme.md
--rw-r--r--  2.0 unx     9815 b- defN 20-Feb-02 00:00 Broken/BrokenEnum/__init__.py
--rw-r--r--  2.0 unx     3815 b- defN 20-Feb-02 00:00 Broken/BrokenEnum/__test__.py
--rw-r--r--  2.0 unx      276 b- defN 20-Feb-02 00:00 Broken/Externals/__init__.py
+Zip file size: 645366 bytes, number of entries: 117
+-rw-r--r--  2.0 unx     1040 b- defN 20-Feb-02 00:00 Broken/Types.py
+-rw-r--r--  2.0 unx     4020 b- defN 20-Feb-02 00:00 Broken/__init__.py
+-rw-r--r--  2.0 unx    22411 b- defN 20-Feb-02 00:00 Broken/__main__.py
+-rw-r--r--  2.0 unx    11807 b- defN 20-Feb-02 00:00 Broken/Core/BrokenEnum.py
+-rw-r--r--  2.0 unx     2586 b- defN 20-Feb-02 00:00 Broken/Core/BrokenLogging.py
+-rw-r--r--  2.0 unx    18578 b- defN 20-Feb-02 00:00 Broken/Core/BrokenPath.py
+-rw-r--r--  2.0 unx     4011 b- defN 20-Feb-02 00:00 Broken/Core/BrokenPlatform.py
+-rw-r--r--  2.0 unx     1741 b- defN 20-Feb-02 00:00 Broken/Core/BrokenProfiler.py
+-rw-r--r--  2.0 unx    12963 b- defN 20-Feb-02 00:00 Broken/Core/BrokenProject.py
+-rw-r--r--  2.0 unx     3364 b- defN 20-Feb-02 00:00 Broken/Core/BrokenResolution.py
+-rw-r--r--  2.0 unx     7259 b- defN 20-Feb-02 00:00 Broken/Core/BrokenScheduler.py
+-rw-r--r--  2.0 unx     2221 b- defN 20-Feb-02 00:00 Broken/Core/BrokenSpinner.py
+-rw-r--r--  2.0 unx     3783 b- defN 20-Feb-02 00:00 Broken/Core/BrokenThread.py
+-rw-r--r--  2.0 unx     2475 b- defN 20-Feb-02 00:00 Broken/Core/BrokenTorch.py
+-rw-r--r--  2.0 unx     3741 b- defN 20-Feb-02 00:00 Broken/Core/BrokenTyper.py
+-rw-r--r--  2.0 unx     4348 b- defN 20-Feb-02 00:00 Broken/Core/BrokenUtils.py
+-rw-r--r--  2.0 unx     9571 b- defN 20-Feb-02 00:00 Broken/Core/__init__.py
+-rw-r--r--  2.0 unx     8147 b- defN 20-Feb-02 00:00 Broken/Core/Staging/BrokenDotmap.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 Broken/Core/Staging/__init__.py
+-rw-r--r--  2.0 unx    18413 b- defN 20-Feb-02 00:00 Broken/Core/Staging/umidi.py
+-rw-r--r--  2.0 unx     1736 b- defN 20-Feb-02 00:00 Broken/Core/Staging/Dotmap/BaseLoader.py
+-rw-r--r--  2.0 unx    12082 b- defN 20-Feb-02 00:00 Broken/Core/Staging/Dotmap/BrokenDotmap.py
+-rw-r--r--  2.0 unx      368 b- defN 20-Feb-02 00:00 Broken/Core/Staging/Dotmap/Readme.md
+-rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 Broken/Core/Staging/Dotmap/__init__.py
+-rw-r--r--  2.0 unx     3568 b- defN 20-Feb-02 00:00 Broken/Core/Staging/Dotmap/__test__.py
+-rw-r--r--  2.0 unx     1467 b- defN 20-Feb-02 00:00 Broken/Core/Staging/Dotmap/Loaders/LoaderPIL.py
+-rw-r--r--  2.0 unx     1263 b- defN 20-Feb-02 00:00 Broken/Core/Staging/Dotmap/Loaders/LoaderTOML.py
+-rw-r--r--  2.0 unx       68 b- defN 20-Feb-02 00:00 Broken/Core/Staging/Dotmap/Loaders/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 Broken/Externals/__init__.py
 -rw-r--r--  2.0 unx     1480 b- defN 20-Feb-02 00:00 Broken/Externals/FFmpeg/Readme.md
--rw-r--r--  2.0 unx    45735 b- defN 20-Feb-02 00:00 Broken/Externals/FFmpeg/__init__.py
--rw-r--r--  2.0 unx     4964 b- defN 20-Feb-02 00:00 Broken/Externals/Upscaler/__init__.py
--rw-r--r--  2.0 unx     5221 b- defN 20-Feb-02 00:00 Broken/Externals/Upscaler/ncnn.py
--rw-r--r--  2.0 unx      811 b- defN 20-Feb-02 00:00 Broken/Loaders/LoaderBytes.py
--rw-r--r--  2.0 unx     1910 b- defN 20-Feb-02 00:00 Broken/Loaders/LoaderPIL.py
--rw-r--r--  2.0 unx      852 b- defN 20-Feb-02 00:00 Broken/Loaders/LoaderString.py
--rw-r--r--  2.0 unx      344 b- defN 20-Feb-02 00:00 Broken/Loaders/__init__.py
+-rw-r--r--  2.0 unx    45643 b- defN 20-Feb-02 00:00 Broken/Externals/FFmpeg/__init__.py
+-rw-r--r--  2.0 unx     4938 b- defN 20-Feb-02 00:00 Broken/Externals/Upscaler/__init__.py
+-rw-r--r--  2.0 unx     6351 b- defN 20-Feb-02 00:00 Broken/Externals/Upscaler/ncnn.py
+-rw-r--r--  2.0 unx      802 b- defN 20-Feb-02 00:00 Broken/Loaders/LoaderBytes.py
+-rw-r--r--  2.0 unx     1999 b- defN 20-Feb-02 00:00 Broken/Loaders/LoaderImage.py
+-rw-r--r--  2.0 unx      856 b- defN 20-Feb-02 00:00 Broken/Loaders/LoaderString.py
+-rw-r--r--  2.0 unx      546 b- defN 20-Feb-02 00:00 Broken/Loaders/__init__.py
 -rw-r--r--  2.0 unx     4765 b- defN 20-Feb-02 00:00 Broken/Resources/Fonts/DejaVu License.txt
 -rw-r--r--  2.0 unx   757076 b- defN 20-Feb-02 00:00 Broken/Resources/Fonts/DejaVuSans.ttf
 -rw-r--r--  2.0 unx     8764 b- defN 20-Feb-02 00:00 Broken/Resources/Images/Broken.ico
 -rw-r--r--  2.0 unx    15418 b- defN 20-Feb-02 00:00 Broken/Resources/Images/Broken.png
 -rw-r--r--  2.0 unx     1444 b- defN 20-Feb-02 00:00 Broken/Resources/Images/Broken.svg
--rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 Broken/Staging/__init__.py
--rw-r--r--  2.0 unx    18408 b- defN 20-Feb-02 00:00 Broken/Staging/umidi.py
--rw-r--r--  2.0 unx     1736 b- defN 20-Feb-02 00:00 Broken/Staging/Dotmap/BaseLoader.py
--rw-r--r--  2.0 unx    12082 b- defN 20-Feb-02 00:00 Broken/Staging/Dotmap/BrokenDotmap.py
--rw-r--r--  2.0 unx      368 b- defN 20-Feb-02 00:00 Broken/Staging/Dotmap/Readme.md
--rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 Broken/Staging/Dotmap/__init__.py
--rw-r--r--  2.0 unx     3568 b- defN 20-Feb-02 00:00 Broken/Staging/Dotmap/__test__.py
--rw-r--r--  2.0 unx     1467 b- defN 20-Feb-02 00:00 Broken/Staging/Dotmap/Loaders/LoaderPIL.py
--rw-r--r--  2.0 unx     1263 b- defN 20-Feb-02 00:00 Broken/Staging/Dotmap/Loaders/LoaderTOML.py
--rw-r--r--  2.0 unx       68 b- defN 20-Feb-02 00:00 Broken/Staging/Dotmap/Loaders/__init__.py
--rw-r--r--  2.0 unx     9545 b- defN 20-Feb-02 00:00 DepthFlow/DepthFlow.py
--rw-r--r--  2.0 unx      356 b- defN 20-Feb-02 00:00 DepthFlow/__init__.py
--rw-r--r--  2.0 unx      350 b- defN 20-Feb-02 00:00 DepthFlow/__main__.py
+-rw-r--r--  2.0 unx     3804 b- defN 20-Feb-02 00:00 Broken/Tests/Enum.py
+-rw-r--r--  2.0 unx       76 b- defN 20-Feb-02 00:00 Broken/Vectron/__init__.py
+-rw-r--r--  2.0 unx     7851 b- defN 20-Feb-02 00:00 DepthFlow/DepthFlow.py
+-rw-r--r--  2.0 unx      324 b- defN 20-Feb-02 00:00 DepthFlow/__init__.py
+-rw-r--r--  2.0 unx      317 b- defN 20-Feb-02 00:00 DepthFlow/__main__.py
 -rw-r--r--  2.0 unx    14623 b- defN 20-Feb-02 00:00 DepthFlow/Resources/Images/DepthFlow.png
 -rw-r--r--  2.0 unx     1445 b- defN 20-Feb-02 00:00 DepthFlow/Resources/Images/DepthFlow.svg
--rw-r--r--  2.0 unx     2499 b- defN 20-Feb-02 00:00 DepthFlow/Resources/Shaders/DepthFlow.frag
+-rw-r--r--  2.0 unx     2477 b- defN 20-Feb-02 00:00 DepthFlow/Resources/Shaders/DepthFlow.frag
 -rw-r--r--  2.0 unx     2499 b- defN 20-Feb-02 00:00 DepthFlow/Resources/Shaders/DepthFlow2D.frag
 -rw-r--r--  2.0 unx     1688 b- defN 20-Feb-02 00:00 DepthFlow/Resources/Shaders/DepthFlowMarch.frag
--rw-r--r--  2.0 unx     3031 b- defN 20-Feb-02 00:00 Pianola/Pianola.py
+-rw-r--r--  2.0 unx     2999 b- defN 20-Feb-02 00:00 Pianola/Pianola.py
 -rw-r--r--  2.0 unx      280 b- defN 20-Feb-02 00:00 Pianola/__init__.py
--rw-r--r--  2.0 unx      302 b- defN 20-Feb-02 00:00 Pianola/__main__.py
+-rw-r--r--  2.0 unx      297 b- defN 20-Feb-02 00:00 Pianola/__main__.py
 -rw-r--r--  2.0 unx    12579 b- defN 20-Feb-02 00:00 Pianola/Resources/Images/Pianola.png
 -rw-r--r--  2.0 unx     3038 b- defN 20-Feb-02 00:00 Pianola/Resources/Images/Pianola.svg
 -rw-r--r--  2.0 unx    27430 b- defN 20-Feb-02 00:00 Pianola/Resources/Midis/Hopeless Sparkle.mid
 -rw-r--r--  2.0 unx     8171 b- defN 20-Feb-02 00:00 Pianola/Resources/Shaders/Pianola.frag
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 ShaderFlow/Imgui.py
--rw-r--r--  2.0 unx     2574 b- defN 20-Feb-02 00:00 ShaderFlow/Message.py
--rw-r--r--  2.0 unx     3321 b- defN 20-Feb-02 00:00 ShaderFlow/Module.py
--rw-r--r--  2.0 unx     3878 b- defN 20-Feb-02 00:00 ShaderFlow/Notes.py
--rw-r--r--  2.0 unx    36552 b- defN 20-Feb-02 00:00 ShaderFlow/Scene.py
--rw-r--r--  2.0 unx    11798 b- defN 20-Feb-02 00:00 ShaderFlow/Shader.py
--rw-r--r--  2.0 unx    12979 b- defN 20-Feb-02 00:00 ShaderFlow/Texture.py
--rw-r--r--  2.0 unx     4219 b- defN 20-Feb-02 00:00 ShaderFlow/Variable.py
--rw-r--r--  2.0 unx      380 b- defN 20-Feb-02 00:00 ShaderFlow/__init__.py
--rw-r--r--  2.0 unx     3562 b- defN 20-Feb-02 00:00 ShaderFlow/__main__.py
--rw-r--r--  2.0 unx    12171 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/Audio.py
--rw-r--r--  2.0 unx     3175 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/Bouncing.py
--rw-r--r--  2.0 unx    17629 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/Camera.py
--rw-r--r--  2.0 unx     9042 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/Dynamics.py
+-rw-r--r--  2.0 unx     2568 b- defN 20-Feb-02 00:00 ShaderFlow/Message.py
+-rw-r--r--  2.0 unx     3215 b- defN 20-Feb-02 00:00 ShaderFlow/Module.py
+-rw-r--r--  2.0 unx     3855 b- defN 20-Feb-02 00:00 ShaderFlow/Notes.py
+-rw-r--r--  2.0 unx    39206 b- defN 20-Feb-02 00:00 ShaderFlow/Scene.py
+-rw-r--r--  2.0 unx    13833 b- defN 20-Feb-02 00:00 ShaderFlow/Shader.py
+-rw-r--r--  2.0 unx    15278 b- defN 20-Feb-02 00:00 ShaderFlow/Texture.py
+-rw-r--r--  2.0 unx     4187 b- defN 20-Feb-02 00:00 ShaderFlow/Variable.py
+-rw-r--r--  2.0 unx      349 b- defN 20-Feb-02 00:00 ShaderFlow/__init__.py
+-rw-r--r--  2.0 unx     3269 b- defN 20-Feb-02 00:00 ShaderFlow/__main__.py
+-rw-r--r--  2.0 unx    12816 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/Audio.py
+-rw-r--r--  2.0 unx     3160 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/Bouncing.py
+-rw-r--r--  2.0 unx    17597 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/Camera.py
+-rw-r--r--  2.0 unx     8763 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/Dynamics.py
 -rw-r--r--  2.0 unx     2332 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/Frametimer.py
 -rw-r--r--  2.0 unx     1494 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/Keyboard.py
 -rw-r--r--  2.0 unx     2475 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/Noise.py
--rw-r--r--  2.0 unx    14001 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/Piano.py
--rw-r--r--  2.0 unx    10943 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/Spectrogram.py
--rw-r--r--  2.0 unx     7218 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/Video.py
--rw-r--r--  2.0 unx     3137 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/Waveform.py
+-rw-r--r--  2.0 unx    14040 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/Piano.py
+-rw-r--r--  2.0 unx    10940 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/Spectrogram.py
+-rw-r--r--  2.0 unx     7203 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/Video.py
+-rw-r--r--  2.0 unx     3088 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/Waveform.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 ShaderFlow/Modules/__init__.py
--rw-r--r--  2.0 unx     3961 b- defN 20-Feb-02 00:00 ShaderFlow/Optional/Monocular.py
+-rw-r--r--  2.0 unx     3503 b- defN 20-Feb-02 00:00 ShaderFlow/Optional/Monocular.py
 -rw-r--r--  2.0 unx        2 b- defN 20-Feb-02 00:00 ShaderFlow/Optional/OpticalFlow.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 ShaderFlow/Optional/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 ShaderFlow/Resources/__init__.py
 -rw-r--r--  2.0 unx    20132 b- defN 20-Feb-02 00:00 ShaderFlow/Resources/Images/ShaderFlow.png
 -rw-r--r--  2.0 unx     1448 b- defN 20-Feb-02 00:00 ShaderFlow/Resources/Images/ShaderFlow.svg
--rw-r--r--  2.0 unx    10158 b- defN 20-Feb-02 00:00 ShaderFlow/Resources/Scenes/Examples/Demo.py
+-rw-r--r--  2.0 unx    10171 b- defN 20-Feb-02 00:00 ShaderFlow/Resources/Scenes/Examples/Demo.py
 -rw-r--r--  2.0 unx      495 b- defN 20-Feb-02 00:00 ShaderFlow/Resources/Scenes/Examples/GLSL/Bars.frag
--rw-r--r--  2.0 unx     1263 b- defN 20-Feb-02 00:00 ShaderFlow/Resources/Scenes/Examples/GLSL/Bouncing.frag
+-rw-r--r--  2.0 unx     1285 b- defN 20-Feb-02 00:00 ShaderFlow/Resources/Scenes/Examples/GLSL/Bouncing.frag
 -rw-r--r--  2.0 unx     1278 b- defN 20-Feb-02 00:00 ShaderFlow/Resources/Scenes/Examples/GLSL/Multipass.frag
 -rw-r--r--  2.0 unx     1380 b- defN 20-Feb-02 00:00 ShaderFlow/Resources/Scenes/Examples/GLSL/RayMarch.frag
 -rw-r--r--  2.0 unx     2399 b- defN 20-Feb-02 00:00 ShaderFlow/Resources/Scenes/Examples/GLSL/ShaderToy.frag
 -rw-r--r--  2.0 unx      525 b- defN 20-Feb-02 00:00 ShaderFlow/Resources/Scenes/Examples/GLSL/Temporal.frag
 -rw-r--r--  2.0 unx      115 b- defN 20-Feb-02 00:00 ShaderFlow/Resources/Scenes/Examples/GLSL/Video.frag
 -rw-r--r--  2.0 unx     1654 b- defN 20-Feb-02 00:00 ShaderFlow/Resources/Scenes/Examples/GLSL/Visualizer.frag
 -rw-r--r--  2.0 unx      341 b- defN 20-Feb-02 00:00 ShaderFlow/Resources/Scenes/Examples/GLSL/Waveform.frag
@@ -91,20 +100,20 @@
 -rw-r--r--  2.0 unx      985 b- defN 20-Feb-02 00:00 ShaderFlow/Resources/Scenes/Examples/GLSL/Life/Visuals.glsl
 -rw-r--r--  2.0 unx     1618 b- defN 20-Feb-02 00:00 ShaderFlow/Resources/Shaders/Fragment/Default.glsl
 -rw-r--r--  2.0 unx       79 b- defN 20-Feb-02 00:00 ShaderFlow/Resources/Shaders/Fragment/Final.glsl
 -rw-r--r--  2.0 unx      895 b- defN 20-Feb-02 00:00 ShaderFlow/Resources/Shaders/Fragment/Loading.frag
 -rw-r--r--  2.0 unx      574 b- defN 20-Feb-02 00:00 ShaderFlow/Resources/Shaders/Fragment/Missing.glsl
 -rw-r--r--  2.0 unx     5079 b- defN 20-Feb-02 00:00 ShaderFlow/Resources/Shaders/Include/Camera.glsl
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 ShaderFlow/Resources/Shaders/Include/Complex.glsl
--rw-r--r--  2.0 unx    10633 b- defN 20-Feb-02 00:00 ShaderFlow/Resources/Shaders/Include/ShaderFlow.glsl
+-rw-r--r--  2.0 unx    11762 b- defN 20-Feb-02 00:00 ShaderFlow/Resources/Shaders/Include/ShaderFlow.glsl
 -rw-r--r--  2.0 unx      538 b- defN 20-Feb-02 00:00 ShaderFlow/Resources/Shaders/Vertex/Default.glsl
 -rw-r--r--  2.0 unx     1965 b- defN 20-Feb-02 00:00 SpectroNote/SpectroNote.py
--rw-r--r--  2.0 unx      290 b- defN 20-Feb-02 00:00 SpectroNote/__init__.py
--rw-r--r--  2.0 unx      342 b- defN 20-Feb-02 00:00 SpectroNote/__main__.py
+-rw-r--r--  2.0 unx      282 b- defN 20-Feb-02 00:00 SpectroNote/__init__.py
+-rw-r--r--  2.0 unx      337 b- defN 20-Feb-02 00:00 SpectroNote/__main__.py
 -rw-r--r--  2.0 unx    20132 b- defN 20-Feb-02 00:00 SpectroNote/Resources/Images/SpectroNote.png
 -rw-r--r--  2.0 unx     1448 b- defN 20-Feb-02 00:00 SpectroNote/Resources/Images/SpectroNote.svg
 -rw-r--r--  2.0 unx     3088 b- defN 20-Feb-02 00:00 SpectroNote/Resources/Shaders/SpectroNote.frag
-?rw-r--r--  2.0 unx     3026 b- defN 20-Feb-02 00:00 broken_source-0.1.3.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 broken_source-0.1.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx      194 b- defN 20-Feb-02 00:00 broken_source-0.1.3.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     9762 b- defN 20-Feb-02 00:00 broken_source-0.1.3.dist-info/RECORD
-108 files, 1388902 bytes uncompressed, 627041 bytes compressed:  54.9%
+?rw-r--r--  2.0 unx     3151 b- defN 20-Feb-02 00:00 broken_source-0.2.0.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 broken_source-0.2.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx      194 b- defN 20-Feb-02 00:00 broken_source-0.2.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    10620 b- defN 20-Feb-02 00:00 broken_source-0.2.0.dist-info/RECORD
+117 files, 1381271 bytes uncompressed, 628380 bytes compressed:  54.5%
```

## zipnote {}

```diff
@@ -1,110 +1,137 @@
-Filename: Broken/Base.py
+Filename: Broken/Types.py
 Comment: 
 
-Filename: Broken/Dotmap.py
+Filename: Broken/__init__.py
 Comment: 
 
-Filename: Broken/Logging.py
+Filename: Broken/__main__.py
 Comment: 
 
-Filename: Broken/Project.py
+Filename: Broken/Core/BrokenEnum.py
 Comment: 
 
-Filename: Broken/Spinner.py
+Filename: Broken/Core/BrokenLogging.py
 Comment: 
 
-Filename: Broken/Types.py
+Filename: Broken/Core/BrokenPath.py
 Comment: 
 
-Filename: Broken/__init__.py
+Filename: Broken/Core/BrokenPlatform.py
 Comment: 
 
-Filename: Broken/__main__.py
+Filename: Broken/Core/BrokenProfiler.py
 Comment: 
 
-Filename: Broken/BrokenEnum/Readme.md
+Filename: Broken/Core/BrokenProject.py
 Comment: 
 
-Filename: Broken/BrokenEnum/__init__.py
+Filename: Broken/Core/BrokenResolution.py
 Comment: 
 
-Filename: Broken/BrokenEnum/__test__.py
+Filename: Broken/Core/BrokenScheduler.py
 Comment: 
 
-Filename: Broken/Externals/__init__.py
+Filename: Broken/Core/BrokenSpinner.py
 Comment: 
 
-Filename: Broken/Externals/FFmpeg/Readme.md
+Filename: Broken/Core/BrokenThread.py
 Comment: 
 
-Filename: Broken/Externals/FFmpeg/__init__.py
+Filename: Broken/Core/BrokenTorch.py
 Comment: 
 
-Filename: Broken/Externals/Upscaler/__init__.py
+Filename: Broken/Core/BrokenTyper.py
 Comment: 
 
-Filename: Broken/Externals/Upscaler/ncnn.py
+Filename: Broken/Core/BrokenUtils.py
 Comment: 
 
-Filename: Broken/Loaders/LoaderBytes.py
+Filename: Broken/Core/__init__.py
 Comment: 
 
-Filename: Broken/Loaders/LoaderPIL.py
+Filename: Broken/Core/Staging/BrokenDotmap.py
 Comment: 
 
-Filename: Broken/Loaders/LoaderString.py
+Filename: Broken/Core/Staging/__init__.py
 Comment: 
 
-Filename: Broken/Loaders/__init__.py
+Filename: Broken/Core/Staging/umidi.py
 Comment: 
 
-Filename: Broken/Resources/Fonts/DejaVu License.txt
+Filename: Broken/Core/Staging/Dotmap/BaseLoader.py
 Comment: 
 
-Filename: Broken/Resources/Fonts/DejaVuSans.ttf
+Filename: Broken/Core/Staging/Dotmap/BrokenDotmap.py
 Comment: 
 
-Filename: Broken/Resources/Images/Broken.ico
+Filename: Broken/Core/Staging/Dotmap/Readme.md
 Comment: 
 
-Filename: Broken/Resources/Images/Broken.png
+Filename: Broken/Core/Staging/Dotmap/__init__.py
 Comment: 
 
-Filename: Broken/Resources/Images/Broken.svg
+Filename: Broken/Core/Staging/Dotmap/__test__.py
+Comment: 
+
+Filename: Broken/Core/Staging/Dotmap/Loaders/LoaderPIL.py
+Comment: 
+
+Filename: Broken/Core/Staging/Dotmap/Loaders/LoaderTOML.py
+Comment: 
+
+Filename: Broken/Core/Staging/Dotmap/Loaders/__init__.py
 Comment: 
 
-Filename: Broken/Staging/__init__.py
+Filename: Broken/Externals/__init__.py
 Comment: 
 
-Filename: Broken/Staging/umidi.py
+Filename: Broken/Externals/FFmpeg/Readme.md
 Comment: 
 
-Filename: Broken/Staging/Dotmap/BaseLoader.py
+Filename: Broken/Externals/FFmpeg/__init__.py
 Comment: 
 
-Filename: Broken/Staging/Dotmap/BrokenDotmap.py
+Filename: Broken/Externals/Upscaler/__init__.py
 Comment: 
 
-Filename: Broken/Staging/Dotmap/Readme.md
+Filename: Broken/Externals/Upscaler/ncnn.py
 Comment: 
 
-Filename: Broken/Staging/Dotmap/__init__.py
+Filename: Broken/Loaders/LoaderBytes.py
 Comment: 
 
-Filename: Broken/Staging/Dotmap/__test__.py
+Filename: Broken/Loaders/LoaderImage.py
 Comment: 
 
-Filename: Broken/Staging/Dotmap/Loaders/LoaderPIL.py
+Filename: Broken/Loaders/LoaderString.py
+Comment: 
+
+Filename: Broken/Loaders/__init__.py
+Comment: 
+
+Filename: Broken/Resources/Fonts/DejaVu License.txt
+Comment: 
+
+Filename: Broken/Resources/Fonts/DejaVuSans.ttf
+Comment: 
+
+Filename: Broken/Resources/Images/Broken.ico
+Comment: 
+
+Filename: Broken/Resources/Images/Broken.png
+Comment: 
+
+Filename: Broken/Resources/Images/Broken.svg
 Comment: 
 
-Filename: Broken/Staging/Dotmap/Loaders/LoaderTOML.py
+Filename: Broken/Tests/Enum.py
 Comment: 
 
-Filename: Broken/Staging/Dotmap/Loaders/__init__.py
+Filename: Broken/Vectron/__init__.py
 Comment: 
 
 Filename: DepthFlow/DepthFlow.py
 Comment: 
 
 Filename: DepthFlow/__init__.py
 Comment: 
@@ -306,20 +333,20 @@
 
 Filename: SpectroNote/Resources/Images/SpectroNote.svg
 Comment: 
 
 Filename: SpectroNote/Resources/Shaders/SpectroNote.frag
 Comment: 
 
-Filename: broken_source-0.1.3.dist-info/METADATA
+Filename: broken_source-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: broken_source-0.1.3.dist-info/WHEEL
+Filename: broken_source-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: broken_source-0.1.3.dist-info/entry_points.txt
+Filename: broken_source-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: broken_source-0.1.3.dist-info/RECORD
+Filename: broken_source-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Broken/Types.py

```diff
@@ -1,8 +1,7 @@
-import time
 import warnings
 from math import pi as PI
 from typing import TypeAlias, Union
 
 # Ignore mostly NumPy warnings
 warnings.filterwarnings("ignore")
 
@@ -27,19 +26,14 @@
 # Recurring math constants
 TAU     = (2*PI)
 SQRT2   = (2**0.5)
 SQRT3   = (3**0.5)
 SQRT_PI = (PI**0.5)
 
 # File extensions. {} are sets !
-AUDIO_EXTENSIONS = {".wav", ".ogg", ".flac", ".mp3"}
-IMAGE_EXTENSIONS = {".png", ".jpg", ".jpeg", ".gif", ".bmp", ".tiff", ".webp"}
-FONTS_EXTENSIONS = {".ttf", ".otf", ".woff", ".woff2"}
-VIDEO_EXTENSIONS = {".mp4", ".mkv", ".webm", ".avi", ".mov", ".wmv", ".flv"}
-FONTS_EXTENSIONS = {".ttf", ".otf", ".woff", ".woff2"}
-MIDI_EXTENSIONS  = {".mid", ".midi"}
-SOUNDFONTS_EXTENSIONS = {".sf2", ".sf3"}
-
-# Count time since.. the big bang with the bang counter. Shebang #!
-# Serious note, a Decoupled client starts at the Python's time origin, others on OS perf counter
-BIG_BANG: Seconds = time.perf_counter()
-time.bang_counter = (lambda: time.perf_counter() - BIG_BANG)
+class FileExtensions:
+    Audio = {".wav", ".ogg", ".flac", ".mp3"}
+    Image = {".png", ".jpg", ".jpeg", ".gif", ".bmp", ".tiff", ".webp"}
+    Video = {".mp4", ".mkv", ".webm", ".avi", ".mov", ".wmv", ".flv"}
+    Font  = {".ttf", ".otf", ".woff", ".woff2"}
+    Midi  = {".mid", ".midi"}
+    Soundfont = {".sf2", ".sf3"}
```

## Broken/__init__.py

```diff
@@ -1,57 +1,103 @@
-# -------------------------------------------------------------------------------------------------|
-
 import os
 import sys
 import typing
 from pathlib import Path
 
-# Keep repository clean of __pycache__ and .pyc files by writing to .venv
-sys.pycache_prefix = str(Path(__file__).parent.parent/".venv"/"pycache")
-
-# Fix: typing.Self was implemented on Python >= 3.11
-if sys.version_info < (3, 11):
-    typing.Self = typing.Any
-
-# PyAPP isn't passing the argument on Linux
-if bool(os.environ.get("PYAPP", False)) and (os.name != "nt"):
-    sys.argv.insert(0, sys.executable)
-
-# -------------------------------------------------------------------------------------------------|
-# Pretty... Errors !
-
 import pretty_errors
 
 pretty_errors.configure(
     filename_display  = pretty_errors.FILENAME_EXTENDED,
     line_color        = pretty_errors.RED + "> \033[1;37m",
     code_color        = '  \033[1;37m',
     line_number_first = True,
     lines_before      = 10,
     lines_after       = 10,
 )
 
+# https://github.com/numpy/numpy/issues/18669#issuecomment-820510379
+os.environ["OMP_NUM_THREADS"] = "1"
+
+# https://forums.developer.nvidia.com/t/glxswapbuffers-gobbling-up-a-full-cpu-core-when-vsync-is-off/156635
+# https://forums.developer.nvidia.com/t/gl-yield-and-performance-issues/27736
+# High CPU usage on glfw.swap_buffers when vsync is off and the GPU is wayy behind own vblank
+os.environ["__GL_YIELD"] = "USLEEP"
+
+# Keep repository clean of __pycache__ and .pyc files by writing to .venv
+if (_venv := Path(__file__).parent.parent/".venv").exists():
+    sys.pycache_prefix = str(_venv/"pycache")
+
+# Fix: typing.Self was implemented on Python >= 3.11
+if sys.version_info < (3, 11):
+    typing.Self = typing.Any
+
+# PyAPP isn't passing the argument on Linux
+if bool(os.environ.get("PYAPP", False)) and (os.name != "nt"):
+    sys.argv.insert(0, sys.executable)
+
+# As a safety measure, make all relative and strings with suffix ok paths absolute. We might run
+# binaries from other cwd, so make sure to always use non-ambiguous absolute paths if found
+# • File name collisions are unlikely with any Monorepo path (?)
+for _index, _item in enumerate(sys.argv):
+    if any((
+        any((_item.startswith(x) for x in ("./", "../", ".\\", "..\\"))),
+        bool(Path(_item).suffix) and Path(_item).exists(),
+    )):
+        sys.argv[_index] = str(Path(_item).expanduser().resolve())
+
 # -------------------------------------------------------------------------------------------------|
-# Broken Library
 
 import importlib.metadata
 import importlib.resources
-import sys
-from pathlib import Path
 
 # Information about the release and version
 PYINSTALLER: bool = bool(getattr(sys, "frozen", False))
 PYAPP:       bool = bool(os.environ.get("PYAPP", False))
 NUITKA:      bool = ("__compiled__" in globals())
-RELEASE:     bool = (NUITKA or PYINSTALLER or PYAPP)
+PYPI:        bool = ("site-packages" in __file__.lower())
+RELEASE:     bool = (NUITKA or PYINSTALLER or PYAPP or PYPI)
 DEVELOPMENT: bool = (not RELEASE)
 VERSION:     str  = importlib.metadata.version("broken-source")
 
 import Broken.Resources as BrokenResources
-from Broken.Project import BrokenProject
+from Broken.Core import (
+    BIG_BANG,
+    apply,
+    clamp,
+    denum,
+    dunder,
+    extend,
+    flatten,
+    have_import,
+    image_hash,
+    last_locals,
+    nearest,
+    shell,
+)
+from Broken.Core.BrokenEnum import BrokenEnum
+from Broken.Core.BrokenLogging import BrokenLogging
+from Broken.Core.BrokenPath import BrokenPath
+from Broken.Core.BrokenPlatform import BrokenPlatform
+from Broken.Core.BrokenProfiler import BrokenProfiler, BrokenProfilerEnum
+from Broken.Core.BrokenProject import BrokenApp, BrokenProject
+from Broken.Core.BrokenResolution import BrokenResolution
+from Broken.Core.BrokenScheduler import BrokenScheduler, BrokenTask
+from Broken.Core.BrokenSpinner import BrokenSpinner
+from Broken.Core.BrokenThread import BrokenThread, BrokenThreadPool
+from Broken.Core.BrokenTorch import BrokenTorch, TorchFlavor
+from Broken.Core.BrokenTyper import BrokenTyper
+from Broken.Core.BrokenUtils import (
+    BrokenAttrs,
+    BrokenFluentBuilder,
+    BrokenRelay,
+    BrokenSingleton,
+    BrokenWatchdog,
+    Ignore,
+    SameTracker,
+)
 
 BROKEN = BrokenProject(
     PACKAGE=__file__,
     APP_NAME="Broken",
     APP_AUTHOR="BrokenSource",
     RESOURCES=BrokenResources,
 )
@@ -65,48 +111,7 @@
 def set_project(project: BrokenProject):
     global PROJECT
     if not isinstance(project, BrokenProject):
         raise TypeError(f"Project must be an instance of BrokenProject, not {type(project)}")
     if PROJECT is not BROKEN:
         return
     PROJECT = project
-
-# -------------------------------------------------------------------------------------------------|
-
-# As a safety measure, make all relative and strings with suffix ok paths absolute. We might run
-# binaries from other cwd, so make sure to always use non-ambiguous absolute paths if found
-# • File name collisions are unlikely with any Monorepo path (?)
-for i, arg in enumerate(sys.argv):
-    if any((
-        any((arg.startswith(x) for x in ("./", "../", ".\\", "..\\"))),
-        bool(Path(arg).suffix) and Path(arg).exists(),
-    )):
-        sys.argv[i] = str(Path(arg).expanduser().resolve())
-
-# Safer measures: Store the first cwd that Broken is run, always start from there
-os.chdir(os.environ.setdefault("BROKEN_PREVIOUS_WORKING_DIRECTORY", os.getcwd()))
-
-# -------------------------------------------------------------------------------------------------|
-# Small fixes
-
-# https://github.com/numpy/numpy/issues/18669#issuecomment-820510379
-os.environ["OMP_NUM_THREADS"] = "1"
-
-# https://forums.developer.nvidia.com/t/glxswapbuffers-gobbling-up-a-full-cpu-core-when-vsync-is-off/156635
-# https://forums.developer.nvidia.com/t/gl-yield-and-performance-issues/27736
-# High CPU usage on glfw.swap_buffers when vsync is off and the GPU is wayy behind own vblank
-os.environ["__GL_YIELD"] = "USLEEP"
-
-# Patch torch.jit requiring inspect.getsource
-# https://github.com/pytorch/vision/issues/1899#issuecomment-598200938
-if PYINSTALLER:
-    try:
-        import torch.jit
-        def patch(object, **kwargs):
-            return object
-        torch.jit.script_method = patch
-        torch.jit.script = patch
-    except (ModuleNotFoundError, ImportError):
-        pass
-
-    import pyi_splash  # type: ignore
-    pyi_splash.close()
```

## Broken/__main__.py

```diff
@@ -1,38 +1,36 @@
 from __future__ import annotations
 
 import os
 import shutil
 import sys
 from pathlib import Path
-from typing import Annotated, List, Self
+from typing import Annotated, Generator, List, Self
 
 import click
 import toml
-import typer
 from attr import Factory, define
 from dotmap import DotMap
+from loguru import logger as log
 from typer import Argument, Context, Option, Typer
 
 import Broken
-from Broken.Base import (
+from Broken import (
+    BROKEN,
+    BrokenEnum,
     BrokenPath,
     BrokenPlatform,
     BrokenProfiler,
     BrokenTorch,
     BrokenTyper,
     TorchFlavor,
     flatten,
     shell,
 )
-from Broken.BrokenEnum import BrokenEnum
-from Broken.Logging import log
-from Broken.Spinner import BrokenSpinner
 
-# -------------------------------------------------------------------------------------------------|
 
 class ProjectLanguage(BrokenEnum):
     Python  = "python"
     Rust    = "rust"
     CPP     = "cpp"
     Unknown = "unknown"
 
@@ -344,17 +342,16 @@
 
 @define
 class BrokenCLI:
     projects:     list[BrokenProjectCLI] = Factory(list)
     broken_typer: BrokenTyper            = None
 
     def __attrs_post_init__(self) -> None:
-        with BrokenSpinner("Finding Projects"):
-            self.find_projects(Broken.BROKEN.DIRECTORIES.BROKEN_PROJECTS)
-            self.find_projects(Broken.BROKEN.DIRECTORIES.BROKEN_META)
+        self.find_projects(Broken.BROKEN.DIRECTORIES.BROKEN_PROJECTS)
+        self.find_projects(Broken.BROKEN.DIRECTORIES.BROKEN_META)
 
     def find_projects(self, path: Path, *, _depth: int=0) -> None:
         if _depth > 4:
             return
         if not path.exists():
             return
 
@@ -382,37 +379,32 @@
                 self.projects.append(project)
 
     # Builds CLI commands and starts Typer
     def cli(self) -> None:
         self.broken_typer = BrokenTyper(description=(
             "🚀 Broken Source Software Monorepo manager script\n\n"
             "• Tip: run \"broken (command) --help\" for options on commands or projects ✨\n\n"
-            "©️ Broken Source Software, AGPL-3.0-only License."
+            "©️ Broken Source Software, AGPL-3.0 License"
         ))
 
         with self.broken_typer.panel("📦 Installation"):
             self.broken_typer.command(self.uninstall)
-            self.broken_typer.command(self.submodules, hidden=True)
-            self.broken_typer.command(self.shortcut)
 
         with self.broken_typer.panel("🛡️ Core"):
-            self.broken_typer.command(self.clean)
             self.broken_typer.command(self.docs)
             self.broken_typer.command(self.pypi)
             self.broken_typer.command(self.sync)
             self.broken_typer.command(self.rust)
             self.broken_typer.command(self.link)
             self.broken_typer.command(self.tremeschin, hidden=True)
-
-        with self.broken_typer.panel("⚠️ Experimental"):
-            self.broken_typer.command(self.pillow, hidden=True)
+            self.broken_typer.command(self.ryedeps, hidden=True)
 
         for project in self.projects:
             self.broken_typer.command(
-                callable=project.cli,
+                target=project.cli,
                 name=project.name.lower(),
                 help=project.description_pretty_language,
                 panel=f"🔥 Projects at [bold]({project.path.parent})[/bold]",
                 add_help_option=False,
                 hidden=("Projects/Others" in str(project.path)),
             )
 
@@ -430,49 +422,30 @@
             url  = f"https://github.com/{username}/{repository}"
             path = Broken.BROKEN.DIRECTORIES.BROKEN_PRIVATE/name
             shell("git", "clone", url, path, "--recurse-submodules")
 
     # ---------------------------------------------------------------------------------------------|
     # Core section
 
-    def clean(self,
-        isort: bool=True,
-        pycache: bool=True,
-        build: bool=False,
-        releases: bool=False,
-        wheels: bool=False,
-        all: bool=False
-    ) -> None:
-        """🧹 Sorts imports, cleans .pyc files and __pycache__ directories"""
-        ROOT = Broken.BROKEN.DIRECTORIES.REPOSITORY
-
-        # Sort imports, ignore "Releases" folder
-        if all or isort:
-            shell("isort", ROOT,
-                "--force-single-line-imports",
-                "--skip", ROOT/".venvs",
-                "--skip", Broken.BROKEN.DIRECTORIES.BROKEN_RELEASES,
-                "--skip", Broken.BROKEN.DIRECTORIES.BROKEN_BUILD,
-            )
-
-        # Remove all .pyc files and __pycache__ folders
-        if all or pycache:
-            for path in ROOT.rglob("__pycache__"):
-                BrokenPath.remove(path)
-            for path in ROOT.rglob("*.pyc"):
-                BrokenPath.remove(path)
-
-        # Remove all .whl files
-        if all or wheels:
-            for path in ROOT.rglob("*.whl"):
-                BrokenPath.remove(path)
-
-        # Remove build and releases folders if requested
-        if all or build:    BrokenPath.remove(Broken.BROKEN.DIRECTORIES.BROKEN_BUILD)
-        if all or releases: BrokenPath.remove(Broken.BROKEN.DIRECTORIES.BROKEN_RELEASES)
+    def ryedeps(self) -> None:
+        """📦 Rye doesn't have a command to bump versions, but (re)adding dependencies does it"""
+        import re
+
+        pyproject = DotMap(toml.loads((BROKEN.DIRECTORIES.REPOSITORY/"pyproject.toml").read_text()))
+
+        def update_dependencies(data: List[str], *, dev: bool=False) -> None:
+            for dependency in data:
+                name, compare, version = re.split("(<|<=|!=|==|>=|>|~=|===)", dependency)
+                if (compare == "=="):
+                    continue
+                shell("rye", "add", name, "--dev"*dev, "--no-sync")
+
+        update_dependencies(pyproject.project.dependencies)
+        update_dependencies(pyproject.tool.rye["dev-dependencies"], dev=True)
+        shell("rye", "sync")
 
     def docs(self, deploy: Annotated[bool, Option("--deploy", "-d", help="Deploy Documentation to GitHub Pages")]=False) -> None:
         """📚 Generate or Deploy Documentation for all Projects"""
         GITHUB_PAGE = "git@github.com:BrokenSource/brokensource.github.io.git"
         if deploy:
             shell("mkdocs", "gh-deploy", "--force", "--remote-name", GITHUB_PAGE)
         else:
@@ -564,139 +537,14 @@
                 (root/".gitignore"),
                 (root/".github"/"Funding.yml"),
                 (root/".github"/"ISSUE_TEMPLATE").glob("*.md"),
             ):
                 target = project.path/file.relative_to(root)
                 BrokenPath.copy(src=file, dst=target)
 
-    # ---------------------------------------------------------------------------------------------|
-    # Installation section
-
-    LINUX_DESKTOP_FILE = Broken.BROKEN.DIRECTORIES.HOME/".local/share/applications/Brakeit.desktop"
-
-    def shortcut(self):
-        """🧭 Creates a Desktop App Shortcut to run the current {brakeit.py}"""
-        if BrokenPlatform.OnLinux:
-            log.info(f"Creating Desktop file at ({BrokenCLI.LINUX_DESKTOP_FILE})")
-            BrokenCLI.LINUX_DESKTOP_FILE.write_text('\n'.join((
-                "[Desktop Entry]",
-                "Type=Application",
-                "Name=Brakeit",
-                f"Exec={Broken.BROKEN.DIRECTORIES.BROKEN_BRAKEIT}",
-                f"Icon={Broken.BROKEN.RESOURCES.ICON}",
-                "Comment=Brakeit Bootstrapper",
-                "Terminal=true",
-                "Categories=Development",
-            )))
-
-        # Workaround: Do not print KeyError of `pyshortcuts.windows.get_conda_active_env`
-        elif BrokenPlatform.OnWindows:
-            os.environ["CONDA_DEFAULT_ENV"] = "base"
-            import pyshortcuts
-            pyshortcuts.make_shortcut(
-                script=str(Broken.BROKEN.DIRECTORIES.BROKEN_BRAKEIT),
-                name="Brakeit",
-                description="Broken Source Software Development Environment Entry Script",
-                icon=str(Broken.BROKEN.RESOURCES.ICON_ICO),
-            )
-        else:
-            log.error(f"Unknown Platform ({BrokenPlatform.Name})")
-            return
-
-    def submodules(self,
-        root:     Annotated[Path, Option("--root",     "-r", help="(Basic) Root path to search for Submodules")]=Broken.BROKEN.DIRECTORIES.REPOSITORY,
-        auth:     Annotated[bool, Option("--auth",     "-a", help="(Basic) Prompt Username and Password privately for Private clones")]=False,
-        username: Annotated[str,  Option("--username", "-u", help="(Auth ) Username to use for git clone")]=None,
-        password: Annotated[str,  Option("--password", "-p", help="(Auth ) Password to use for git clone")]=None,
-        pull:     Annotated[bool, Option("--pull",           help="(Git  ) Run git pull on all submodules")]=False,
-        force:    Annotated[bool, Option("--force",    "-f", help="(Git  ) Force pull (overrides local changes)")]=False,
-    ):
-        """🔽 Safely init and clone submodules, skip private ones, optional authentication"""
-
-        # --------------------------------------| Pathing
-
-        root = BrokenPath(root)
-
-        # Read .gitmodules if it exists
-        if not (gitmodules := root/".gitmodules").exists():
-            return
-
-        # Init submodules
-        with BrokenPath.pushd(root, echo=False):
-            shell("git", "submodule", "init")
-            shell("git", "pull", "--quiet", "--force"*force, do=pull)
-
-        # --------------------------------------| Authentication
-
-        # Maybe get username and password from env
-        username = os.environ.get("GIT_USERNAME", None)
-        password = os.environ.get("GIT_PASSWORD", None)
-
-        # Ask for authentication if requested but not provided yet
-        if auth and not (username and password):
-            username = username or typer.prompt("Git Username")
-            password = password or typer.prompt("Git Password", hide_input=True)
-
-        # Update credentials on env vars (it might have been just prompted)
-        os.environ["GIT_USERNAME"] = username or ""
-        os.environ["GIT_PASSWORD"] = password or ""
-
-        # `auth` now means if we have credentials
-        auth = auth or bool(username and password)
-
-        # --------------------------------------| Reading dot file
-        # Read .gitmodules
-        import configparser
-        config = configparser.ConfigParser()
-        config.read(gitmodules)
-
-        # Get all submodules
-        for section in config.sections():
-            submodule = config[section]
-
-            # Build the absolute path
-            path = root/submodule["path"]
-            url  = submodule["url"]
-
-            # Skip private submodule
-            if submodule.get("private", False) and not auth:
-                log.skip(f"Submodule is private ({path})")
-                continue
-
-            # Clone with authentication
-            url = url.replace("https://", f"https://{username}:{password}@") if auth else url
-
-            # Clone the submodule
-            with BrokenPath.pushd(path, echo=False):
-
-                # Fixme: Any better way to check if a submodule is healthy?
-                if not list(path.iterdir()):
-
-                    # Set the url to clone this repository with authentication
-                    shell("git", "remote", "set-url", "origin", url)
-
-                    # Fetch the submodule's content with the credentials provided
-                    if shell("git", "fetch").returncode != 0:
-                        log.warning(f"Failed to Fetch Submodule ({path})")
-                        log.warning("• You can safely ignore this if you don't need this submodule")
-                        log.warning("• You might not have permissions to this repository")
-                        log.warning("• You might have provided wrong credentials")
-                        continue
-
-                    # Init and update submodule we know we have access to
-                    # Switch to main branch, as detached head is clumsy
-                    shell("git", "submodule", "update", "--init", path)
-                    shell("git", "checkout", "Master")
-                    log.success(f"Submodule cloned  ({path})")
-
-                # Pull changes after initial clone
-                shell("git", "pull", "--quiet", "--force"*force, do=pull)
-
-            self.submodules(path, username=username, password=password)
-
     def uninstall(self):
         """➖ Selectively removes Data or Artifacts created by Projects outside of the Repository"""
         log.warning("Selectively Uninstalling Broken Source Convenience and Projects Data")
 
         if BrokenPlatform.OnLinux and BrokenCLI.LINUX_DESKTOP_FILE.exists():
             log.minor("Now deleting Linux dot Desktop Shortcut file")
             BrokenPath.remove(BrokenCLI.LINUX_DESKTOP_FILE, echo=False, confirm=True)
@@ -704,30 +552,23 @@
         # Remove all known projects stuff
         for project in self.projects:
             log.note()
             log.note(f"Project: {project.name}")
             log.note(f"• Path: {project.path}")
 
             # Follow Project's Workspace folder
-            if (workspace := BrokenPath(project.path/"Workspace", valid=True)):
+            if (workspace := BrokenPath(project.path/"Workspace").valid()):
                 log.minor("Now removing the Project Workspace directory")
                 BrokenPath.remove(workspace, echo=False, confirm=True)
 
         # Finally, remove the root venv
-        if (venv := BrokenPath(Broken.BROKEN.DIRECTORIES.REPOSITORY/".venv", valid=True)):
+        if (venv := BrokenPath(Broken.BROKEN.DIRECTORIES.REPOSITORY/".venv").valid()):
             log.minor("Now removing the Repository Virtual Environment")
             BrokenPath.remove(venv, echo=False, confirm=True)
 
-    # # Experimental
-
-    def pillow(self):
-        """Use Pillow-SIMD for faster Image processing"""
-        os.environ["CC"] = "cc -mavx2"
-        shell("pip", "install", "-U", "--force-reinstall", "pillow-simd")
-
 # -------------------------------------------------------------------------------------------------|
 
 def main():
     with BrokenProfiler("BROKEN"):
         broken = BrokenCLI()
         broken.cli()
```

## Broken/Externals/__init__.py

```diff
@@ -1,18 +0,0 @@
-00000000: 6672 6f6d 2061 6263 2069 6d70 6f72 7420  from abc import 
-00000010: 4142 432c 2061 6273 7472 6163 746d 6574  ABC, abstractmet
-00000020: 686f 640a 6672 6f6d 2074 7970 696e 6720  hod.from typing 
-00000030: 696d 706f 7274 2054 7970 650a 0a0a 636c  import Type...cl
-00000040: 6173 7320 4272 6f6b 656e 4578 7465 726e  ass BrokenExtern
-00000050: 616c 2841 4243 293a 0a0a 2020 2020 4070  al(ABC):..    @p
-00000060: 726f 7065 7274 790a 2020 2020 4061 6273  roperty.    @abs
-00000070: 7472 6163 746d 6574 686f 640a 2020 2020  tractmethod.    
-00000080: 6465 6620 6269 6e61 7279 2873 656c 6629  def binary(self)
-00000090: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
-000000a0: 202e 2e2e 0a0a 636c 6173 7320 4272 6f6b   .....class Brok
-000000b0: 656e 4578 7465 726e 616c 4d61 6e61 6765  enExternalManage
-000000c0: 723a 0a20 2020 2064 6566 2067 6574 2873  r:.    def get(s
-000000d0: 656c 662c 2065 7874 6572 6e61 6c3a 2054  elf, external: T
-000000e0: 7970 655b 4272 6f6b 656e 4578 7465 726e  ype[BrokenExtern
-000000f0: 616c 5d29 202d 3e20 4272 6f6b 656e 4578  al]) -> BrokenEx
-00000100: 7465 726e 616c 3a0a 2020 2020 2020 2020  ternal:.        
-00000110: 2e2e 2e0a                                ....
```

## Broken/Externals/FFmpeg/__init__.py

```diff
@@ -25,28 +25,28 @@
     Union,
 )
 
 import numpy
 import PIL
 from attr import Factory, define, field
 from dotmap import DotMap
+from loguru import logger as log
 
-from Broken.Base import (
+from Broken import (
+    BrokenEnum,
     BrokenPath,
     BrokenPlatform,
+    BrokenSpinner,
     BrokenThread,
-    BrokenUtils,
     apply,
     denum,
     flatten,
+    nearest,
     shell,
 )
-from Broken.BrokenEnum import BrokenEnum
-from Broken.Logging import log
-from Broken.Spinner import BrokenSpinner
 from Broken.Types import Hertz, Range, Seconds
 
 # ----------------------------------------------|
 # Resolution
 
 @define
 class FFmpegResolution:
@@ -597,15 +597,15 @@
             self.no_audio,
             self.advanced,
             self.audio_codec,
         )
 
     @staticmethod
     def install() -> None:
-        if all(BrokenPath.which("ffmpeg", "ffprobe")):
+        if all(map(BrokenPath.which, ("ffmpeg", "ffprobe"))):
             return
 
         if not BrokenPlatform.OnMacOS:
             log.info("FFmpeg wasn't found on System Path, will download a BtbN's Build")
             BrokenPath.get_external(''.join((
                 "https://github.com/BtbN/FFmpeg-Builds/releases/download/latest/",
                 "ffmpeg-master-latest-",
@@ -670,15 +670,15 @@
         return self
 
     def __skip__(self, *a, **k):
         """
         Some Fluent option errored out, continue the chain
         · It is dangerous, can yield to unexpected results and broken commands, but we shouldn't exit()
         """
-        log.warning(f"Skipped Fluent Option with args {a} and kwargs {k}")
+        log.warning(f"Skipped Fluent Option with args {a or None} and kwargs {k or None}")
         return self
 
     def __smart__(self,
         *items: list[Any],
         delete: Union[callable, list[callable]]=None,
         add:    Union[callable, list[callable]]=None,
     ) -> Self:
@@ -826,15 +826,15 @@
             self.pixel_format,
             self.no_video
         ))
         return self
 
     def output(self, path: str) -> Self:
         """Output some audio file, video file"""
-        BrokenPath.mkdir(Path(path).parent, echo=False)
+        BrokenPath.mkdirs(Path(path).parent, echo=False)
 
         # Add video filters
         if self.filters:
             log.debug("BrokenFFmpeg Filters:")
             for filter in self.filters:
                 log.debug(f"• {filter}")
             self.__command__ += ["-vf", ",".join(self.filters)]
@@ -1074,15 +1074,15 @@
     # ---------------------------------------------------------------------------------------------|
     # High level functions
 
     @staticmethod
     @functools.lru_cache
     def get_resolution(path: Path, *, echo: bool=True) -> Tuple[Optional[int], Optional[int]]:
         """Get the resolution of a video in a smart way"""
-        if not (path := BrokenPath(path, valid=True)):
+        if not (path := BrokenPath.valid(path)):
             return (None, None)
         BrokenFFmpeg.install()
         log.minor(f"Getting Video Resolution of ({path})")
         return PIL.Image.open(io.BytesIO(
             (BrokenFFmpeg()
                 .quiet()
                 .input(path)
@@ -1091,15 +1091,15 @@
                 .output("-")
             ).run(stdout=PIPE, echo=echo).stdout
         ), formats=["jpeg"]).size
 
     @staticmethod
     def get_frames(path: Path, *, skip: int=0, echo: bool=True) -> Optional[Iterable[numpy.ndarray]]:
         """Generator for every frame of the video as numpy arrays, FAST!"""
-        if not (path := BrokenPath(path, valid=True)):
+        if not (path := BrokenPath.valid(path)):
             return None
         BrokenFFmpeg.install()
         log.minor(f"Streaming Video Frames from file ({path})")
         (width, height) = BrokenFFmpeg.get_resolution(path)
         ffmpeg = (BrokenFFmpeg()
             .hwaccel(FFmpegHWAccel.Auto)
             .vsync(FFmpegVsync.ConstantFramerate)
@@ -1117,30 +1117,30 @@
         while (raw := ffmpeg.stdout.read(width * height * 3)):
             yield numpy.frombuffer(raw, dtype=numpy.uint8).reshape((height, width, 3))
 
     @staticmethod
     @functools.lru_cache
     def get_total_frames(path: Path, *, echo: bool=True) -> Optional[int]:
         """Count the total frames of a video by decode voiding and parsing stats output"""
-        if not (path := BrokenPath(path, valid=True)):
+        if not (path := BrokenPath.valid(path)):
             return None
         BrokenFFmpeg.install()
         with BrokenSpinner(log.minor(f"Getting video total frames of ({path}), might take a while..")):
             return int(re.compile(r"frame=\s*(\d+)").findall((BrokenFFmpeg()
                 .vsync(FFmpegVsync.ConstantFramerate)
                 .input(path)
                 .format(FFmpegFormat.Null)
                 .output("-")
             ).run(stderr=PIPE, echo=echo).stderr.decode())[-1])
 
     @staticmethod
     @functools.lru_cache
     def get_video_duration(path: Path, *, echo: bool=True) -> Optional[Seconds]:
         """Get the duration of a video"""
-        if not (path := BrokenPath(path, valid=True)):
+        if not (path := BrokenPath.valid(path)):
             return None
         BrokenFFmpeg.install()
         log.minor(f"Getting Video Duration of file ({path})")
         return float(shell(
             BrokenPath.which("ffprobe"),
             "-i", path,
             "-show_entries", "format=duration",
@@ -1148,15 +1148,15 @@
             output=True, echo=echo
         ))
 
     @staticmethod
     @functools.lru_cache
     def get_framerate(path: Path, *, precise: bool=False, echo: bool=True) -> Optional[Hertz]:
         """Get the framerate of a video"""
-        if not (path := BrokenPath(path, valid=True)):
+        if not (path := BrokenPath.valid(path)):
             return None
         BrokenFFmpeg.install()
         log.minor(f"Getting Video Framerate of file ({path})", echo=echo)
         if precise:
             A = BrokenFFmpeg.get_total_frames(path, echo=False)
             B = BrokenFFmpeg.get_video_duration(path, echo=False)
             return (A/B)
@@ -1169,15 +1169,15 @@
                 output=True, echo=echo
             ).splitlines()[0]))[0])
 
     @staticmethod
     @functools.lru_cache
     def get_samplerate(path: Path, *, stream: int=0, echo: bool=True) -> Optional[Hertz]:
         """Get the samplerate of a audio file"""
-        if not (path := BrokenPath(path, valid=True)):
+        if not (path := BrokenPath.valid(path)):
             return None
         BrokenFFmpeg.install()
         log.minor(f"Getting Audio Samplerate of file ({path})", echo=echo)
         return int(shell(
             BrokenPath.which("ffprobe"),
             "-i", path,
             "-show_entries", "stream=sample_rate",
@@ -1185,29 +1185,29 @@
             output=True, echo=echo
         ).strip().splitlines()[stream])
 
     @staticmethod
     @functools.lru_cache
     def get_audio_channels(path: Path, *, stream: int=0, echo: bool=True) -> Optional[int]:
         """Get the number of channels of a audio file"""
-        if not (path := BrokenPath(path, valid=True)):
+        if not (path := BrokenPath.valid(path)):
             return None
         BrokenFFmpeg.install()
         log.minor(f"Getting Audio Channels of file ({path})", echo=echo)
         return int(shell(
             BrokenPath.which("ffprobe"),
             "-i", path,
             "-show_entries", "stream=channels",
             "-v", "quiet", "-of", "csv=p=0",
             output=True, echo=echo
         ).strip().splitlines()[stream])
 
     @staticmethod
     def get_audio_duration(path: Path, *, echo: bool=True) -> Optional[Seconds]:
-        if not (path := BrokenPath(path, valid=True)):
+        if not (path := BrokenPath.valid(path)):
             return
         try:
             generator = BrokenAudioReader(path=path, chunk=10).stream
             while next(generator) is not None: ...
         except StopIteration as result:
             return result.value
 
@@ -1253,15 +1253,15 @@
 
     @property
     def bytes_per_sample(self) -> int:
         return (self.size * self.channels)
 
     @property
     def stream(self) -> Generator[numpy.ndarray, None, None]:
-        self.path = BrokenPath(self.path, valid=True)
+        self.path = BrokenPath(self.path).valid()
         if (self.path is None):
             return None
 
         # Get audio file attributes
         self._channels   = BrokenFFmpeg.get_audio_channels(self.path, echo=self.echo)
         self._samplerate = BrokenFFmpeg.get_samplerate(self.path, echo=self.echo)
         self.format = FFmpegPCM.get(self.format)
@@ -1297,15 +1297,15 @@
         target = 0
 
         while (target := target + self.chunk):
 
             # Calculate the length of the next read to best match the target time
             # but do not carry over temporal conversion errors
             length = (target - self.time) * self.bytes_per_second
-            length = BrokenUtils.round(length, self.bytes_per_sample, type=int)
+            length = nearest(length, self.bytes_per_sample, type=int)
             length = max(length, self.bytes_per_sample)
             data   = self._ffmpeg.stdout.read(length)
             if len(data) == 0: break
 
             # Increment precise time and read time
             self._time += len(data)/self.bytes_per_second
             yield numpy.frombuffer(data, dtype=self.dtype).reshape(-1, self.channels)
```

## Broken/Externals/Upscaler/__init__.py

```diff
@@ -1,30 +1,28 @@
 import contextlib
 import shutil
 import tempfile
 from abc import ABC, abstractmethod
-from ctypes import Union
 from pathlib import Path
-from typing import Generator
+from typing import Generator, Union
 
 import PIL
 from attr import define, field
-from Base import BrokenPath
+from loguru import logger as log
 from PIL.Image import Image
 
-from Broken.Externals import BrokenExternal
-from Broken.Loaders.LoaderPIL import LoadableImage, LoaderImage
-from Broken.Logging import log
+from Broken import BrokenPath
+from Broken.Loaders import LoadableImage, LoaderImage
 
 
 @define
-class BrokenUpscaler(BrokenExternal, ABC):
-    scale:  int = field(default=2, converter=int)
+class BrokenUpscaler(ABC):
     width:  int = field(default=0, converter=int)
     height: int = field(default=0, converter=int)
+    scale:  int = field(default=2, converter=int)
     passes: int = field(default=1, converter=int)
 
     @property
     def s(self) -> int:
         return self.scale
     @s.setter
     def s(self, value: int):
@@ -42,88 +40,91 @@
         return self.height
     @h.setter
     def h(self, value: int):
         self.height = value
 
     def output_size(self, width: int, height: int):
         """Get the output size after upscaling some input size"""
+
+        # Forces final resolution
         if (self.width and self.height):
             return (self.width, self.height)
 
-        # We upscale current times ratio at each pass
+        # Upscales input
         upscale_ratio = self.scale**self.passes
-
         return (width*upscale_ratio, height*upscale_ratio)
 
     # # Implementations
 
     @abstractmethod
     def __upscale__(self, input: Path, output: Path, *, echo: bool=True):
         """Proper upscale method"""
         ...
 
     def upscale(self,
         input:  LoadableImage,
         output: Union[Path, Image]=Image,
         *,
-        echo: bool=True
+        echo: bool=True,
+        **config
     ) -> Union[Path, Image]:
         """
         Upscale some input image given by its path or Image object.
 
         Args:
             `input`:  The input image to upscale
             `output`: The output path to save or `Image` class for a Image object
             `echo`:   Log the upscale process or commands
 
         Returns:
             The upscaled image as a PIL Image object if `output` is `Image`, else the output Path
         """
+        for key, val in config.items():
+            setattr(self, key, val)
         self.__validate__()
 
         # Load a Image out of the input or output, else Empty image
         Empty  = PIL.Image.new("RGB", (1, 1))
         iimage = LoaderImage(input ) or Empty
         oimage = LoaderImage(output) or Empty
 
         # Get the upscaled size of the input image
         target = self.output_size(iimage.width, iimage.height)
 
         # No need to upscaled if already on target size
         if (oimage.size == target):
-            log.success(f"Already upscaled to target size ({self.width}, {self.height}): {input}")
+            log.success(f"Already upscaled to target size ({self.width}, {self.height}): {oimage}")
             if output is Image:
                 return oimage
             return output
+
         if (iimage.size == target):
-            log.success(f"Already upscaled to target size ({self.width}, {self.height}): {input}")
+            log.success(f"Already upscaled to target size ({self.width}, {self.height}): {iimage}")
             if output is Image:
                 return iimage
             return output
 
         # Upscale the image
         with self.temp_image(input) as temp_input:
             with self.temp_image(output) as temp_output:
 
                 # Upscale once then on top of itself for each pass
                 for _ in range(self.passes):
                     self.__upscale__(input=temp_input, output=temp_output, echo=echo)
                     input = temp_output
 
+                # Load the upscaled final image
+                final = PIL.Image.open(temp_output)
+                final = final.resize(target, PIL.Image.LANCZOS)
+
                 # Return the Path of the Image
                 if isinstance(output, Path):
-                    oimage = PIL.Image.open(temp_output)
-                    oimage = oimage.resize(target, PIL.Image.LANCZOS)
-                    oimage.save(output, quality=95)
+                    final.save(output, quality=95)
                     return output
-
-                # Return an Image object
-                output = PIL.Image.open(temp_output)
-                output = output.resize(target, PIL.Image.LANCZOS)
-                return output
+                return final
 
     @abstractmethod
     def __validate__(self):
         """
         Validate parameters for the current upscaler
         """
 
@@ -142,19 +143,20 @@
             `format`: The format of the temporary file
 
         Returns:
             The Path to the temporary file, deleted on context exit
         """
         image = LoaderImage(image) or image
 
-        with tempfile.NamedTemporaryFile(suffix=f".{format}") as file:
+        try:
+            file = tempfile.NamedTemporaryFile(delete=False, suffix=f".{format}")
             file = BrokenPath(file.name)
-
             if isinstance(image, Image):
                 image.save(file, quality=95)
             elif image is Image:
                 pass
             elif Path(image).exists():
-                shutil.copyfile(image, file)
-
+                PIL.Image.open(image).save(file, quality=95)
             yield file
+        finally:
+            file.unlink()
```

## Broken/Externals/Upscaler/ncnn.py

```diff
@@ -1,16 +1,15 @@
-from abc import ABC
+from abc import ABC, abstractmethod
 from pathlib import Path
 from subprocess import DEVNULL
 
 from attr import define, field
-from Base import shell
-from Externals.Upscaler import BrokenUpscaler
 
-from Broken.BrokenEnum import BrokenEnum
+from Broken import BrokenEnum, BrokenPath, BrokenPlatform, shell
+from Broken.Externals.Upscaler import BrokenUpscaler
 
 
 @define
 class BrokenUpscalerNCNN(BrokenUpscaler, ABC):
     noise_level:  int  = field(default=1, converter=int)
     tile_size:    int  = field(default=0, converter=int)
     gpu:          int  = field(default=0, converter=int)
@@ -75,27 +74,51 @@
     @property
     def p(self) -> int:
         return self.passes
     @p.setter
     def p(self, value: int):
         self.passes = value
 
+    # # Metadata for automatic downloads
+
+    @staticmethod
+    @abstractmethod
+    def _base_download() -> str:
+        """https://.../stuff-{platform}.zip"""
+        ...
+
+    @staticmethod
+    @abstractmethod
+    def _binary_name() -> str:
+        ...
+
+    def binary(self) -> Path:
+        if (binary := BrokenPath.which(self._binary_name())):
+            return BrokenPath(binary)
+        DOWNLOAD = self._base_download().format(BrokenPlatform.Name.replace("linux", "ubuntu"))
+        EXECUTABLE = self._binary_name() + (".exe"*BrokenPlatform.OnWindows)
+        return BrokenPath.make_executable(next(BrokenPath.get_external(DOWNLOAD).rglob(EXECUTABLE)))
+
 # -------------------------------------------------------------------------------------------------|
 
 class BrokenWaifu2xModel(BrokenEnum):
     Cunet = "models-cunet"
     Anime = "models-upconv_7_anime_style_art_rgb"
     Photo = "models-upconv_7_photo"
 
 @define
 class BrokenWaifu2x(BrokenUpscalerNCNN):
     model: BrokenWaifu2xModel = BrokenWaifu2xModel.Cunet.field()
 
-    @property
-    def binary(self) -> str:
+    @staticmethod
+    def _base_download() -> str:
+        return "https://github.com/nihui/waifu2x-ncnn-vulkan/releases/download/20220728/waifu2x-ncnn-vulkan-20220728-{}.zip"
+
+    @staticmethod
+    def _binary_name() -> str:
         return "waifu2x-ncnn-vulkan"
 
     def __validate__(self):
         if not all(things := (
             self.noise_level in {-1, 0, 1, 2, 3},
             self.scale in {1, 2, 4, 8, 16, 32},
             (self.tile_size == 0) or (self.tile_size >= 32),
@@ -105,26 +128,27 @@
             self.proc_threads >= 1,
             self.save_threads >= 1,
         )):
             raise ValueError(f"Invalid parameters for {self.__class__.__name__}: {things}")
 
     def __upscale__(self, input: Path, output: Path, *, echo: bool=True):
         shell(
-            self.binary,
+            self.binary(),
             "-i", input,
             "-o", output,
             "-n", self.noise_level,
             "-s", self.scale,
             "-t", self.tile_size,
             "-g", self.gpu if not self.cpu else -1,
             "-j", f"{self.load_threads}:{self.proc_threads}:{self.save_threads}",
             "-x"*self.tta,
             # "-m", self.model.value, # Fixme: Doko?
             stderr=DEVNULL,
             preexec_fn=self.preexec_fn,
+            cwd=self.binary().parent,
             echo=echo,
         )
 
 # -------------------------------------------------------------------------------------------------|
 
 class BrokenRealEsrganModel(BrokenEnum):
     AnimeVideoV3 = "realesr-animevideov3"
@@ -132,41 +156,46 @@
     X4PlusAnime  = "realesrgan-x4plus-anime"
     X4PlusNet    = "realesrnet-x4plus"
 
 @define
 class BrokenRealEsrgan(BrokenUpscalerNCNN):
     model: BrokenRealEsrganModel = BrokenRealEsrganModel.AnimeVideoV3.field()
 
-    @property
-    def binary(self) -> str:
+    @staticmethod
+    def _base_download() -> str:
+        return "https://github.com/xinntao/Real-ESRGAN/releases/download/v0.2.5.0/realesrgan-ncnn-vulkan-20220424-{}.zip"
+
+    @staticmethod
+    def _binary_name() -> str:
         return "realesrgan-ncnn-vulkan"
 
     def __validate__(self):
         if not all(things := (
             self.passes >= 1,
-            self.scale in {2, 3, 4},
+            self.scale in {1, 2, 3, 4},
             (self.tile_size == 0) or (self.tile_size >= 32),
             self.model is not None,
             self.gpu >= 0,
             self.load_threads >= 1,
             self.proc_threads >= 1,
             self.save_threads >= 1,
         )):
             raise ValueError(f"Invalid parameters for {self.__class__.__name__}: {things}")
 
     def __upscale__(self, input: Path, output: Path, *, echo: bool=True):
         shell(
-            self.binary,
+            self.binary(),
             "-i", input,
             "-o", output,
             "-n", self.model.value,
             "-s", self.scale,
             "-t", self.tile_size,
             "-g", self.gpu,
             "-j", f"{self.load_threads}:{self.proc_threads}:{self.save_threads}",
             "-x"*self.tta,
             stderr=DEVNULL,
             preexec_fn=self.preexec_fn,
+            cwd=self.binary().parent,
             echo=echo,
         )
 
 # -------------------------------------------------------------------------------------------------|
```

## Broken/Loaders/LoaderBytes.py

```diff
@@ -1,34 +1,34 @@
 from pathlib import Path
 from typing import Any, Optional, Union
-from Broken.Logging import log
 
 from attr import define
+from loguru import logger as log
 
-from Broken.Base import BrokenPath
+from Broken import BrokenPath
 
 from . import BrokenLoader
 
 
 @define
 class LoaderBytes(BrokenLoader):
 
     @staticmethod
     def load(value: Any=None, **kwargs) -> Optional[bytes]:
         if not value:
             return b""
 
         elif isinstance(value, bytes):
-            log.debug(f"Loading Bytes from Bytes")
+            log.debug("Loading Bytes from Bytes")
             return value
 
         elif isinstance(value, str):
-            log.debug(f"Loading Bytes from String")
+            log.debug("Loading Bytes from String")
             return value.encode()
 
-        elif (path := BrokenPath(value, valid=True)):
+        elif (path := BrokenPath(value).valid()):
             log.debug(f"Loading Bytes from Path ({path})")
             return path.read_bytes()
 
         return None
 
 LoadableBytes = Union[bytes, str, Path, None]
```

## Broken/Loaders/LoaderString.py

```diff
@@ -1,16 +1,15 @@
 from pathlib import Path
 from typing import Any, Optional, Union
 
 from attr import define
-from Broken.Logging import log
+from loguru import logger as log
 
-from Broken.Base import BrokenPath
-
-from . import BrokenLoader
+from Broken import BrokenPath
+from Broken.Loaders import BrokenLoader
 
 
 @define
 class LoaderString(BrokenLoader):
 
     @staticmethod
     def load(value: Any=None, **kwargs) -> Optional[str]:
@@ -18,17 +17,17 @@
             return ""
 
         elif isinstance(value, str):
             log.debug(f"Loading String from String {value}")
             return value
 
         elif isinstance(value, bytes):
-            log.debug(f"Loading String from Bytes")
+            log.debug("Loading String from Bytes")
             return value.decode(encoding="utf-8")
 
-        elif (path := BrokenPath(value, valid=True)):
+        elif (path := BrokenPath(value).valid()):
             log.debug(f"Loading String from Path ({path})")
             return path.read_text(encoding="utf-8")
 
         return None
 
 LoadableString = Union[str, bytes, Path, None]
```

## Broken/Loaders/__init__.py

```diff
@@ -10,7 +10,11 @@
     def __new__(cls, *args, **kwargs) -> Optional[Type]:
         return cls.load(*args, **kwargs)
 
     @staticmethod
     @abstractmethod
     def load(value: Any=None, **kwargs) -> Optional[Type]:
         ...
+
+from Broken.Loaders.LoaderBytes import LoadableBytes, LoaderBytes
+from Broken.Loaders.LoaderImage import LoadableImage, LoaderImage
+from Broken.Loaders.LoaderString import LoadableString, LoaderString
```

## DepthFlow/DepthFlow.py

```diff
@@ -1,24 +1,24 @@
 import math
-from threading import Thread
 from typing import Annotated, Iterable, Tuple
 
 import imgui
 from attr import define, field
-from PIL import Image
 from ShaderFlow import SHADERFLOW
 from ShaderFlow.Message import Message
 from ShaderFlow.Optional.Monocular import Monocular
 from ShaderFlow.Scene import ShaderScene
 from ShaderFlow.Texture import ShaderTexture
 from ShaderFlow.Variable import ShaderVariable
 from typer import Option
 
-from Broken.Base import BrokenThread
-from Broken.Loaders.LoaderPIL import LoaderImage
+from Broken import image_hash
+from Broken.Externals.Upscaler import BrokenUpscaler
+from Broken.Externals.Upscaler.ncnn import BrokenRealEsrgan
+from Broken.Loaders import LoaderImage
 from DepthFlow import DEPTHFLOW
 
 
 @define
 class DepthFlowScene(ShaderScene):
     """🌊 Image to → 2.5D Parallax Effect Video. High quality, user first."""
     __name__ = "DepthFlow"
@@ -26,109 +26,39 @@
     # Constants
     DEFAULT_IMAGE  = "https://w.wallhaven.cc/full/pk/wallhaven-pkz5r9.png"
     DEPTH_SHADER   = (DEPTHFLOW.RESOURCES.SHADERS/"DepthFlow.frag")
     LOADING_SHADER = (SHADERFLOW.RESOURCES.FRAGMENT/"Loading.frag")
 
     # DepthFlow objects
     monocular: Monocular = field(factory=Monocular)
+    upscaler: BrokenUpscaler = field(factory=BrokenRealEsrgan)
 
     # ------------------------------------------|
     # Parallax MDE and Loading screen tricky implementation
 
-    _loading:    Thread = None
-    _load_image: Image  = None
-    _load_depth: Image  = None
-
     def input(self,
-        image:  Annotated[str,   Option("--image",  "-i", help="Image to parallax (Path, URL, NumPy, PIL)")],
-        depth:  Annotated[str,   Option("--depth",  "-d", help="Depth map of the Image, None to estimate")]=None,
-        cache:  Annotated[bool,  Option("--cache",  "-c", help="Cache the Depth Map estimations")]=True,
-        width:  Annotated[int,   Option("--width",  "-w", help="Final video Width,  None for the Image's one. Adjusts to Aspect Ratio")]=None,
-        height: Annotated[int,   Option("--height", "-h", help="Final video Height, None for the Image's one. Adjusts to Aspect Ratio")]=None,
-        scale:  Annotated[float, Option("--scale",  "-s", help="Post-multiply the Image resolution by a factor")]=1.0,
-        block:  Annotated[bool,  Option("--block",  "-b", help="Freeze until Depth Map is estimated, no loading screen")]=False
+        image: Annotated[str,  Option("--image",   "-i", help="• (Basic  ) Image to Parallax (Path, URL, NumPy, PIL)")],
+        depth: Annotated[str,  Option("--depth",   "-d", help="• (Basic  ) Depthmap of the Image, None to estimate")]=None,
+        cache: Annotated[bool, Option(" /--nc",          help="• (Basic  ) Cache the Depthmap estimations on Disk")]=True,
+        ratio: Annotated[Tuple[int, int], Option("--upscale", "-u", help="• (Upscale) Upscale the Input and Depthmap respectively with Realesrgan (1, 2, 3, 4)")]=(1, 1),
     ):
-        # Already loading something
-        if self._loading and not block:
-            return
-
-        def load():
-            nonlocal image, depth, cache, width, height, scale
-            self._load_image = LoaderImage(image)
-            iwidth, iheight = self._load_image.size
-            aspect_ratio = (iwidth/iheight)
-
-            # Force resolution if both set or image's one, else ajust to aspect ratio
-            if (bool(width) == bool(height)):
-                resolution = ((width or iwidth), (height or iheight))
-            else:
-                resolution = (
-                    ((height or 0)*aspect_ratio) or width,
-                    ((width  or 0)/aspect_ratio) or height,
-                )
-
-            # The order of calling imports here for rendering
-            self.eloop.once(callback=self.resize, args=[x*scale for x in resolution])
-            self._load_depth = LoaderImage(depth) or self.monocular(image, cache=cache)
-            self.time = 0
-
-        # Start loading process
-        self.shader.fragment = self.LOADING_SHADER
-        self.shader.load_shaders()
-        self._loading = BrokenThread.new(load)
-
-        # Wait until loading finish
-        if block: self._loading.join()
-
-    # ------------------------------------------|
-
-    def ui(self) -> None:
-        if (state := imgui.slider_float("Height", self.parallax_height, 0, 1, "%.2f"))[0]:
-            self.parallax_height = max(0, state[1])
-        if (state := imgui.slider_float("Focus", self.parallax_focus, 0, 1, "%.2f"))[0]:
-            self.parallax_focus = max(0, state[1])
-        if (state := imgui.slider_float("Invert", self.parallax_invert, 0, 1, "%.2f"))[0]:
-            self.parallax_invert = max(0, state[1])
-        if (state := imgui.slider_float("Zoom", self.parallax_zoom, 0, 2, "%.2f"))[0]:
-            self.parallax_zoom = max(0, state[1])
-        if (state := imgui.slider_float("Isometric", self.parallax_isometric, 0, 1, "%.2f"))[0]:
-            self.parallax_isometric = max(0, state[1])
-        if (state := imgui.slider_float("Dolly", self.parallax_dolly, 0, 5, "%.2f"))[0]:
-            self.parallax_dolly = max(0, state[1])
-        if (state := imgui.slider_float("Offset X", self.parallax_offset[0], -2, 2, "%.2f"))[0]:
-            self.parallax_offset[0] = state[1]
-        if (state := imgui.slider_float("Offset Y", self.parallax_offset[1], -2, 2, "%.2f"))[0]:
-            self.parallax_offset[1] = state[1]
-        if (state := imgui.slider_float("Center X", self.parallax_center[0], -2, 2, "%.2f"))[0]:
-            self.parallax_center[0] = state[1]
-        if (state := imgui.slider_float("Center Y", self.parallax_center[1], -2, 2, "%.2f"))[0]:
-            self.parallax_center[1] = state[1]
-
-    def _load_new_or_default(self):
-
-        # Set default image if none provided
-        if self.image.is_empty():
-            self.input(image=DepthFlowScene.DEFAULT_IMAGE)
-
-        # Block when rendering (first Scene update)
-        if self.rendering and self.image.is_empty():
-            self._loading.join()
-
-        # Load new parallax images and parallax shader
-        if self._load_image and self._load_depth:
-            self._load_image = self.image.from_image(self._load_image) and None
-            self._load_depth = self.depth.from_image(self._load_depth) and None
-            self.shader.fragment = self.DEPTH_SHADER
-            self.shader.load_shaders()
-            self._loading = None
-            self.time = 0
+        image = LoaderImage(image)
+        depth = LoaderImage(depth) or self.monocular.estimate(image, cache=cache)
+        width, height = image.size
+        cache = DEPTHFLOW.DIRECTORIES.CACHE/f"{image_hash(image)}"
+        depth = self.upscaler.upscale(depth, scale=ratio[1])
+        image = self.upscaler.upscale(image, scale=ratio[0])
+        self.aspect_ratio = (width/height)
+        self.image.from_image(image)
+        self.depth.from_image(depth)
+        self.time = 0
 
     # ------------------------------------------|
 
-    parallax_height: float = field(default=0.3)
+    parallax_height: float = field(default=0.2)
     """Peak value of the Depth Map, in the range [0, 1]. The camera is 1 distance away from depth=0
     at the z=1 plane, so this also controls the intensity of the effect"""
 
     parallax_focus: float = field(default=0.0)
     """Focal depth of the effect, in the range [0, 1]. A value of 0 makes the background (depth=0)
     stationary, while a value of 1 makes the foreground (depth=1) stationary on displacements"""
 
@@ -141,33 +71,34 @@
     parallax_isometric: float = field(default=0.0)
     """Isometric factor of the camera projection. Zero is fully perspective, 1 is orthographic"""
 
     parallax_dolly: float = field(default=0.0)
     """Same effect as isometric, but with "natural units" of AFAIK `isometric = atan(dolly)*(2/pi)`.
     Keeps the ray target constant and move back ray origins by this amount"""
 
-    parallax_offset: Tuple[float, float] = field(factory=lambda: [0, 0])
+    parallax_offset: Tuple[float, float] = field(factory=lambda: [0.0, 0.0])
     """The effect displacement offset, change this over time for the 3D parallax effect"""
 
-    parallax_center: Tuple[float, float] = field(factory=lambda: [0, 0])
+    parallax_center: Tuple[float, float] = field(factory=lambda: [0.0, 0.0])
     """Focal point of the offsets, use this to center off-screen objects"""
 
     def commands(self):
         self.broken_typer.command(self.input)
 
     def setup(self):
-        self._load_new_or_default()
+        if self.image.is_empty():
+            self.input(image=DepthFlowScene.DEFAULT_IMAGE)
 
     def build(self):
         ShaderScene.build(self)
         self.image = ShaderTexture(scene=self, name="image").repeat(False)
         self.depth = ShaderTexture(scene=self, name="depth").repeat(False)
+        self.shader.fragment = self.DEPTH_SHADER
 
     def update(self):
-        self._load_new_or_default()
 
         # In and out dolly zoom
         self.parallax_dolly = 0.5*(1 + math.cos(self.time))
 
         # Infinite 8 loop shift
         self.parallax_offset = [
             0.1 * math.sin(self.time),
@@ -181,14 +112,15 @@
         )
 
         # Zoom in on the start
         # self.parallax_zoom = 1.2 - 0.2*(2/math.pi)*math.atan(self.time)
 
     def handle(self, message: Message):
         ShaderScene.handle(self, message)
+
         if isinstance(message, Message.Window.FileDrop):
             files = iter(message.files)
             self.input(image=next(files), depth=next(files, None))
 
     def pipeline(self) -> Iterable[ShaderVariable]:
         yield from ShaderScene.pipeline(self)
         yield ShaderVariable("uniform", "float", "iParallaxHeight",    self.parallax_height)
@@ -196,14 +128,38 @@
         yield ShaderVariable("uniform", "float", "iParallaxInvert",    self.parallax_invert)
         yield ShaderVariable("uniform", "float", "iParallaxZoom",      self.parallax_zoom)
         yield ShaderVariable("uniform", "float", "iParallaxIsometric", self.parallax_isometric)
         yield ShaderVariable("uniform", "float", "iParallaxDolly",     self.parallax_dolly)
         yield ShaderVariable("uniform", "vec2",  "iParallaxOffset",    self.parallax_offset)
         yield ShaderVariable("uniform", "vec2",  "iParallaxCenter",    self.parallax_center)
 
+    # ------------------------------------------|
+
+    def ui(self) -> None:
+        if (state := imgui.slider_float("Height", self.parallax_height, 0, 1, "%.2f"))[0]:
+            self.parallax_height = max(0, state[1])
+        if (state := imgui.slider_float("Focus", self.parallax_focus, 0, 1, "%.2f"))[0]:
+            self.parallax_focus = max(0, state[1])
+        if (state := imgui.slider_float("Invert", self.parallax_invert, 0, 1, "%.2f"))[0]:
+            self.parallax_invert = max(0, state[1])
+        if (state := imgui.slider_float("Zoom", self.parallax_zoom, 0, 2, "%.2f"))[0]:
+            self.parallax_zoom = max(0, state[1])
+        if (state := imgui.slider_float("Isometric", self.parallax_isometric, 0, 1, "%.2f"))[0]:
+            self.parallax_isometric = max(0, state[1])
+        if (state := imgui.slider_float("Dolly", self.parallax_dolly, 0, 5, "%.2f"))[0]:
+            self.parallax_dolly = max(0, state[1])
+        if (state := imgui.slider_float("Offset X", self.parallax_offset[0], -2, 2, "%.2f"))[0]:
+            self.parallax_offset[0] = state[1]
+        if (state := imgui.slider_float("Offset Y", self.parallax_offset[1], -2, 2, "%.2f"))[0]:
+            self.parallax_offset[1] = state[1]
+        if (state := imgui.slider_float("Center X", self.parallax_center[0], -2, 2, "%.2f"))[0]:
+            self.parallax_center[0] = state[1]
+        if (state := imgui.slider_float("Center Y", self.parallax_center[1], -2, 2, "%.2f"))[0]:
+            self.parallax_center[1] = state[1]
+
 # -------------------------------------------------------------------------------------------------|
 
 class YourFlow(DepthFlowScene):
     """Example of defining your own class based on DepthFlowScene"""
 
     def update(self):
         DepthFlowScene.update(self)
```

## DepthFlow/__init__.py

```diff
@@ -1,16 +1,14 @@
 
 import Broken
 import DepthFlow.Resources as DepthFlowResources
-from Broken.Base import BrokenTorch
-from Broken.Project import BrokenProject
+from Broken import BrokenProject, BrokenTorch
 
 DEPTHFLOW = BrokenProject(
     PACKAGE=__file__,
     APP_NAME="DepthFlow",
     APP_AUTHOR="BrokenSource",
     RESOURCES=DepthFlowResources,
 )
 
 Broken.set_project(DEPTHFLOW)
-
 BrokenTorch.manage(DEPTHFLOW.RESOURCES)
```

## DepthFlow/__main__.py

```diff
@@ -1,16 +1,15 @@
 import sys
 
-from Broken.Base import BrokenProfiler
+from Broken import BrokenProfiler
 from DepthFlow import DEPTHFLOW
 from DepthFlow.DepthFlow import DepthFlowScene
 
 
 def main():
     with BrokenProfiler("DEPTHFLOW"):
         DEPTHFLOW.welcome()
         depthflow = DepthFlowScene()
         depthflow.cli(sys.argv[1:])
-        depthflow.destroy()
 
 if __name__ == "__main__":
     main()
```

## DepthFlow/Resources/Shaders/DepthFlow.frag

```diff
@@ -38,38 +38,38 @@
 
     // The distance Beta we care for the depth map
     float delta = abs(tan(theta) * (1 - iCamera.origin.z - iParallaxHeight));
     float alpha = abs(tan(theta) * (1 - iCamera.origin.z));
     float beta  = abs(alpha - delta);
 
     // Start the parallax on the point itself
-    vec2 parallax = gluv2stuv(sigma);
+    vec2 parallax = sigma;
 
     // The quality of the parallax effect is how tiny the steps are
-    const float min_quality = 0.07;
+    const float min_quality = 0.05;
     const float max_quality = 0.002;
     float quality = mix(min_quality, max_quality, iQuality);
 
     // Note: The Very Expensive Loop
     // Fixme: Can we smartly cache the last walk distance?
     // Fixme: Calculate walk distance based on pixel and angle?
     for (float i=1; i>0; i-=quality) {
 
         // Get the uv we'll check for the heights
-        vec2 sample = gluv2stuv(sigma + i*beta*walk);
+        vec2 sample = sigma + (i*beta*walk);
 
         // Interpolate between (0=max) and (0=min) depending on focus
-        float height       = draw_image(depth, sample).r;
+        float height       = gmtexture(depth, sample).r;
         float depth_height = iParallaxHeight * mix(height, 1-height, iParallaxInvert);
         float walk_height  = (i*beta) / tan(theta);
 
         // Stop whenever an intersection is found
         if (depth_height >= walk_height) {
             parallax = sample;
             break;
         }
     }
 
     // Draw the parallax image
-    fragColor = draw_image(image, parallax);
+    fragColor = gmtexture(image, parallax);
 }
```

## Pianola/Pianola.py

```diff
@@ -1,20 +1,19 @@
 from pathlib import Path
 from typing import Annotated
 
 from attr import define
+from loguru import logger as log
 from ShaderFlow.Message import Message
 from ShaderFlow.Modules.Audio import ShaderAudio
 from ShaderFlow.Modules.Piano import ShaderPiano
 from ShaderFlow.Scene import ShaderScene
 from typer import Option
 
-from Broken.Base import BrokenPath
-from Broken.BrokenEnum import BrokenEnum
-from Broken.Logging import log
+from Broken import BrokenEnum, BrokenPath
 from Pianola import PIANOLA
 
 
 class PianolaSoundFont(BrokenEnum):
     Salamander = "https://freepats.zenvoid.org/Piano/SalamanderGrandPiano/SalamanderGrandPiano-SF2-V3+20200602.tar.xz"
     """# Note: Salamander Grand Piano, Licensed under CC BY 3.0, by Alexander Holm"""
```

## Pianola/__main__.py

```diff
@@ -1,10 +1,10 @@
 import sys
 
-from Broken.Base import BrokenProfiler
+from Broken import BrokenProfiler
 from Pianola import PIANOLA
 from Pianola.Pianola import PianolaScene
 
 
 def main():
     with BrokenProfiler("PIANOLA"):
         PIANOLA.welcome()
```

## ShaderFlow/Message.py

```diff
@@ -111,15 +111,15 @@
     class Shader:
 
         @define
         class RecreateTextures:
             ...
 
         @define
-        class ReloadShaders:
+        class Compile:
             ...
 
         @define
         class Render:
             ...
 
     # # Keyboard
```

## ShaderFlow/Module.py

```diff
@@ -1,26 +1,18 @@
 from __future__ import annotations
 
 import itertools
 from abc import abstractmethod
-from typing import Any
-from typing import Iterable
-from typing import Self
-from typing import Type
-from typing import Union
-
-from attr import Factory
-from attr import define
-from attr import field
-
-from Broken.Base import BrokenAttrs
-from Broken.Base import BrokenFluentBuilder
-from Broken.Base import BrokenUtils
+from typing import Any, Iterable, Self, Type, Union
+
+from attr import Factory, define, field
+from loguru import logger as log
+
+from Broken import BrokenAttrs, BrokenFluentBuilder, extend
 from Broken.Externals.FFmpeg import BrokenFFmpeg
-from Broken.Logging import log
 from ShaderFlow.Message import Message
 from ShaderFlow.Variable import ShaderVariable
 
 
 @define
 class ShaderModule(BrokenFluentBuilder, BrokenAttrs):
     scene: Any = field(default=None, repr=False)
@@ -30,25 +22,25 @@
     def __post__(self):
         self.scene = self.scene or self
         self.scene.modules.append(self)
         log.info(f"{self.who} Module added to the Scene")
 
     @property
     def who(self) -> str:
-        return f"({self.uuid:>2}) [{{color}}]{type(self).__name__[:18].ljust(18)}[/{{color}}] │ ▸"
+        return f"({self.uuid:>2}) {type(self).__name__[:18].ljust(18)} │ ▸"
 
     def find(self, type: Type[ShaderModule]) -> Iterable[ShaderModule]:
         for module in self.scene.modules:
             if isinstance(module, type):
                 yield module
 
     @staticmethod
     def make_findable(type: ShaderModule) -> None:
         name = type.__name__.lower()
-        BrokenUtils.extend(ShaderModule, name=name, as_property=True)(
+        extend(ShaderModule, name=name, as_property=True)(
             lambda self: next(self.find(type=type))
         )
 
     # # Messaging
 
     def relay(self, message: Union[Message, Type[Message]]) -> Self:
         if isinstance(message, type):
@@ -70,14 +62,19 @@
 
     @abstractmethod
     def defines(self) -> Iterable[str]:
         yield None
 
     # ------------------------------------------|
 
+    @property
+    @abstractmethod
+    def duration(self) -> float:
+        return 0.0
+
     @abstractmethod
     def build(self) -> None:
         pass
 
     @abstractmethod
     def setup(self) -> None:
         pass
```

## ShaderFlow/Notes.py

```diff
@@ -1,15 +1,14 @@
 import functools
 import math
-from typing import Any
-from typing import Self
+from typing import Any, Self
 
 from attr import define
 
-from Broken.Base import BrokenFluentBuilder
+from Broken import BrokenFluentBuilder
 
 PIANO_NOTES = "C C# D D# E F F# G G# A A# B".split()
 
 @define(eq=False)
 class BrokenPianoNote(BrokenFluentBuilder):
     note:     int   = 60
     start:    float = 0
```

## ShaderFlow/Scene.py

```diff
@@ -1,147 +1,215 @@
 import importlib
 import math
 import os
+import time
 from abc import abstractmethod
 from collections import deque
 from pathlib import Path
 from subprocess import PIPE
-from typing import Annotated, Any, Deque, Dict, Iterable, List, Optional, Self, Tuple
+from typing import (
+    Annotated,
+    Any,
+    Deque,
+    Dict,
+    Iterable,
+    List,
+    Optional,
+    Self,
+    Tuple,
+)
 
 import glfw
 import imgui
 import moderngl
 import PIL
 import tqdm
 from attr import Factory, define, field
 from dotmap import DotMap
+from loguru import logger as log
 from moderngl_window.context.base import BaseWindow as ModernglWindow
 from moderngl_window.integrations.imgui import ModernglWindowRenderer as ModernglImgui
 from typer import Option
 
 import Broken
-from Broken import BROKEN
-from Broken.Base import (
-    BrokenEventClient,
-    BrokenEventLoop,
+from Broken import (
+    BrokenEnum,
     BrokenPath,
     BrokenPlatform,
+    BrokenResolution,
+    BrokenScheduler,
+    BrokenTask,
     BrokenThread,
     BrokenTyper,
-    BrokenUtils,
-    Ignore,
     SameTracker,
     clamp,
     denum,
     flatten,
 )
-from Broken.BrokenEnum import BrokenEnum
 from Broken.Externals.FFmpeg import (
     BrokenFFmpeg,
     FFmpegAudioCodec,
     FFmpegFilterFactory,
     FFmpegFormat,
     FFmpegH264Preset,
     FFmpegH264Quality,
     FFmpegH264Tune,
     FFmpegHWAccel,
     FFmpegPixelFormat,
     FFmpegVideoCodec,
 )
-from Broken.Loaders.LoaderBytes import LoaderBytes
-from Broken.Loaders.LoaderString import LoaderString
-from Broken.Logging import log
+from Broken.Loaders import LoaderBytes, LoaderString
 from Broken.Types import Hertz, Seconds, Unchanged
 from ShaderFlow import SHADERFLOW
 from ShaderFlow.Message import Message
 from ShaderFlow.Module import ShaderModule
-from ShaderFlow.Modules.Audio import ShaderAudio
 from ShaderFlow.Modules.Camera import ShaderCamera
 from ShaderFlow.Modules.Dynamics import DynamicNumber
 from ShaderFlow.Modules.Frametimer import ShaderFrametimer
 from ShaderFlow.Modules.Keyboard import ShaderKeyboard
-from ShaderFlow.Shader import Shader
+from ShaderFlow.Shader import ShaderObject
 from ShaderFlow.Variable import ShaderVariable
 
 
 class ShaderBackend(BrokenEnum):
     Headless = "headless"
     GLFW     = "glfw"
 
 @define
 class ShaderScene(ShaderModule):
     __name__ = "Scene"
 
+    # # Base modules
+
     modules: Deque[ShaderModule] = Factory(deque)
     """Deque of all Modules on the Scene, not a set for order preservation"""
 
+    # Scheduling
+    scheduler: BrokenScheduler = Factory(BrokenScheduler)
+    vsync: BrokenTask = None
+
+    # ShaderFlow modules
+    camera: ShaderCamera = None
+    keyboard: ShaderKeyboard = None
+    ffmpeg: BrokenFFmpeg = None
+
+    # # Fractional SSAA
+
+    _final: ShaderObject = None
     """
-    Implementing Fractional SSAA is a bit tricky:
+    Implementing Fractional Super-Sampling Anti-Aliasing (SSAA) is a bit tricky:
     • A Window's FBO always match its real resolution (can't final render in other resolution)
     • We need a final shader to sample from some other SSAA-ed texture to the window
 
-    For that, a internal self._final is used to sample from the user's main self.engine
+    For that, a internal self._final is used to sample from the user's main self.shader
     • _final: Uses the FBO of the Window, simply samples from a `final` texture to the screen
-    • engine: Scene's main engine, where the user's final shader is rendered to
+    • shader: Scene's main Shader, where the user's final shader is rendered to
     """
-    _final: Shader = None
-    shader: Shader = None
-    camera: ShaderCamera = None
-    keyboard: ShaderKeyboard = None
+
+    shader: ShaderObject = None
+    """The main ShaderObject of the Scene, the visible content of the Window"""
+
+    alpha: bool = False
+    """Makes the final texture have an alpha channel, useful for transparent windows. Exporting
+    videos might fail, perhaps output a Chroma Key compatible video - add this to the shader:
+    - `fragColor.rgb = mix(vec3(0, 1, 0), fragColor.rgb, fragColor.a);`"""
 
     def build(self):
 
         # Init Imgui
         imgui.create_context()
         self.imguio = imgui.get_io()
-        self.imguio.font_global_scale = SHADERFLOW.CONFIG.imgui.default("font_scale", 1.0)
+        self.imguio.font_global_scale = 1
         self.imguio.fonts.add_font_from_file_ttf(
-            str(BROKEN.RESOURCES.FONTS/"DejaVuSans.ttf"),
+            str(Broken.BROKEN.RESOURCES.FONTS/"DejaVuSans.ttf"),
             16*self.imguio.font_global_scale,
         )
 
         # Default modules
         self.init_window()
         log.info(f"{self.who} Adding default base Scene modules")
         ShaderFrametimer(scene=self)
         self.keyboard = ShaderKeyboard(scene=self)
         self.camera   = ShaderCamera(scene=self)
 
         # Create the SSAA Workaround engines
         log.info(f"{self.who} Creating SSAA Implementation")
-        self.shader = Shader(self)
+        self.shader = ShaderObject(self)
         self.shader.texture.name = "iScreen"
         self.shader.texture.track = True
-        self._final = Shader(self)
-        self._final.texture.components = 3
+        self._final = ShaderObject(self)
+        self._final.texture.components = 3 + int(self.alpha)
         self._final.texture.dtype = "f1"
         self._final.texture.final = True
         self._final.texture.track = True
         self._final.fragment = (SHADERFLOW.RESOURCES.FRAGMENT/"Final.glsl")
 
     # ---------------------------------------------------------------------------------------------|
-    # Basic information
+    # Temporal
+
+    time: Seconds = 0.0
+    """Current time in seconds. Ideally, everything should depend on time, for flexibility"""
+
+    tempo: float = Factory(lambda: DynamicNumber(value=1, frequency=3))
+    """Time scale factor, used for `dt`, which integrates to `time`"""
+
+    runtime: float = field(default=10.0, converter=float)
+    """The longest module duration; overriden by the user; or default length of 10s"""
 
-    time:       Seconds = 0.0
-    duration:   Seconds = 10.0
-    time_scale: float   = Factory(lambda: DynamicNumber(value=1, frequency=5))
-    frame:      int     = 0
-    fps:        Hertz   = 60.0
-    dt:         Seconds = 0.0
-    rdt:        Seconds = 0.0
-
-    # Base classes and utils for a Scene
-    eloop:  BrokenEventLoop   = Factory(BrokenEventLoop)
-    vsync:  BrokenEventClient = None
-    ffmpeg: BrokenFFmpeg      = None
+    fps: Hertz = 60.0
+    """Target frames per second rendering speed"""
+
+    dt: Seconds = 0.0
+    """Virtual delta time since last frame, time scaled by `tempo`"""
+
+    rdt: Seconds = 0.0
+    """Real life, physical delta time since last frame"""
+
+    @property
+    def tau(self) -> float:
+        """Normalized time value between 0 and 1"""
+        return self.time / self.runtime
 
     @property
     def frametime(self) -> Seconds:
+        """Ideal time between two frames, coupled with `fps`"""
         return 1/self.fps
 
+    @frametime.setter
+    def frametime(self, value: Seconds) -> None:
+        self.fps = 1/value
+
+    @property
+    def frame(self) -> int:
+        """Current frame being rendered. Coupled with 'time' and 'fps'"""
+        return int(self.time * self.fps)
+
+    @frame.setter
+    def frame(self, value: int) -> None:
+        self.time = value / self.fps
+
+    # Total Duration
+
+    @property
+    def duration(self) -> float:
+        return self.runtime
+
+    def set_duration(self, override: float=None, *, default: float=10) -> float:
+        self.runtime = (override or default)
+        for module in (not bool(override)) * self.modules:
+            self.runtime = max(self.runtime, module.duration)
+        return self.runtime
+
+    @property
+    def total_frames(self) -> int:
+        return int(self.runtime * self.fps)
+
+    # ---------------------------------------------------------------------------------------------|
+    # Window synchronized properties
+
     # # Title
 
     _title: str = "ShaderFlow"
 
     @property
     def title(self) -> str:
         return self._title
@@ -176,75 +244,124 @@
 
     @visible.setter
     def visible(self, value: bool) -> None:
         log.info(f"{self.who} Changing Window Visibility to ({value})")
         self.window.visible = value
         self._visible = value
 
+    # # Window Fullscreen
+
+    _fullscreen: bool = False
+
+    @property
+    def fullscreen(self) -> bool:
+        return self._fullscreen
+
+    @fullscreen.setter
+    def fullscreen(self, value: bool) -> None:
+        log.info(f"{self.who} Changing Window Fullscreen to ({value})")
+        self._fullscreen = value
+        try:
+            self.window.fullscreen = value
+        except AttributeError:
+            pass
+
+    # # Window Exclusive
+
+    _exclusive: bool = False
+
+    @property
+    def exclusive(self) -> bool:
+        return self._exclusive
+
+    @exclusive.setter
+    def exclusive(self, value: bool) -> None:
+        log.info(f"{self.who} Changing Window Exclusive to ({value})")
+        self.window.mouse_exclusivity = value
+        self._exclusive = value
+
     # # Video modes and monitor
 
     monitor: int = os.environ.get("MONITOR", 0)
 
     @property
     def glfw_monitor(self) -> Optional[glfw._GLFWmonitor]:
         if (monitors := glfw.get_monitors()):
             return monitors[self.monitor]
 
     @property
-    def video_mode(self) -> Optional[Dict]:
+    def glfw_video_mode(self) -> Optional[Dict]:
         if (monitor := self.glfw_monitor):
             return glfw.get_video_mode(monitor)
 
     @property
-    def monitor_framerate(self) -> Optional[float]:
-        if (mode := self.video_mode):
-            return mode.refresh_rate
+    def monitor_framerate(self) -> float:
+        """Note: Defaults to 60 if no monitor is found"""
+        if (mode := self.glfw_video_mode):
+            return mode.refresh_rate or 60.0
+        return 60.0
 
     @property
-    def monitor_resolution(self) -> Optional[Tuple[int, int]]:
-        if (mode := self.video_mode):
+    def monitor_size(self) -> Optional[Tuple[int, int]]:
+        if self.exporting:
+            return None
+        if (mode := self.glfw_video_mode):
             return (mode.size.width, mode.size.height)
 
-    # # Resolution
+    @property
+    def monitor_width(self) -> Optional[int]:
+        if (resolution := self.monitor_size):
+            return resolution[0]
+
+    @property
+    def monitor_height(self) -> Optional[int]:
+        if (resolution := self.monitor_size):
+            return resolution[1]
+
+    # ---------------------------------------------------------------------------------------------|
+    # Resolution
 
     quality: float = field(default=80,   converter=lambda x: clamp(x, 0, 100))
     _ssaa:   float = field(default=1.0,  converter=lambda x: max(0.01, x))
-    _width:  int   = field(default=1920, converter=lambda x: max(1, x))
-    _height: int   = field(default=1080, converter=lambda x: max(1, x))
+    _width:  int   = field(default=1920, converter=lambda x: int(max(1, x)))
+    _height: int   = field(default=1080, converter=lambda x: int(max(1, x)))
 
-    def resize(self, width: int=Unchanged, height: int=Unchanged) -> Self:
+    def resize(self, width: int=Unchanged, height: int=Unchanged, *, scale: float=1) -> Tuple[int, int]:
         """
         Resize the true final rendering resolution of the Scene
         - Rounded to nearest multiple of 2, so FFmpeg is happy
         - Limited by the Monitor resolution if Realtime
         - Safe to use floats as input arguments
-        - Use None to not change the resolution component
+        - Use None to not change this resolution component
         - Doesn't signal a resize if same resolution as before
 
         Args:
             width:  New width of the Scene, None to not change
             height: New height of the Scene, None to not change
 
         Returns:
-            Self, Fluent interface
+            Self: Fluent interface
         """
-        resolution = BrokenUtils.round_resolution(width or self._width, height or self._height)
-        limited    = tuple(map(min, resolution, self.monitor_resolution or resolution))
-        resolution = resolution if (not self.realtime) else limited
+        resolution = BrokenResolution.fit(
+            ow=self.width, oh=self.height, nw=width, nh=height,
+            mw=self.monitor_width, mh=self.monitor_height,
+            sc=scale, ar=self._aspect_ratio,
+        )
 
         # Optimization: Only resize when resolution changes
         if resolution != (self._width, self._height):
-            log.info(f"{self.who} Resizing window to resolution {self.resolution}")
+            log.info(f"{self.who} Resizing window to resolution {resolution}")
+            self.window.fbo.viewport = (0, 0, self.width, self.height)
             self._width, self._height = resolution
-            self.opengl.screen.viewport = (0, 0, self.width, self.height)
-            self.window.size = self.resolution
-        return self
+            self.window.size = resolution
+            self.relay(Message.Shader.RecreateTextures)
+        return self.resolution
 
     def read_screen(self) -> bytes:
-        return self.opengl.screen.read(viewport=(0, 0, self.width, self.height))
+        return self.window.fbo.read(viewport=(0, 0, self.width, self.height))
 
     # # Resolution related
 
     @property
     def width(self) -> int:
         return self._width
 
@@ -276,50 +393,35 @@
     def ssaa(self, value: float) -> None:
         log.info(f"{self.who} Changing Fractional SSAA to {value}")
         self._ssaa = value
         self.relay(Message.Shader.RecreateTextures)
 
     @property
     def render_resolution(self) -> Tuple[int, int]:
-        return BrokenUtils.round_resolution(self.width*self.ssaa, self.height*self.ssaa)
-
-    @property
-    def aspect_ratio(self) -> float:
-        return self.width / self.height
-
-    # # Window Fullscreen
-
-    _fullscreen: bool = False
-
-    @property
-    def fullscreen(self) -> bool:
-        return self._fullscreen
-
-    @fullscreen.setter
-    def fullscreen(self, value: bool) -> None:
-        log.info(f"{self.who} Changing Window Fullscreen to ({value})")
-        self._fullscreen = value
-
-    # # Window Exclusive
+        return BrokenResolution.round(self.width*self.ssaa, self.height*self.ssaa)
 
-    _exclusive: bool = False
+    _aspect_ratio: float = None
 
     @property
-    def exclusive(self) -> bool:
-        return self._exclusive
+    def aspect_ratio(self) -> float:
+        """Either the forced `self._aspect_ratio` or dynamic from `self.width/self.height`"""
+        return self._aspect_ratio or (self.width/self.height)
 
-    @exclusive.setter
-    def exclusive(self, value: bool) -> None:
-        log.info(f"{self.who} Changing Window Exclusive to ({value})")
-        self.window.mouse_exclusivity = value
-        self._exclusive = value
+    @aspect_ratio.setter
+    def aspect_ratio(self, value: float) -> None:
+        log.info(f"{self.who} Changing Aspect Ratio to {value}")
+        self._aspect_ratio = value
+
+        if (self.backend == ShaderBackend.GLFW):
+            w, h = (int(10000*value), 10000) if bool(value) else (glfw.DONT_CARE, glfw.DONT_CARE)
+            glfw.set_window_aspect_ratio(self.window._window, w, h)
 
     # # Backend
 
-    _backend: ShaderBackend = ShaderBackend.get(os.environ.get("SHADERFLOW_BACKEND", ShaderBackend.GLFW))
+    backend: ShaderBackend = ShaderBackend.get(os.environ.get("SHADERFLOW_BACKEND", ShaderBackend.GLFW))
     """The ModernGL Window Backend. Cannot be changed after creation."""
 
     opengl: moderngl.Context = None
     """ModernGL Context of this Scene"""
 
     window: ModernglWindow = None
     """ModernGL Window object with context/backend defined on self._backend"""
@@ -333,25 +435,30 @@
     # Todo: Proper UI classes? For main menu, settings, exporting, etc
     render_ui: bool = False
     """Whether to render the Main UI"""
 
     def init_window(self) -> None:
         """Create the window and the OpenGL context"""
         log.info(f"{self.who} Creating Window and OpenGL Context")
-        log.info(f"{self.who} • Backend:    {denum(self._backend)}")
+        log.info(f"{self.who} • Backend:    {denum(self.backend)}")
         log.info(f"{self.who} • Resolution: {self.resolution}")
 
-        module = f"moderngl_window.context.{denum(self._backend).lower()}"
+        # Provide GPU Acceleration on headless rendering, as xvfb-run is software rendering
+        # https://forums.developer.nvidia.com/t/81412 - Comments 2 and 6
+        backend = "egl" * (self.backend == ShaderBackend.Headless) * (BrokenPlatform.OnLinux) or None
+
+        module = f"moderngl_window.context.{denum(self.backend).lower()}"
         self.window = importlib.import_module(module).Window(
             size=self.resolution,
             title=self.title,
             resizable=self.resizable,
             visible=self.visible,
             fullscreen=self.fullscreen,
             vsync=False,
+            backend=backend
         )
         ShaderKeyboard.set_keymap(self.window.keys)
         self.imgui  = ModernglImgui(self.window)
         self.opengl = self.window.ctx
 
         # Bind window events to relay
         self.window.resize_func               = self.__window_resize__
@@ -362,347 +469,183 @@
         self.window.mouse_press_event_func    = self.__window_mouse_press_event__
         self.window.mouse_release_event_func  = self.__window_mouse_release_event__
         self.window.mouse_drag_event_func     = self.__window_mouse_drag_event__
         self.window.mouse_scroll_event_func   = self.__window_mouse_scroll_event__
         self.window.unicode_char_entered_func = self.__window_unicode_char_entered__
         self.window.files_dropped_event_func  = self.__window_files_dropped_event__
 
-        if (self._backend == ShaderBackend.GLFW):
-            BrokenThread.new(target=self.window.set_icon, icon_path=Broken.PROJECT.RESOURCES.ICON)
+        if (self.backend == ShaderBackend.GLFW):
+            BrokenThread.new(target=self.window.set_icon, icon_path=Broken.PROJECT.RESOURCES.ICON, daemon=True)
             glfw.set_cursor_enter_callback(self.window._window, lambda _, enter: self.__window_mouse_enter_event__(inside=enter))
             glfw.set_drop_callback(self.window._window, self.__window_files_dropped_event__)
             ShaderKeyboard.Keys.LEFT_SHIFT = glfw.KEY_LEFT_SHIFT
             ShaderKeyboard.Keys.LEFT_CTRL  = glfw.KEY_LEFT_CONTROL
             ShaderKeyboard.Keys.LEFT_ALT   = glfw.KEY_LEFT_ALT
             # glfw.maximize_window(self.window._window)
 
         log.debug(f"{self.who} Finished Window creation")
 
     # ---------------------------------------------------------------------------------------------|
-    # Module
-
-    def handle(self, message: Message) -> None:
-
-        if isinstance(message, Message.Window.Close):
-            log.info(f"{self.who} Received Window Close Event")
-            self.quit()
-
-        elif isinstance(message, Message.Keyboard.KeyDown):
-            if message.key == ShaderKeyboard.Keys.O:
-                log.info(f"{self.who} (  O) Resetting the Scene")
-                for module in self.modules:
-                    module.setup()
-
-            elif message.key == ShaderKeyboard.Keys.R:
-                log.info(f"{self.who} (  R) Reloading Shaders")
-                for module in self.modules:
-                    if isinstance(module, Shader):
-                        module.load_shaders()
+    # User actions
 
-            elif message.key == ShaderKeyboard.Keys.TAB:
-                log.info(f"{self.who} (TAB) Toggling Menu")
-                self.render_ui  = not self.render_ui
+    @abstractmethod
+    def commands(self) -> None:
+        """Configure commands for the Scene. Add with self.broken_typer.command(...)"""
+        ...
 
-            elif message.key == ShaderKeyboard.Keys.F1:
-                log.info(f"{self.who} ( F1) Toggling Exclusive Mode")
-                self.exclusive  = not self.exclusive
+    _built: SameTracker = Factory(SameTracker)
 
-            elif message.key == ShaderKeyboard.Keys.F2:
-                import arrow
-                time  = arrow.now().format("YYYY-MM-DD_HH-mm-ss")
-                image = PIL.Image.frombytes("RGB", self.resolution, self.read_screen())
-                image = image.transpose(PIL.Image.FLIP_TOP_BOTTOM)
-                path  = Broken.PROJECT.DIRECTORIES.SCREENSHOTS/f"({time}) {self.__name__}.jpg"
-                BrokenThread.new(target=image.save, fp=path, mode="JPEG", quality=95)
-                log.minor(f"{self.who} ( F2) Saved Screenshot to ({path})")
+    def cli(self, *args: List[str]):
+        args = flatten(args)
+        self.broken_typer = BrokenTyper(chain=True)
+        self.broken_typer.command(self.main, context=True, default=True)
+        self.commands()
+        if ("--help" not in args) and (not self._built(True)):
+            self.build()
+        self.broken_typer(args)
 
-            elif message.key == ShaderKeyboard.Keys.F11:
-                log.info(f"{self.who} (F11) Toggling Fullscreen")
-                self.fullscreen = not self.fullscreen
+    @property
+    def directory(self) -> Path:
+        """Directory of the current Scene script"""
+        # Fixme: How to deal with ShaderFlow as a dependency scenario?
+        return BrokenPath(SHADERFLOW.DIRECTORIES.CURRENT_SCENE)
 
-        elif isinstance(message, (Message.Mouse.Drag, Message.Mouse.Position)):
-            self.mouse_gluv = (message.u, message.v)
+    def read_file(self, file: Path, bytes: bool=False) -> str | bytes:
+        """
+        Read a file relative to the current Scene Python script
 
-    def pipeline(self) -> Iterable[ShaderVariable]:
-        yield ShaderVariable("uniform", "float", "iTime",        self.time)
-        yield ShaderVariable("uniform", "float", "iDuration",    self.duration)
-        yield ShaderVariable("uniform", "float", "iDeltaTime",   self.dt)
-        yield ShaderVariable("uniform", "vec2",  "iResolution",  self.resolution)
-        yield ShaderVariable("uniform", "float", "iQuality",     self.quality/100)
-        yield ShaderVariable("uniform", "float", "iSSAA",        self.ssaa)
-        yield ShaderVariable("uniform", "float", "iFrameRate",   self.fps)
-        yield ShaderVariable("uniform", "int",   "iFrame",       self.frame)
-        yield ShaderVariable("uniform", "bool",  "iRealtime",    self.realtime)
-        yield ShaderVariable("uniform", "vec2",  "iMouse",       self.mouse_gluv)
-        yield ShaderVariable("uniform", "bool",  "iMouseInside", self.mouse_inside)
-        for i in range(1, 6):
-            yield ShaderVariable("uniform", "bool", f"iMouse{i}", self.mouse_buttons[i])
+        Args:
+            `file`:  File to read, relative to the current Scene script directory
+            `bytes`: Whether to read the file as bytes, defaults to text
 
-    # Todo: Move to a Utils class for other stuff such as theming?
-    # Fixme: Move to somewhere better
-    def _render_ui(self):
-        if not self.render_ui:
-            return
+        Returns:
+            File contents as text or bytes
+        """
+        file = (self.directory/file)
+        log.info(f"{self.who} Reading file ({file})")
+        return LoaderBytes(file) if bytes else LoaderString(file)
 
-        self._final.texture.fbo().use()
-        imgui.push_style_var(imgui.STYLE_WINDOW_BORDERSIZE, 0.0)
-        imgui.push_style_var(imgui.STYLE_WINDOW_ROUNDING, 8)
-        imgui.push_style_var(imgui.STYLE_TAB_ROUNDING, 8)
-        imgui.push_style_var(imgui.STYLE_GRAB_ROUNDING, 8)
-        imgui.push_style_var(imgui.STYLE_FRAME_ROUNDING, 8)
-        imgui.push_style_var(imgui.STYLE_CHILD_ROUNDING, 8)
-        imgui.push_style_color(imgui.COLOR_FRAME_BACKGROUND, 0.1, 0.1, 0.1, 0.5)
-        imgui.new_frame()
-        imgui.set_next_window_position(0, 0)
-        imgui.set_next_window_bg_alpha(0.6)
-        imgui.begin(f"{self.__name__}", False, imgui.WINDOW_NO_MOVE | imgui.WINDOW_NO_RESIZE | imgui.WINDOW_NO_COLLAPSE  | imgui.WINDOW_ALWAYS_AUTO_RESIZE)
+    # ---------------------------------------------------------------------------------------------|
+    # Main event loop
 
-        # Render every module
-        for module in self.modules:
-            if imgui.tree_node(f"{module.uuid:>2} - {type(module).__name__.replace('ShaderFlow', '')}", imgui.TREE_NODE_BULLET):
-                imgui.separator()
-                module.__shaderflow_ui__()
-                imgui.separator()
-                imgui.spacing()
-                imgui.tree_pop()
+    _quit: bool = False
+    """Should the the main event loop end on Realtime mode?"""
 
-        imgui.end()
-        imgui.pop_style_color()
-        imgui.pop_style_var(6)
-        imgui.render()
-        self.imgui.render(imgui.get_draw_data())
+    def quit(self) -> None:
+        if self.realtime:
+            self._quit = True
 
     def next(self, dt: float) -> Self:
 
         # Fixme: Windows: https://github.com/glfw/glfw/pull/1426
         # Immediately swap the buffer with previous frame for vsync
-        if not self.headless:
+        if self.realtime:
             self.window.swap_buffers()
 
         # Temporal logic
         dt = min(dt, 1)
-        self.time_scale.next(dt=abs(dt))
+        self.tempo.next(dt=abs(dt))
         self.rdt       = dt
-        self.dt        = dt * self.time_scale
+        self.dt        = dt * self.tempo
         self.time     += self.dt
-        self.frame     = int(self.time * self.fps)
         self.vsync.fps = self.fps
 
-        # Update modules in reverse order of addition
+        # Note: Updates in reverse order of addition (child -> parent)
         # Note: Non-engine first as pipeline might change
         for module in self.modules:
-            if not isinstance(module, Shader):
+            if not isinstance(module, ShaderObject):
                 module.update()
         for module in self.modules:
-            if isinstance(module, Shader):
+            if isinstance(module, ShaderObject):
                 module.update()
 
         self._render_ui()
         return self
 
-    def __ui__(self) -> None:
-
-        # Render status
-        imgui.text(f"Resolution: {self.render_resolution} -> {self.resolution} @ {self.ssaa}x SSAA")
-
-        # Framerate
-        imgui.spacing()
-        if (state := imgui.slider_float("Framerate", self.fps, 10, 240, "%.0f"))[0]:
-            self.fps = round(state[1])
-        for fps in (options := [24, 30, 60, 120, 144, 240]):
-            if (state := imgui.button(f"{fps} Hz")):
-                self.fps = fps
-            if fps != options[-1]:
-                imgui.same_line()
-
-        # Temporal
-        imgui.spacing()
-        if (state := imgui.slider_float("Time Scale", self.time_scale.target, -2, 2, "%.2f"))[0]:
-            self.time_scale.target = state[1]
-        for scale in (options := [-10, -5, -2, -1, 0, 1, 2, 5, 10]):
-            if (state := imgui.button(f"{scale}x")):
-                self.time_scale.target = scale
-            if scale != options[-1]:
-                imgui.same_line()
-
-        # SSAA
-        imgui.spacing()
-        if (state := imgui.slider_float("SSAA", self.ssaa, 0.01, 2, "%.2f"))[0]:
-            self.ssaa = state[1]
-        for ssaa in (options := [0.1, 0.25, 0.5, 1.0, 1.25, 1.5, 2.0]):
-            if (state := imgui.button(f"{ssaa}x")):
-                self.ssaa = ssaa
-            if ssaa != options[-1]:
-                imgui.same_line()
-
-        # Quality
-        imgui.spacing()
-        if (state := imgui.slider_float("Quality", self.quality, 0, 100, "%.0f%%"))[0]:
-            self.quality = state[1]
-
-    # ---------------------------------------------------------------------------------------------|
-    # User actions
-
-    @abstractmethod
-    def commands(self) -> None:
-        """
-        Let the user configure commands for the Scene
-        """
-        ...
-
-    # Todo: Make this a ShaderModule standard
-    def destroy(self):
-        getattr(self.ffmpeg, "close", Ignore())()
-        if (self._backend == ShaderBackend.GLFW):
-            glfw.terminate()
-
-    _built: SameTracker = Factory(SameTracker)
-
-    def cli(self, *args: List[str]):
-        args = flatten(args)
-        self.broken_typer = BrokenTyper(chain=True)
-        self.broken_typer.command(self.main,     context=True, default=True)
-        self.broken_typer.command(self.settings, context=True)
-        self.commands()
-        if ("--help" not in args) and (not self._built(True)):
-            self.build()
-        self.broken_typer(args)
-
-    @abstractmethod
-    def settings(self):
-        """Optional scene settings to be configured on the CLI"""
-        pass
-
-    _quit: bool = False
-    """Should the the main event loop end on Realtime mode?"""
-
-    exporting: bool = False
-    """Is this Scene exporting a video file?"""
-
-    benchmark: bool = False
-    """Stress test the rendering speed of the Scene"""
+    exporting: bool = True
+    """Is this Scene exporting to a video file?"""
 
     rendering: bool = False
-    """Either Exporting or Benchmarking. 'Not Realtime' mode"""
+    """Either Exporting, Rendering or Benchmarking. 'Not Realtime' mode"""
 
     realtime:  bool = False
-    """Running on Realtime mode, with a window and user interaction"""
+    """Running with a window and user interaction"""
 
     headless:  bool = False
-    """Running on Headless mode, without a window and user interaction"""
-
-    def quit(self) -> None:
-        if self.realtime:
-            self._quit = True
-
-    @property
-    def directory(self) -> Path:
-        """Directory of the current Scene script"""
-        # Fixme: How to deal with ShaderFlow as a dependency scenario?
-        return BrokenPath(SHADERFLOW.DIRECTORIES.CURRENT_SCENE)
-
-    def read_file(self, file: Path, bytes: bool=False) -> str | bytes:
-        """
-        Read a file relative to the current Scene Python script
+    """Running Headlessly, without a window and user interaction"""
 
-        Args:
-            `file`:  File to read, relative to the current Scene script directory
-            `bytes`: Whether to read the file as bytes, defaults to text
-
-        Returns:
-            File contents as text or bytes
-        """
-        file = (self.directory/file)
-        log.info(f"{self.who} Reading file ({file})")
-        return LoaderBytes(file) if bytes else LoaderString(file)
+    benchmark: bool = False
+    """Stress test the rendering speed of the Scene"""
 
     def main(self,
-        width:      Annotated[int,   Option("--width",      "-w", help="(🌵 Basic    ) Width  of the Rendering Resolution. None to not change (1920 on initialization")]=None,
-        height:     Annotated[int,   Option("--height",     "-h", help="(🌵 Basic    ) Height of the Rendering Resolution. None to not change (1080 on initialization")]=None,
-        scale:      Annotated[float, Option("--scale",      "-x", help="(🌵 Quality  ) Pre-multiply Width and Height by a Scale Factor")]=1.0,
-        fps:        Annotated[float, Option("--fps",        "-f", help="(🌵 Basic    ) Target Frames per Second. On Realtime, defaults to Monitor framerate else 60")]=None,
-        fullscreen: Annotated[bool,  Option("--fullscreen",       help="(🌵 Basic    ) Start the Real Time Window in Fullscreen Mode")]=False,
-        benchmark:  Annotated[bool,  Option("--benchmark",  "-b", help="(🌵 Basic    ) Benchmark the Scene's speed on raw rendering")]=False,
-        quality:    Annotated[float, Option("--quality",    "-q", help="(💎 Quality  ) Shader Quality level if supported (0-100%)")]=80,
-        ssaa:       Annotated[float, Option("--ssaa",       "-s", help="(💎 Quality  ) Fractional Super Sampling Anti Aliasing factor, O(N²) GPU cost")]=1.0,
-        render:     Annotated[bool,  Option("--render",     "-r", help="(📦 Exporting) Export the current Scene to a Video File defined on --output")]=False,
-        base:       Annotated[Path,  Option("--base",             help="(📦 Exporting) Output File Base Directory")]=Broken.PROJECT.DIRECTORIES.DATA,
-        output:     Annotated[str,   Option("--output",     "-o", help="(📦 Exporting) Output File Name: Absolute, Relative Path or Plain Name. Saved on ($BASE/$(plain_name or $scene-$date))")]=None,
-        format:     Annotated[str,   Option("--format",           help="(📦 Exporting) Output Video Container (mp4, mkv, webm, avi..), overrides --output one")]="mp4",
-        time:       Annotated[float, Option("--time-end",   "-t", help="(📦 Exporting) How many seconds to render, defaults to 10 or longest Audio")]=None,
-        raw:        Annotated[bool,  Option("--raw",              help="(📦 Exporting) Send raw OpenGL Frames before GPU SSAA to FFmpeg (Enabled if SSAA < 1)")]=False,
-        open:       Annotated[bool,  Option("--open",             help="(📦 Exporting) Open the Video's Output Directory after render finishes")]=False,
+        width:      Annotated[int,   Option("--width",      "-w", help="(🔴 Basic    ) Width  of the Rendering Resolution. None to keep or find by Aspect Ratio (1920 on init)")]=None,
+        height:     Annotated[int,   Option("--height",     "-h", help="(🔴 Basic    ) Height of the Rendering Resolution. None to keep or find by Aspect Ratio (1080 on init)")]=None,
+        scale:      Annotated[float, Option("--scale",      "-x", help="(🔴 Basic    ) Post-multiply Width and Height by a Scale Factor")]=1.0,
+        aspect:     Annotated[str,   Option("--ar",         "-a", help="(🔴 Basic    ) Force resolution aspect ratio, None for dynamic. Examples: '16:9', '16/9', '1.777'")]=None,
+        fps:        Annotated[float, Option("--fps",        "-f", help="(🔴 Basic    ) Target Frames per Second. On Realtime, defaults to the monitor framerate else 60")]=None,
+        fullscreen: Annotated[bool,  Option("--fullscreen",       help="(🔴 Basic    ) Start the Real Time Window in Fullscreen Mode")]=False,
+        quality:    Annotated[float, Option("--quality",    "-q", help="(🟡 Quality  ) Shader Quality level, if supported (0-100%)")]=80,
+        ssaa:       Annotated[float, Option("--ssaa",       "-s", help="(🟡 Quality  ) Fractional Super Sampling Anti Aliasing factor, O(N^2) GPU cost")]=1.0,
+        render:     Annotated[bool,  Option("--render",     "-r", help="(🟢 Exporting) Export the Scene to a Video File (defined on --output, and implicit if so)")]=False,
+        output:     Annotated[str,   Option("--output",     "-o", help="(🟢 Exporting) Output File Name: Absolute, Relative Path or Plain Name. Saved on ($base/$(plain_name or $scene-$date))")]=None,
+        end:        Annotated[float, Option("--end",        "-t", help="(🟢 Exporting) How many seconds to render, defaults to 10 or longest advertised module")]=None,
+        format:     Annotated[str,   Option("--format",           help="(🟢 Exporting) Output Video Container (mp4, mkv, webm, avi..), overrides --output one")]="mp4",
+        base:       Annotated[Path,  Option("--base",             help="(🟢 Exporting) Output File Base Directory")]=Broken.PROJECT.DIRECTORIES.DATA,
+        benchmark:  Annotated[bool,  Option("--benchmark",  "-b", help="(🔵 Special  ) Benchmark the Scene's speed on raw rendering. Use SKIP_GPU=1 for CPU only benchmark")]=False,
+        raw:        Annotated[bool,  Option("--raw",              help="(🔵 Special  ) Send raw OpenGL Frames before GPU SSAA to FFmpeg (Enabled if SSAA < 1)")]=False,
+        open:       Annotated[bool,  Option("--open",             help="(🔵 Special  ) Open the Video's Output Directory after render finishes")]=False,
     ) -> Optional[Path]:
+        """Main Event Loop of the Scene. Options to start a realtime window, exports to a file, or stress test speeds"""
 
-        self.relay(Message.Shader.ReloadShaders)
-        self.eloop.all_once()
-
-        video_resolution = (
-            (width  or self.width )*scale,
-            (height or self.height)*scale,
-        )
-
-        # Note: Implicit render mode if output is provided or benchmark
-        # Set useful state flags
-        self.exporting = render
-        self.rendering = (render or benchmark or bool(output))
-        self.realtime  = not self.rendering
-        self.benchmark = benchmark
-        self.headless  = (self.rendering or self.benchmark)
-
-        # Window configuration based on launch mode
-        self.resolution = video_resolution
-        self.resizable  = not self.rendering
-        self.visible    = not self.headless
-        self.fps        = (fps or self.monitor_framerate or 60.0) if self.realtime else 60.0
+        self.relay(Message.Shader.Compile)
+        self.exporting  = (render or bool(output))
+        self.rendering  = (self.exporting or benchmark)
+        self.realtime   = (not self.rendering)
+        self.benchmark  = benchmark
+        self.headless   = (self.rendering)
+        self.fps        = (fps or self.monitor_framerate)
+        self.title      = f"ShaderFlow | {self.__name__}"
+        self.fullscreen = fullscreen
         self.quality    = quality
         self.ssaa       = ssaa
         self.time       = 0
-        self.duration   = 0
-        self.fullscreen = fullscreen
-        self.title      = f"ShaderFlow | {self.__name__}"
 
-        # When rendering, let FFmpeg apply the SSAA, I trust it more (higher quality?)
-        if self.rendering and (raw or self.ssaa < 1):
+        # Maybe keep or force aspect ratio, and find best resolution
+        self.aspect_ratio = eval((aspect or "0").replace(":", "/")) or self._aspect_ratio
+        video_resolution = self.resize(width=width, height=height, scale=scale)
+
+        # Optimization: Save bandwidth by piping native frames on ssaa < 1
+        if self.rendering and (raw or ssaa < 1):
             self.resolution = self.render_resolution
             self.ssaa = 1
 
-        # Setup
-        log.info(f"{self.who} Setting up Modules")
         for module in self.modules:
             module.setup()
-        self.eloop.all_once()
 
-        # Find the longest audio duration or set duration
-        for module in (not bool(time)) * self.rendering * list(self.find(ShaderAudio)):
-            self.duration = max(self.duration, module.duration or 0)
-        else:
-            self.duration = self.duration or time or 10
+        self.set_duration(end)
 
         # Configure FFmpeg and Popen it
         if (self.rendering):
             import arrow
 
             # Get video output path - if not absolute, save to data directory
             output = Path(output or f"({arrow.utcnow().format('YYYY-MM-DD_HH-mm-ss')}) {self.__name__}")
             output = output if output.is_absolute() else base/output
             output = output.with_suffix(output.suffix or f".{format}")
 
-            # Create FFmpeg process
             self.ffmpeg = (
                 BrokenFFmpeg()
                 .quiet()
-                .overwrite()
-                .hwaccel(FFmpegHWAccel.Auto)
                 .format(FFmpegFormat.Rawvideo)
-                .pixel_format(FFmpegPixelFormat.RGB24)
+                .pixel_format(FFmpegPixelFormat.RGBA if self.alpha else FFmpegPixelFormat.RGB24)
                 .resolution(self.resolution)
                 .framerate(self.fps)
                 .filter(FFmpegFilterFactory.scale(video_resolution))
                 .filter(FFmpegFilterFactory.flip_vertical())
+                .overwrite()
                 .input("-")
             )
 
             # Fixme: Is this the correct point for modules to manage FFmpeg?
             for module in self.modules:
                 module.ffmpeg(self.ffmpeg)
 
@@ -719,125 +662,171 @@
                 .video_codec(FFmpegVideoCodec.H264)
                 .audio_codec(FFmpegAudioCodec.AAC)
                 .audio_bitrate("300k")
                 .preset(FFmpegH264Preset.Slow)
                 .tune(FFmpegH264Tune.Film)
                 .quality(FFmpegH264Quality.High)
                 .pixel_format(FFmpegPixelFormat.YUV420P)
-                .custom("-t", self.duration)
+                .custom("-t", self.runtime)
                 .custom("-movflags", "+faststart")
             )
 
-            # Add output video
             self.ffmpeg.output(output)
 
-            # Don't allocate new buffer on each read
-            buffer = self.opengl.buffer(
-                reserve=self._final.texture.length,
-                dynamic=True,
-            )
+            # Optimization: Don't allocate new buffers on each read for piping
+            buffer = self.opengl.buffer(reserve=self._final.texture.length)
 
+            # Fixme: Why Popen on Linux is slower on main thread (blocking?)
+            # Idea: Python 3.13 Sub-interpreters could help, but require >= 3.13
             if self.exporting:
                 if BrokenPlatform.OnWindows:
                     self.ffmpeg = self.ffmpeg.Popen(stdin=PIPE)
                 else:
                     self.ffmpeg = self.ffmpeg.pipe()
 
-            # Add progress bar
-            progress_bar = tqdm.tqdm(
-                total=int(self.duration*self.fps),
-                desc=f"Scene ({type(self).__name__}) → Video",
-                dynamic_ncols=True,
-                colour="#43BFEF",
-                leave=False,
-                unit=" Frames",
-                mininterval=1/60,
-                maxinterval=0.1,
-                smoothing=0.1,
+            # Status tracker
+            status = DotMap(
+                start=time.perf_counter(),
+                bar=tqdm.tqdm(
+                    total=self.total_frames,
+                    desc=f"Scene ({type(self).__name__}) → Video",
+                    dynamic_ncols=True,
+                    colour="#43BFEF",
+                    leave=False,
+                    unit=" frames",
+                    mininterval=1/60,
+                    maxinterval=0.1,
+                    smoothing=0.1,
+                )
             )
 
-        import time
-
-        # Benchmark and stats data
-        RenderStatus = DotMap(
-            render_start=time.perf_counter(),
-            total_frames=0,
-        )
-
-        # Create the Vsync event loop
-        self.vsync = self.eloop.new(
-            callback=self.next,
+        # Add self.next to the event loop
+        self.vsync = self.scheduler.new(
+            task=self.next,
             frequency=self.fps,
             decoupled=self.rendering,
             precise=True,
         )
 
+        # Some scenes might take a while to setup
+        self.visible = not self.headless
+
         # Main rendering loop
         while (self.rendering) or (not self._quit):
+            task = self.scheduler.next()
 
-            # Keep calling event loop until self was updated
-            if (_call := self.eloop.next().output) is not self:
+            # Only continue if exporting
+            if (task.output is not self):
                 continue
-
-            # Rendering logic
             if self.realtime:
                 continue
 
-            progress_bar.update(1)
-            RenderStatus.total_frames += 1
+            status.bar.update(1)
 
-            # Write new frame to FFmpeg
             if self.exporting:
                 self._final.texture.fbo().read_into(buffer)
                 self.ffmpeg.stdin.write(buffer.read())
 
-            # Render until time and end are Close
-            if (self.duration - self.time) > 1.5*self.frametime:
+            if status.bar.n < self.total_frames:
                 continue
 
-            # Close FFmpeg
             if self.exporting:
                 self.ffmpeg.stdin.close()
 
             # Log stats
-            progress_bar.refresh()
-            progress_bar.close()
-            RenderStatus.took = (time.perf_counter() - RenderStatus.render_start)
+            status.bar.refresh()
+            status.bar.close()
+            status.took = (time.perf_counter() - status.start)
             log.info(f"Finished rendering ({output})", echo=not self.benchmark)
             log.info((
                 f"• Stats: "
-                f"(Took {RenderStatus.took:.2f} s) at "
-                f"({self.frame/RenderStatus.took:.2f} FPS | "
-                f"{self.duration/RenderStatus.took:.2f} x Realtime) with "
-                f"({RenderStatus.total_frames} Total Frames)"
+                f"(Took {status.took:.2f} s) at "
+                f"({self.frame/status.took:.2f} FPS | "
+                f"{self.runtime/status.took:.2f} x Realtime) with "
+                f"({status.bar.n} Total Frames)"
             ))
 
             if self.benchmark:
-                return
+                return None
+            if open:
+                BrokenPath.open_in_file_explorer(output.parent)
+            return output
 
-            # Open output directory
-            if open: BrokenPath.open_in_file_explorer(output.parent)
-            break
+    # ---------------------------------------------------------------------------------------------|
+    # Module
 
-        return output
+    def handle(self, message: Message) -> None:
 
-    # # Window related events
+        if isinstance(message, Message.Window.Close):
+            log.info(f"{self.who} Received Window Close Event")
+            self.quit()
+
+        elif isinstance(message, Message.Keyboard.KeyDown):
+            if message.key == ShaderKeyboard.Keys.O:
+                log.info(f"{self.who} (O  ) Resetting the Scene")
+                for module in self.modules:
+                    module.setup()
+
+            elif message.key == ShaderKeyboard.Keys.R:
+                log.info(f"{self.who} (R  ) Reloading Shaders")
+                for module in self.modules:
+                    if isinstance(module, ShaderObject):
+                        module.compile()
+
+            elif message.key == ShaderKeyboard.Keys.TAB:
+                log.info(f"{self.who} (TAB) Toggling Menu")
+                self.render_ui  = not self.render_ui
+
+            elif message.key == ShaderKeyboard.Keys.F1:
+                log.info(f"{self.who} (F1 ) Toggling Exclusive Mode")
+                self.exclusive  = not self.exclusive
+
+            elif message.key == ShaderKeyboard.Keys.F2:
+                import arrow
+                time  = arrow.now().format("YYYY-MM-DD_HH-mm-ss")
+                image = PIL.Image.frombytes("RGB", self.resolution, self.read_screen())
+                image = image.transpose(PIL.Image.FLIP_TOP_BOTTOM)
+                path  = Broken.PROJECT.DIRECTORIES.SCREENSHOTS/f"({time}) {self.__name__}.png"
+                BrokenThread.new(target=image.save, fp=path)
+                log.minor(f"{self.who} (F2 ) Saved Screenshot to ({path})")
+
+            elif message.key == ShaderKeyboard.Keys.F11:
+                log.info(f"{self.who} (F11) Toggling Fullscreen")
+                self.fullscreen = not self.fullscreen
+
+        elif isinstance(message, (Message.Mouse.Drag, Message.Mouse.Position)):
+            self.mouse_gluv = (message.u, message.v)
+
+    def pipeline(self) -> Iterable[ShaderVariable]:
+        yield ShaderVariable("uniform", "float", "iTime",        self.time)
+        yield ShaderVariable("uniform", "float", "iDuration",    self.duration)
+        yield ShaderVariable("uniform", "float", "iDeltaTime",   self.dt)
+        yield ShaderVariable("uniform", "vec2",  "iResolution",  self.resolution)
+        yield ShaderVariable("uniform", "float", "iQuality",     self.quality/100)
+        yield ShaderVariable("uniform", "float", "iSSAA",        self.ssaa)
+        yield ShaderVariable("uniform", "float", "iFrameRate",   self.fps)
+        yield ShaderVariable("uniform", "int",   "iFrame",       self.frame)
+        yield ShaderVariable("uniform", "bool",  "iRealtime",    self.realtime)
+        yield ShaderVariable("uniform", "vec2",  "iMouse",       self.mouse_gluv)
+        yield ShaderVariable("uniform", "bool",  "iMouseInside", self.mouse_inside)
+        for i in range(1, 6):
+            yield ShaderVariable("uniform", "bool", f"iMouse{i}", self.mouse_buttons[i])
+
+    # ---------------------------------------------------------------------------------------------|
+    # Internal window events
 
     def __window_resize__(self, width: int, height: int) -> None:
 
         # Don't listen to resizes when exporting, as the final resolution might be
         # greater than the monitor and the window will resize down to fit
         if self.exporting:
             return
-
-        # Apply new resolution
-        width, height = max(10, width), max(10, height)
         self.imgui.resize(width, height)
         self._width, self._height = width, height
-        self.relay(Message.Window.Resize(width=width, height=height))
+        self.relay(Message.Shader.RecreateTextures)
         self.relay(Message.Shader.Render)
 
     def __window_close__(self) -> None:
         self.relay(Message.Window.Close())
 
     def __window_iconify__(self, state: bool) -> None:
         self.relay(Message.Window.Iconify(state=state))
@@ -873,15 +862,15 @@
             v=2*(y/self.height - 0.5)*(-1),
             x=x, y=y,
         )
 
     def __dxdy2dudv__(self, dx: int=0, dy: int=0) -> dict[str, float]:
         """Convert a dx dy pixel coordinate into a Center-UV normalized coordinate"""
         return dict(
-            du=2*(dx/self.width)*self.aspect_ratio,
+            du=2*(dx/self.width)*(self.width/self.height),
             dv=2*(dy/self.height)*(-1),
             dx=dx, dy=dy,
         )
 
     mouse_buttons: Dict[int, bool] = Factory(lambda: {k: False for k in range(1, 6)})
 
     def __window_mouse_press_event__(self, x: int, y: int, button: int) -> None:
@@ -911,15 +900,15 @@
         self.relay(Message.Mouse.Enter(state=inside))
 
     def __window_mouse_scroll_event__(self, dx: int, dy: int) -> None:
         self.imgui.mouse_scroll_event(dx, dy)
         if self.imguio.want_capture_mouse and self.render_ui:
             return
         elif self.keyboard(ShaderKeyboard.Keys.LEFT_ALT):
-            self.time_scale.target += (dy)*0.2
+            self.tempo.target += (dy)*0.2
             return
         self.relay(Message.Mouse.Scroll(
             **self.__dxdy2dudv__(dx=dx, dy=dy)
         ))
 
     def __window_mouse_position_event__(self, x: int, y: int, dx: int, dy: int) -> None:
         self.imgui.mouse_position_event(x, y, dx, dy)
@@ -956,7 +945,83 @@
             self.time -= self._mouse_drag_time_factor * (dy/self.height)
             return
 
         self.relay(Message.Mouse.Drag(
             **self.__dxdy2dudv__(dx=dx, dy=dy),
             **self.__xy2uv__(x=x, y=y)
         ))
+
+    # ---------------------------------------------------------------------------------------------|
+    # Todo: Move UI to own class
+
+    # Fixme: Move to somewhere better
+    def _render_ui(self):
+        if not self.render_ui:
+            return
+
+        self._final.texture.fbo().use()
+        imgui.push_style_var(imgui.STYLE_WINDOW_BORDERSIZE, 0.0)
+        imgui.push_style_var(imgui.STYLE_WINDOW_ROUNDING, 8)
+        imgui.push_style_var(imgui.STYLE_TAB_ROUNDING, 8)
+        imgui.push_style_var(imgui.STYLE_GRAB_ROUNDING, 8)
+        imgui.push_style_var(imgui.STYLE_FRAME_ROUNDING, 8)
+        imgui.push_style_var(imgui.STYLE_CHILD_ROUNDING, 8)
+        imgui.push_style_color(imgui.COLOR_FRAME_BACKGROUND, 0.1, 0.1, 0.1, 0.5)
+        imgui.new_frame()
+        imgui.set_next_window_position(0, 0)
+        imgui.set_next_window_bg_alpha(0.6)
+        imgui.begin(f"{self.__name__}", False, imgui.WINDOW_NO_MOVE | imgui.WINDOW_NO_RESIZE | imgui.WINDOW_NO_COLLAPSE  | imgui.WINDOW_ALWAYS_AUTO_RESIZE)
+
+        # Render every module
+        for module in self.modules:
+            if imgui.tree_node(f"{module.uuid:>2} - {type(module).__name__.replace('ShaderFlow', '')}", imgui.TREE_NODE_BULLET):
+                imgui.separator()
+                module.__shaderflow_ui__()
+                imgui.separator()
+                imgui.spacing()
+                imgui.tree_pop()
+
+        imgui.end()
+        imgui.pop_style_color()
+        imgui.pop_style_var(6)
+        imgui.render()
+        self.imgui.render(imgui.get_draw_data())
+
+    def __ui__(self) -> None:
+
+        # Render status
+        imgui.text(f"Resolution: {self.render_resolution} -> {self.resolution} @ {self.ssaa}x SSAA")
+
+        # Framerate
+        imgui.spacing()
+        if (state := imgui.slider_float("Framerate", self.fps, 10, 240, "%.0f"))[0]:
+            self.fps = round(state[1])
+        for fps in (options := [24, 30, 60, 120, 144, 240]):
+            if (state := imgui.button(f"{fps} Hz")):
+                self.fps = fps
+            if fps != options[-1]:
+                imgui.same_line()
+
+        # Temporal
+        imgui.spacing()
+        if (state := imgui.slider_float("Time Scale", self.tempo.target, -2, 2, "%.2f"))[0]:
+            self.tempo.target = state[1]
+        for scale in (options := [-10, -5, -2, -1, 0, 1, 2, 5, 10]):
+            if (state := imgui.button(f"{scale}x")):
+                self.tempo.target = scale
+            if scale != options[-1]:
+                imgui.same_line()
+
+        # SSAA
+        imgui.spacing()
+        if (state := imgui.slider_float("SSAA", self.ssaa, 0.01, 2, "%.2f"))[0]:
+            self.ssaa = state[1]
+        for ssaa in (options := [0.1, 0.25, 0.5, 1.0, 1.25, 1.5, 2.0]):
+            if (state := imgui.button(f"{ssaa}x")):
+                self.ssaa = ssaa
+            if ssaa != options[-1]:
+                imgui.same_line()
+
+        # Quality
+        imgui.spacing()
+        if (state := imgui.slider_float("Quality", self.quality, 0, 100, "%.0f%%"))[0]:
+            self.quality = state[1]
```

## ShaderFlow/Shader.py

```diff
@@ -1,35 +1,103 @@
+from __future__ import annotations
+
 import contextlib
 import errno
 import itertools
+import os
+import re
 from pathlib import Path
 from typing import Any, Iterable, List, Self, Set, Tuple, Union
 
+import _moderngl
 import imgui
 import moderngl
 import numpy
+import rich
 import watchdog
 import watchdog.observers
 from attr import Factory, define
+from loguru import logger as log
+from rich.panel import Panel
+from rich.syntax import Syntax
 
 import Broken
-from Broken.Base import BrokenPath, denum
-from Broken.Loaders.LoaderString import LoaderString
-from Broken.Logging import log
+from Broken import BrokenPath, denum
+from Broken.Loaders import LoaderString
 from ShaderFlow import SHADERFLOW
 from ShaderFlow.Message import Message
 from ShaderFlow.Module import ShaderModule
 from ShaderFlow.Texture import ShaderTexture
 from ShaderFlow.Variable import ShaderVariable, ShaderVariableDirection
 
 WATCHDOG = watchdog.observers.Observer()
 WATCHDOG.start()
 
 @define
-class Shader(ShaderModule):
+class ShaderDumper:
+    shader: ShaderObject # Fixme: Extending a parent class with refactored functionality
+    """Parent ShaderObject instance"""
+
+    error: str
+    """str(_moderngl.Error) exception"""
+
+    fragment: str
+    """Potentially faulty Fragment shader"""
+
+    vertex: str
+    """Potentially faulty Vertex shader"""
+
+    context: int = 5
+    """Number of lines to show before and after the faulty line"""
+
+    _parser = re.compile(r"^0\((\d+)\)\s*:\s*error\s* (\w+):\s(.*)", re.MULTILINE)
+
+    @property
+    def code(self) -> str:
+        """Simple heuristic to choose what shader cause the error"""
+        if ("fragment_shader" in self.error):
+            return self.fragment
+        elif ("vertex_shader" in self.error):
+            return self.vertex
+        raise RuntimeError(f"Cannot determine shader from error: {self.error}")
+
+    @property
+    def lines(self) -> List[str]:
+        return self.code.splitlines()
+
+    def dump(self):
+        directory = Broken.PROJECT.DIRECTORIES.DUMP
+        log.error(f"{self.shader.who} Dumping shaders to {directory}")
+        (directory/f"{self.shader.uuid}.frag").write_text(self.fragment, encoding="utf-8")
+        (directory/f"{self.shader.uuid}.vert").write_text(self.vertex, encoding="utf-8")
+        (directory/f"{self.shader.uuid}-error.md" ).write_text(self.error, encoding="utf-8")
+
+        # Visual only: Print highlighted code panels of all errors
+        for match in ShaderDumper._parser.finditer(self.error):
+            lineno, errno, message = match.groups()
+            lineno = int(lineno)
+            start  = max(0, lineno - self.context - 1)
+            end    = min(len(self.lines), lineno + self.context)
+            code   = []
+
+            for i, line in enumerate(self.lines[start:end]):
+                i += start + 1
+
+                if (i == lineno):
+                    code.append(f"({i:3d}) > {line}")
+                else:
+                    code.append(f"({i:3d}) | {line}")
+
+            rich.print(Panel(
+                Syntax(code='\n'.join(code), lexer="glsl"),
+                title=f"({errno} at Module #{self.shader.uuid}, Line {lineno}): {message}",
+            ))
+
+@define
+class ShaderObject(ShaderModule):
     version: int = 330
     """OpenGL Version to use for the shader. Must be <= than the Window Backend version."""
 
     program: moderngl.Program = None
     """ModernGL 'Compiled Shaders' object"""
 
     vao: moderngl.VertexArray = None
@@ -41,39 +109,39 @@
     texture: ShaderTexture = None
     """ShaderTexture Module that this Shader renders to in layers and temporal"""
 
     clear: bool = False
     """Clear the Final Texture before rendering"""
 
     instances: int = 1
-    """Number of gl_InstanceIDs to render"""
+    """Number of gl_InstanceID's to render"""
 
     vertices: List[float] = Factory(list)
-    """Vertices of the shader. More often than not a Fullscreen Quad"""
+    """Vertices of the shader. More often than not, a Fullscreen Quad"""
 
     vertex_variables: Set[ShaderVariable] = Factory(set)
     """Variables metaprogramming that will be added to the Vertex Shader"""
 
     fragment_variables: Set[ShaderVariable] = Factory(set)
     """Variables metaprogramming that will be added to the Fragment Shader"""
 
     def __post__(self):
         """Set default values for some variables"""
         self.texture = ShaderTexture(scene=self.scene, name=self.name, track=True)
         self.fragment_variable("out vec4 fragColor")
         self.vertex_variable("in vec2 vertex_position")
         self.vertex_variable("in vec2 vertex_gluv")
-        self.vertex_io("flat int instance")
-        self.vertex_io("vec2 gluv")
-        self.vertex_io("vec2 stuv")
-        self.vertex_io("vec2 astuv")
-        self.vertex_io("vec2 agluv")
-        self.vertex_io("vec2 fragCoord")
-        self.vertex_io("vec2 glxy")
-        self.vertex_io("vec2 stxy")
+        self.passthrough("flat int instance")
+        self.passthrough("vec2 gluv")
+        self.passthrough("vec2 stuv")
+        self.passthrough("vec2 astuv")
+        self.passthrough("vec2 agluv")
+        self.passthrough("vec2 fragCoord")
+        self.passthrough("vec2 glxy")
+        self.passthrough("vec2 stxy")
 
         # Add a fullscreen center-(0, 0) uv rectangle
         for x, y in itertools.product((-1, 1), (-1, 1)):
             self.add_vertice(x=x, y=y, u=x, v=y)
 
         # Load default vertex and fragment shaders
         self.vertex   = (SHADERFLOW.RESOURCES.VERTEX/  "Default.glsl")
@@ -92,15 +160,15 @@
     def fragment_variable(self, variable: ShaderVariable) -> Self:
         self.fragment_variables.add(ShaderVariable.smart(variable))
 
     def common_variable(self, variable: ShaderVariable) -> Self:
         self.vertex_variable(variable)
         self.fragment_variable(variable)
 
-    def vertex_io(self, variable: ShaderVariable) -> Self:
+    def passthrough(self, variable: ShaderVariable) -> Self:
         variable = ShaderVariable.smart(variable)
         self.vertex_variable(variable.copy(direction="out"))
         self.fragment_variable(variable.copy(direction="in"))
 
     @property
     def vao_definition(self) -> Tuple[str]:
         """("2f 2f", "render_vertex", "coords_vertex")"""
@@ -148,24 +216,24 @@
 
     # # Vertex shader content
 
     def _watchshader(self, path: Path) -> None:
 
         @define(eq=False)
         class Handler(watchdog.events.FileSystemEventHandler):
-            shader: Shader
+            shader: ShaderObject
             def on_modified(self, event):
                 if self.shader.scene.rendering:
                     return
-                self.shader.scene.eloop.once(callback=self.shader.load_shaders)
+                self.shader.scene.scheduler.once(self.shader.compile)
 
         # Add the Shader Path to the watchdog for changes. Only ignore 'File Too Long'
         # exceptions when non-path strings as we can't get max len easily per system
         try:
-            if (path := BrokenPath(path, valid=True)):
+            if (path := BrokenPath(path).valid()):
                 WATCHDOG.schedule(Handler(self), path)
         except OSError as error:
             if error.errno != errno.ENAMETOOLONG:
                 raise error
 
     _vertex: Union[Path, str] = ""
     """The 'User Content' of the Vertex Shader, interted after the Metaprogramming.
@@ -209,48 +277,44 @@
             uniform.value = denum(value)
 
     def get_uniform(self, name: str) -> Any | None:
         return self.program.get(name, None)
 
     # # Rendering
 
-    def dump_shaders(self, error: str=""):
-        import rich
-        directory = Broken.PROJECT.DIRECTORIES.DUMP
-        log.error(f"{self.who} Dumping shaders to {directory}")
-        (directory/f"{self.uuid}-frag.glsl").write_text(self.fragment, encoding="utf-8")
-        (directory/f"{self.uuid}-vert.glsl").write_text(self.vertex, encoding="utf-8")
-        (directory/f"{self.uuid}-error.md" ).write_text(error, encoding="utf-8")
-        # Process(target=functools.partial(
-        #     rich.print, self, file=(directory/f"{self.uuid}-module.prop").open("w", encoding="utf-8")
-        # )).start()
-
     def _full_pipeline(self) -> Iterable[ShaderVariable]:
         for module in self.scene.modules:
             yield from module.pipeline()
 
-    def load_shaders(self, _vertex: str=None, _fragment: str=None) -> Self:
+    def compile(self, _vertex: str=None, _fragment: str=None) -> Self:
         log.info(f"{self.who} Compiling shaders")
 
         # Add pipeline variable definitions
         for variable in self._full_pipeline():
             self.common_variable(variable)
 
+        # Metaprogram either injected or proper shaders
+        fragment = self.make_fragment(_fragment or self._fragment)
+        vertex = self.make_vertex(_vertex or self._vertex)
+
         try:
-            self.program = self.scene.opengl.program(
-                self.make_vertex(_vertex or self._vertex),
-                self.make_fragment(_fragment or self._fragment)
-            )
-        except Exception as error:
+            self.program = self.scene.opengl.program(vertex, fragment)
+        except _moderngl.Error as error:
+            ShaderDumper(
+                shader=self,
+                error=str(error),
+                vertex=vertex,
+                fragment=fragment
+            ).dump()
+
             if (_vertex or _fragment):
                 raise RuntimeError(log.error("Recursion on Missing Texture Shader Loading"))
 
             log.error(f"{self.who} Error compiling shaders, loading missing texture shader")
-            self.dump_shaders(error=str(error))
-            self.load_shaders(
+            self.compile(
                 _vertex  =LoaderString(SHADERFLOW.RESOURCES.VERTEX/"Default.glsl"),
                 _fragment=LoaderString(SHADERFLOW.RESOURCES.FRAGMENT/"Missing.glsl")
             )
 
         # Render the vertices that are defined on the shader
         self.vbo = self.scene.opengl.buffer(numpy.array(self.vertices, dtype="f4"))
         self.vao = self.scene.opengl.vertex_array(
@@ -260,21 +324,25 @@
 
         return self
 
     # # Module
 
     def update(self) -> None:
         if not self.program:
-            self.load_shaders()
+            self.compile()
         self.render()
 
+    SKIP_GPU: bool = (os.environ.get("SKIP_GPU", "0") == "1")
+    """Do not render shaders, useful for benchmarking raw Python performance"""
+
     def render_fbo(self, fbo: moderngl.Framebuffer, clear: bool=True) -> None:
+        if self.SKIP_GPU:
+            return
         fbo.use()
-        if clear:
-            fbo.clear()
+        clear or fbo.clear()
         self.vao.render(
             moderngl.TRIANGLE_STRIP,
             instances=self.instances
         )
 
     def use_pipeline(self, pipeline: Iterable[ShaderVariable]) -> None:
         for index, variable in enumerate(pipeline):
@@ -288,39 +356,39 @@
             self.set_uniform(variable.name, variable.value)
 
     def render(self) -> None:
 
         # Optimization: Final shader doesn't need the full pipeline
         if self.texture.final:
             self.use_pipeline(self.scene.shader.texture.pipeline())
-            self.render_fbo(self.texture.fbo(), clear=self.clear)
+            self.render_fbo(self.texture.fbo(), clear=False)
             return
 
         self.use_pipeline(self._full_pipeline())
 
-        for layer, container in enumerate(self.texture.matrix[0]):
+        for layer, box in enumerate(self.texture.row(0)):
             self.set_uniform("iLayer", layer)
-            self.render_fbo(fbo=container.fbo, clear=container.clear)
+            self.render_fbo(fbo=box.fbo, clear=box.clear)
 
         self.texture.roll()
 
     def handle(self, message: Message) -> None:
-        if isinstance(message, Message.Shader.ReloadShaders):
-            self.load_shaders()
+        if isinstance(message, Message.Shader.Compile):
+            self.compile()
 
         elif isinstance(message, Message.Shader.Render):
             self.render()
 
             # Fixme: Should this be on a proper User Interface class?
             if self.texture.final:
                 self.scene._render_ui()
 
     def __ui__(self) -> None:
         if imgui.button("Reload"):
-            self.load_shaders()
+            self.compile()
         imgui.same_line()
         if imgui.button("Dump"):
             self.dump_shaders()
         if imgui.tree_node("Pipeline"):
             for variable in self._full_pipeline():
                 imgui.text(f"{variable.name.ljust(16)}: {variable.value}")
             imgui.tree_pop()
```

## ShaderFlow/Texture.py

```diff
@@ -5,17 +5,16 @@
 from typing import Any, Deque, Iterable, List, Optional, Self, Tuple, Type, Union
 
 import moderngl
 import numpy
 import PIL
 from attr import Factory, define, field
 
-from Broken.Base import Ignore, Maybe
-from Broken.BrokenEnum import BrokenEnum
-from Broken.Loaders.LoaderPIL import LoadableImage, LoaderImage
+from Broken import BrokenEnum, Ignore
+from Broken.Loaders import LoadableImage, LoaderImage
 from ShaderFlow.Message import Message
 from ShaderFlow.Module import ShaderModule
 from ShaderFlow.Variable import ShaderVariable
 
 
 class TextureType(BrokenEnum):
 
@@ -76,129 +75,175 @@
     name: str = None
 
     def __post__(self):
         self.make()
         self.apply()
 
     # ------------------------------------------|
-    # Filters, Types Repeat, Mipmaps
+    # Special
+
+    final: bool = field(default=False, converter=bool)
+    """Is this bound to the final FSSAA ShaderObject?"""
+
+    _track: bool = field(default=False, converter=bool)
+    """Should this ShaderTexture match the resolution of the Scene?"""
+
+    @property
+    def track(self) -> bool:
+        return self._track
+
+    @track.setter
+    def track(self, value: bool):
+        if (self._track == value):
+            return
+        self._track = value
+        self.make()
+
+    # ------------------------------------------|
+
+    # Filter
 
     _filter: TextureFilter = TextureFilter.Linear
 
     @property
     def filter(self) -> TextureFilter:
         return TextureFilter.get(self._filter)
+
     @filter.setter
     def filter(self, value: TextureFilter):
         self._filter = TextureFilter.get(value)
         self.apply()
 
+    # Anisotropy
+
     _anisotropy: Anisotropy = Anisotropy.x16
 
     @property
     def anisotropy(self) -> Anisotropy:
         return Anisotropy.get(self._anisotropy)
+
     @anisotropy.setter
     def anisotropy(self, value: Anisotropy):
         self._anisotropy = Anisotropy.get(value)
         self.apply()
 
+    # Mipmaps
+
+    _mipmaps: bool = field(default=False, converter=bool)
+
+    @property
+    def mipmaps(self) -> bool:
+        return self._mipmaps
+
+    @mipmaps.setter
+    def mipmaps(self, value: bool):
+        if (self._mipmaps == value):
+            return
+        self._mipmaps = value
+        self.apply()
+
+    # ModernGL Filter
+
     @property
     def moderngl_filter(self) -> int:
         return dict(
             linear=moderngl.LINEAR,
             nearest=moderngl.NEAREST,
             linear_mipmap=moderngl.LINEAR_MIPMAP_LINEAR,
             nearest_mipmap=moderngl.NEAREST_MIPMAP_NEAREST,
         ).get(self.filter.value + ("_mipmap"*self.mipmaps))
 
+    # Dtype
+
     _dtype: TextureType = TextureType.f4
 
     @property
     def dtype(self) -> TextureType:
         return TextureType.get(self._dtype)
+
     @dtype.setter
     def dtype(self, value: TextureType):
         self._dtype = TextureType.get(value)
         self.make()
 
-    _mipmaps: bool = field(default=False, converter=bool)
-
-    @property
-    def mipmaps(self) -> bool:
-        return self._mipmaps
-    @mipmaps.setter
-    def mipmaps(self, value: bool):
-        if (self._mipmaps == value):
-            return
-        self._mipmaps = value
-        self.apply()
+    # Repeat X
 
     _repeat_x: bool = field(default=True, converter=bool)
-    _repeat_y: bool = field(default=True, converter=bool)
 
     @property
     def repeat_x(self) -> bool:
         return self._repeat_x
-    @property
-    def repeat_y(self) -> bool:
-        return self._repeat_y
 
     @repeat_x.setter
     def repeat_x(self, value: bool):
         if (self._repeat_x == value):
             return
         self._repeat_x = value
         self.apply()
+
+    # Repeat Y
+
+    _repeat_y: bool = field(default=True, converter=bool)
+
+    @property
+    def repeat_y(self) -> bool:
+        return self._repeat_y
+
     @repeat_y.setter
     def repeat_y(self, value: bool):
         if (self._repeat_y == value):
             return
         self._repeat_y = value
         self.apply()
 
+    # Repeat XY
+
     def repeat(self, value: bool) -> Self:
         self.repeat_x = self.repeat_y = bool(value)
         return self.apply()
 
     # ------------------------------------------|
-    # Resolution
 
-    _width:  int = field(default=1, converter=int)
-    _height: int = field(default=1, converter=int)
+    # Width
+
+    _width: int = field(default=1, converter=int)
 
     @property
     def width(self) -> int:
         if not self.track:
             return self._width
         return self.resolution[0]
-    @property
-    def height(self) -> int:
-        if not self.track:
-            return self._height
-        return self.resolution[1]
 
     @width.setter
     def width(self, value: int):
         value = int(value)
         if (self._width == value):
             return
         self._width = value
         self.make()
+
+    # Height
+
+    _height: int = field(default=1, converter=int)
+
+    @property
+    def height(self) -> int:
+        if not self.track:
+            return self._height
+        return self.resolution[1]
+
     @height.setter
     def height(self, value: int):
         value = int(value)
         if (self._height == value):
             return
         self._height = value
         self.make()
 
-    @property
-    def aspect_ratio(self) -> float:
-        return self.width/(self.height or 1)
+    # Size (Width, Height)
 
     @property
     def resolution(self) -> Tuple[int, int]:
         if not self.track:
             return (self.width, self.height)
         if self.final:
             return self.scene.resolution
@@ -213,91 +258,89 @@
         if not self.track:
             self.width, self.height = value
 
     @size.setter
     def size(self, value: Tuple[int, int]) -> None:
         self.resolution = value
 
+    @property
+    def aspect_ratio(self) -> float:
+        return self.width/(self.height or 1)
+
+    # Components
+
     _components: int = field(default=4, converter=int)
 
     @property
     def components(self) -> int:
+        """Number of color channels per pixel (1 Grayscale, 2 RG, 3 RGB, 4 RGBA)"""
         return self._components
+
     @components.setter
     def components(self, value: int):
         if (self._components == value):
             return
         self._components = value
         self.make()
 
-    _track: bool = field(default=False, converter=bool)
-
-    @property
-    def track(self) -> bool:
-        return self._track
-    @track.setter
-    def track(self, value: bool):
-        if (self._track == value):
-            return
-        self._track = value
-        self.make()
+    # Bytes size and Zero filling
 
     @property
     def zeros(self) -> numpy.ndarray:
         return numpy.zeros((*self.size, self.components), dtype=self.dtype.value)
 
     @property
     def length(self) -> int:
         """Length of the texture in bytes"""
         return self.width * self.height * self.components
 
     # ------------------------------------------|
-    # Matrix and Special
+
+    # Matrix
+
+    _matrix: Deque[Deque[TextureBox]] = Factory(deque)
+    """Matrix of previous frames (temporal) and their layers (layers)"""
+
+    @property
+    def matrix(self) -> Deque[Deque[TextureBox]]:
+        return self._matrix
+
+    # Temporal
 
     _temporal: int = field(default=1, converter=int)
+    """Number of previous frames to be stored"""
 
     @property
     def temporal(self) -> int:
         return self._temporal
+
     @temporal.setter
     def temporal(self, value: int):
         if (self._temporal == value):
             return
         self._temporal = value
         self.make()
 
+    # Layers
+
     _layers: int = field(default=1, converter=int)
+    """Number of layers to be stored, useful in single-shader multipass"""
 
     @property
     def layers(self) -> int:
         return self._layers
+
     @layers.setter
     def layers(self, value: int):
         if (self._layers == value):
             return
         self._layers = value
         self.make()
 
-    _matrix: Deque[Deque[TextureBox]] = Factory(deque)
-
-    @property
-    def matrix(self) -> Deque[Deque[TextureBox]]:
-        return self._matrix
-
-    _final: bool = field(default=False, converter=bool)
-
-    @property
-    def final(self) -> bool:
-        return self._final
-    @final.setter
-    def final(self, value: bool):
-        self._final = value
-
     # ------------------------------------------|
-    # Matrix operations
 
     def _pop_fill(self, list: Union[List, Deque], fill: Type[Any], length: int) -> List:
         """Pop right or fill until a list's length is met"""
         while len(list) > length:
             list.pop()
         while len(list) < length:
             list.append(fill())
@@ -306,60 +349,65 @@
     def _populate(self) -> Self:
         self._pop_fill(self.matrix, deque, self.temporal)
         for row in self.matrix:
             self._pop_fill(row, TextureBox, self.layers)
 
     @property
     def boxes(self) -> Iterable[Tuple[int, int, TextureBox]]:
-        for T, temporal in enumerate(self.matrix):
-            for B, box in enumerate(temporal):
-                yield (T, B, box)
+        for t, temporal in enumerate(self.matrix):
+            for b, box in enumerate(temporal):
+                yield (t, b, box)
+
+    def row(self, n: int=0) -> Iterable[TextureBox]:
+        yield from self.matrix[n]
 
     def make(self) -> Self:
         self._populate()
-        for (_, _, Box) in self.boxes:
-            Box.release()
-            Box.texture = self.scene.opengl.texture(
+        for (_, _, box) in self.boxes:
+            box.release()
+            box.texture = self.scene.opengl.texture(
                 components=self.components,
                 dtype=self.dtype.name,
                 size=self.size,
             )
-            Box.fbo = self.scene.opengl.framebuffer(
-                color_attachments=[Box.texture]
+            box.fbo = self.scene.opengl.framebuffer(
+                color_attachments=[box.texture]
             )
         return self.apply()
 
     def apply(self) -> Self:
-        for (_, _, Box) in self.boxes:
-            Maybe(Box.texture.build_mipmaps, self.mipmaps)
-            Box.texture.filter     = (self.moderngl_filter, self.moderngl_filter)
-            Box.texture.anisotropy = self.anisotropy.value
-            Box.texture.repeat_x   = self.repeat_x
-            Box.texture.repeat_y   = self.repeat_y
+        for (_, _, box) in self.boxes:
+            if self.mipmaps:
+                box.texture.build_mipmaps()
+            box.texture.filter     = (self.moderngl_filter, self.moderngl_filter)
+            box.texture.anisotropy = self.anisotropy.value
+            box.texture.repeat_x   = self.repeat_x
+            box.texture.repeat_y   = self.repeat_y
         return self
 
-    def get_box(self, temporal: int=0, layer: int=-1) -> Optional[TextureBox]:
+    def box(self, temporal: int=0, layer: int=-1) -> Optional[TextureBox]:
         """Note: Points to the current final box"""
         if (self.temporal <= temporal):
-            return
+            return None
         if (self.layers <= layer):
-            return
+            return None
         return self.matrix[temporal][layer]
 
     def fbo(self) -> moderngl.Framebuffer:
         """Final and most Recent FBO of this Texture"""
         if self.final and self.scene.realtime:
             return self.scene.window.fbo
-        return self.get_box().fbo
+        return self.box().fbo
 
     def texture(self) -> moderngl.Texture:
         """Final and most Recent Texture of this Texture"""
-        return self.get_box().texture
+        return self.box().texture
 
     def roll(self, n: int=1) -> Self:
+        """Rotate the temporal layers by $n times"""
         self.matrix.rotate(n)
         return self
 
     # ------------------------------------------|
     # Input and Output
 
     def from_image(self, image: LoadableImage) -> Self:
@@ -377,72 +425,95 @@
         if len(size) == 3:
             components = size[2]
             size = size[:2][::-1]
         else:
             components = 1
         self.width, self.height = size
         self.components = components
-
-        # Get proper numpy dtype "float32" -> "f4"
-        # Split until the number, can be float, int, double
-        alpha, number = re.match(r"([a-z]+)(\d+)", str(data.dtype)).groups()
-        self.dtype = TextureType.get(f"{alpha[0]}{int(number)//8}")
-        # print("Got dtype", f"{alpha[0]}{int(number)//8}", self.dtype)
-
+        self.dtype = TextureType.get(data.dtype)
         self.make()
         self.write(data)
         return self
 
     def write(self,
         data: bytes=None,
         *,
         temporal: int=0,
         layer: int=-1,
         viewport: Tuple[int, int, int, int]=None,
     ) -> Self:
-        Box = self.get_box(temporal, layer)
-        Box.texture.write(data, viewport=viewport)
+        box = self.box(temporal, layer)
+        box.texture.write(data, viewport=viewport)
         if not viewport:
-            Box.data = data
-        Box.empty = False
+            box.data = bytes(data)
+        box.empty = False
         return self
 
     def clear(self, temporal: int=0, layer: int=-1) -> Self:
         return self.write(self.zeros, temporal=temporal, layer=layer)
 
     def is_empty(self, temporal: int=0, layer: int=-1) -> bool:
-        return self.get_box(temporal, layer).empty
+        return self.box(temporal, layer).empty
+
+    # ------------------------------------------|
+
+    @property
+    def nbytes(self) -> int:
+        return self.dtype.value().nbytes * self.components
+
+    def sample_xy(self, x: float, y: float, temporal: int=0, layer: int=-1) -> numpy.ndarray:
+        """Get the Pixel at a XY coordinate: Origin at Top Right (0, 0); Bottom Left (width, height)"""
+        box   = self.box(temporal=temporal, layer=layer)
+        data  = (box.data or box.texture.read())
+        start = int((y*self.width + x) * self.nbytes)
+        return numpy.frombuffer(data, dtype=self.dtype.value)[start:start + self.nbytes]
+
+    def sample_stxy(self, x: float, y: float, temporal: int=0, layer: int=-1) -> numpy.ndarray:
+        """Get the Pixel at a XY coordinate: Origin at Bottom left (0, 0); Top right (width, height)"""
+        return self.sample_xy(x=x, y=(self.height - y - 1), temporal=temporal, layer=layer)
+
+    def sample_glxy(self, x: float, y: float, temporal: int=0, layer: int=-1) -> numpy.ndarray:
+        """Get the Pixel at a XY coordinate: Origin at Center (0, 0); Any Edge either (±w/2, 0), (0, ±h/2)"""
+        return self.sample_xy(x=int(x + (self.width/2)), y=int(y + (self.height/2)), temporal=temporal, layer=layer)
+
+    def sample_uv(self, u: float, v: float, temporal: int=0, layer: int=-1) -> numpy.ndarray:
+        """Get the Pixel at a UV coordinate: Origin at Top Right (0, 0); Bottom Left (1, 1)"""
+        return self.sample_xy(u*self.width, v*self.height, temporal=temporal, layer=layer)
+
+    def sample_stuv(self, u: float, v: float, temporal: int=0, layer: int=-1) -> numpy.ndarray:
+        """Get the Pixel at a UV coordinate: Origin at Bottom Left (0, 0); Top Right (1, 1)"""
+        return self.sample_uv(u=u, v=(1-v), temporal=temporal, layer=layer)
+
+    def sample_gluv(self, u: float, v: float, temporal: int=0, layer: int=-1) -> numpy.ndarray:
+        """Get the Pixel at a UV coordinate: Origin at Center (0, 0); Any Edge either (±1, 0), (0, ±1)"""
+        return self.sample_uv(u=(u/2 + 0.5), v=(v/2 + 0.5), temporal=temporal, layer=layer)
 
     # ------------------------------------------|
     # Module
 
     def _coord2name(self, old: int, layer: int) -> str:
         return f"{self.name}{old}x{layer}"
 
     def defines(self) -> Iterable[str]:
-        # Define last frames as plain name (iTex0x(-1) -> iTex, iTex1x(-1) -> iTex1)
+        """Define last frames as plain name (iTex0x(-1) -> iTex, iTex1x(-1) -> iTex1)"""
         for old in range(self.temporal):
             yield f"#define {self.name}{old or ''} {self.name}{old}x{self.layers-1}"
 
     def handle(self, message: Message):
         if self.track:
-            if isinstance(message, Message.Window.Resize):
-                self.make()
-            elif isinstance(message, Message.Shader.RecreateTextures):
+            if isinstance(message, Message.Shader.RecreateTextures):
                 self.make()
 
     def pipeline(self) -> Iterable[ShaderVariable]:
         if not self.name:
             return
 
         # Common
         yield ShaderVariable("uniform", "vec2",  f"{self.name}Size",        self.size)
         yield ShaderVariable("uniform", "float", f"{self.name}AspectRatio", self.aspect_ratio)
         yield ShaderVariable("uniform", "int",   f"{self.name}Layers",      self.layers)
         yield ShaderVariable("uniform", "int",   f"{self.name}Temporal",    self.temporal)
 
         # Matrix
-        for (T, B, Box) in self.boxes:
-            yield ShaderVariable("uniform", "sampler2D", self._coord2name(T, B), Box.texture)
-
-        # Special
+        for (t, b, box) in self.boxes:
+            yield ShaderVariable("uniform", "sampler2D", self._coord2name(t, b), box.texture)
         yield ShaderVariable("uniform", "int", "iLayer", 0)
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## ShaderFlow/Variable.py

```diff
@@ -1,16 +1,15 @@
 from __future__ import annotations
 
 from typing import Any
 
 from attr import define
+from loguru import logger as log
 
-from Broken.Base import BrokenFluentBuilder
-from Broken.BrokenEnum import BrokenEnum
-from Broken.Logging import log
+from Broken import BrokenEnum, BrokenFluentBuilder
 
 
 class ShaderVariableQualifier(BrokenEnum):
     """Guidance enum for GLSL variable qualifiers options"""
     Uniform   = "uniform"
     Attribute = "attribute"
     Varying   = "varying"
```

## ShaderFlow/__init__.py

```diff
@@ -1,11 +1,10 @@
 import Broken
 import ShaderFlow.Resources as ShaderFlowResources
-from Broken.Base import BrokenPath
-from Broken.Project import BrokenProject
+from Broken import BrokenPath, BrokenProject
 
 SHADERFLOW = BrokenProject(
     PACKAGE=__file__,
     APP_NAME="ShaderFlow",
     APP_AUTHOR="BrokenSource",
     RESOURCES=ShaderFlowResources,
 )
```

## ShaderFlow/__main__.py

```diff
@@ -1,49 +1,46 @@
 import re
 import sys
 from pathlib import Path
 
+from loguru import logger as log
 from typer import Context
 
-
-import Broken
-from Broken.Base import (
+from Broken import (
+    BrokenApp,
     BrokenPath,
-    BrokenPlatform,
     BrokenProfiler,
     BrokenTyper,
 )
-from Broken.Logging import log
-from Broken.Project import BrokenApp
+from Broken.Loaders import LoaderString
 from ShaderFlow import SHADERFLOW
 
-from Broken.Loaders.LoaderString import LoaderString
-
 SHADERFLOW_ABOUT = """
 🌵 Imagine ShaderToy, on a Manim-like architecture. That's ShaderFlow.\n
 • Tip: run "shaderflow (scene) --help" for More Options ✨
+• Warn: Make sure you trust the File you are running
 
-©️ Broken Source Software, AGPL-3.0-only License.
+©️ Broken Source Software, AGPL-3.0 License.
 """
 
 class ShaderFlowManager(BrokenApp):
     def cli(self):
         self.broken_typer = BrokenTyper(description=SHADERFLOW_ABOUT)
         self.find_all_scenes()
-        self.broken_typer(sys.argv[1:], shell=Broken.RELEASE and BrokenPlatform.OnWindows)
+        self.broken_typer(sys.argv[1:])
 
     def find_all_scenes(self) -> list[Path]:
         """Find all Scenes: Project directory and current directory"""
         direct = sys.argv[1] if (len(sys.argv) > 1) else ""
         files = set()
 
         # The user might point to a file or directory
         if (direct.endswith(".py")):
             files.add(BrokenPath(sys.argv.pop(1)))
-        elif BrokenPath(direct, valid=True):
+        elif BrokenPath.valid(direct):
             files.update(BrokenPath(sys.argv.pop(1)).rglob("*.py"))
         else:
             files.update(SHADERFLOW.DIRECTORIES.REPOSITORY.glob("Community/**/*.py"))
             files.update(SHADERFLOW.RESOURCES.SCENES.rglob("*.py"))
             files.update(Path.cwd().glob("*.py"))
 
         # Add the files, exit if no scene was added
@@ -54,40 +51,34 @@
     docscene = re.compile(r"^class\s+(\w+)\s*\(.*?(?:Scene).*\):\s*(?:\"\"\"((?:\n|.)*?)\"\"\")?", re.MULTILINE)
     """Matches any valid Python class that contains "Scene" on the inheritance and its docstring"""
 
     def add_scene_file(self, file: Path) -> bool:
         """Add classes that inherit from Scene from a file to the CLI"""
 
         # Must be a valid path with string content
-        if not (file := BrokenPath(file, valid=True)):
+        if not (file := BrokenPath(file).valid()):
             return False
         if not (code := LoaderString(file)):
             return False
 
         def partial_run(file, name, code):
             def run_scene(ctx: Context):
                 SHADERFLOW.DIRECTORIES.CURRENT_SCENE = file.parent
-                try:
-                    # Note: Point of trust transfer to the file the user is running
-                    exec(compile(code, file.stem, "exec"), namespace := {})
-                    scene = namespace[name]
-                    instance = scene()
-                    instance.cli(*ctx.args)
-                finally:
-                    try:
-                        instance.destroy()
-                    except Exception:
-                        pass
+                # Note: Point of trust transfer to the file the user is running
+                exec(compile(code, file, "exec"), namespace := {})
+                scene = namespace[name]
+                instance = scene()
+                instance.cli(*ctx.args)
             return run_scene
 
         # Match all scenes and their optional docstrings
         for match in ShaderFlowManager.docscene.finditer(code):
             name, docstring = match.groups()
             self.broken_typer.command(
-                callable=partial_run(file, name, code),
+                target=partial_run(file, name, code),
                 name=name.lower(),
                 help=(docstring or "No description available"),
                 panel=f"🎥 ShaderScenes at [bold]({file})[/bold]",
                 add_help_option=False,
                 context=True,
             )
```

## ShaderFlow/Modules/Audio.py

```diff
@@ -4,27 +4,45 @@
 from collections import deque
 from pathlib import Path
 from typing import Any, Deque, Generator, Iterable, List, Optional, Self, Tuple
 
 import numpy
 import soundcard
 from attr import Factory, define, field
+from loguru import logger as log
 
-from Broken.Base import BrokenPath, BrokenPlatform, BrokenThread, BrokenUtils, Ignore
-from Broken.BrokenEnum import BrokenEnum
+from Broken import (
+    BrokenEnum,
+    BrokenPath,
+    BrokenPlatform,
+    BrokenThread,
+    Ignore,
+)
 from Broken.Externals.FFmpeg import BrokenAudioReader, BrokenFFmpeg
-from Broken.Logging import log
 from Broken.Types import Channels, Hertz, Samples, Seconds
 from ShaderFlow.Module import ShaderModule
 from ShaderFlow.Modules.Dynamics import ShaderDynamics
 
 # Disable runtime warnings on SoundCard, it's ok to read nothing on Windows
 if BrokenPlatform.OnWindows:
     warnings.filterwarnings("ignore", category=soundcard.SoundcardRuntimeWarning)
 
+def fuzzy_string_search(string: str, choices: List[str], many: int=1, minimum_score: int=0) -> list[tuple[str, int]]:
+    """Fuzzy search a string in a list of strings, returns a list of matches"""
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore")
+        import thefuzz.process
+        result = thefuzz.process.extract(string, choices, limit=many)
+        if many == 1:
+            return result[0]
+        return result
+
+def root_mean_square(data) -> float:
+    return numpy.sqrt(numpy.mean(numpy.square(data)))
+
 class BrokenAudioMode(BrokenEnum):
     Realtime = "realtime"
     File     = "file"
 
 
 @define(slots=False)
 class BrokenAudio:
@@ -132,17 +150,22 @@
 
     @property
     def file(self) -> Path:
         return self._file
 
     @file.setter
     def file(self, value: Path):
-        self._file = BrokenPath(value, valid=True)
+        self._file = BrokenPath(value)
+        if not (_file := BrokenPath(value)):
+            return
+        if not (_file := _file.valid()):
+            return
+        self._file = _file
         if (self._file is None):
-            log.warning(f"Audio File doesn't exist ({value})")
+            log.minor(f"Audio File doesn't exist ({value})")
             return
         self.samplerate = BrokenFFmpeg.get_samplerate(self._file, echo=False)
         self.channels   = BrokenFFmpeg.get_audio_channels(self._file, echo=False)
         self.mode       = BrokenAudioMode.File
         self.close_recorder()
 
         # Create Broken readers
@@ -171,15 +194,15 @@
         yield from map(lambda device: device.name, BrokenAudio.recorders())
 
     @staticmethod
     def speakers_names() -> Iterable[str]:
         yield from map(lambda device: device.name, BrokenAudio.speakers())
 
     def __fuzzy__(self, name: str, devices: Iterable[str]) -> Optional[str]:
-        device_name = BrokenUtils.fuzzy_string_search(name, devices)[0]
+        device_name = fuzzy_string_search(name, devices)[0]
         return next(filter(lambda x: x.name == device_name, devices), None)
 
     def open_speaker(self,
         name: str=None,
         *,
         samplerate: Hertz=None,
     ) -> Self:
@@ -350,24 +373,24 @@
         if (self.final and self.scene.realtime):
             if (self.mode == BrokenAudioMode.File):
                 self.open_speaker()
             else:
                 self.open_recorder()
 
     def ffmpeg(self, ffmpeg: BrokenFFmpeg) -> None:
-        if self.final and BrokenPath(self.file, valid=True):
+        if self.final and BrokenPath(self.file).valid():
             ffmpeg.input(self.file)
 
     def update(self):
         try:
             if self._file_stream:
                 self._file_reader.chunk = self.scene.rdt
                 data = next(self._file_stream).T
                 self.add_data(data)
                 self.play(data)
         except StopIteration:
             pass
 
-        self.volume.target = 2 * BrokenUtils.rms(self.get_last_n_seconds(0.1)) * (2**0.5)
+        self.volume.target = 2 * root_mean_square(self.get_last_n_seconds(0.1)) * (2**0.5)
         self.std.target    = numpy.std(self.get_last_n_seconds(0.1))
 
 # -------------------------------------------------------------------------------------------------|
```

## ShaderFlow/Modules/Bouncing.py

```diff
@@ -1,16 +1,16 @@
 import random
 from math import cos, sin
 from typing import Iterable
 
 import numpy
 from attr import define
 
-from Broken.Base import clamp
-from Broken.Loaders.LoaderPIL import LoadableImage, LoaderImage
+from Broken import clamp
+from Broken.Loaders import LoadableImage, LoaderImage
 from Broken.Types import TAU, Degrees
 from ShaderFlow.Module import ShaderModule
 from ShaderFlow.Texture import ShaderTexture
 from ShaderFlow.Variable import ShaderVariable
 
 
 @define
```

## ShaderFlow/Modules/Camera.py

```diff
@@ -30,18 +30,17 @@
 
 import math
 from typing import Iterable, Self, Union
 
 import numpy
 import quaternion
 from attr import define
+from loguru import logger as log
 
-from Broken.Base import clamp
-from Broken.BrokenEnum import BrokenEnum
-from Broken.Logging import log
+from Broken import BrokenEnum, clamp
 from Broken.Types import Degrees
 from ShaderFlow import SHADERFLOW
 from ShaderFlow.Message import Message
 from ShaderFlow.Module import ShaderModule
 from ShaderFlow.Modules.Dynamics import DynamicNumber, ShaderDynamics
 from ShaderFlow.Modules.Keyboard import ShaderKeyboard
 from ShaderFlow.Variable import ShaderVariable
```

## ShaderFlow/Modules/Dynamics.py

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import math
 from ast import Tuple
 from copy import deepcopy
 from ctypes import Union
 from math import pi, tau
 from numbers import Number
 from typing import Iterable, Optional, Self
 
@@ -25,16 +26,14 @@
     - https://en.wikipedia.org/wiki/Semi-implicit_Euler_method
     - Control System classes on my university which I got 6/10 final grade
 
     This is a Python-port of the video's math, with custom implementation and extras
     """
 
     def _convert(self, value):
-        if isinstance(value, int):
-            value = float(value)
         return numpy.array(value, dtype=getattr(value, "dtype", self.dtype))
 
     def _set_target(self, attribute, value):
         target = self._convert(value)
         if (target.shape != self.value.shape):
             self.initial = deepcopy(target)
             self.value = deepcopy(target)
@@ -135,36 +134,32 @@
 
         # "Estimate velocity"
         velocity      = (self.target - self.previous)/dt
         self.previous = self.target
 
         # "Clamp k2 to stable values without jitter"
         if (self.radians*dt < self.zeta):
+            k2 = max(self.k1*dt, self.k2, 0.5*(self.k1+dt)*dt)
             k1 = self.k1
-            k2 = max(self.k2, 0.5*(self.k1+dt)*dt, self.k1*dt)
 
         # "Use pole matching when the system is very fast"
         else:
-            t1 = numpy.exp(-1 * self.zeta * self.radians * dt)
-            a1 = 2 * t1 * (numpy.cos if self.zeta <= 1 else numpy.cosh)(self.damping*dt)
+            t1 = math.exp(-1 * self.zeta * self.radians * dt)
+            a1 = 2 * t1 * (math.cos if self.zeta <= 1 else math.cosh)(self.damping*dt)
             t2 = 1/(1 + t1*t1 - a1) * dt
             k1 = t2 * (1 - t1*t1)
             k2 = t2 * dt
 
         # Integrate values
         self.value       += (self.derivative * dt)
         self.acceleration = (self.target + self.k3*velocity - self.value - k1*self.derivative)/k2
         self.derivative  += (self.acceleration * dt)
         self.integral    += (self.value * dt)
         return self.value
 
-    def __call__(self, target: Number=None, dt: float=1.0) -> Number:
-        """Wraps around self.next"""
-        return self.next(target, dt=dt)
-
     def reset(self, instant: bool=False):
         """Reset the system to its initial state"""
         self.target = deepcopy(self.initial)
         if instant:
             self.value = deepcopy(self.initial)
         self.integral = 0
         self.derivative = 0
@@ -248,27 +243,28 @@
         self.next(dt=dt)
 
     @property
     def type(self) -> Optional[str]:
 
         if isinstance(self.value, int):
             return "int"
+
         elif isinstance(self.value, float):
             return "float"
 
-        # Guess type based on shape
-        match self.value.shape:
-            case ():
-                return "float"
-            case (2,):
-                return "vec2"
-            case (3,):
-                return "vec3"
-            case (4,):
-                return "vec4"
+        shape = self.value.shape
+
+        if len(shape) == 0:
+            return "float"
+
+        return {
+            2: "vec2",
+            3: "vec3",
+            4: "vec4",
+        }.get(shape[0], None)
 
     def pipeline(self) -> Iterable[ShaderVariable]:
         if not self.type:
             return
         yield ShaderVariable("uniform", self.type, f"{self.name}", self.value)
         yield ShaderVariable("uniform", self.type, f"{self.name}Integral", self.integral)
         yield ShaderVariable("uniform", self.type, f"{self.name}Derivative", self.derivative)
```

## ShaderFlow/Modules/Piano.py

```diff
@@ -5,20 +5,18 @@
 import tempfile
 from collections import deque
 from pathlib import Path
 from typing import Any, Deque, Dict, Iterable, List, Optional, Tuple
 
 import numpy
 from attr import Factory, define
+from loguru import logger as log
 
-from Broken import BROKEN
-from Broken.Base import BrokenPath, BrokenPlatform, shell
+from Broken import BROKEN, BrokenPath, BrokenPlatform, BrokenSpinner, shell
 from Broken.Externals.FFmpeg import BrokenFFmpeg, FFmpegAudioCodec
-from Broken.Logging import log
-from Broken.Spinner import BrokenSpinner
 from Broken.Types import BPM, Seconds
 from ShaderFlow.Module import ShaderModule
 from ShaderFlow.Modules.Dynamics import DynamicNumber
 from ShaderFlow.Notes import BrokenPianoNote
 from ShaderFlow.Texture import ShaderTexture
 from ShaderFlow.Variable import ShaderVariable
 
@@ -205,14 +203,17 @@
         # No need to check for the entire range 😉
         for midi in range(self.global_minimum_note, self.global_maximum_note+1):
             simultaneous = 0
 
             for note in self.notes_between(midi, time, time+lookup):
                 upcoming.add(midi)
 
+                if (note.start >= time+self.roll_time):
+                    continue
+
                 # This note is being played
                 if (playing := (note.start <= time <= note.end)):
                     self.key_press_dynamics.target[midi] = note.velocity
                     channels[midi] = note.channel
 
                 # Build a 2D Grid of the piano keys being played
                 # • Coordinate: (Note, #offset) @ (Start, End, Channel, Velocity)
```

## ShaderFlow/Modules/Spectrogram.py

```diff
@@ -3,17 +3,17 @@
 from typing import Callable, Iterable, Tuple, Union
 
 import cachetools
 import numpy
 import samplerate
 import scipy
 from attr import Factory, define, field
+from loguru import logger as log
 
-from Broken.Base import SameTracker
-from Broken.Logging import log
+from Broken import SameTracker
 from Broken.Types import Hertz, Samples, Seconds
 from ShaderFlow.Module import ShaderModule
 from ShaderFlow.Modules.Audio import BrokenAudio
 from ShaderFlow.Modules.Dynamics import DynamicNumber
 from ShaderFlow.Notes import BrokenPianoNote
 from ShaderFlow.Texture import ShaderTexture, TextureType
 from ShaderFlow.Variable import ShaderVariable
```

## ShaderFlow/Modules/Video.py

```diff
@@ -5,18 +5,18 @@
 from pathlib import Path
 from typing import Any, Callable, Dict, Tuple
 
 import cv2
 import numpy
 import PIL
 from attr import Factory, define
+from loguru import logger as log
 
-from Broken.Base import BrokenAttrs, BrokenThread, BrokenUtils, SameTracker
+from Broken import BrokenAttrs, BrokenThread, SameTracker, have_import
 from Broken.Externals.FFmpeg import BrokenFFmpeg
-from Broken.Logging import log
 from Broken.Types import Hertz, Seconds
 from ShaderFlow.Module import ShaderModule
 from ShaderFlow.Texture import ShaderTexture
 
 
 @define(slots=False)
 class BrokenSmartVideoFrames(BrokenAttrs):
@@ -72,15 +72,15 @@
             self.decode = lambda frame: frame
 
         elif (self._turbo is not None):
             log.success("Using TurboJPEG for compression. Best speeds available")
             self.encode = lambda frame: self._turbo.encode(frame, quality=self.quality)
             self.decode = lambda frame: self._turbo.decode(frame)
 
-        elif BrokenUtils.have_import("cv2"):
+        elif have_import("cv2"):
             log.success("Using OpenCV for compression. Slower than TurboJPEG but enough")
             self.encode = lambda frame: cv2.imencode(".jpeg", frame)[1]
             self.decode = lambda frame: cv2.imdecode(frame, cv2.IMREAD_COLOR)
 
         else:
             log.warning("Using PIL for compression. Performance killer GIL fallback")
             self.decode = lambda frame: PIL.Image.open(io.BytesIO(frame))
```

## ShaderFlow/Modules/Waveform.py

```diff
@@ -1,15 +1,14 @@
 import math
 from typing import Iterable
 
 import numpy
 from attr import Factory, define
 
-from Broken.Base import BrokenUtils, SameTracker
-from Broken.BrokenEnum import BrokenEnum
+from Broken import BrokenEnum, SameTracker, nearest
 from Broken.Types import Hertz, Samples, Seconds
 from ShaderFlow.Module import ShaderModule
 from ShaderFlow.Modules.Audio import BrokenAudio
 from ShaderFlow.Texture import ShaderTexture, TextureType
 from ShaderFlow.Variable import ShaderVariable
 
 
@@ -70,18 +69,18 @@
 
     @property
     def _offset(self) -> int:
         return self.audio.read % self.chunk_size
 
     @property
     def _cutoff(self) -> Samples:
-        return BrokenUtils.round(
+        return nearest(
             number=self.audio.buffer_size,
             multiple=self.chunk_size,
-            operation=math.floor,
+            operator=math.floor,
             type=int,
         )
 
     _same: SameTracker = Factory(SameTracker)
 
     def update(self):
         self.texture.filter     = ("linear" if self.smooth else "nearest")
```

## ShaderFlow/Optional/Monocular.py

```diff
@@ -1,66 +1,54 @@
-import hashlib
 from typing import Any
 
 import numpy
 import PIL
+import PIL.ImageFilter
 from attr import define
+from loguru import logger as log
 from PIL import Image
 
 import Broken
-from Broken.Loaders.LoaderPIL import LoadableImage, LoaderImage
-from Broken.Logging import log
-from Broken.Spinner import BrokenSpinner
+from Broken import BrokenSpinner, image_hash
+from Broken.Loaders import LoadableImage, LoaderImage
 
 
 @define
 class Monocular:
     _model:     Any = None
     _processor: Any = None
 
     @property
     def device(self) -> str:
         import torch
         if torch.cuda.is_available():
             return "cuda"
         return "cpu"
 
-    def __call__(self,
-        image: LoadableImage,
-        cache: bool=True,
-    ) -> Image:
-        """Alias for .estimate()"""
-        return self.estimate(image=image, cache=cache)
-
     def estimate(self,
         image: LoadableImage,
         cache: bool=True,
     ) -> Image:
         """
         Estimate a Depth Map from an input image with a Monocular Depth Estimation model.
 
         Args:
-            image:      The input image to estimate the depth map from, path, url, PIL
-            cache:      Whether to cache the depth map to the cache directory
+            image: The input image to estimate the depth map from, path, url, PIL
+            cache: Whether to cache the depth map to the cache directory
 
         Returns:
             The estimated depth map as a normalized PIL uint8 Image
         """
 
         # -----------------------------------------------------------------------------------------|
         # Caching
 
         # Load the image
         image = LoaderImage(image).convert("RGB")
-
-        # Calculate hash of the image for caching
-        reduced    = image.resize((256, 256), PIL.Image.NEAREST).convert("L")
-        reduced    = numpy.average(reduced, axis=1)
-        image_hash = hashlib.md5(reduced).hexdigest()
-        cache_path = Broken.PROJECT.DIRECTORIES.CACHE/f"{image_hash}.jpeg"
+        cache_path = Broken.PROJECT.DIRECTORIES.CACHE/f"{image_hash(image)}.depth.png"
 
         # If the depth map is cached, return it
         if (cache and cache_path.exists()):
             log.success(f"DepthMap already cached on ({cache_path})")
             return LoaderImage(cache_path).convert("L")
         log.info(f"DepthMap will be cached on ({cache_path})")
 
@@ -70,15 +58,15 @@
         with BrokenSpinner("Importing PyTorch"):
             import torch
         with BrokenSpinner("Importing Transformers"):
             import transformers
 
         # Load the model
         if not all((self._model, self._processor)):
-            HUGGINGFACE_MODEL = ("LiheYoung/depth-anything-large-hf")
+            HUGGINGFACE_MODEL = ("LiheYoung/depth-anything-base-hf")
             self._processor = transformers.AutoImageProcessor.from_pretrained(HUGGINGFACE_MODEL)
             self._model = transformers.AutoModelForDepthEstimation.from_pretrained(HUGGINGFACE_MODEL)
             self._model.to(self.device)
 
         # Estimate Depth Map
         with BrokenSpinner(f"Estimating Depth Map for the input image (CUDA: {torch.cuda.is_available()})"):
             inputs = self._processor(images=image, return_tensors="pt")
@@ -87,28 +75,21 @@
             # Inference the model
             with torch.no_grad():
                 depth = self._model(**inputs).predicted_depth
 
         # -----------------------------------------------------------------------------------------|
         # Post-processing
 
-        # Resize to the original size
-        depth = torch.nn.functional.interpolate(
-            depth.unsqueeze(1),
-            size=image.size[::-1],
-            mode="bicubic",
-            align_corners=False,
-        )
-
-        # Normalize the depth map
-        depth = depth.squeeze().cpu().numpy()
+        # Normalize image and "fatten" the edges, it's too accurate :^)
+        depth = depth.squeeze(1).cpu().numpy()[0]
         depth = (depth - depth.min()) / ((depth.max() - depth.min()) or 1)
-
-        # Convert array to PIL Image RGB24
         depth = PIL.Image.fromarray((255*depth).astype(numpy.uint8))
+        depth = depth.filter(PIL.ImageFilter.MaxFilter(5))
+        # depth = depth.filter(PIL.ImageFilter.GaussianBlur(1.5))
+        # depth = depth.resize(image.size, PIL.Image.LANCZOS)
 
         # -----------------------------------------------------------------------------------------|
         # Caching
 
         # Save image to Cache
         if cache:
             log.success(f"Saving depth map to cache path ({cache_path})")
```

## ShaderFlow/Resources/Scenes/Examples/Demo.py

```diff
@@ -7,19 +7,19 @@
 from ShaderFlow.Modules.Dynamics import ShaderDynamics
 from ShaderFlow.Modules.Noise import ShaderNoise
 from ShaderFlow.Modules.Spectrogram import ShaderSpectrogram
 from ShaderFlow.Modules.Video import ShaderVideo
 from ShaderFlow.Modules.Waveform import ShaderWaveform
 from ShaderFlow.Notes import BrokenPianoNote
 from ShaderFlow.Scene import ShaderScene
-from ShaderFlow.Shader import Shader
+from ShaderFlow.Shader import ShaderObject
 from ShaderFlow.Texture import ShaderTexture, TextureFilter
 from ShaderFlow.Variable import ShaderVariable
 
-from Broken.Base import BrokenPath
+from Broken import BrokenPath
 
 BACKGROUND = "https://w.wallhaven.cc/full/e7/wallhaven-e778vr.jpg"
 
 # -------------------------------------------------------------------------------------------------|
 
 class Default(ShaderScene):
     """The most basic ShaderFlow Scene, the default shader"""
@@ -38,15 +38,15 @@
 
 class Nested(ShaderScene):
     """Basic scene with two shaders acting together, main shader referencing the child"""
     __name__ = "Nested Shaders"
 
     def build(self):
         ShaderScene.build(self)
-        self.child = Shader(scene=self, name="child")
+        self.child = ShaderObject(scene=self, name="child")
 
         # - Left screen is black, right screen is red
         # - Adds content of child shader to final image
         self.shader.fragment = ("""
             void main() {
                 fragColor.rgb = vec3(stuv.x, 0, 0);
                 fragColor.rgb += texture(child, astuv).rgb;
@@ -240,15 +240,15 @@
         width, height = 192, 108
         random = numpy.random.randint(0, 2, (width, height), dtype=bool)
         self.simulation.texture.size = (width, height)
         self.simulation.texture.write(random.astype(numpy.float32), temporal=1)
 
     def build(self):
         ShaderScene.build(self)
-        self.simulation = Shader(scene=self, name="iLife")
+        self.simulation = ShaderObject(scene=self, name="iLife")
         self.simulation.texture.temporal = 10
         self.simulation.texture.filter = TextureFilter.Nearest
         self.simulation.texture.components = 1
         self.simulation.texture.track = False
         self.simulation.fragment = (self.directory/"GLSL"/"Life/Simulation.glsl")
         self.shader.fragment = (self.directory/"GLSL"/"Life/Visuals.glsl")
```

## ShaderFlow/Resources/Scenes/Examples/GLSL/Bouncing.frag

```diff
@@ -39,10 +39,12 @@
     bool _y = mod(glxy.y, grid_spacing) > (grid_spacing - grid_thick);
     if (_x || _y) {
     	fragColor = vec4(vec3(0.2), 1);
     }
 
     // // Draw the bouncing logo
 
-    fragColor = alpha_composite(fragColor, draw_image(logo, g2s(uv), false));
+    if (!agluv_oob(uv)) {
+        fragColor = alpha_composite(fragColor, gtexture(logo, uv));
+    }
 }
```

## ShaderFlow/Resources/Shaders/Include/ShaderFlow.glsl

```diff
@@ -27,36 +27,44 @@
     return (b*c)/a;
 }
 
 // Smooth relative interpolation between two values given a magnitude difference factor
 // • Applied whenever |b - a| > difference
 // • Positive difference gives min(a, b) else max(a, b)
 float smoothlerp(float a, float b, float difference) {
-    float t = clamp((a-b)/difference + 0.5, 0, 1);
-    float offset = difference*t*(1-t)/2;
+    float t = clamp((a - b)/difference + 0.5, 0, 1);
+    float offset = difference*t*(1 - t)/2;
     return mix(a, b, t) - offset;
 }
 
 // Aliases to smoothlerp, smooth versions of min and max
 float smin(float a, float b, float k) {return smoothlerp(a, b,  k);}
 float smax(float a, float b, float k) {return smoothlerp(a, b, -k);}
-float smin(float a, float b) {return smin(a, b, 1);}
-float smax(float a, float b) {return smax(a, b, 1);}
+float smin(float a, float b) {return smoothlerp(a, b,  1);}
+float smax(float a, float b) {return smoothlerp(a, b, -1);}
 
 // Smoothstep linear interpolation between two values
 // • Useful when a=f(x), b=f(x) and the transition is [x0, x1]
 float smoothmix(float a, float b, float x0, float x1, float x) {
     return mix(a, b, smoothstep(x0, x1, x));
 }
 
 // Aliases to smoothmix, smooth versions of mix
 float smix(float a, float b, float x0, float x1, float x) {
     return smoothmix(a, b, x0, x1, x);
 }
 
+// // Waveforms
+
+// Triangle wave that starts in zero, amplitude 1, range (-1, 1)
+float triangle_wave(float x, float period) {
+    return 2*abs(mod(2*x/period - 0.5, 2) - 1) - 1;
+    // return asin(cos(2*PI*x/period - PI/2)) * (2/PI);
+}
+
 // // Angles and Rotations
 
 // Angle between two vectors for any dimensions
 float angle(vec4 A, vec4 B) {return acos(dot(A, B) / (length(A)*length(B)));}
 float angle(vec3 A, vec3 B) {return acos(dot(A, B) / (length(A)*length(B)));}
 float angle(vec2 A, vec2 B) {return acos(dot(A, B) / (length(A)*length(B)));}
 
@@ -100,14 +108,30 @@
 vec2 astuv2stuv(vec2 astuv) {
     return vec2(astuv.x*iAspectRatio + (1 - iAspectRatio)/2, astuv.y);
 }
 vec2 stuv2astuv(vec2 stuv) {
     return vec2((stuv.x - (1 - iAspectRatio)/2)/iAspectRatio, stuv.y);
 }
 
+// Apply a virtual GL_MIRRORED_REPEAT to a AGLUV coordinate
+vec2 agluv_mirrored_repeat(vec2 agluv) {
+    return vec2(
+        triangle_wave(agluv.x, 4),
+        triangle_wave(agluv.y, 4)
+    );
+}
+
+// Apply a virtual GL_MIRRORED_REPEAT to a GLUV coordinate
+vec2 gluv_mirrored_repeat(vec2 gluv) {
+    return vec2(
+        iAspectRatio * triangle_wave(gluv.x, 4*iAspectRatio),
+        triangle_wave(gluv.y, 4)
+    );
+}
+
 // Out of Bounds checks
 bool astuv_oob(vec2 astuv) {
     return (astuv.x<0)||(astuv.x>1)||(astuv.y<0)||(astuv.y>1);
 }
 bool stuv_oob(vec2 stuv) {
     return astuv_oob(stuv2astuv(stuv));
 }
@@ -128,32 +152,50 @@
     return vec3(
         radius*sin(theta)*cos(phi),
         radius*sin(theta)*sin(phi),
         radius*cos(theta)
     );
 }
 
-// Draws an image on the center considering its aspect ratio (stretches horizontally)
-vec4 draw_image(sampler2D image, vec2 stuv, bool repeat) {
+// // Textures
+
+// GLUV Coordinate texture
+vec4 gtexture(sampler2D image, vec2 gluv) {
     vec2 resolution = textureSize(image, 0);
     vec2 scale = vec2(resolution.y/resolution.x, 1);
-    vec2 gluv  = stuv2gluv(stuv);
-    vec2 uv    = gluv2stuv(gluv*scale);
-    if (!repeat) {
-        if (uv.x<0||uv.x>1||uv.y<0||uv.y>1) {
-            return vec4(0);
-        }
-    }
-    return texture(image, uv);
+    return texture(image, gluv2stuv(gluv*scale));
+}
+
+// GLUV Coordinate + Mirrored Repeat texture
+// Note: Have .repeat(False) (CLAMP_TO_EDGE) on the sampler
+vec4 gmtexture(sampler2D image, vec2 gluv) {
+    return gtexture(image, gluv_mirrored_repeat(gluv));
 }
 
-vec4 draw_image(sampler2D image, vec2 stuv) {
-    return draw_image(image, stuv, true);
+// AGLUV Coordinate texture
+vec4 agtexture(sampler2D image, vec2 agluv) {
+    return gtexture(image, agluv2gluv(agluv));
 }
 
+// AGLUV Coordinate + Mirrored Repeat texture
+// Note: Have .repeat(False) (CLAMP_TO_EDGE) on the sampler
+vec4 agmtexture(sampler2D image, vec2 agluv) {
+    return agtexture(image, agluv_mirrored_repeat(agluv));
+}
+
+vec4 stexture(sampler2D image, vec2 stuv) {
+    return gtexture(image, stuv2gluv(stuv));
+}
+
+vec4 astexture(sampler2D image, vec2 astuv) {
+    return agtexture(image, stuv2gluv(astuv));
+}
+
+#define draw_image stexture
+
 // // Palettes
 
 vec3 palette(float t, vec3 A, vec3 B, vec3 C, vec3 D) {
     if (t < 0.25) {
         return mix(A, B, t*4);
     } else if (t < 0.5) {
         return mix(B, C, (t - 0.25)*4);
@@ -164,15 +206,14 @@
 
 #define PALETTE_MAGMA_1 vec3(0.01060815, 0.01808215, 0.10018654)
 #define PALETTE_MAGMA_2 vec3(0.38092887, 0.12061482, 0.32506528)
 #define PALETTE_MAGMA_3 vec3(0.79650140, 0.10506637, 0.31063031)
 #define PALETTE_MAGMA_4 vec3(0.95922872, 0.53307513, 0.37488950)
 #define palette_magma(x) palette(x, PALETTE_MAGMA_1, PALETTE_MAGMA_2, PALETTE_MAGMA_3, PALETTE_MAGMA_4)
 
-
 // // Piano and Midi Keys
 
 // Black keys have a constant index relative to the octave
 bool isBlackKey(int index) {
     int key = index % 12;
     return key==1||key==3||key==6||key==8||key==10;
 }
@@ -207,15 +248,15 @@
     vec3 d = abs(origin - point) - size/2;
     return min(max(d.x, max(d.y, d.z)), 0) + length(max(d, 0));
 }
 
 // SDF to a Octahedron defined by a point and a size
 float sdOctahedron(vec3 origin, vec3 point, float size) {
     vec3 p = abs(origin - point);
-    return (p.x + p.y + p.z - size) * SQRT3;
+    return SQRT3 * (p.x + p.y + p.z - size);
 }
 
 // Operators
 
 // Union of two SDFs: Join two SDFs into one
 float sdUnion(float a, float b) {
     return min(a, b);
@@ -226,15 +267,15 @@
 float sdSmoothUnion(float a, float b, float width) {
     float k = clamp(0.5 + 0.5*(b-a)/width, 0, 1);
     return mix(b, a, k) - width*k*(1 - k);
 }
 
 // Subtraction of two SDFs: Get the difference between A and B
 float sdSubtraction(float a, float b) {
-    return max(-a, b);
+    return max(b, -a);
 }
 
 // Smooth subtraction of two SDFs: "
 // • width defines the relative value range of the transition
 float sdSmoothSubtraction(float a, float b, float width) {
     float k = clamp(0.5 - 0.5*(b+a)/width, 0, 1);
     return mix(b, -a, k) + width*k*(1 - k);
@@ -248,14 +289,19 @@
 // Smooth intersection of two SDFs: "Opposite of union, so k' = 1 - k"
 // • width defines the relative value range of the transition
 float sdSmoothIntersection(float a, float b, float width) {
     float k = clamp(0.5 - 0.5*(b-a)/width, 0, 1);
     return mix(b, a, k) + width*k*(1 - k);
 }
 
+
+
+
+
+
 // ------------------------------------------------------------------------------------------------|
 // The Bad Code - Accumulated Tech Debt
 
 // // Utils
 
 vec4 alpha_composite(vec4 a, vec4 b) {
     return a*(1 - b.a) + (b * b.a);
```

## SpectroNote/__init__.py

```diff
@@ -1,10 +1,10 @@
 import Broken
 import SpectroNote.Resources as SpectroNoteResources
-from Broken.Project import BrokenProject
+from Broken import BrokenProject
 
 SPECTRONOTE = BrokenProject(
     PACKAGE=__file__,
     APP_NAME="SpectroNote",
     APP_AUTHOR="BrokenSource",
     RESOURCES=SpectroNoteResources,
 )
```

## SpectroNote/__main__.py

```diff
@@ -1,10 +1,10 @@
 import sys
 
-from Broken.Base import BrokenProfiler
+from Broken import BrokenProfiler
 from SpectroNote import SPECTRONOTE
 from SpectroNote.SpectroNote import SpectroNoteScene
 
 
 def main():
     with BrokenProfiler("SPECTRONOTE"):
         SPECTRONOTE.welcome()
```

## Comparing `Broken/Dotmap.py` & `Broken/Core/Staging/BrokenDotmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import contextlib
 from pathlib import Path
 from typing import Any, Dict, Generator, Self, Union
 
-from Broken.Base import BrokenPath
-from Broken.Logging import log
+from loguru import logger as log
+
+from Broken.Core.Path import BrokenPath
 
 
 class BrokenDotmap:
     """
     Trivia
     • Tremeschin 🐙 🎲 🌿 🔱 🪶, [7/7/23 1:29 AM]
     • I just made the most cursed user friendly lazy dictionary you'll ever see
```

## Comparing `Broken/Project.py` & `Broken/Core/BrokenProject.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 import importlib.resources
 import os
 import sys
 import tempfile
 from abc import ABC, abstractmethod
 from pathlib import Path
 
+import diskcache
 import dotenv
 from appdirs import AppDirs
 from attr import define, field
+from loguru import logger as log
 from rich import print as rprint
 from rich.align import Align
 from rich.panel import Panel
 from typer import Typer
 
 import Broken
-from Broken.Base import BrokenPath
-from Broken.Dotmap import BrokenDotmap
-from Broken.Logging import log
+from Broken import BrokenLogging, BrokenPath
 
 
 @define(slots=False)
 class _BrokenProjectDirectories:
     """# Info: You shouldn't really use this class directly"""
 
     # Note: A reference to the main BrokenProject
@@ -32,261 +32,252 @@
     # App basic information
     APP_DIRS: AppDirs = field(default=None)
 
     def __attrs_post_init__(self):
         args = (self.BROKEN_PROJECT.APP_AUTHOR, self.BROKEN_PROJECT.APP_NAME)
         self.APP_DIRS = AppDirs(*reversed(args) if (os.name == "nt") else args)
 
+    def mkdir(self, path: Path, resolve: bool=True) -> Path:
+        """Make a directory and return it"""
+        path = Path(path).resolve() if resolve else Path(path)
+        if not path.exists():
+            log.info(f"Creating directory: {path}")
+            path.mkdir(parents=True, exist_ok=True)
+        return path
+
     @property
     def PACKAGE(self) -> Path:
         """
         When running from the Source Code:
             - The current project's __init__.py location
 
         When running from a Release:
             - Directory where the executable is located
         """
-        if Broken.PYINSTALLER:
+        if Broken.RELEASE:
             return Path(sys.executable).parent.resolve()
-        elif Broken.NUITKA:
-            return Path(sys.argv[0]).parent.resolve()
-        else:
-            return Path(self.BROKEN_PROJECT.PACKAGE).parent.resolve()
+
+        return Path(self.BROKEN_PROJECT.PACKAGE).parent.resolve()
 
     # # Convenience properties
 
     @property
     def APP_NAME(self) -> str:
         return self.BROKEN_PROJECT.APP_NAME
 
     @property
     def APP_AUTHOR(self) -> str:
         return self.BROKEN_PROJECT.APP_AUTHOR
 
-    # # Internal methods
-
-    def __mkdir__(self, path: Path, resolve: bool=True) -> Path:
-        """Make a directory and return it"""
-        path = Path(path).resolve() if resolve else Path(path)
-        if not path.exists():
-            log.info(f"Creating directory: {path}")
-            path.mkdir(parents=True, exist_ok=True)
-        return path
-
     # # Unknown / new project directories
 
     def __set__(self, name: str, value: Path) -> Path:
         """Create a new directory property if Path is given, else set the value"""
-        self.__dict__[name] = value if not isinstance(value, Path) else self.__mkdir__(value)
+        self.__dict__[name] = value if not isinstance(value, Path) else self.mkdir(value)
 
     def __setattr__(self, name: str, value: Path) -> Path:
         self.__set__(name, value)
 
     def __setitem__(self, name: str, value: Path) -> Path:
         self.__set__(name, value)
 
     # # Base directories
 
     @property
     def REPOSITORY(self) -> Path:
         """Broken Source's Monorepo directory"""
-        return self.__mkdir__(self.PACKAGE.parent)
+        return self.mkdir(self.PACKAGE.parent)
 
     @property
     def HOME(self) -> Path:
         """(Unix: /home/$USER), (Windows: C://Users//$USER)"""
-        return self.__mkdir__(Path.home())
+        return self.mkdir(Path.home())
 
     # # Common system directories
 
     @property
     def SYSTEM_ROOT(self) -> Path:
         """(Unix: /), (Windows: C://)"""
-        return self.__mkdir__("/")
+        return self.mkdir("/")
 
     @property
     def SYSTEM_TEMP(self) -> Path:
         """(Unix: /tmp), (Windows: C://Windows//Temp)"""
-        return self.__mkdir__(tempfile.gettempdir())
+        return self.mkdir(tempfile.gettempdir())
 
     # # Broken monorepo specific, potentially useful
 
     @property
-    def BROKEN_BRAKEIT(self) -> Path:
-        """Brakeit bootstrap script"""
-        return self.__mkdir__(self.REPOSITORY/"brakeit.py")
-
-    @property
     def BROKEN_RELEASES(self) -> Path:
         """Broken Source's Monorepo general Releases directory"""
-        return self.__mkdir__(self.REPOSITORY/"Release")
+        return self.mkdir(self.REPOSITORY/"Release")
 
     @property
     def BROKEN_BUILD(self) -> Path:
         """Broken Source's Monorepo general Build directory"""
-        return self.__mkdir__(self.REPOSITORY/"Build")
+        return self.mkdir(self.REPOSITORY/"Build")
 
     @property
     def BROKEN_WINEPREFIX(self) -> Path:
         """Broken Source's Monorepo Wineprefix directory for Build"""
-        return self.__mkdir__(self.BROKEN_BUILD/"Wineprefix")
+        return self.mkdir(self.BROKEN_BUILD/"Wineprefix")
 
     @property
     def BROKEN_WHEELS(self) -> Path:
         """Broken Source's Monorepo Wheels directory for Build"""
-        return self.__mkdir__(self.BROKEN_BUILD/"Wheels")
+        return self.mkdir(self.BROKEN_BUILD/"Wheels")
 
     @property
     def BROKEN_PROJECTS(self) -> Path:
         """Broken Source's Monorepo Projects directory"""
-        return self.__mkdir__(self.REPOSITORY/"Projects")
+        return self.mkdir(self.REPOSITORY/"Projects")
 
     @property
     def BROKEN_HOOK(self) -> Path:
         """Hook directory for other projects to be managed by Broken"""
-        return self.__mkdir__(self.PROJECTS/"Hook")
+        return self.mkdir(self.PROJECTS/"Hook")
 
     @property
     def BROKEN_META(self) -> Path:
         """Broken Source's Monorepo Meta directory (Many submodules there)"""
-        return self.__mkdir__(self.REPOSITORY/"Meta")
+        return self.mkdir(self.REPOSITORY/"Meta")
 
     @property
     def BROKEN_FORK(self) -> Path:
         """Broken Source's Monorepo Forks directory"""
-        return self.__mkdir__(self.BROKEN_META/"Fork")
+        return self.mkdir(self.BROKEN_META/"Fork")
 
     @property
     def BROKEN_PRIVATE(self) -> Path:
         """Broken Source's Monorepo Private directory"""
-        return self.__mkdir__(self.REPOSITORY/"Private")
+        return self.mkdir(self.REPOSITORY/"Private")
 
     # # Meta directories - Broken monorepo specific
 
     @property
     def DOCS(self) -> Path:
         """Broken Source's Monorepo Docs directory"""
-        return self.__mkdir__(self.REPOSITORY/"Docs")
+        return self.mkdir(self.REPOSITORY/"Docs")
 
     @property
     def WEBSITE(self) -> Path:
         """Broken Source's Website directory"""
-        return self.__mkdir__(self.REPOSITORY/"Website")
+        return self.mkdir(self.REPOSITORY/"Website")
 
     @property
     def PAPERS(self) -> Path:
         """Broken Source's Monorepo Papers directory"""
-        return self.__mkdir__(self.META/"Papers")
+        return self.mkdir(self.META/"Papers")
 
     @property
     def TEMPLATES(self) -> Path:
         """Broken Source's Monorepo Templates directory"""
-        return self.__mkdir__(self.META/"Templates")
+        return self.mkdir(self.META/"Templates")
 
     # # Workspace directories
 
     @property
     def WORKSPACE(self) -> Path:
         """Root for the current Project's Workspace"""
         if (path := os.environ.get("WORKSPACE", None)):
-            return self.__mkdir__(Path(path)/self.APP_AUTHOR/self.APP_NAME)
+            return self.mkdir(Path(path)/self.APP_AUTHOR/self.APP_NAME)
         if (os.name == "nt"):
-            return self.__mkdir__(Path(self.APP_DIRS.user_data_dir))
+            return self.mkdir(Path(self.APP_DIRS.user_data_dir))
         else:
-            return self.__mkdir__(Path(self.APP_DIRS.user_data_dir)/self.APP_NAME)
+            return self.mkdir(Path(self.APP_DIRS.user_data_dir)/self.APP_NAME)
 
     @property
     def CONFIG(self) -> Path:
         """General config directory"""
-        return self.__mkdir__(self.WORKSPACE/"Config")
+        return self.mkdir(self.WORKSPACE/"Config")
 
     @property
     def LOGS(self) -> Path:
         """General logs directory"""
-        return self.__mkdir__(self.WORKSPACE/"Logs")
+        return self.mkdir(self.WORKSPACE/"Logs")
 
     @property
     def CACHE(self) -> Path:
         """General cache directory"""
-        return self.__mkdir__(self.WORKSPACE/"Cache")
+        return self.mkdir(self.WORKSPACE/"Cache")
 
     @property
     def DATA(self) -> Path:
         """General Data directory"""
-        return self.__mkdir__(self.WORKSPACE/"Data")
+        return self.mkdir(self.WORKSPACE/"Data")
 
     @property
     def MOCK(self) -> Path:
         """Mock directory for testing"""
-        return self.__mkdir__(self.WORKSPACE/"Mock")
+        return self.mkdir(self.WORKSPACE/"Mock")
 
     @property
     def PROJECTS(self) -> Path:
         """Projects directory (e.g. Video Editor or IDEs)"""
-        return self.__mkdir__(self.WORKSPACE/"Projects")
+        return self.mkdir(self.WORKSPACE/"Projects")
 
     @property
     def OUTPUT(self) -> Path:
         """Output directory if it makes more sense than .DATA or .PROJECTS"""
-        return self.__mkdir__(self.WORKSPACE/"Output")
+        return self.mkdir(self.WORKSPACE/"Output")
 
     @property
     def DOWNLOADS(self) -> Path:
         """Downloads directory"""
-        return self.__mkdir__(self.WORKSPACE/"Downloads")
+        return self.mkdir(self.WORKSPACE/"Downloads")
 
     @property
     def EXTERNALS(self) -> Path:
         """Third party dependencies"""
-        return self.__mkdir__(self.WORKSPACE/"Externals")
+        return self.mkdir(self.WORKSPACE/"Externals")
 
     @property
     def EXTERNAL_ARCHIVES(self) -> Path:
         """Third party archives"""
-        return self.__mkdir__(self.EXTERNALS/"Archives")
+        return self.mkdir(self.EXTERNALS/"Archives")
 
     @property
     def EXTERNAL_IMAGES(self) -> Path:
         """Third party images"""
-        return self.__mkdir__(self.EXTERNALS/"Images")
+        return self.mkdir(self.EXTERNALS/"Images")
 
     @property
     def EXTERNAL_AUDIO(self) -> Path:
         """Third party audio"""
-        return self.__mkdir__(self.EXTERNALS/"Audio")
+        return self.mkdir(self.EXTERNALS/"Audio")
 
     @property
     def EXTERNAL_FONTS(self) -> Path:
         """Third party fonts"""
-        return self.__mkdir__(self.EXTERNALS/"Fonts")
+        return self.mkdir(self.EXTERNALS/"Fonts")
 
     @property
     def EXTERNAL_SOUNDFONTS(self) -> Path:
         """Third party soundfonts"""
-        return self.__mkdir__(self.EXTERNALS/"Soundfonts")
+        return self.mkdir(self.EXTERNALS/"Soundfonts")
 
     @property
     def EXTERNAL_MIDIS(self) -> Path:
         """Third party midis"""
-        return self.__mkdir__(self.EXTERNALS/"Midis")
+        return self.mkdir(self.EXTERNALS/"Midis")
 
     @property
     def TEMP(self) -> Path:
         """Temporary directory for working files"""
-        return self.__mkdir__(self.WORKSPACE/"Temp")
+        return self.mkdir(self.WORKSPACE/"Temp")
 
     @property
     def DUMP(self) -> Path:
         """Dump directory for debugging (e.g. Shaders)"""
-        return self.__mkdir__(self.WORKSPACE/"Dump")
+        return self.mkdir(self.WORKSPACE/"Dump")
 
     @property
     def SCREENSHOTS(self) -> Path:
         """Screenshots directory"""
-        return self.__mkdir__(self.WORKSPACE/"Screenshots")
+        return self.mkdir(self.WORKSPACE/"Screenshots")
 
 # -------------------------------------------------------------------------------------------------|
 
 @define(slots=False)
 class _BrokenProjectResources:
     """# Info: You shouldn't really use this class directly"""
 
@@ -380,39 +371,27 @@
     # App information
     APP_NAME:   str = field(default="Broken")
     APP_AUTHOR: str = field(default="BrokenSource")
 
     # Standard Broken objects for a project
     DIRECTORIES: _BrokenProjectDirectories = None
     RESOURCES:   _BrokenProjectResources   = None
-    CONFIG:      BrokenDotmap              = None
-    CACHE:       BrokenDotmap              = None
     VERSION:     str                       = None
 
     def __attrs_post_init__(self):
 
         # Create Directories class
         self.DIRECTORIES = _BrokenProjectDirectories(BROKEN_PROJECT=self)
         self.RESOURCES   = _BrokenProjectResources  (BROKEN_PROJECT=self)
         self.PACKAGE     = Path(self.PACKAGE)
 
-        # Assign version - Package's parent folder name
         # Fixme: Split the projects into many packages
+        # self.VERSION = importlib.metadata.version(self.PACKAGE.parent.name.replace("Broken", "broken-source"))
         self.VERSION = Broken.VERSION
-        # self.VERSION = importlib.metadata.version(self.PACKAGE.parent.name
-        #     .replace("Broken", "broken-source")
-        # )
-
-        # Create default config
-        self.CONFIG = BrokenDotmap(path=self.DIRECTORIES.CONFIG/f"{self.APP_NAME}.toml")
-        self.CACHE  = BrokenDotmap(path=self.DIRECTORIES.SYSTEM_TEMP/f"{self.APP_NAME}.pickle")
-
-        # Create logger based on configuration
-        os.environ["BROKEN_CURRENT_PROJECT_NAME"] = self.APP_NAME
-        self.__START_LOGGING__()
+        BrokenLogging.set_project(self.APP_NAME)
 
         # Convenience: Symlink Workspace to projects data directory
         if Broken.DEVELOPMENT:
             try:
                 BrokenPath.symlink(
                     virtual=self.DIRECTORIES.REPOSITORY/"Workspace",
                     real=self.DIRECTORIES.WORKSPACE,
@@ -442,42 +421,14 @@
             )),
             padding=1,
             title_align="center",
             subtitle_align="center",
         ))
         print()
 
-    @property
-    def LOGLEVEL(self) -> str:
-        return (
-            os.environ.get("LOGLEVEL", "").upper()
-            or self.CONFIG.logging.default("level", "info").upper()
-        )
-
-    @LOGLEVEL.setter
-    def LOGLEVEL(self, value: str):
-        self.CONFIG.logging.level = value
-        self.__START_LOGGING__()
-
-    def __START_LOGGING__(self):
-        log.stdout(self.LOGLEVEL)
-        # log.file(self.DIRECTORIES.LOGS/f"{self.APP_NAME}.log", self.LOGLEVEL)
-
-        # # Fixme: Two logging instances on the same file on Windows?
-        # try:
-        #     log.file(self.DIRECTORIES.LOGS/f"{self.APP_NAME}.log", self.LOGLEVEL)
-        # except PermissionError as e:
-        #     # Fixme: Two logging instances for the same file on Windows doesn't work
-        #     if os.name == "nt":
-        #         pass
-        #     else:
-        #         raise e
-        # except Exception as e:
-        #     raise e
-
 # -------------------------------------------------------------------------------------------------|
 
 @define
 class BrokenApp(ABC):
     broken_typer: Typer = None
 
     @abstractmethod
```

## Comparing `Broken/Spinner.py` & `Broken/Core/BrokenSpinner.py`

 * *Files identical despite different names*

## Comparing `Broken/BrokenEnum/__init__.py` & `Broken/Core/BrokenEnum.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,87 @@
+"""
+<div align="justify">
+
+<div align="center">
+  <h1>♻️ BrokenEnum ♻️</h1>
+
+  **Smarter** Python **Enum classes** with builtin **Automation** and **Safety**
+</div>
+
+<br>
+
+# 🔥 Description
+
+This package adds lots of utilities to the standard `Enum` class in Python
+
+- **Convenient**: Find members by name or value (or both)
+- **Cycling**: You can cycle through the options of an enum
+- **Fast**: Functions are cached with `functools.lru_cache`
+
+<br>
+
+# 🚀 Examples
+```python
+# Import package
+from Broken import BrokenEnum
+
+# Define a render quality enum
+class Quality(BrokenEnum):
+    Low    = 0
+    Medium = 1
+    High   = 2
+
+# Get values from key or name
+assert Quality.get(0)     == Quality.Low
+assert Quality.get("Low") == Quality.Low
+assert Quality.get("low") == Quality.Low
+assert Quality(2)         == Quality.High
+
+# It is safe to .get(member) themselves
+assert Quality.get(Quality.Low) == Quality.Low
+
+# If you want to search only by value or name
+assert Quality.from_value(0)       == Quality.Low
+assert Quality.from_value("low")   == None
+assert Quality.from_name("medium") == Quality.Medium
+Quality.from_name(2) # Raises ValueError
+
+# Cycling through the options
+assert Quality.Low.next()         == Quality.Medium
+assert Quality.High.next()        == Quality.Low
+assert Quality.Low.next(offset=2) == Quality.High
+
+# Can cycle through the options in reverse and from member
+value = Quality.Low
+assert value.previous() == Quality.High
+assert (value := value.previous(2)) == Quality.Medium
+
+# Getting list of members or names, keys
+assert Quality.values  == (0, 1, 2)
+assert Quality.names   == ("Low", "Medium", "High")
+assert Quality.keys    == ("Low", "Medium", "High")
+assert Quality.options == (
+    Quality.Low,
+    Quality.Medium,
+    Quality.High,
+)
+
+# Get tuples or key, value
+assert Quality.items == (
+    ("Low",    0),
+    ("Medium", 1),
+    ("High",   2),
+)
+
+# Get options as a dictionary
+assert Quality.dict == dict(Low=0, Medium=1, High=2)
+```
+
+</div>
+"""
 import enum
 import functools
 from typing import Any, Dict, Optional, Self, Tuple, Union
 
 import attrs
```

## Comparing `Broken/BrokenEnum/__test__.py` & `Broken/Tests/Enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from Broken.BrokenEnum import BrokenEnum
+from Broken import BrokenEnum
 
 # -------------------------------------------------------------------------------------------------|
 # Basic usage
 
 def get_fruits():
     # A translation enum example
     class Fruits(BrokenEnum):
```

## Comparing `Broken/Loaders/LoaderPIL.py` & `Broken/Loaders/LoaderImage.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,71 @@
 import io
 from pathlib import Path
-from Broken.Logging import log
 from typing import Any, Optional, Union
 
 import numpy
 import PIL
 import validators
 from attr import define
+from loguru import logger as log
 from PIL.Image import Image
 
-from Broken import BROKEN
-from Broken.Base import BrokenPath
+import Broken
+from Broken.Loaders import BrokenLoader
 from Broken.Types import URL
 
-from . import BrokenLoader
-
 
 @define
 class LoaderImage(BrokenLoader):
     _cache = None
 
     @staticmethod
     def cache() -> Any:
         try:
             import requests_cache
             if not LoaderImage._cache:
                 LoaderImage._cache = requests_cache.CachedSession(
-                    BROKEN.DIRECTORIES.CACHE/"LoaderImage.sqlite",
+                    Broken.BROKEN.DIRECTORIES.CACHE/"LoaderImage.sqlite",
                 )
         except ImportError:
             return None
 
         return LoaderImage._cache
 
     @staticmethod
     def load(value: Any=None, **kwargs) -> Optional[Image]:
+
         if value is None:
             return None
 
         elif isinstance(value, Image):
-            log.debug(f"Loading Image from Image")
+            log.debug("Loading already an Instance of Image")
+            return value
+
+        elif value is Image:
+            log.debug("Loading already an Class of Image")
             return value
 
         elif isinstance(value, numpy.ndarray):
-            log.debug(f"Loading Image from Numpy Array")
+            log.debug("Loading Image from Numpy Array")
             return PIL.Image.fromarray(value, **kwargs)
 
-        elif (path := BrokenPath(value, valid=True)):
+        elif (path := Path(value)).exists():
             log.debug(f"Loading Image from Path ({path})")
             return PIL.Image.open(path, **kwargs)
 
         elif validators.url(value):
             log.debug(f"Loading Image from URL ({value})")
 
             if LoaderImage.cache():
                 return PIL.Image.open(io.BytesIO(LoaderImage.cache().get(value).content), **kwargs)
 
             import requests
             return PIL.Image.open(io.BytesIO(requests.get(value).content), **kwargs)
 
         elif isinstance(value, bytes):
-            log.debug(f"Loading Image from Bytes")
+            log.debug("Loading Image from Bytes")
             return PIL.Image.open(io.BytesIO(value), **kwargs)
 
         return None
 
 LoadableImage = Union[Image, Path, URL, numpy.ndarray, bytes, None]
```

## Comparing `Broken/Staging/umidi.py` & `Broken/Core/Staging/umidi.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import math
 from collections import deque
 from pathlib import Path
 from typing import Any, Deque, Iterable, Self, Tuple, TypeAlias, Union
 
 from attr import Factory, define
 
-from Broken.Types import Seconds
+from Broken.Core.Types import Seconds
 
 __all__ = ["Midi", "Events", "Note"]
 
 # -------------------------------------------------------------------------------------------------|
 
 PIANO_NOTES = "C C# D D# E F F# G G# A A# B".split()
 MICROSECONDS_PER_MINUTE: int = 60_000_000
```

## Comparing `Broken/Staging/Dotmap/BaseLoader.py` & `Broken/Core/Staging/Dotmap/BaseLoader.py`

 * *Files identical despite different names*

## Comparing `Broken/Staging/Dotmap/BrokenDotmap.py` & `Broken/Core/Staging/Dotmap/BrokenDotmap.py`

 * *Files identical despite different names*

## Comparing `Broken/Staging/Dotmap/__test__.py` & `Broken/Core/Staging/Dotmap/__test__.py`

 * *Files identical despite different names*

## Comparing `Broken/Staging/Dotmap/Loaders/LoaderPIL.py` & `Broken/Core/Staging/Dotmap/Loaders/LoaderPIL.py`

 * *Files identical despite different names*

## Comparing `Broken/Staging/Dotmap/Loaders/LoaderTOML.py` & `Broken/Core/Staging/Dotmap/Loaders/LoaderTOML.py`

 * *Files identical despite different names*

## Comparing `broken_source-0.1.3.dist-info/METADATA` & `broken_source-0.2.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: broken-source
-Version: 0.1.3
+Version: 0.2.0
 Summary: Broken Source Software Framework
 Project-URL: repository, https://github.com/BrokenSource/BrokenSource
 Project-URL: homepage, https://brokensrc.dev
 Project-URL: documentation, https://brokensrc.dev
 Project-URL: issues, https://brokensrc.dev/contact
 Author-email: Tremeschin <29046864+Tremeschin@users.noreply.github.com>
 License-Expression: AGPL-3.0
@@ -12,51 +12,55 @@
 Requires-Dist: appdirs>=1.4.4
 Requires-Dist: arrow>=1.3.0
 Requires-Dist: attrs>=23.2.0
 Requires-Dist: audioread>=3.0.1
 Requires-Dist: cachetools>=5.3.3
 Requires-Dist: cattrs>=23.2.3
 Requires-Dist: datetime>=5.5
+Requires-Dist: diskcache>=5.6.3
 Requires-Dist: distro>=1.9.0
 Requires-Dist: dotmap>=1.3.30
 Requires-Dist: glcontext>=2.5.0
 Requires-Dist: glfw>=2.7.0
+Requires-Dist: imageio>=2.34.1
 Requires-Dist: imgui>=2.0.0
 Requires-Dist: intervaltree>=3.1.0
+Requires-Dist: loguru>=0.7.2
 Requires-Dist: midi2audio>=0.1.1
 Requires-Dist: mido>=1.3.2
 Requires-Dist: moderngl-window>=2.4.6
 Requires-Dist: moderngl>=5.10.0
 Requires-Dist: numpy-quaternion>=2023.0.3
-Requires-Dist: numpy>=1.26.3
+Requires-Dist: numpy>=1.26.4
 Requires-Dist: opencv-contrib-python>=4.9.0.80
-Requires-Dist: opensimplex>=0.4.5
-Requires-Dist: pillow==10.2.0
+Requires-Dist: opensimplex>=0.4.5.1
+Requires-Dist: pillow>=10.3.0
 Requires-Dist: pip>=24.0
 Requires-Dist: pretty-errors>=1.2.25
 Requires-Dist: pretty-midi>=0.2.10
+Requires-Dist: pydantic>=2.7.1
 Requires-Dist: pyfiglet>=1.0.2
 Requires-Dist: pyfluidsynth>=1.3.3
 Requires-Dist: pygame>=2.5.2
 Requires-Dist: python-dotenv>=1.0.1
 Requires-Dist: python-rtmidi>=1.5.8
 Requires-Dist: pyturbojpeg>=1.7.3
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: requests-cache>=1.2.0
-Requires-Dist: requests>=2.28.1
+Requires-Dist: requests>=2.31.0
 Requires-Dist: rich>=13.7.1
 Requires-Dist: samplerate>=0.2.1
 Requires-Dist: schedule>=1.2.1
-Requires-Dist: scipy>=1.12.0
+Requires-Dist: scipy>=1.13.0
 Requires-Dist: soundcard>=0.4.3
 Requires-Dist: thefuzz>=0.22.1
 Requires-Dist: toml>=0.10.2
-Requires-Dist: tqdm>=4.64.1
-Requires-Dist: typer>=0.10.0
-Requires-Dist: validators>=0.24.0
+Requires-Dist: tqdm>=4.66.4
+Requires-Dist: typer>=0.12.3
+Requires-Dist: validators>=0.28.1
 Requires-Dist: watchdog>=4.0.0
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://brokensrc.dev"><img src="https://raw.githubusercontent.com/BrokenSource/BrokenSource/Master/Broken/Resources/Images/Broken.png" width="200"></a>
   <h2>Broken Source Software</h2>
   <br>
```

### html2text {}

```diff
@@ -1,34 +1,35 @@
-Metadata-Version: 2.3 Name: broken-source Version: 0.1.3 Summary: Broken Source
+Metadata-Version: 2.3 Name: broken-source Version: 0.2.0 Summary: Broken Source
 Software Framework Project-URL: repository, https://github.com/BrokenSource/
 BrokenSource Project-URL: homepage, https://brokensrc.dev Project-URL:
 documentation, https://brokensrc.dev Project-URL: issues, https://
 brokensrc.dev/contact Author-email: Tremeschin
 <29046864+Tremeschin@users.noreply.github.com> License-Expression: AGPL-3.0
 Requires-Python: >=3.10 Requires-Dist: appdirs>=1.4.4 Requires-Dist:
 arrow>=1.3.0 Requires-Dist: attrs>=23.2.0 Requires-Dist: audioread>=3.0.1
 Requires-Dist: cachetools>=5.3.3 Requires-Dist: cattrs>=23.2.3 Requires-Dist:
-datetime>=5.5 Requires-Dist: distro>=1.9.0 Requires-Dist: dotmap>=1.3.30
-Requires-Dist: glcontext>=2.5.0 Requires-Dist: glfw>=2.7.0 Requires-Dist:
-imgui>=2.0.0 Requires-Dist: intervaltree>=3.1.0 Requires-Dist:
+datetime>=5.5 Requires-Dist: diskcache>=5.6.3 Requires-Dist: distro>=1.9.0
+Requires-Dist: dotmap>=1.3.30 Requires-Dist: glcontext>=2.5.0 Requires-Dist:
+glfw>=2.7.0 Requires-Dist: imageio>=2.34.1 Requires-Dist: imgui>=2.0.0
+Requires-Dist: intervaltree>=3.1.0 Requires-Dist: loguru>=0.7.2 Requires-Dist:
 midi2audio>=0.1.1 Requires-Dist: mido>=1.3.2 Requires-Dist: moderngl-
 window>=2.4.6 Requires-Dist: moderngl>=5.10.0 Requires-Dist: numpy-
-quaternion>=2023.0.3 Requires-Dist: numpy>=1.26.3 Requires-Dist: opencv-
-contrib-python>=4.9.0.80 Requires-Dist: opensimplex>=0.4.5 Requires-Dist:
-pillow==10.2.0 Requires-Dist: pip>=24.0 Requires-Dist: pretty-errors>=1.2.25
-Requires-Dist: pretty-midi>=0.2.10 Requires-Dist: pyfiglet>=1.0.2 Requires-
-Dist: pyfluidsynth>=1.3.3 Requires-Dist: pygame>=2.5.2 Requires-Dist: python-
-dotenv>=1.0.1 Requires-Dist: python-rtmidi>=1.5.8 Requires-Dist:
-pyturbojpeg>=1.7.3 Requires-Dist: pyyaml>=6.0.1 Requires-Dist: requests-
-cache>=1.2.0 Requires-Dist: requests>=2.28.1 Requires-Dist: rich>=13.7.1
-Requires-Dist: samplerate>=0.2.1 Requires-Dist: schedule>=1.2.1 Requires-Dist:
-scipy>=1.12.0 Requires-Dist: soundcard>=0.4.3 Requires-Dist: thefuzz>=0.22.1
-Requires-Dist: toml>=0.10.2 Requires-Dist: tqdm>=4.64.1 Requires-Dist:
-typer>=0.10.0 Requires-Dist: validators>=0.24.0 Requires-Dist: watchdog>=4.0.0
-Description-Content-Type: text/markdown
+quaternion>=2023.0.3 Requires-Dist: numpy>=1.26.4 Requires-Dist: opencv-
+contrib-python>=4.9.0.80 Requires-Dist: opensimplex>=0.4.5.1 Requires-Dist:
+pillow>=10.3.0 Requires-Dist: pip>=24.0 Requires-Dist: pretty-errors>=1.2.25
+Requires-Dist: pretty-midi>=0.2.10 Requires-Dist: pydantic>=2.7.1 Requires-
+Dist: pyfiglet>=1.0.2 Requires-Dist: pyfluidsynth>=1.3.3 Requires-Dist:
+pygame>=2.5.2 Requires-Dist: python-dotenv>=1.0.1 Requires-Dist: python-
+rtmidi>=1.5.8 Requires-Dist: pyturbojpeg>=1.7.3 Requires-Dist: pyyaml>=6.0.1
+Requires-Dist: requests-cache>=1.2.0 Requires-Dist: requests>=2.31.0 Requires-
+Dist: rich>=13.7.1 Requires-Dist: samplerate>=0.2.1 Requires-Dist:
+schedule>=1.2.1 Requires-Dist: scipy>=1.13.0 Requires-Dist: soundcard>=0.4.3
+Requires-Dist: thefuzz>=0.22.1 Requires-Dist: toml>=0.10.2 Requires-Dist:
+tqdm>=4.66.4 Requires-Dist: typer>=0.12.3 Requires-Dist: validators>=0.28.1
+Requires-Dist: watchdog>=4.0.0 Description-Content-Type: text/markdown
   _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_B_r_o_k_e_n_S_o_u_r_c_e_/_B_r_o_k_e_n_S_o_u_r_c_e_/_M_a_s_t_e_r_/_B_r_o_k_e_n_/
                          _R_e_s_o_u_r_c_e_s_/_I_m_a_g_e_s_/_B_r_o_k_e_n_._p_n_g_]
                       ********** BBrrookkeenn SSoouurrccee SSooffttwwaarree **********
 
     Here lies BBrrookkeenn: The SShhaarreedd LLiibbrraarryy and MMaannaaggeerr + SSuubbmmoodduulleess of all my
                                    PPrroojjeeccttss
```

## Comparing `broken_source-0.1.3.dist-info/RECORD` & `broken_source-0.2.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,97 @@
-Broken/Base.py,sha256=V9KsoObvT72cEyAWYbZSQMjuMHssEQCT32kNFk4yKWo,61304
-Broken/Dotmap.py,sha256=5ZAgSo2nv0lE33r14i-j4Bb_iVFzRHWpllR9bNzGUEw,8139
-Broken/Logging.py,sha256=rxVXHDQFdBKYKwhv9UBd8ehIFq9rxV08tx62lEsLymM,6363
-Broken/Project.py,sha256=on9OzegxJcfy00jxktBO5kfen--i8CFUZEDyqS8R20A,14839
-Broken/Spinner.py,sha256=J9bX0PBQ_myn55h8a_TNnCYz97AbQ3h43XU_cdDS7Z4,2221
-Broken/Types.py,sha256=GZiW_njBuTIM_UYx7yrLG5_SJaZupyW6KFPvCZWJ9Ls,1395
-Broken/__init__.py,sha256=-cXW7nlCVSNCzFosWOsk1bXqONl_CjtCCbMXMygrNow,3983
-Broken/__main__.py,sha256=PJSGcON9fXSd5JMrzKa50NJQ6U6QNpjXSa1hZC6fUtE,29393
-Broken/BrokenEnum/Readme.md,sha256=86oajJkRmzWKoC_2eTEEc1fXMJ8-QOfrUDIzAHqkujQ,1983
-Broken/BrokenEnum/__init__.py,sha256=gw-wbYTgKPyQdh57riiPUb63ZR1zZ8FhLC3q_lSyk7g,9815
-Broken/BrokenEnum/__test__.py,sha256=9wMz89O0FSrKUaSgF24r39ReKNqPXN0Eey4bM9qzPvo,3815
-Broken/Externals/__init__.py,sha256=OZQHtHaBYL-u0mDfTJFwMY3_NDNhzQl0gpOXKcn8fX4,276
+Broken/Types.py,sha256=iOmSBAm5_-lpim5TkCsNAkLwO4WSCg4E-RmehIpiyV8,1040
+Broken/__init__.py,sha256=TWh2Onfkkw93mcLTBr3bP38eKzqrkWYheVi8WHth0ks,4020
+Broken/__main__.py,sha256=kg04NdJSt6tZHvB5xm7EFW9PMSvFT_fug7_etJboWro,22411
+Broken/Core/BrokenEnum.py,sha256=b-ZT2h2qpudgTpRI82ST4QjJw3jzXruZPY_Ntr9r5LM,11807
+Broken/Core/BrokenLogging.py,sha256=ux-yuPvxUQC1Z5RBlNzfH_w4DlnKJQtK2d2Qy6HAnZ0,2586
+Broken/Core/BrokenPath.py,sha256=FXmboI3mHGr23wRhlsRQdI-gG_sNRIzo3DfMUFmys3M,18578
+Broken/Core/BrokenPlatform.py,sha256=cUHhJpzpOcAxikWhbJVvMIOeAlYiY7tvNBS1qicOp00,4011
+Broken/Core/BrokenProfiler.py,sha256=pkjB98aI6PCzI-XdOwSRTJvMfhEPS179WsVQ1NBVwL4,1741
+Broken/Core/BrokenProject.py,sha256=Lg4X58FmdHtUxoHGftRi4seTEYezmeLMvZSl3Tcz4_8,12963
+Broken/Core/BrokenResolution.py,sha256=L0_nt5tgMYEXxJ8bJhOac5lndCPgNQO38mBdnVB8AOY,3364
+Broken/Core/BrokenScheduler.py,sha256=3vP7Xc1XxeRhVvDbqE9wPM9i4M0oboBW5ho4wKGTbOA,7259
+Broken/Core/BrokenSpinner.py,sha256=J9bX0PBQ_myn55h8a_TNnCYz97AbQ3h43XU_cdDS7Z4,2221
+Broken/Core/BrokenThread.py,sha256=AhSMix25ykZ7pLg8n5rczYwq1PleOqfrj4BIlrHGG2o,3783
+Broken/Core/BrokenTorch.py,sha256=CrkFA9uFBrdso2I6iXK2s-QO7GMU5VF536fF3VOsXgY,2475
+Broken/Core/BrokenTyper.py,sha256=7eiu_ZKKe_q2HQ7gml2zBSbneA7h6VeiQ2b_Jn2-G3M,3741
+Broken/Core/BrokenUtils.py,sha256=RYckFtQ47KG66oJEmFwOgFwetmH3mvT36fvU3Ru_zzg,4348
+Broken/Core/__init__.py,sha256=RVeebkreqe53-jRQQjvrbhjiA-L16-5iYaEoP0vR0yg,9571
+Broken/Core/Staging/BrokenDotmap.py,sha256=GtSoGtbiHyCb_d__5R2rwsMKyd9FHesVNPVVq_xr6Ac,8147
+Broken/Core/Staging/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+Broken/Core/Staging/umidi.py,sha256=mKi37fOFNWE4yNQWL9Hv6H_eob8cphZKq3dGhbCUV08,18413
+Broken/Core/Staging/Dotmap/BaseLoader.py,sha256=omvfs7KqJKswYiY-HVFFLF6XlXU2hjDIHQCvubCP43k,1736
+Broken/Core/Staging/Dotmap/BrokenDotmap.py,sha256=PDYmq1qojJMc71Y7Gf8LPlPTN4ZOqIuAW88vd-piDJQ,12082
+Broken/Core/Staging/Dotmap/Readme.md,sha256=vnlwmb2qAeivLvsh3weieTyf4HgGbUoGxmeQgPLGkLc,368
+Broken/Core/Staging/Dotmap/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+Broken/Core/Staging/Dotmap/__test__.py,sha256=Hg-kTzP8AvGt_mCg241Uz5cbOtXnTebuLb7cl594U5Y,3568
+Broken/Core/Staging/Dotmap/Loaders/LoaderPIL.py,sha256=X1U6O2v0sx6Wcqd-vbudWh-h-y2lqCwdCx_a-AoHsJ8,1467
+Broken/Core/Staging/Dotmap/Loaders/LoaderTOML.py,sha256=VvruuBpPEXKgWnkiRlmW6JPxBsb0Ni0fJQ6lyopaOlc,1263
+Broken/Core/Staging/Dotmap/Loaders/__init__.py,sha256=wcJEGoWRpwKIgSR4sEwyrjk-LQ9jIKYXDJ3CZxwDagg,68
+Broken/Externals/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 Broken/Externals/FFmpeg/Readme.md,sha256=8ejqL6Ca5P9UNIGUuD7DMELdmJ9JepavQ_RYU-6ZdQI,1480
-Broken/Externals/FFmpeg/__init__.py,sha256=BhI3BUlUJgfU82unXecshyMQn7IvzX-lVKZaKbXaw4M,45735
-Broken/Externals/Upscaler/__init__.py,sha256=amnD0zakvjj8mmeRAHsriNUPC2MmEc4I-xtPZqBYoGI,4964
-Broken/Externals/Upscaler/ncnn.py,sha256=Y8dFz-ywLBbG7iGKfd9it_5Pk6P5dbk-1lTj-8ort8c,5221
-Broken/Loaders/LoaderBytes.py,sha256=m_1_ZRLbsrYIdauMNE26TiGd5Lj93V7PsvY49jgb5HY,811
-Broken/Loaders/LoaderPIL.py,sha256=7O26XiKwE2ukS_mP59ciQ4sDIKaNbNJ8D1cl_pBixvk,1910
-Broken/Loaders/LoaderString.py,sha256=HOo9n2n0oB9ARRQsrfrVRBwaPC6fYwG41rLa7X1MsVI,852
-Broken/Loaders/__init__.py,sha256=SOWCiS2vpyNHFvXrD_qjyrtwjvTNQsSyPWIVXvvxZRI,344
+Broken/Externals/FFmpeg/__init__.py,sha256=dqJ3JfGjrQlYKYeqK9urqnMdZyRYg3Go2uUjZBB7oWs,45643
+Broken/Externals/Upscaler/__init__.py,sha256=mC4PForcceM0ToLi4jei8CFWh4Oz8trwTIJyySJ9WJ8,4938
+Broken/Externals/Upscaler/ncnn.py,sha256=jGbE9KrPoDPzxfLQWJGC-LV4M0T-FR-H7MSHnY1v_IY,6351
+Broken/Loaders/LoaderBytes.py,sha256=X-KgsslbPf4DfRZdl3uCIegJjnZ2VaqiFloVO27ZLSk,802
+Broken/Loaders/LoaderImage.py,sha256=RzKG6LHgTEkXHp8s8NJmnoc0xWGYpVArARy0RKWeeTY,1999
+Broken/Loaders/LoaderString.py,sha256=tGvHBrrAHBT8rIWfpoSeOp50Qew_ODFH6xBgVM93wiE,856
+Broken/Loaders/__init__.py,sha256=v8l8a4dNmWISNPTXaTIgrzGtmoFsxSNe5RnlAOhAmZ0,546
 Broken/Resources/Fonts/DejaVu License.txt,sha256=ow8kZqlc0erv9gQWkvQ0ae3MoFLQAuh3AVqBnG4xwZQ,4765
 Broken/Resources/Fonts/DejaVuSans.ttf,sha256=faGVp0xVvvmI0NSPlQi9XYSUJcF3Dbpde_xs6e2EiVQ,757076
 Broken/Resources/Images/Broken.ico,sha256=Geb0VBYO_QIKhbWCqiG58LYo_6mVa1Yq-XjPI8NodL8,8764
 Broken/Resources/Images/Broken.png,sha256=9zBkD7_ZiWnTXXFXLqmIpnS0qfb_5C3dh-3PZ2Kn4uQ,15418
 Broken/Resources/Images/Broken.svg,sha256=dxfZZVKPutJOriOfGtjnaF8mCQkGu8K1oHM1zF-8DDE,1444
-Broken/Staging/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-Broken/Staging/umidi.py,sha256=wWCvakjkukVid6XWGYbmLN-QVdJFFAmuIIKyAC4gDb8,18408
-Broken/Staging/Dotmap/BaseLoader.py,sha256=omvfs7KqJKswYiY-HVFFLF6XlXU2hjDIHQCvubCP43k,1736
-Broken/Staging/Dotmap/BrokenDotmap.py,sha256=PDYmq1qojJMc71Y7Gf8LPlPTN4ZOqIuAW88vd-piDJQ,12082
-Broken/Staging/Dotmap/Readme.md,sha256=vnlwmb2qAeivLvsh3weieTyf4HgGbUoGxmeQgPLGkLc,368
-Broken/Staging/Dotmap/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-Broken/Staging/Dotmap/__test__.py,sha256=Hg-kTzP8AvGt_mCg241Uz5cbOtXnTebuLb7cl594U5Y,3568
-Broken/Staging/Dotmap/Loaders/LoaderPIL.py,sha256=X1U6O2v0sx6Wcqd-vbudWh-h-y2lqCwdCx_a-AoHsJ8,1467
-Broken/Staging/Dotmap/Loaders/LoaderTOML.py,sha256=VvruuBpPEXKgWnkiRlmW6JPxBsb0Ni0fJQ6lyopaOlc,1263
-Broken/Staging/Dotmap/Loaders/__init__.py,sha256=wcJEGoWRpwKIgSR4sEwyrjk-LQ9jIKYXDJ3CZxwDagg,68
-DepthFlow/DepthFlow.py,sha256=6AdySEHDSm3bUmD32GzUuWN2xUTsXTPIZdvoVoQOKcg,9545
-DepthFlow/__init__.py,sha256=9DEp3wDXKhx7FdpSyqnFfaa8L8hQTssrqYBpApGlgZI,356
-DepthFlow/__main__.py,sha256=K0Sg8hwj4oXg79dJfjfC-2gmpRg2ARW9jmazocqH-hs,350
+Broken/Tests/Enum.py,sha256=4QRl4FckF-eUGueY25uH_8vumX_ifyB6_pMhmUV8Qcc,3804
+Broken/Vectron/__init__.py,sha256=9uaHmCgKSry93BVoitAcSEsumiRYizJZ-uejQP4ByrM,76
+DepthFlow/DepthFlow.py,sha256=KN_1Yc6Z07PZY7fgID83bRByQNCFHspqpAr084h9_SM,7851
+DepthFlow/__init__.py,sha256=mj1BTYiVIBMSfoWDRNnwURevgS8FVHFMLbomSw34ekE,324
+DepthFlow/__main__.py,sha256=WaRiKNdBcyVZnTo2lFQVp-GbSoFMatRXt_CCfvpoHCU,317
 DepthFlow/Resources/Images/DepthFlow.png,sha256=oUlRG-luFGw_D4vEEK4YX_fyNlJVoosIp3fYTXRUld8,14623
 DepthFlow/Resources/Images/DepthFlow.svg,sha256=PJ4PG-Bg9guS_kCOrmWrjPAF4R7i9WG26zJIIjT4rmc,1445
-DepthFlow/Resources/Shaders/DepthFlow.frag,sha256=GFI9dBaL5CBgVFCB4v9-OgBxLs9KEwwzqAuviUnl0Kg,2499
+DepthFlow/Resources/Shaders/DepthFlow.frag,sha256=88ViFDfKsOiOi8NPpCUMQyrXgEspqT6anWjAXZw6x9k,2477
 DepthFlow/Resources/Shaders/DepthFlow2D.frag,sha256=2bbH0HQQjkidtB2d2_szqktFMQ_cSsXErzj03RiCOyw,2499
 DepthFlow/Resources/Shaders/DepthFlowMarch.frag,sha256=ynyTiNw9tyUqXijUfg-xtKKsN1Cyia8HEYJEGmohvh4,1688
-Pianola/Pianola.py,sha256=7EkVf8BbguyVjnj9odzfKx3WO9MTThf6cCv-pkhF5Mw,3031
+Pianola/Pianola.py,sha256=m8U8ATscFBVj3ugWHVU0gs-25li9DXWxM8yVLxIe2NA,2999
 Pianola/__init__.py,sha256=TMR-5n6kjD_cR-Wf774y74SFr9bWM9WRyG1qtgJUncU,280
-Pianola/__main__.py,sha256=_hwG3KAM5fG6520XE_QLsXYGs1bcZKnuOuHPYQbhXcw,302
+Pianola/__main__.py,sha256=9V9BhWRoMyz879A1984JDGKR0XcjR2LDnpdnF3hs5X4,297
 Pianola/Resources/Images/Pianola.png,sha256=8gOx3TNtazAUt4tbm0bs5NAf32KzMBBZpZJ-P6Q0SiE,12579
 Pianola/Resources/Images/Pianola.svg,sha256=JRXhOtJMihRQdALQtm1b-i7HLsnwryFHZxKHll1zxOk,3038
 Pianola/Resources/Midis/Hopeless Sparkle.mid,sha256=LIVjUHMXzl_8vKH2cIUbpMsYbxntvY7IdYLosYNiQNQ,27430
 Pianola/Resources/Shaders/Pianola.frag,sha256=9aoTG2z5r21v8jrmIjooF84laqP-jVGmTKM8tGskfwE,8171
 ShaderFlow/Imgui.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ShaderFlow/Message.py,sha256=0RMNw1WBrSaF5wDjl9G_BFaFSxwOA8hszi2zKfcZ7Yk,2574
-ShaderFlow/Module.py,sha256=uNS-Yrop8j_zLabM0mChjPsb66BDfN9_xSBz4q3dr1Y,3321
-ShaderFlow/Notes.py,sha256=UAaxG2FsYyKQBHTmOhlBE2sJTtHDXIPwbjfcxXczzO4,3878
-ShaderFlow/Scene.py,sha256=rBpVzXwYEfYLmLtmavMdyQwpGOQICBvkhhJ0bb7-d9k,36552
-ShaderFlow/Shader.py,sha256=Atv5i6ELtxurUslluVUZ8UHRSoKXm9lhYVwAeThsHOc,11798
-ShaderFlow/Texture.py,sha256=TjvJBRae8rhPyhcm-XnGjmEBCdxTv2mil_pBmkEUFW4,12979
-ShaderFlow/Variable.py,sha256=78H8K1hUKtIfK56u9HiEB6fs3Xr3HS66UR-EjbpC2iA,4219
-ShaderFlow/__init__.py,sha256=pZLBMXybUnLb4mRtaM54uq5pmcsBbmpx9LQRJ1C5oWQ,380
-ShaderFlow/__main__.py,sha256=K1edpNBwznHr1HH7RRcm778RMX56_JGRmGRZpPBvNrw,3562
-ShaderFlow/Modules/Audio.py,sha256=2mtzHxdnyh89ftUR5hguH8abX5WbUeehbUF9UxrDi_s,12171
-ShaderFlow/Modules/Bouncing.py,sha256=LV4H2pty8G69v9YkBayH8Cnb6eJI8PfxQ9eF2QxbiWc,3175
-ShaderFlow/Modules/Camera.py,sha256=BmJ2yI-cIIR-i4qTf8VeM0BGLl_TTUYfBEOiqcW0sMI,17629
-ShaderFlow/Modules/Dynamics.py,sha256=TpOZ19SDa1g4h2GOZGDBQr3Wfn9dOOa24VkRWp-e1qw,9042
+ShaderFlow/Message.py,sha256=_Z2ixBbyo0kqBL22pArnHOaSd7MYzsW_SXBlG6XjmuU,2568
+ShaderFlow/Module.py,sha256=K2KXnya9NF7-aPTln1tlzyvt1ulZiqQ_8ypdtQ5h228,3215
+ShaderFlow/Notes.py,sha256=wFm9qJbQDfnp_HwJo_-ntk9O4WeADCF6b36MTl7tNqQ,3855
+ShaderFlow/Scene.py,sha256=QAxRUR4aurckD78h72Tv2_Cw4KYwsg3Yc2ihx-DA9gw,39206
+ShaderFlow/Shader.py,sha256=1Z8HwRvKZCqmeLa4YhHIE_h0XP-zlj7S7qjU0GBWq3g,13833
+ShaderFlow/Texture.py,sha256=zNtQo9BBVQy-0Ypa1lpHGyMH_4sRyOYyC84qft1t5QU,15278
+ShaderFlow/Variable.py,sha256=Q6JFGMMusiUN6ysF23oRqq0Hl7j_r6XRCBe-mkFjZik,4187
+ShaderFlow/__init__.py,sha256=kAz0EgJUkDTstsNM6ZNhHpg2AJ5suEb_tBQxIlOTTv0,349
+ShaderFlow/__main__.py,sha256=cgYNA2gUJcj4DGEuFNEL8VigpZkvMtyDpjU9fQVYVwk,3269
+ShaderFlow/Modules/Audio.py,sha256=hLQu6x2u7B7kzpWu_nt7aTs3_-Mvc-z9KrTgLkNkOcU,12816
+ShaderFlow/Modules/Bouncing.py,sha256=T57agYc9JzTQaljOo9z3ZBECXxyN5zPJl4C-fT0CE9A,3160
+ShaderFlow/Modules/Camera.py,sha256=BGJHtmZrobjdGh1DNF_e3PjXo3X9XNiAP9BkumZEApk,17597
+ShaderFlow/Modules/Dynamics.py,sha256=RW9kdLkgVIsomjTo85mCd-4XGUtmF_0v2oj5t3pe0Vo,8763
 ShaderFlow/Modules/Frametimer.py,sha256=9fsVLPoV90v6cXeyv5wszxv9v4_lLSUazCMhCPgIv_w,2332
 ShaderFlow/Modules/Keyboard.py,sha256=uSq0WKVcZA3gNklF9vdtnKa1ZQWH92MA533cXSNvoLU,1494
 ShaderFlow/Modules/Noise.py,sha256=MDUHEA4kS-5iUCHaKgdyDXRnRBqplIBSUVNMuGEYlvY,2475
-ShaderFlow/Modules/Piano.py,sha256=rMuzdkxYzlAhSez7bJM3vV5Mt_VugrX4ROiL9l30PPk,14001
-ShaderFlow/Modules/Spectrogram.py,sha256=QZ_lnIkq471wvYHnJMoCHKKAIrAztLwH1IOZY_vIjBw,10943
-ShaderFlow/Modules/Video.py,sha256=bvEisvFEeehzy7QS2kglj4G3mJ1DQpZsQjUReMGjp2c,7218
-ShaderFlow/Modules/Waveform.py,sha256=DxKDXhhh-Sy2yOuPXK8FKq8Bp_IEz3of1yqnjJFTo3U,3137
+ShaderFlow/Modules/Piano.py,sha256=SQP5LiwNwQo2QbLW0c94q-rFdBlcLaU-p4PkzcpF0qA,14040
+ShaderFlow/Modules/Spectrogram.py,sha256=FWWS6kpUdCxGc6zgKOmjAfnamuk0-75aFcoV8tY97fA,10940
+ShaderFlow/Modules/Video.py,sha256=GLupGgbp5AigsD640sx0IBMURFr4FeLmCV4BJ5Vmlck,7203
+ShaderFlow/Modules/Waveform.py,sha256=ND7q53uDX8mILSlnm4wR9f5pCIWv0loCdVCKbinAXPI,3088
 ShaderFlow/Modules/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ShaderFlow/Optional/Monocular.py,sha256=RTV4P44FlDU10WVtOnVQRS30Unf5iv3PGlRb_d3MKX8,3961
+ShaderFlow/Optional/Monocular.py,sha256=Ks8k6DCFxwZLQ1em8wG7aUuOULdVZl4qmr7qX-wmD8E,3503
 ShaderFlow/Optional/OpticalFlow.py,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
 ShaderFlow/Optional/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ShaderFlow/Resources/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ShaderFlow/Resources/Images/ShaderFlow.png,sha256=Z7DL7FqIiwG6o6U3inHe1QmipsRkcmnjXNPxM5-xlWs,20132
 ShaderFlow/Resources/Images/ShaderFlow.svg,sha256=5SlxYmSOAODpXpClTSI2DceG8gbmfKViU1EX2scIbDE,1448
-ShaderFlow/Resources/Scenes/Examples/Demo.py,sha256=XVEBJkzHYzW-fHKTSmrpufGJH_vIObwlQ3wH5eIM7x0,10158
+ShaderFlow/Resources/Scenes/Examples/Demo.py,sha256=SW7NgQ1nyF38pj2lNFO-K0Zoi1F1JiJjE7IXIQjA_eg,10171
 ShaderFlow/Resources/Scenes/Examples/GLSL/Bars.frag,sha256=5clkqgKlg4Hhp4UqAVu2_XrpJz01LWbbcjR83546ylc,495
-ShaderFlow/Resources/Scenes/Examples/GLSL/Bouncing.frag,sha256=L0nfKM5G1N1X24wkZQeF6TDGW948JPS4dgZ8OJjpJqI,1263
+ShaderFlow/Resources/Scenes/Examples/GLSL/Bouncing.frag,sha256=sV7saaaHtHTjkpdAsoOLFseXQfzdTPYvQ0XyjXyBOF0,1285
 ShaderFlow/Resources/Scenes/Examples/GLSL/Multipass.frag,sha256=OxXZ0ILKUPtIbNOaaHsOjHvRNGtqm5Bk7GZ8wRbCKkk,1278
 ShaderFlow/Resources/Scenes/Examples/GLSL/RayMarch.frag,sha256=q42osayKA9xMRHfUkWVJkIiNNT3hLlVdt1tT6B3a4Y8,1380
 ShaderFlow/Resources/Scenes/Examples/GLSL/ShaderToy.frag,sha256=C18Z5sAe5kC-KxDWRZ8sA1KQVf8qU0k-ibCZUkty_8A,2399
 ShaderFlow/Resources/Scenes/Examples/GLSL/Temporal.frag,sha256=8OKokh9ASiEhHQguqTRL6vye3Nx33LwGvc_HQqAQA6k,525
 ShaderFlow/Resources/Scenes/Examples/GLSL/Video.frag,sha256=Lc6iAW8I9qA7C_SB4V4dI1oI9-knVfKN4lzss_TKKoM,115
 ShaderFlow/Resources/Scenes/Examples/GLSL/Visualizer.frag,sha256=Q8OQyKsaaTvDH00VCfOIAgr_XQmB0iijJOVHmjL2S04,1654
 ShaderFlow/Resources/Scenes/Examples/GLSL/Waveform.frag,sha256=uvF0F9D4OKN92SGrU42rhGdnpEOUi5MWgqjx2ODK4SY,341
@@ -90,19 +99,19 @@
 ShaderFlow/Resources/Scenes/Examples/GLSL/Life/Visuals.glsl,sha256=AO4KwxUSPalAOetlgoP2JlkGPSw17RPX2F6otfgKiR0,985
 ShaderFlow/Resources/Shaders/Fragment/Default.glsl,sha256=syBoZdAkdvRF2_3GkEb3iwW-OseAYFzYhBxs-kx_ifo,1618
 ShaderFlow/Resources/Shaders/Fragment/Final.glsl,sha256=nM-L5WSYKRoU1kz1UZBYegGlzPxLoFWeY_eHZW2sQno,79
 ShaderFlow/Resources/Shaders/Fragment/Loading.frag,sha256=gIGMnh611vEJsOpB-DmjBI9EW6_4clkghbZVqB1czDA,895
 ShaderFlow/Resources/Shaders/Fragment/Missing.glsl,sha256=NEiuErlE1z0CE2r6WGS_rn6k7Wd4q9qnCoq7E1wBGfs,574
 ShaderFlow/Resources/Shaders/Include/Camera.glsl,sha256=NOQGK6LidzDO7oUKCnRrssfIECwwAItEaRz-SFmJ66w,5079
 ShaderFlow/Resources/Shaders/Include/Complex.glsl,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ShaderFlow/Resources/Shaders/Include/ShaderFlow.glsl,sha256=a4dPN53khQmV5WbMbI362f2j8mf32iW9YyHtxgAVBOE,10633
+ShaderFlow/Resources/Shaders/Include/ShaderFlow.glsl,sha256=NSWqZ875seP929VOwMxpCn8OUieYxFp0wwOmVKr6LdE,11762
 ShaderFlow/Resources/Shaders/Vertex/Default.glsl,sha256=mptLPRKopeWq7ybJL5kV4xT_yL3hMeUAxe2LsJYX4gA,538
 SpectroNote/SpectroNote.py,sha256=ldoN5iXHaxLpxYt-PE9Aa2NtG2P98WIvm1qQDdfgrr8,1965
-SpectroNote/__init__.py,sha256=eTj2Y_jbZgApkTk-d8z2UM1AnofAMRZPnlbd6nc3z1w,290
-SpectroNote/__main__.py,sha256=gT5JAcy6y0HMfOAlnKJUxx_Va1qsOUQuMYL7yfP6gx0,342
+SpectroNote/__init__.py,sha256=FzjJdWJPcbcDlu8oT4LYJa41Q0TK1RC6qlMdKEvkHXU,282
+SpectroNote/__main__.py,sha256=PlbxnFkEiUIS-h1LjO4Am3rX1wMcCn2ashl_diQ7vgk,337
 SpectroNote/Resources/Images/SpectroNote.png,sha256=Z7DL7FqIiwG6o6U3inHe1QmipsRkcmnjXNPxM5-xlWs,20132
 SpectroNote/Resources/Images/SpectroNote.svg,sha256=5SlxYmSOAODpXpClTSI2DceG8gbmfKViU1EX2scIbDE,1448
 SpectroNote/Resources/Shaders/SpectroNote.frag,sha256=EO1NrbDp8yZGo6X5ZV0g7NKmGMk68jNL3NX4UnmPYjo,3088
-broken_source-0.1.3.dist-info/METADATA,sha256=UarfC0mrWyejE6bIpjY6vVOtJVGmURkaQJHoUXZ_mjE,3026
-broken_source-0.1.3.dist-info/WHEEL,sha256=as-1oFTWSeWBgyzh0O_qF439xqBe6AbBgt4MfYe5zwY,87
-broken_source-0.1.3.dist-info/entry_points.txt,sha256=sliTXdLGMPAHvny75SJgCoSIb556KPPyvqTew_2EI98,194
-broken_source-0.1.3.dist-info/RECORD,,
+broken_source-0.2.0.dist-info/METADATA,sha256=BWPwtjCXMav8Xr9NC6BcMl8F3nRnhbrEk3b-nKyLyjo,3151
+broken_source-0.2.0.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+broken_source-0.2.0.dist-info/entry_points.txt,sha256=sliTXdLGMPAHvny75SJgCoSIb556KPPyvqTew_2EI98,194
+broken_source-0.2.0.dist-info/RECORD,,
```

