# Misaka-PCB



## BOM智能配单

https://bom.szlcsc.com/bom.html



为了BOM配单方便，尽可能使用JLC-SMT库

[嘉立创](https://www.sz-jlc.com/)把 SMT支持的器件做成了要一个集成库

下载方法:   [嘉立创SMT](https://gitee.com/JLC_SMT) **/** [JLCSMT_LIB](https://gitee.com/JLC_SMT/JLCSMT_LIB)

导入Project Outputs for Miscellaneous Devices LC中的Miscellaneous Devices LC.IntLib



## USB 2.0 to USB Type-C

[**How to easily move from USB 2.0 to USB Type-C**](http://e2e.ti.com/blogs_/b/analogwire/archive/2015/09/02/how-to-easily-move-from-usb-2-0-to-usb-type-c)

[Oh Say Can You C? – Grappling with the USB type-C Connector](https://resources.orcad.com/orcad-blog/oh-say-can-you-c-grappling-with-the-usb-type-c-connector)

[Type-A接口改成Type-c接口的实验设计](http://www.elecfans.com/emb/jiekou/20190505929062.html)



## PCB Design Rules

SMD Pads Clearance -- 0.2 mil

TH Pads Clearance -- 0.15 mil



## 元件选型说明

原Mega 2560中 LMV358IDGKR 立创商城需订货，改为LM358DR2G通用运放

原Mega 2560中 MH2029-300Y 磁珠 ，改为 BLM21PG300SN1D 0805 30 欧 @ 100MHz

MF-MSMF050 0.5A 15V 自恢复保险丝 立创商城需订货，改为 https://item.szlcsc.com/13192.html （相同封装）

俩RESET不要选元件

CG0603MLC-05E  ESD 抑制器/TVS 二极管，立创商城无货，改为[**0603ESDA-05N**](https://item.szlcsc.com/297742.html)



## PCB注意事项

和DTR 隔着100nF的Reset要连着和+5V隔着10kOhm的焊盘，以便SMT跳线能起作用。

X为水平左右翻转；Y为垂直上下翻转