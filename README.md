
# Hackintosh-EFI-for-FUJITSU-S762

## Hello！！ <img src="https://raw.githubusercontent.com/MartinHeinz/MartinHeinz/master/wave.gif" width="30px">这是我使用的富士通笔记本S762黑苹果引导文件，包含了 Clover 引导。直接下载zip文件即可，本引导适用于BigSur 11.1 20C69 ，原则上支持10.15以及10.14系统，已经测试没有问题。
****
# 电脑配置
CPU: Intel Core i5-3340M  
GPU: Intel HD Graphics 4000  
声卡: Realtek ALC269（layout-id = 6）  
网卡: 无线网卡（已更换为 Broadcom BCM94360hmb，需要屏蔽阵脚，51有教程）+ 有线intel 82579V
****
# Clover 配置说明
Clover 版本 为 5128，支持安装和引导 macOS Big Sur 11.2 Beta开发版。
序列号已经洗白，但已经被使用过。请参照教程自行洗白。机型建议不用修改。
亮度调节可以使用FN+快捷键控制，音量可以使用FN+F8/F9来控制。
键盘可以在安装的时候直接设置为ANSI美版键盘，避免使用日版键盘导致符号和输出对不上，建议购买一张标准键盘膜，打字一目了然。
****
# 关于 外接显示器DP接口 转HDMI数字音频输出
使用 AppleALC.kext + FakePCIID.kext + FakePCIID_Intel_HDMI_Audio.kext ，layoutid=6即可完美输出，如果显示器不带音箱功能，可以用外接音箱直接连接笔记本3.5mm耳机输出接口，完美切换。如果显示器带3.5mm音频输出接口，则可以直接用外接音箱线插入显示器输出接口即可使用，唯一的缺点是显示器无法通过软件或者其他调整音量，默认是最大的音量。
****
# 已知问题（待解决）
触摸板无法驱动手势，系统偏好设置触摸板无法显示，但是触摸板可以使用简单的单击、滑动等类似于鼠标的功能。
****
其他功能比如蓝牙，电量显示，睡眠，睡眠唤醒（需要按开机键），隔空播放，隔空投送，接力，随航（需要改机型）等完美。
