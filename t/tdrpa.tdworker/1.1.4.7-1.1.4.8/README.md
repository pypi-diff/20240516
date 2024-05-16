# Comparing `tmp/tdrpa.tdworker-1.1.4.7-py3-none-any.whl.zip` & `tmp/tdrpa.tdworker-1.1.4.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 422508 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat  1181696 b- defN 24-May-14 21:46 tdrpa/tdworker.cp38-win_amd64.pyd
--rw-rw-rw-  2.0 fat       57 b- defN 24-May-14 21:32 tdrpa/tdworker/__init__.pyi
--rw-rw-rw-  2.0 fat    16314 b- defN 24-May-14 21:32 tdrpa/tdworker/winElement.pyi
--rw-rw-rw-  2.0 fat     5063 b- defN 24-May-14 21:33 tdrpa/tdworker/winKeyboard.pyi
--rw-rw-rw-  2.0 fat     7386 b- defN 24-May-14 21:33 tdrpa/tdworker/winMouse.pyi
--rw-rw-rw-  2.0 fat     3655 b- defN 24-May-14 21:32 tdrpa/tdworker/window.pyi
--rw-rw-rw-  2.0 fat      663 b- defN 24-May-14 21:47 tdrpa.tdworker-1.1.4.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 21:47 tdrpa.tdworker-1.1.4.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-May-14 21:47 tdrpa.tdworker-1.1.4.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      847 b- defN 24-May-14 21:47 tdrpa.tdworker-1.1.4.7.dist-info/RECORD
-10 files, 1215779 bytes uncompressed, 421056 bytes compressed:  65.4%
+Zip file size: 430899 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat  1213952 b- defN 24-May-16 02:27 tdrpa/tdworker.cp38-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      167 b- defN 24-May-16 02:23 tdrpa/tdworker/__init__.pyi
+-rw-rw-rw-  2.0 fat     4254 b- defN 24-May-16 02:23 tdrpa/tdworker/_w.pyi
+-rw-rw-rw-  2.0 fat    17361 b- defN 24-May-16 02:23 tdrpa/tdworker/_winE.pyi
+-rw-rw-rw-  2.0 fat     5395 b- defN 24-May-16 02:23 tdrpa/tdworker/_winK.pyi
+-rw-rw-rw-  2.0 fat     7908 b- defN 24-May-16 02:23 tdrpa/tdworker/_winM.pyi
+-rw-rw-rw-  2.0 fat      663 b- defN 24-May-16 02:27 tdrpa.tdworker-1.1.4.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-16 02:27 tdrpa.tdworker-1.1.4.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-May-16 02:27 tdrpa.tdworker-1.1.4.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      830 b- defN 24-May-16 02:27 tdrpa.tdworker-1.1.4.8.dist-info/RECORD
+10 files, 1250628 bytes uncompressed, 429483 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -1,31 +1,31 @@
 Filename: tdrpa/tdworker.cp38-win_amd64.pyd
 Comment: 
 
 Filename: tdrpa/tdworker/__init__.pyi
 Comment: 
 
-Filename: tdrpa/tdworker/winElement.pyi
+Filename: tdrpa/tdworker/_w.pyi
 Comment: 
 
-Filename: tdrpa/tdworker/winKeyboard.pyi
+Filename: tdrpa/tdworker/_winE.pyi
 Comment: 
 
-Filename: tdrpa/tdworker/winMouse.pyi
+Filename: tdrpa/tdworker/_winK.pyi
 Comment: 
 
-Filename: tdrpa/tdworker/window.pyi
+Filename: tdrpa/tdworker/_winM.pyi
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.7.dist-info/METADATA
+Filename: tdrpa.tdworker-1.1.4.8.dist-info/METADATA
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.7.dist-info/WHEEL
+Filename: tdrpa.tdworker-1.1.4.8.dist-info/WHEEL
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.7.dist-info/top_level.txt
+Filename: tdrpa.tdworker-1.1.4.8.dist-info/top_level.txt
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.7.dist-info/RECORD
+Filename: tdrpa.tdworker-1.1.4.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tdrpa/tdworker/__init__.pyi

```diff
@@ -1 +1,4 @@
-from . import winElement, winKeyboard, winMouse, window
+from ._w import Window as Window
+from ._winE import WinElement as WinElement
+from ._winK import WinKeyboard as WinKeyboard
+from ._winM import WinMouse as WinMouse
```

## Comparing `tdrpa/tdworker/winElement.pyi` & `tdrpa/tdworker/_winE.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,213 +1,228 @@
 import uiautomation as uia
 
