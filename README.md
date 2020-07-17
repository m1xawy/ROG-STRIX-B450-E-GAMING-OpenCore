<b>我的机器信息<b>
<p>主板：华硕ROG B450-E           是  "E"  !!!
<p>CPU:AMD R7 1700
<p>显卡：XFX RX480 4G黑狼版
<p>我看各大论坛都几乎没有我这款主板的EFI文件分享 甚至都没有人用这款主板玩黑果 所以特意将我自己的分享给大家
显卡硬解  支持视频剪辑之类的工作
<p>更新OpenCore 0.5.9版本，可以正常引导黑苹果和WIN10。
<p>更新所有Kext。
<p>目前除随航以外的功能几乎都是正常使用的。

<b>推荐一个修复Adobe全家桶的网站<b>
<p>优点是可以用最新版本的Camera RAW 缺点是可能需要手动去删除文件（终端执行命令有时会出错 应该是路径不对导致的 手动删除即可）

https://kb.amd-osx.com/guides/adobe/

下面的链接会帮助你将Photoshop修复至几乎没有问题（修复AMD平台的Photoshop的液化等一部分功能）

http://bbs.pcbeta.com/viewthread-1858910-1-1.html



<b>更改 关于本机 里错误显示的处理器名称<b>
  

需要用到的工具 BBEdit  下放下载链接

https://www.lanzous.com/ia8ejxe

前往文件夹

/System/Library/PrivateFrameworks/AppleSystemInfo.framework/Versions/A/Resources/zh_CN.lproj/Processors.strings

复制一份  Processors.strings  到桌面  然后用BBEdit打开桌面的Processors.strings 找到里面和你的关于本机显示的一样的地方 将其修改为你想要显示的名字 然后将原版Processors.strings替换掉即可
