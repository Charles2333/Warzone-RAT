# Warzone-RAT
# **Warzone RAT远控木马样本分析**

## RAT信息

Warzone RAT又名AveMaria RAT，是一款纯C/C++开发的商业木马程序，该程序自2018年开始便在网络上以软件订阅的方式公开售卖，适配目前Windows 10以下系统，具备远程桌面、密码窃取、键盘记录、远程命令、权限提升、下载执行等多种远程控制功能。自售卖以来便被多个APT组织使用，已知的便有魔罗桫(Confucius)、蔓灵花(Bitter)、盲眼鹰(APT-Q-98)等组织使用过该商业木马。

```
该恶意软件具有以下功能：
不需要.NET
可通过VNC使用远程桌面
可通过RDPWrap获得隐藏的远程桌面
提权（包括最新的Win10）
远程WebCam控件
密码采集（Chrome，Firefox，IE，Edge，Outlook，Thunderbird，Foxmail）
下载并执行任何文件
实时键盘记录器
Remote Shell
文件管理器
进程管理
反向代理
```

## 技术细节

该软件是一种用C ++编写并与所有Windows版本兼容的RAT。恶意软件开发人员在此之上提供了DNS服务，购买者不受IP地址更改的影响。该软件还可绕过UAC（用户帐户控制）与Windows Defender，并写入启动程序列表中，处理C＆C命令。 它有几种不同的版本，同时在不断改进， 某些描述可能会因版本变化而不同。
