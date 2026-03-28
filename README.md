主要提供Pixel，Xiaomi，Oneplus等品牌部分机型的ROM，基于LineageOS，添加功能包括：5G（针对Pixel手机在部分国家不能开启5G NR），电话通话录音，微信/WhatsApp/Messager等语音通话自动播放音频文件。
功能开发及机型适配有序进行中，以下是进度：<br><br>
📳ROM（Android 16）<br>
1️⃣5G NR<br>
适配机型：Pixel6<br>
2️⃣电话通话录音<br>
适配机型：TODO<br>
3️⃣语音通话自动播放音频文件<br>
适配机型：TODO<br><br>
✅刷机方法
👉手机当前Android版本必须是16，没有请先升级或降级到谷歌官方Android版本16<br>
👉如果第一次安装我们ROM（LineageOS）,需要先刷入3个img，<br>
👉fastboot flash boot d:\YourDir\boot.img<br>
fastboot flash dtbo d:\YourDir\dtbo.img<br>
fastboot flash vendor_boot d:\YourDir\vendor_boot.img<br>
👉其中3个img文件可以通过如下方法获得：payload-dumper-go.exe -o imgs payload.bin<br>
<a href="https://github.com/ssut/payload-dumper-go" target="_blank">payload-dumper-go</a> 请自行下载，payload.bin从ROM解压，imgs是payload-dumper的生成目录。<br>
👉然后 fastboot reboot bootloader ，enter recovery，此时能看到recovery的彩色界面，一定要先进入bootloader再recovery，否则看不到彩色界面，后面sideload会失败。<br>
👉Apply update<br>
👉Apply from ADB<br>
👉adb sideload d:\YourDir\lineage-xx.zip<br><br>
❇️需求交流：<br>





