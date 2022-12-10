# Py_FontMaker_Beta
这个版本是测试版本，外部字库只支持2个字号文件，正式版本请关注公众号：Bluetooth-BLE，QQ群：177341833

fake字库只支持2bpp和24像素，内部字库也只支持2bpp和24像素

验证代码：https://github.com/ZJ-TEK/ZJ_RT_Thread_LVGL_Font
## Py_FontMaker介绍
- help信息

  ![Py_FontMaker -h](/image/pictures/Py_FontMaker.jpg) 

- 工具生成的代码

  ![Py_FontMaker -h](/image/pictures/工具生成的demo代码.jpg) 

- 命令描述

|命令	|描述	|使用者	|默认|
| ------------------------ | ------------------------ | ------------------------ | ------------------------ |
|-h,	|显示此帮助消息并退出|||		
|--XBF	|功能项-> ttf 生成 XBF|		|False|
|--LIB	|功能项-> xbf生成font_lib|		|False|
|--CODE |	功能项-> 产生内部字库|		|False|
|--min	|参数-> unicode最小值	|XBF使用	|0x00|
|--max 	|参数-> unicode最大值	|XBF使用	|0xffff|
|--ttf 	|参数-> 字体文件路径	|XBF,LIB(fake字库使用)和CODE	|.\font_xbf\TTF_file\HarmonyOS_Sans_SC_Medium.ttf|
|--bpp	|参数-> 灰度位	|XBF,LIB(fake字库使用)和CODE	|2|
|--height 	|参数-> 字符像素高度	|XBF,LIB(fake字库使用)和CODE	|24|
|--lib_file	|参数-> 生成Font_Lib时的字库类型文件	|LIB使用	|.\font_type\all_font_type_to_generate.txt|
|--fake_file	|参数-> 生成Fake font字符的txt文件	|LIB(fake字库使用)	|.\font_type\FAKE_FONT_CODE_POINT.txt|
|--inte_file	|参数-> 生成内部字库字符的txt文件	|CODE使用	|.\font_type\INTERIOR_FONT_CODE_POINT.txt|
|--lvgl	|参数-> 支持LVGL的字库	|LIB使用	|True|
|--hash	|参数-> cmap支持hash查找	|LIB使用	|True|
|--rle	|参数-> 支持Run Length Encode压缩	|LIB使用	|True|
|--cache	|参数-> 字库支持字符描述缓存	|LIB使用	|True|

## 字库显示效果
- LVGL显示效果

  ![LVGL显示效果](/image/pictures/LVGL显示效果.jpg) 
  
- 裸机显示效果

  ![裸机显示效果](/image/pictures/非LVGL显示效果.jpg)

### 公众号:Bluetooth-BLE  
  ![公众号:Bluetooth-BLE](/image/QR/公众号.jpg  "公众号:Bluetooth-BLE") 
### QQ群:177341833  
  ![QQ群:177341833](/image/QR/qq群.jpg  "QQ群:177341833") 
