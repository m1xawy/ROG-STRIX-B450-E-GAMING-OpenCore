<h2><div><b>我的机器信息</b><div></h2>
<p>主板：华硕ROG B450-E 是"E"!</p>
<p>CPU:AMD R7 1700</p>
<p>显卡：XFX RX480 4G黑狼版</p><br>
<p>我看各大论坛都几乎没有我这款主板的EFI文件分享 甚至都没有人用这款主板玩黑果 所以特意将我自己的分享给大家</p>
<p>目前系统版本为MacOS10.15.5</p>
<p>显卡硬解 支持视频剪辑之类的工作  声卡、网卡正常运行（AMD通病：麦克风无法使用，我自己的解决方案为：外置音响播放声音，USB耳机拾取声音）</p>
<p>更新OpenCore 0.5.9版本，可以正常引导黑苹果和WIN10。</p>
<p>更新所有Kext。</p>
<p>目前除随航以外的功能几乎都是正常使用的。</p>
<h2>推荐一个修复Adobe全家桶的网站</h2>
<p>优点是可以用最新版本的Camera RAW 缺点是可能需要手动去删除文件（终端执行命令有时会出错 应该是路径不对导致的 手动删除即可）</p>
<p>https://kb.amd-osx.com/guides/adobe/</p>
<p>下面的链接会帮助你将Photoshop修复至几乎没有问题（修复AMD平台的Photoshop的液化等一部分功能）</p>
<p>http://bbs.pcbeta.com/viewthread-1858910-1-1.html</p>
<h2>更改 关于本机 里错误显示的处理器名称</h2>
<p>需要用到的工具 BBEdit  下放下载链接</b>
<p>https://www.lanzous.com/ia8ejxe</b>
<p>前往文件夹</p>
<p>/System/Library/PrivateFrameworks/AppleSystemInfo.framework/Versions/A/Resources/zh_CN.lproj/Processors.strings</b>
<p>复制一份  Processors.strings  到桌面  然后用BBEdit打开桌面的Processors.strings 找到里面和你的关于本机显示的一样的地方 将其修改为你想要显示的名字 然后将原版Processors.strings替换掉即可</b>
