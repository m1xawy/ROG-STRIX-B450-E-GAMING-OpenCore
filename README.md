分享一份我自己的EFI
主板：华硕ROG B450-E        是  "E"  !!!
CPU:AMD R7 1700
显卡：XFX RX480 4G黑狼版
我看各大论坛都几乎没有我这款主板的EFI文件分享 甚至都没有人用这款主板玩黑果 所以特意将我自己的分享给大家
显卡硬解  支持视频剪辑之类的工作

还有附上Adobe全家桶闪退解决方法（一神提供  我只是个搬运工）：
https://www.kancloud.cn/q952008898/hei_ping_guo/1087365后面还会更新OC文件

2020年02月22日
更新一下OC引导
最近我重新安装了黑苹果系统，发现我之前版本的引导好像无法引导了，故重新制作一份，并分享给大家。


2020年03月18日
更新OpenCore引导  具体更新内容：
1:将OpenCore版本升级到目前最新的正式版  0.5.6
2:修复了NVME协议SSD显示为外置磁盘（橙色磁盘）


推荐一个修复Adobe全家桶的网站
优点是可以用最新版本的Camera RAW 缺点是可能需要手动去删除文件（终端执行命令有时会出错 应该是路径不对导致的 手动删除即可）
https://kb.amd-osx.com/guides/adobe/



更改 关于本机 里错误显示的处理器名称
需要用到的工具 BBEdit  下放链接
https://www.lanzous.com/ia8ejxe
前往文件夹
/System/Library/PrivateFrameworks/AppleSystemInfo.framework/Versions/A/Resources/zh_CN.lproj/Processors.strings
复制一份  Processors.strings  到桌面  然后用BBEdit打开桌面的Processors.strings 找到里面和你的关于本机显示的一样的地方 将其修改为你想要显示的名字 然后将原版Processors.strings替换掉即可



2020年03月21日
1:添加了AMD的传感器kext，有了传感器就得有软件看温度，附上一个吧。https://www.lanzous.com/iahbxzg
2:睡眠问题已经解决，方法是论坛上已有的将所有USB3.0的插口都空出来，设备插USB2.0或USB3.1   这样就能睡眠了，很简单。


2020年03月26日
更新最新AMD内核补丁，可直接升级最新的10.15.4系统版本。
新添加SSDT-PLUG.aml ，开启原生电源管理，建议节能中勾选启用电源小憩，开启小憩可自动进入睡眠，可能会导致睡眠过程会自动唤醒，我已经添加补丁，修复了自动唤醒，睡的很死，一觉到天亮。
目前使用基本无障碍，可以自动睡眠，可以鼠标键盘唤醒，只有Adobe是硬伤，本人常用的Photoshop目前发现不能使用的功能我总结一下给大家：液化、色彩范围、黑白、内容识别填充、自适应广角、差不多就这些。如果有人其他功能不能使用可跟帖回馈，也可以给大家提个醒。


2020年04月15日
更新OpenCore 0.5.7版本，可以正常引导黑苹果和WIN10。
更新所有Kext。


2020年06月10日
更新OpenCore 0.5.9版本，可以正常引导黑苹果和WIN10。
更新所有Kext。
