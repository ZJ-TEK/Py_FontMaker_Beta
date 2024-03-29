# Py_FontMaker
一款嵌入式通用字库生成工具，自动生成通用访问代码，支持LVGL，非LVGL，支持hash查表，二分法查表，支持RLE压缩，支持cmap缓存，支持外部bin和内部.c生成，支持多语言，多字号多字体，支持图标字库和emoji混合消息展示。

关注公众号：Bluetooth-BLE，QQ群：177341833

验证代码：https://gitee.com/woowill/ZJ_RT_Thread_LVGL_Font_Nordic.git

验证板子：https://item.taobao.com/item.htm?id=694863934116

Py_FontMaker验证下载工具：https://item.taobao.com/item.htm?id=624639720338

## Py_FontMaker介绍
- help信息

  ![Py_FontMaker -h](/image/pictures/Py_FontMaker.jpg) 

- 工具生成的代码

  ![Py_FontMaker -h](/image/pictures/工具生成的demo代码.jpg) 

- 工具多语言excle转换的代码

  ![多语言代码](/image/pictures/多语言excle转换的代码.jpg) 

- 命令描述

|命令	|描述	|使用者	|默认|
| ------------------------ | ------------------------ | ------------------------ | ------------------------ |
|-h, |显示此帮助消息并退出| ||
|--XBF |功能项-> ttf 生成 XBF| |False|
|--LIB |功能项-> xbf生成font_lib| |False|
|--INNER| 功能项-> 产生内部字库| |False|
|--ICON |功能项-> 产生图标字库| |False|
|--EMOJI| 功能项-> 产生emoji字库| |False|
|--LANG| 功能项-> 将多语言Excel表转为.c和.h| |False|
|--min |参数-> unicode最小值 |XBF使用 |0x00|
|--max |参数-> unicode最大值 |XBF使用 |0xffff|
|--ttf |参数-> 字体文件路径	|XBF,LIB(fake)和INNER |.\font_xbf\TTF_file\HarmonyOS_Sans_SC_Medium.ttf|
|--bpp |参数-> 灰度位 |XBF,LIB(fake)和INNER	|2|
|--height |参数-> 字符像素高度 |XBF,LIB(fake)和INNER|24|
|--lib_file |参数-> 生成Font_Lib时的字库类型文件 |LIB使用 |.\font_type\all_font_type_to_generate.txt|
|--fake_file |参数-> 生成Fake font字符的txt文件 |LIB(fake) |.\font_type\FAKE_FONT_CODE_POINT.txt|
|--inner_file |参数-> 生成内部字库字符的txt文件 |INNER使用 |.\font_type\INTERIOR_FONT_CODE_POINT.txt|
|--icon_file |参数-> 生成图标字库字符的txt文件 |ICON 使用 |.\font_type\ICON_FONT_CODE_POINT.txt|
|--emoji_file |参数-> 生成emoji字库字符的txt文件 |EMOJI使用 |.\font_type\EMOJI_FONT_CODE_POINT.txt|
|--emoimgpath |参数-> 生成emoji的图片资源路径 |EMOJI使用|.\UI_resource\emoji\32|
|--lvgl	|参数-> 支持LVGL的字库 |LIB使用	|True|
|--hash	|参数-> cmap支持hash查找 |LIB使用| True|
|--rle	|参数-> 支持Run Length Encode压缩 |LIB使用|	True|
|--cache| 参数-> 字库支持字符描述缓存 |LIB使用 |True|

## GUI_Py_FontMaker介绍
命令行用着不不习惯，那就搞个界面，本来是搞成web应用的，发现自己能力不够，算了，就单机版吧！界面如下：
- 输出路径选择

  ![输出路径选择](/image/pictures/GUI1.jpg) 

- 生成XBF

  ![生成XBF](/image/pictures/GUI2.jpg) 


- 生成LIB和代码

  ![生成LIB和代码](/image/pictures/GUI3.jpg) 


- 生成INNER代码

  ![生成INNER代码](/image/pictures/GUI4.jpg) 


- 生成EMOJI

  ![生成EMOJI](/image/pictures/GUI5.jpg) 


- 生成ICON

  ![生成ICON](/image/pictures/GUI6.jpg) 

- 多语言Excel表转为.c和.h

  ![多语言Excel表转为.c和.h](/image/pictures/GUI7.jpg) 

## JLink下载SPI Flash
- JLink SPI接口定义

  ![JLink SPI接口定义](/image/pictures/Jtag的SPI接口.jpg) 

- JLink下载spiflash接线

  ![JLink SPI接口定义](/image/pictures/spi下载接线.png) 

- JLink下载spiflash接线

  ![JLink SPI接口定义](/image/pictures/jlink下载spiflash接线.jpg) 

## 字库显示效果  
- LVGL显示效果

  ![LVGL显示效果](/image/pictures/LVGL显示效果.jpg) 
  
- 裸机显示效果

  ![裸机显示效果](/image/pictures/非LVGL显示效果.jpg)

## 公众号:Bluetooth-BLE  
  ![公众号:Bluetooth-BLE](/image/QR/公众号.jpg  "公众号:Bluetooth-BLE") 
## QQ群:177341833  
  ![QQ群:177341833](/image/QR/qq群.jpg  "QQ群:177341833") 
