<h1 style="text-align: center;width: fit-content;margin: 0 auto;">Pixel ROM 5G</h1>
专注Pixel系列的ROM，基于LineageOS，核心功能包括：5G（针对Pixel在部分国家5G NR功能受限），电话通话录音。<br><br>

<b>❇️主要功能</b><br>
1️⃣5G NR<br>
适配机型：Pixel6<br>
2️⃣电话通话录音<br>
适配机型：Pixel6<br>
3️⃣谷歌三件套，谷歌输入法<br><br>
<b>❇️刷机方法</b><br>
<ul>
<li>手机当前Android版本必须是16，没有请先升级或降级到谷歌官方Android版本16</li>
<li>如果第一次安装我们ROM（LineageOS）,需要先刷入3个img，</li>
<li>fastboot flash boot d:\YourDir\boot.img<br>
fastboot flash dtbo d:\YourDir\dtbo.img<br>
fastboot flash vendor_boot d:\YourDir\vendor_boot.img</li>
<li>其中3个img文件可以通过如下方法获得：payload-dumper-go.exe -o imgs -partitions boot,dtbo,vendor_boot payload.bin</li>
<li><a href="https://github.com/ssut/payload-dumper-go" target="_blank">payload-dumper-go</a> 请自行下载，payload.bin从ROM解压，imgs是payload-dumper的生成目录。</li>
<li>然后 fastboot reboot bootloader ，enter recovery，此时能看到recovery的彩色界面，一定要先进入bootloader再recovery，否则看不到彩色界面，后面sideload会失败。</li>
<li>Apply update<br>
Apply from ADB<br>
adb sideload d:\YourDir\lineage-xx.zip</li>
  </ul>
<b>❇️需求交流</b><br>
Wechat:<br>
<img style="width:150px;height:150px;" src="https://raw.githubusercontent.com/joyou-io/rom/refs/heads/main/wecha2.png"><br>WhatsApp<br><img style="width:150px;height:150px;" src="https://raw.githubusercontent.com/joyou-io/rom/refs/heads/main/whatsapp2.png">