-def findElement(tdTargetStr: str = None, anchorsElement: uia.Control = None, searchDelay: int = 10000, continueOnError: bool = False) -> uia.Control | None:
-    """
-    获取元素
-
-    winElement.findElement('', anchorsElement=None, searchDelay=10000, continueOnError=False)
-
-    :param tdTargetStr: 目标元素特征码(tdrpa拾取器获取)
-    :param anchorsElement: 从哪个元素开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）
-    :param searchDelay: 查找延时（豪秒）。默认10000
-    :param continueOnError: 错误继续执行。默认False
-    :return: 目标元素 or None
-    """
-def getChildren(target: str | uia.Control, searchType: str = 'all', searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> list | uia.Control:
-    '''
-    获取子元素
-
-    winElement.getChildren(target, searchType=\'all\', searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象(指定被获取子元素的根节点元素)
-    :param searchType: [可选参数]搜索方式。全部子元素:"all" 首个子元素:"first" 最后一个子元素:"last"。默认"all"
-    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
-    :param continueOnError: [可选参数]错误继续执行。默认False
-    :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
-    :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
-    :return: 目标元素对象的子元素列表 或 首个子元素 或 最后一个子元素
-    '''
-def getParent(target: str | uia.Control, searchDelay: int = 10000, anchorsElement: uia.Control = None, searchTop: bool = False, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> uia.Control:
-    """
-    获取父元素
-
-    winElement.getParent(target, searchDelay=10000, anchorsElement=None, searchTop=False, continueOnError=False, delayAfter=100, delayBefore=100)
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
-    :param searchTop: [可选参数]是否搜索顶级父元素。搜索临近一层的父元素:False 搜索顶级的父元素:True。默认False
-    :param continueOnError: [可选参数]错误继续执行。默认False
-    :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
-    :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
-    :return: 目标元素对象的上一层父级元素 或 顶层父级元素
-    """
-def getSibling(target: str | uia.Control, position: str = 'next', searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> uia.Control | None:
-    '''
-    获取相邻元素
-
-    winElement.getSibling(target, position="next", searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param position: [可选参数]相邻位置。下一个："next"  上一个："previous"。默认"next"
-    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
-    :param continueOnError: [可选参数]错误继续执行。默认False
-    :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
-    :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
-    :return: 目标元素对象的下一个相邻元素对象 或 上一个相邻元素对象，没有返回None
-    '''
-def exists(target: str | uia.Control, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> bool:
-    """
-    判断元素是否存在
-
-    winElement.exists(target, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
-    :param continueOnError: [可选参数]错误继续执行。默认False
-    :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
-    :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
-    :return: bool
-    """
-def getCheck(target: str | uia.Control, searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> bool:
-    """
-    获取元素勾选
-
-    winElement.getCheck(target, searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
-    :param continueOnError: [可选参数]错误继续执行。默认False
-    :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
-    :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
-    :return: bool
-    """
-def setCheck(target: str | uia.Control, searchDelay: int = 10000, isCheck: bool = True, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> None:
-    """
-    设置元素勾选
-
-    winElement.setCheck(target, searchDelay=10000, isCheck=True, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
-    :param isCheck: [可选参数]设置勾选:True 设置取消勾选:False。默认True
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
-    :param continueOnError: [可选参数]错误继续执行。默认False
-    :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
-    :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
-    :return: None
-    """
-def getSelect(target: str | uia.Control, searchDelay: int = 10000, mode: str = 'text', anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> str | int:
-    '''
-    获取元素选择
-
-    winElement.getSelect(target, searchDelay=10000, mode=\'text\', anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
-    :param mode: [可选参数]获取文本："text" 获取序号：“index” 获取值：“value”。默认"text"
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
-    :param continueOnError: [可选参数]错误继续执行。默认False
-    :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
-    :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
-    :return: 已选项的文本 或 序号 或 值，没有则返回None
-    '''
-def setSelect(target: str | uia.Control, option: str | int, searchDelay: int = 10000, mode: str = 'text', anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100, setForeground: bool = True, cursorPosition: str = 'center', cursorOffsetX: int = 0, cursorOffsetY: int = 0, simulateType: str = 'simulate') -> None:
-    '''
-    设置元素选择
-
-    winElement.setSelect(target, \'\', searchDelay=10000, mode="text", anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100, setForeground=True, cursorPosition=\'center\', cursorOffsetX=0, cursorOffsetY=0, simulateType=\'simulate\')
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param option: [必选参数]选择选项
-    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
-    :param mode: [可选参数]选择文本："text" 选择序号：“index” 选择值：“value”。默认"text"
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
-    :param continueOnError: [可选参数]错误继续执行。默认False
-    :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
-    :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
-    :param setForeground: [可选参数]激活窗口。默认True
-    :param cursorPosition: [可选参数]光标位置。中心:"center" 左上角:"topLeft" 右上角:"topRight" 左下角:"bottomLeft" 右下角:"bottomRight"。默认"center"
-    :param cursorOffsetX: [可选参数]横坐标偏移。默认0
-    :param cursorOffsetY: [可选参数]纵坐标偏移。默认0
-    :param simulateType: [可选参数]鼠标点击选中项时的模式。模拟操作:"simulate" 消息操作:"message"。默认"simulate"
-    :return: None
-    '''
-def getValue(target: str | uia.Control, getMethod: str = 'auto', searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> str:
-    '''
-    获取元素文本
-
-    winElement.getValue(target, getMethod="auto", searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param getMethod: [可选参数]获取方式。自动方式："auto" 搜元素Name方式："name" 搜元素Value方式："value"。默认"auto"
-    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
-    :param continueOnError: [可选参数]错误继续执行。默认False
-    :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
-    :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
-    :return: 元素文本
-    '''
-def setValue(target: str | uia.Control, value: str, searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> None:
-    '''
-    设置元素文本
-
-    winElement.setValue(target, "", searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param value: [必选参数]待写入UI界面元素的文本内容
-    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
-    :param continueOnError: [可选参数]错误继续执行。默认False
-    :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
-    :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
-    :return: None
-    '''
-def getRect(target: str | uia.Control, relativeType: str = 'parent', searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> dict:
-    '''
-    获取元素区域
-
-    winElement.getRect(target, relativeType="parent", searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param relativeType: [可选参数]返回元素位置是相对于哪一个坐标而言的。 相对父元素:"parent" 相对窗口客户区:"root" 相对屏幕坐标:"screen"。默认"parent"
-    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
-    :param continueOnError: [可选参数]错误继续执行。默认False
-    :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
-    :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
-    :return: {"height" : int, "width" : int, "x" : int, "y" : int}
-    '''
-def screenCapture(target: str | uia.Control, filePath: str, rect: dict = None, searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> bool:
-    '''
-    元素截图
-
-    winElement.screenCapture(target, \'D:/1.png\', rect=None, searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param filePath: [必选参数]图片存储的绝对路径。如 \'D:/1.png\'(支持图片保存格式：bmp、jpg、jpeg、png、gif、tif、tiff)
-    :param rect: [可选参数]对指定界面元素截图的范围，若传None，则截取该元素的全区域。若传{"x":int,"y":int,"width":int,"height":int}，则以该元素左上角位置偏移x,y的坐标为原点，根据高宽进行截图。默认None
-    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
-    :param continueOnError: [可选参数]错误继续执行。默认False
-    :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
-    :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
-    :return: bool(截图成功返回True，否则返回假)
-    '''
-def wait(target: str | uia.Control, waitType: str = 'show', searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> None:
-    '''
-    等待元素（等待元素显示或消失）
-
-    winElement.wait(target, waitType=\'show\', searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param waitType: [可选参数]等待方式。 等待显示："show" 等待消失:"hide"。默认"show"
-    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
-    :param continueOnError: [可选参数]错误继续执行。默认False
-    :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
-    :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
-    :return: None
-    '''
+class WinElement:
+    @staticmethod
+    def findElementByTd(tdTargetStr: str = None, anchorsElement: uia.Control = None, searchDelay: int = 10000, continueOnError: bool = False):
+        """
+        依据tdrpa拾取器获取的元素特征码查找元素
+
+        WinElement.findElementByTd('', anchorsElement=None, searchDelay=10000, continueOnError=False)
+
+        :param tdTargetStr: 目标元素特征码(tdrpa拾取器获取)
+        :param anchorsElement: 从哪个元素开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）
+        :param searchDelay: 查找延时（豪秒）。默认10000
+        :param continueOnError: 错误继续执行。默认False
+        :return: 目标元素 or None
+        """
+    @staticmethod
+    def getChildren(target: str | uia.Control, searchType: str = 'all', searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> list | uia.Control:
+        '''
+        获取子元素
+
+        WinElement.getChildren(target, searchType=\'all\', searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象(指定被获取子元素的根节点元素)
+        :param searchType: [可选参数]搜索方式。全部子元素:"all" 首个子元素:"first" 最后一个子元素:"last"。默认"all"
+        :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+        :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
+        :param continueOnError: [可选参数]错误继续执行。默认False
+        :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
+        :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
+        :return: 目标元素对象的子元素列表 或 首个子元素 或 最后一个子元素
+        '''
+    @staticmethod
+    def getParent(target: str | uia.Control, searchDelay: int = 10000, anchorsElement: uia.Control = None, searchTop: bool = False, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> uia.Control:
+        """
+        获取父元素
+
+        WinElement.getParent(target, searchDelay=10000, anchorsElement=None, searchTop=False, continueOnError=False, delayAfter=100, delayBefore=100)
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
+        :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+        :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
+        :param searchTop: [可选参数]是否搜索顶级父元素。搜索临近一层的父元素:False 搜索顶级的父元素:True。默认False
+        :param continueOnError: [可选参数]错误继续执行。默认False
+        :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
+        :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
+        :return: 目标元素对象的上一层父级元素 或 顶层父级元素
+        """
+    @staticmethod
+    def getSibling(target: str | uia.Control, position: str = 'next', searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> uia.Control | None:
+        '''
+        获取相邻元素
+
+        WinElement.getSibling(target, position="next", searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
+        :param position: [可选参数]相邻位置。下一个："next"  上一个："previous"。默认"next"
+        :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+        :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
+        :param continueOnError: [可选参数]错误继续执行。默认False
+        :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
+        :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
+        :return: 目标元素对象的下一个相邻元素对象 或 上一个相邻元素对象，没有返回None
+        '''
+    @staticmethod
+    def exists(target: str | uia.Control, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> bool:
+        """
+        判断元素是否存在
+
+        WinElement.exists(target, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
+        :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
+        :param continueOnError: [可选参数]错误继续执行。默认False
+        :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
+        :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
+        :return: bool
+        """
+    @staticmethod
+    def getCheck(target: str | uia.Control, searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> bool:
+        """
+        获取元素勾选
+
+        WinElement.getCheck(target, searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
+        :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+        :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
+        :param continueOnError: [可选参数]错误继续执行。默认False
+        :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
+        :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
+        :return: bool
+        """
+    @staticmethod
+    def setCheck(target: str | uia.Control, searchDelay: int = 10000, isCheck: bool = True, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> None:
+        """
+        设置元素勾选
+
+        WinElement.setCheck(target, searchDelay=10000, isCheck=True, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
+        :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+        :param isCheck: [可选参数]设置勾选:True 设置取消勾选:False。默认True
+        :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
+        :param continueOnError: [可选参数]错误继续执行。默认False
+        :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
+        :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
+        :return: None
+        """
+    @staticmethod
+    def getSelect(target: str | uia.Control, searchDelay: int = 10000, mode: str = 'text', anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> str | int:
+        '''
+        获取元素选择
+
+        WinElement.getSelect(target, searchDelay=10000, mode=\'text\', anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
+        :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+        :param mode: [可选参数]获取文本："text" 获取序号：“index” 获取值：“value”。默认"text"
+        :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
+        :param continueOnError: [可选参数]错误继续执行。默认False
+        :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
+        :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
+        :return: 已选项的文本 或 序号 或 值，没有则返回None
+        '''
+    @staticmethod
+    def setSelect(target: str | uia.Control, option: str | int, searchDelay: int = 10000, mode: str = 'text', anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100, setForeground: bool = True, cursorPosition: str = 'center', cursorOffsetX: int = 0, cursorOffsetY: int = 0, simulateType: str = 'simulate') -> None:
+        '''
+        设置元素选择
+
+        WinElement.setSelect(target, \'\', searchDelay=10000, mode="text", anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100, setForeground=True, cursorPosition=\'center\', cursorOffsetX=0, cursorOffsetY=0, simulateType=\'simulate\')
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
+        :param option: [必选参数]选择选项
+        :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+        :param mode: [可选参数]选择文本："text" 选择序号：“index” 选择值：“value”。默认"text"
+        :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
+        :param continueOnError: [可选参数]错误继续执行。默认False
+        :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
+        :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
+        :param setForeground: [可选参数]激活窗口。默认True
+        :param cursorPosition: [可选参数]光标位置。中心:"center" 左上角:"topLeft" 右上角:"topRight" 左下角:"bottomLeft" 右下角:"bottomRight"。默认"center"
+        :param cursorOffsetX: [可选参数]横坐标偏移。默认0
+        :param cursorOffsetY: [可选参数]纵坐标偏移。默认0
+        :param simulateType: [可选参数]鼠标点击选中项时的模式。模拟操作:"simulate" 消息操作:"message"。默认"simulate"
+        :return: None
+        '''
+    @staticmethod
+    def getValue(target: str | uia.Control, getMethod: str = 'auto', searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> str:
+        '''
+        获取元素文本
+
+        WinElement.getValue(target, getMethod="auto", searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
+        :param getMethod: [可选参数]获取方式。自动方式："auto" 搜元素Name方式："name" 搜元素Value方式："value"。默认"auto"
+        :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+        :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
+        :param continueOnError: [可选参数]错误继续执行。默认False
+        :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
+        :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
+        :return: 元素文本
+        '''
+    @staticmethod
+    def setValue(target: str | uia.Control, value: str, searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> None:
+        '''
+        设置元素文本
+
+        WinElement.setValue(target, "", searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
+        :param value: [必选参数]待写入UI界面元素的文本内容
+        :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+        :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
+        :param continueOnError: [可选参数]错误继续执行。默认False
+        :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
+        :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
+        :return: None
+        '''
+    @staticmethod
+    def getRect(target: str | uia.Control, relativeType: str = 'parent', searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> dict:
+        '''
+        获取元素区域
+
+        WinElement.getRect(target, relativeType="parent", searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
+        :param relativeType: [可选参数]返回元素位置是相对于哪一个坐标而言的。 相对父元素:"parent" 相对窗口客户区:"root" 相对屏幕坐标:"screen"。默认"parent"
+        :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+        :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
+        :param continueOnError: [可选参数]错误继续执行。默认False
+        :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
+        :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
+        :return: {"height" : int, "width" : int, "x" : int, "y" : int}
+        '''
+    @staticmethod
+    def screenCapture(target: str | uia.Control, filePath: str, rect: dict = None, searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> bool:
+        '''
+        元素截图
+
+        WinElement.screenCapture(target, \'D:/1.png\', rect=None, searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
+        :param filePath: [必选参数]图片存储的绝对路径。如 \'D:/1.png\'(支持图片保存格式：bmp、jpg、jpeg、png、gif、tif、tiff)
+        :param rect: [可选参数]对指定界面元素截图的范围，若传None，则截取该元素的全区域。若传{"x":int,"y":int,"width":int,"height":int}，则以该元素左上角位置偏移x,y的坐标为原点，根据高宽进行截图。默认None
+        :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+        :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
+        :param continueOnError: [可选参数]错误继续执行。默认False
+        :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
+        :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
+        :return: bool(截图成功返回True，否则返回假)
+        '''
+    @staticmethod
+    def wait(target: str | uia.Control, waitType: str = 'show', searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> None:
+        '''
+        等待元素（等待元素显示或消失）
+
+        WinElement.wait(target, waitType=\'show\', searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100)
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
+        :param waitType: [可选参数]等待方式。 等待显示："show" 等待消失:"hide"。默认"show"
+        :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+        :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
+        :param continueOnError: [可选参数]错误继续执行。默认False
+        :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
+        :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
+        :return: None
+        '''
```

## Comparing `tdrpa/tdworker/winKeyboard.pyi` & `tdrpa/tdworker/_winK.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,69 +1,74 @@
 import uiautomation as uia
 
-def inputText(target: str | uia.Control, content: str, clearOldText: bool = True, inputInterval: int = 10, searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100, setForeground: bool = True, simulateType: str = 'message', validate: bool = False, clickBeforeInput: bool = False) -> uia.Control:
-    '''
-    在目标中输入
-
-    winKeyboard.inputText(target, \'\', clearOldText=True, inputInterval=10, searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100, setForeground=True, simulateType=\'message\', validate=False, clickBeforeInput=False)
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param content: [必选参数]写入文本
-    :param clearOldText: [可选参数]是否清空原内容。默认True
-    :param inputInterval: [可选参数]键入间隔(毫秒)。默认10
-    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
-    :param continueOnError: [可选参数]错误继续执行。默认False
-    :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
-    :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
-    :param setForeground: [可选参数]激活窗口。默认True
-    :param simulateType: [可选参数]操作类型。模拟操作:"simulate" 消息操作:"message"。默认"message"
-    :param validate: [可选参数]验证写入文本。默认False
-    :param clickBeforeInput: [可选参数]输入前点击。默认False
-    :return: 目标元素对象
-    '''
-def pressKey(target: str | uia.Control, button: str, searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100, setForeground: bool = True, keyModifiers: list = None, simulateType: str = 'message', clickBeforeInput: bool = False) -> uia.Control:
-    '''
-    在目标中按键
-
-    winKeyboard.pressKey(target, "Enter", searchDelay=10000, continueOnError=False, delayAfter=100, delayBefore=100, setForeground=True, keyModifiers=None, simulateType=\'message\', clickBeforeInput=False)
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param button: [必选参数]键盘按键上的符号。如"Enter"
-    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
-    :param continueOnError: [可选参数]错误继续执行。默认False
-    :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
-    :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
-    :param setForeground: [可选参数]激活窗口。默认True
-    :param keyModifiers: [可选参数]辅助按键 "Alt","Ctrl","Shift","Win",可多选。默认None
-    :param simulateType: [可选参数]操作类型。模拟操作:"simulate" 消息操作:"message"。默认"message"
-    :param clickBeforeInput: [可选参数]输入前点击。默认False
-    :return: 目标元素对象
-    '''
-def inputAct(content: str, inputInterval: int = 10, delayAfter: int = 100, delayBefore: int = 100, simulateType: str = 'message') -> None:
-    '''
-    输入文本
-
-    winKeyboard.inputAct(\'\', inputInterval=10, delayAfter=100, delayBefore=100, simulateType=\'message\')
-
-    :param content: [必选参数]输入内容
-    :param inputInterval: [可选参数]键入间隔(毫秒)。默认10
-    :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
-    :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
-    :param simulateType: [可选参数]操作类型。模拟操作:"simulate" 消息操作:"message"。默认"message"
-    :return: None
-    '''
-def pressAct(button: str, pressType: str = 'press', keyModifiers: list = None, delayAfter: int = 100, delayBefore: int = 100, simulateType: str = 'message') -> None:
-    '''
-    模拟按键
-
-    winKeyboard.pressAct(\'Enter\', pressType=\'press\', keyModifiers=None, delayAfter=100, delayBefore=100, simulateType=\'message\')
-
-    :param button: [必选参数]键盘按键上的符号，如“Enter”
-    :param pressType: [可选参数]点击类型。单击:"press" 按下:"down" 弹起:"up"。默认"press"
-    :param keyModifiers: [可选参数]辅助按键["Alt","Ctrl","Shift","Win"]可多选。默认None
-    :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
-    :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
-    :param simulateType: [可选参数]操作类型。模拟操作:"simulate" 消息操作:"message"。默认"message"
-    :return: None
-    '''
+class WinKeyboard:
+    @staticmethod
+    def inputText(target: str | uia.Control, content: str, clearOldText: bool = True, inputInterval: int = 10, searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100, setForeground: bool = True, simulateType: str = 'message', validate: bool = False, clickBeforeInput: bool = False) -> uia.Control:
+        '''
+        在目标中输入
+
+        WinKeyboard.inputText(target, \'\', clearOldText=True, inputInterval=10, searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100, setForeground=True, simulateType=\'message\', validate=False, clickBeforeInput=False)
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
+        :param content: [必选参数]写入文本
+        :param clearOldText: [可选参数]是否清空原内容。默认True
+        :param inputInterval: [可选参数]键入间隔(毫秒)。默认10
+        :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+        :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
+        :param continueOnError: [可选参数]错误继续执行。默认False
+        :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
+        :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
+        :param setForeground: [可选参数]激活窗口。默认True
+        :param simulateType: [可选参数]操作类型。模拟操作:"simulate" 消息操作:"message"。默认"message"
+        :param validate: [可选参数]验证写入文本。默认False
+        :param clickBeforeInput: [可选参数]输入前点击。默认False
+        :return: 目标元素对象
+        '''
+    @staticmethod
+    def pressKey(target: str | uia.Control, button: str, searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100, setForeground: bool = True, keyModifiers: list = None, simulateType: str = 'message', clickBeforeInput: bool = False) -> uia.Control:
+        '''
+        在目标中按键
+
+        WinKeyboard.pressKey(target, "Enter", searchDelay=10000, continueOnError=False, delayAfter=100, delayBefore=100, setForeground=True, keyModifiers=None, simulateType=\'message\', clickBeforeInput=False)
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
+        :param button: [必选参数]键盘按键上的符号。如"Enter"
+        :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+        :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
+        :param continueOnError: [可选参数]错误继续执行。默认False
+        :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
+        :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
+        :param setForeground: [可选参数]激活窗口。默认True
+        :param keyModifiers: [可选参数]辅助按键 "Alt","Ctrl","Shift","Win",可多选。默认None
+        :param simulateType: [可选参数]操作类型。模拟操作:"simulate" 消息操作:"message"。默认"message"
+        :param clickBeforeInput: [可选参数]输入前点击。默认False
+        :return: 目标元素对象
+        '''
+    @staticmethod
+    def inputAct(content: str, inputInterval: int = 10, delayAfter: int = 100, delayBefore: int = 100, simulateType: str = 'message') -> None:
+        '''
+        输入文本
+
+        WinKeyboard.inputAct(\'\', inputInterval=10, delayAfter=100, delayBefore=100, simulateType=\'message\')
+
+        :param content: [必选参数]输入内容
+        :param inputInterval: [可选参数]键入间隔(毫秒)。默认10
+        :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
+        :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
+        :param simulateType: [可选参数]操作类型。模拟操作:"simulate" 消息操作:"message"。默认"message"
+        :return: None
+        '''
+    @staticmethod
+    def pressAct(button: str, pressType: str = 'press', keyModifiers: list = None, delayAfter: int = 100, delayBefore: int = 100, simulateType: str = 'message') -> None:
+        '''
+        模拟按键
+
+        WinKeyboard.pressAct(\'Enter\', pressType=\'press\', keyModifiers=None, delayAfter=100, delayBefore=100, simulateType=\'message\')
+
+        :param button: [必选参数]键盘按键上的符号，如“Enter”
+        :param pressType: [可选参数]点击类型。单击:"press" 按下:"down" 弹起:"up"。默认"press"
+        :param keyModifiers: [可选参数]辅助按键["Alt","Ctrl","Shift","Win"]可多选。默认None
+        :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
+        :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
+        :param simulateType: [可选参数]操作类型。模拟操作:"simulate" 消息操作:"message"。默认"message"
+        :return: None
+        '''
```

## Comparing `tdrpa/tdworker/winMouse.pyi` & `tdrpa/tdworker/_winM.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,109 +1,117 @@
 import uiautomation as uia
 
-def action(target: str | uia.Control, button: str = 'left', clickType: str = 'click', searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100, setForeground: bool = True, cursorPosition: str = 'center', cursorOffsetX: int = 0, cursorOffsetY: int = 0, keyModifiers: list = None, simulateType: str = 'simulate', moveSmoothly: bool = False) -> uia.Control:
-    '''
-    点击目标元素
-
-    winMouse.action(target, button="left", clickType="click", searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100, setForeground=True, cursorPosition=\'center\', cursorOffsetX=0, cursorOffsetY=0, keyModifiers=None, simulateType=\'simulate\', moveSmoothly=False)
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param button: [可选参数]鼠标点击。鼠标左键:"left" 鼠标右键:"right" 鼠标中键:"middle"。默认"left"
-    :param clickType: [可选参数]点击类型。单击:"click" 双击:"dbclick" 按下:"down" 弹起:"up"。默认"click"
-    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
-    :param continueOnError: [可选参数]错误继续执行。默认False
-    :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
-    :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
-    :param setForeground: [可选参数]激活窗口。默认True
-    :param cursorPosition: [可选参数]光标位置。中心:"center" 左上角:"topLeft" 右上角:"topRight" 左下角:"bottomLeft" 右下角:"bottomRight"。默认"center"
-    :param cursorOffsetX: [可选参数]横坐标偏移。默认0
-    :param cursorOffsetY: [可选参数]纵坐标偏移。默认0
-    :param keyModifiers: [可选参数]辅助按键["Alt","Ctrl","Shift","Win"]可多选。默认None
-    :param simulateType: [可选参数]操作类型。模拟操作:"simulate" 消息操作:"message"。默认"simulate"
-    :param moveSmoothly: [可选参数]平滑移动。默认False
-    :return:目标元素对象
-    '''
-def hover(target: str | uia.Control, searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100, setForeground: bool = True, cursorPosition: str = 'center', cursorOffsetX: int = 0, cursorOffsetY: int = 0, keyModifiers: list = None, simulateType: str = 'simulate', moveSmoothly: bool = True) -> uia.Control:
-    '''
-    移动到目标上
-
-    winMouse.hover(target, searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100, setForeground=True, cursorPosition=\'center\', cursorOffsetX=0, cursorOffsetY=0, keyModifiers=None, simulateType=\'simulate\', moveSmoothly=False)
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
-    :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
-    :param continueOnError: [可选参数]错误继续执行。默认False
-    :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
-    :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
-    :param setForeground: [可选参数]激活窗口。默认True
-    :param cursorPosition: [可选参数]光标位置。中心:"center" 左上角:"topLeft" 右上角:"topRight" 左下角:"bottomLeft" 右下角:"bottomRight"。默认"center"
-    :param cursorOffsetX: [可选参数]横坐标偏移。默认0
-    :param cursorOffsetY: [可选参数]纵坐标偏移。默认0
-    :param keyModifiers: [可选参数]辅助按键["Alt","Ctrl","Shift","Win"]可多选。默认None
-    :param simulateType: [可选参数]操作类型。模拟操作:"simulate" 消息操作:"message"。默认"simulate"
-    :param moveSmoothly: [可选参数]平滑移动。默认True
-    :return:目标元素对象
-    '''
-def click(button: str = 'left', clickType: str = 'click', keyModifiers: list = None, delayAfter: int = 100, delayBefore: int = 100) -> None:
-    '''
-    模拟点击
-
-    winMouse.click(button="left", clickType="click", keyModifiers=None, delayAfter=100, delayBefore=100)
-
-    :param button: [可选参数]鼠标点击。鼠标左键:"left" 鼠标右键:"right" 鼠标中键:"middle"。默认"left"
-    :param clickType: [可选参数]点击类型。单击:"click" 双击:"dbclick" 按下:"down" 弹起:"up"。默认"click"
-    :param keyModifiers: [可选参数]辅助按键["Alt","Ctrl","Shift","Win"]可多选。默认None
-    :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
-    :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
-    :return: None
-    '''
-def move(x: int, y: int, isRelativeMove: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> None:
-    """
-    # 模拟移动
-
-    winMouse.move(0, 0, isRelativeMove=False, delayAfter=100, delayBefore=100)
-
-    :param x: [必选参数]横坐标
-    :param y: [必选参数]纵坐标
-    :param isRelativeMove: [可选参数]是否相对目前位置移动。默认False
-    :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
-    :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
-    :return: None
-    """
-def getPos() -> tuple[int, int]:
-    """
-    获取鼠标位置
-
-    winMouse.getPos()
-
-    :return:pointX, pointY
-    """
-def drag(x1: int, y1: int, x2: int, y2: int, button: str = 'left', keyModifiers: list = None, delayAfter: int = 100, delayBefore: int = 100) -> None:
-    '''
-    模拟拖动
-
-    winMouse.drag(0, 0, 0, 0, button=\'left\', keyModifiers=None, delayAfter=100, delayBefore=100)
-
-    :param x1: [必选参数]起始横坐标
-    :param y1: [必选参数]起始纵坐标
-    :param x2: [必选参数]结束横坐标
-    :param y2: [必选参数]结束纵坐标
-    :param button: [可选参数]鼠标按键。鼠标左键:"left" 鼠标右键:"right" 鼠标中键:"middle"。默认"left"
-    :param keyModifiers: [可选参数]辅助按键["Alt","Ctrl","Shift","Win"]可多选。默认None
-    :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
-    :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
-    :return: None
-    '''
-def wheel(scrollNum: int, scrollDirection: str = 'down', keyModifiers: list = None, delayAfter: int = 100, delayBefore: int = 100) -> None:
-    '''
-    模拟滚轮
-
-    winMouse.wheel(1, scrollDirection="down", keyModifiers=None, delayAfter=100, delayBefore=100)
-
-    :param scrollNum: [必选参数]滚动次数
-    :param scrollDirection: [可选参数]滚动方向。向上:"up" 向下:"down"。默认"down"
-    :param keyModifiers: [可选参数]辅助按键["Alt","Ctrl","Shift","Win"]可多选。默认None
-    :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
-    :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
-    :return: None
-    '''
+class WinMouse:
+    @staticmethod
+    def action(target: str | uia.Control, button: str = 'left', clickType: str = 'click', searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100, setForeground: bool = True, cursorPosition: str = 'center', cursorOffsetX: int = 0, cursorOffsetY: int = 0, keyModifiers: list = None, simulateType: str = 'simulate', moveSmoothly: bool = False) -> uia.Control:
+        '''
+        点击目标元素
+
+        WinMouse.action(target, button="left", clickType="click", searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100, setForeground=True, cursorPosition=\'center\', cursorOffsetX=0, cursorOffsetY=0, keyModifiers=None, simulateType=\'simulate\', moveSmoothly=False)
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
+        :param button: [可选参数]鼠标点击。鼠标左键:"left" 鼠标右键:"right" 鼠标中键:"middle"。默认"left"
+        :param clickType: [可选参数]点击类型。单击:"click" 双击:"dbclick" 按下:"down" 弹起:"up"。默认"click"
+        :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+        :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
+        :param continueOnError: [可选参数]错误继续执行。默认False
+        :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
+        :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
+        :param setForeground: [可选参数]激活窗口。默认True
+        :param cursorPosition: [可选参数]光标位置。中心:"center" 左上角:"topLeft" 右上角:"topRight" 左下角:"bottomLeft" 右下角:"bottomRight"。默认"center"
+        :param cursorOffsetX: [可选参数]横坐标偏移。默认0
+        :param cursorOffsetY: [可选参数]纵坐标偏移。默认0
+        :param keyModifiers: [可选参数]辅助按键["Alt","Ctrl","Shift","Win"]可多选。默认None
+        :param simulateType: [可选参数]操作类型。模拟操作:"simulate" 消息操作:"message"。默认"simulate"
+        :param moveSmoothly: [可选参数]平滑移动。默认False
+        :return:目标元素对象
+        '''
+    @staticmethod
+    def hover(target: str | uia.Control, searchDelay: int = 10000, anchorsElement: uia.Control = None, continueOnError: bool = False, delayAfter: int = 100, delayBefore: int = 100, setForeground: bool = True, cursorPosition: str = 'center', cursorOffsetX: int = 0, cursorOffsetY: int = 0, keyModifiers: list = None, simulateType: str = 'simulate', moveSmoothly: bool = True) -> uia.Control:
+        '''
+        移动到目标上
+
+        WinMouse.hover(target, searchDelay=10000, anchorsElement=None, continueOnError=False, delayAfter=100, delayBefore=100, setForeground=True, cursorPosition=\'center\', cursorOffsetX=0, cursorOffsetY=0, keyModifiers=None, simulateType=\'simulate\', moveSmoothly=False)
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
+        :param searchDelay: [可选参数]超时时间(毫秒)。默认10000
+        :param anchorsElement: [可选参数]锚点元素，从它开始找，不传则从桌面顶级元素开始找（有值可提高查找速度）。默认None
+        :param continueOnError: [可选参数]错误继续执行。默认False
+        :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
+        :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
+        :param setForeground: [可选参数]激活窗口。默认True
+        :param cursorPosition: [可选参数]光标位置。中心:"center" 左上角:"topLeft" 右上角:"topRight" 左下角:"bottomLeft" 右下角:"bottomRight"。默认"center"
+        :param cursorOffsetX: [可选参数]横坐标偏移。默认0
+        :param cursorOffsetY: [可选参数]纵坐标偏移。默认0
+        :param keyModifiers: [可选参数]辅助按键["Alt","Ctrl","Shift","Win"]可多选。默认None
+        :param simulateType: [可选参数]操作类型。模拟操作:"simulate" 消息操作:"message"。默认"simulate"
+        :param moveSmoothly: [可选参数]平滑移动。默认True
+        :return:目标元素对象
+        '''
+    @staticmethod
+    def click(button: str = 'left', clickType: str = 'click', keyModifiers: list = None, delayAfter: int = 100, delayBefore: int = 100) -> None:
+        '''
+        模拟点击
+
+        WinMouse.click(button="left", clickType="click", keyModifiers=None, delayAfter=100, delayBefore=100)
+
+        :param button: [可选参数]鼠标点击。鼠标左键:"left" 鼠标右键:"right" 鼠标中键:"middle"。默认"left"
+        :param clickType: [可选参数]点击类型。单击:"click" 双击:"dbclick" 按下:"down" 弹起:"up"。默认"click"
+        :param keyModifiers: [可选参数]辅助按键["Alt","Ctrl","Shift","Win"]可多选。默认None
+        :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
+        :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
+        :return: None
+        '''
+    @staticmethod
+    def move(x: int, y: int, isRelativeMove: bool = False, delayAfter: int = 100, delayBefore: int = 100) -> None:
+        """
+        # 模拟移动
+
+        WinMouse.move(0, 0, isRelativeMove=False, delayAfter=100, delayBefore=100)
+
+        :param x: [必选参数]横坐标
+        :param y: [必选参数]纵坐标
+        :param isRelativeMove: [可选参数]是否相对目前位置移动。默认False
+        :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
+        :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
+        :return: None
+        """
+    @staticmethod
+    def getPos() -> tuple[int, int]:
+        """
+        获取鼠标位置
+
+        WinMouse.getPos()
+
+        :return:pointX, pointY
+        """
+    @staticmethod
+    def drag(x1: int, y1: int, x2: int, y2: int, button: str = 'left', keyModifiers: list = None, delayAfter: int = 100, delayBefore: int = 100) -> None:
+        '''
+        模拟拖动
+
+        WinMouse.drag(0, 0, 0, 0, button=\'left\', keyModifiers=None, delayAfter=100, delayBefore=100)
+
+        :param x1: [必选参数]起始横坐标
+        :param y1: [必选参数]起始纵坐标
+        :param x2: [必选参数]结束横坐标
+        :param y2: [必选参数]结束纵坐标
+        :param button: [可选参数]鼠标按键。鼠标左键:"left" 鼠标右键:"right" 鼠标中键:"middle"。默认"left"
+        :param keyModifiers: [可选参数]辅助按键["Alt","Ctrl","Shift","Win"]可多选。默认None
+        :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
+        :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
+        :return: None
+        '''
+    @staticmethod
+    def wheel(scrollNum: int, scrollDirection: str = 'down', keyModifiers: list = None, delayAfter: int = 100, delayBefore: int = 100) -> None:
+        '''
+        模拟滚轮
+
+        WinMouse.wheel(1, scrollDirection="down", keyModifiers=None, delayAfter=100, delayBefore=100)
+
+        :param scrollNum: [必选参数]滚动次数
+        :param scrollDirection: [可选参数]滚动方向。向上:"up" 向下:"down"。默认"down"
+        :param keyModifiers: [可选参数]辅助按键["Alt","Ctrl","Shift","Win"]可多选。默认None
+        :param delayAfter: [可选参数]执行后延时(毫秒)。默认100
+        :param delayBefore: [可选参数]执行前延时(毫秒)。默认100
+        :return: None
+        '''
```

## Comparing `tdrpa/tdworker/window.pyi` & `tdrpa/tdworker/_w.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,115 +1,128 @@
 import uiautomation as uia
 
-def close(target: str | uia.Control) -> None:
-    """
-    关闭窗口
-
-    window.close(target)
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象(指定被获取子元素的根节点元素)
-    :return: None
-    """
-def getActive() -> uia.Control:
-    """
-    获取活动窗口
-
-    window.getActive()
-
-    :return:control
-    """
-def setActive(target: str | uia.Control) -> bool:
-    """
-    设置活动窗口
-
-    window.setActive(target)
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :return: bool。激活成功返回True，否则返回False
-    """
-def show(target: str | uia.Control, showStatus: str) -> bool:
-    '''
-    更改窗口显示状态
-
-    window.show(target, "show")
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param showStatus: [必选参数] 显示：\'show\' 隐藏：\'hide\' 最大化：\'max\' 最小化：\'min\' 还原：\'restore\'
-    :return: bool。执行成功返回True，否则返回False
-    '''
-def exists(target: str | uia.Control) -> bool:
-    """
-    判断窗口是否存在
-
-    window.exists(target)
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :return: bool。窗口存在返回True,否则返回False
-    """
-def getSize(target: str | uia.Control) -> dict:
-    '''
-    获取窗口大小
-
-    window.getSize(target)
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :return: {"height":int, "width":int, "x":int, "y":int}
-    '''
-def setSize(target: str | uia.Control, width: int, height: int) -> None:
-    """
-    改变窗口大小
-
-    window.setSize(target, 800, 600)
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param width: [必选参数]窗口宽度
-    :param height: [必选参数]窗口高度
-    :return: None
-    """
-def move(target: str | uia.Control, x: int, y: int) -> None:
-    """
-    移动窗口位置
-
-    window.move(target, 0, 0)
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param x: [必选参数]移动到新位置的横坐标
-    :param y: [必选参数]移动到新位置的纵坐标
-    :return: None
-    """
-def topMost(target: str | uia.Control, isTopMost: bool = True) -> None:
-    """
-    窗口置顶
-
-    window.topMost(target, isTopMost=True)
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :param isTopMost: [可选参数]是否使窗口置顶，窗口置顶:true 窗口取消置顶:false。默认True
-    :return: None
-    """
-def getClass(target: str | uia.Control) -> str:
-    """
-    获取窗口类名
-
-    window.getClass(target)
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :return: 窗口的类名称
-    """
-def getPath(target: str | uia.Control) -> str:
-    """
-    获取窗口程序的文件路径
-
-    window.getPath(target)
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :return: 文件绝对路径
-    """
-def getPID(target: str | uia.Control) -> int:
-    """
-    获取进程PID
-
-    window.getPID(target)
-
-    :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
-    :return: PID
-    """
+class Window:
+    @staticmethod
+    def close(target: str | uia.Control) -> None:
+        """
+        关闭窗口
+
+        window.close(target)
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象(指定被获取子元素的根节点元素)
+        :return: None
+        """
+    @staticmethod
+    def getActive() -> uia.Control:
+        """
+        获取活动窗口
+
+        window.getActive()
+
+        :return:control
+        """
+    @staticmethod
+    def setActive(target: str | uia.Control) -> bool:
+        """
+        设置活动窗口
+
+        window.setActive(target)
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
+        :return: bool。激活成功返回True，否则返回False
+        """
+    @staticmethod
+    def show(target: str | uia.Control, showStatus: str) -> bool:
+        '''
+        更改窗口显示状态
+
+        window.show(target, "show")
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
+        :param showStatus: [必选参数] 显示：\'show\' 隐藏：\'hide\' 最大化：\'max\' 最小化：\'min\' 还原：\'restore\'
+        :return: bool。执行成功返回True，否则返回False
+        '''
+    @staticmethod
+    def exists(target: str | uia.Control) -> bool:
+        """
+        判断窗口是否存在
+
+        window.exists(target)
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
+        :return: bool。窗口存在返回True,否则返回False
+        """
+    @staticmethod
+    def getSize(target: str | uia.Control) -> dict:
+        '''
+        获取窗口大小
+
+        window.getSize(target)
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
+        :return: {"height":int, "width":int, "x":int, "y":int}
+        '''
+    @staticmethod
+    def setSize(target: str | uia.Control, width: int, height: int) -> None:
+        """
+        改变窗口大小
+
+        window.setSize(target, 800, 600)
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
+        :param width: [必选参数]窗口宽度
+        :param height: [必选参数]窗口高度
+        :return: None
+        """
+    @staticmethod
+    def move(target: str | uia.Control, x: int, y: int) -> None:
+        """
+        移动窗口位置
+
+        window.move(target, 0, 0)
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
+        :param x: [必选参数]移动到新位置的横坐标
+        :param y: [必选参数]移动到新位置的纵坐标
+        :return: None
+        """
+    @staticmethod
+    def topMost(target: str | uia.Control, isTopMost: bool = True) -> None:
+        """
+        窗口置顶
+
+        window.topMost(target, isTopMost=True)
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
+        :param isTopMost: [可选参数]是否使窗口置顶，窗口置顶:true 窗口取消置顶:false。默认True
+        :return: None
+        """
+    @staticmethod
+    def getClass(target: str | uia.Control) -> str:
+        """
+        获取窗口类名
+
+        window.getClass(target)
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
+        :return: 窗口的类名称
+        """
+    @staticmethod
+    def getPath(target: str | uia.Control) -> str:
+        """
+        获取窗口程序的文件路径
+
+        window.getPath(target)
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
+        :return: 文件绝对路径
+        """
+    @staticmethod
+    def getPID(target: str | uia.Control) -> int:
+        """
+        获取进程PID
+
+        window.getPID(target)
+
+        :param target: [必选参数]拾取器获取的目标元素特征字符串或目标元素对象
+        :return: PID
+        """
```

## Comparing `tdrpa.tdworker-1.1.4.7.dist-info/METADATA` & `tdrpa.tdworker-1.1.4.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdrpa.tdworker
-Version: 1.1.4.7
+Version: 1.1.4.8
 Summary: tdworker for tdrpa developers. supports python3.8+, windows x64
 Home-page: https://tdrpa.thingswell.cn
 Author: vx:RPA_CREATOR
 Author-email: oldplayerliu@gmail.com
 License: Apache 2.0
 Keywords: RPA,tdRPA,tdworker,rpaworker,worker,uiautomation,uia,creator,windows,python,bot,robot,aigc,ai
 Platform: Windows Only
```

