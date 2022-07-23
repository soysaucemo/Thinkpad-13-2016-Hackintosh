# Thinkpad-13-2016-Hackintosh
Thinkpad 13 hackintosh, OpenCore 0.8.0 + MacOS Monterey 12.4.
- same platform as Thinkpad S2 2016 / 据资料显示与Thinkpad S2 2016款硬件基本一致
- OpenCore in this repository is mod version, which forces not to disturb the WINDOWS OS. / 本库中OPENCORE软件是修改版，不对windows系统生效
## Hardware/硬件
- CPU : Intel i7 6500u 
- GPU : Intel HD Graphics 520 [2048MB Share]
- MEM : 8GB 2133MHz DDR4
- HardDisk : SanDisk SD7SN6S-512G 512GB SATA SSD
- LAN : Intel I219-V
- WiFi + Bluetooth : Intel AC 3165
- Audio : Realtek ALC293
- USB : USB 3.0 x 3 + type-C x 1
## Function/功能
- Fn+F1 : Mute
- Fn+F2 : Volume Down
- Fn+F5 : Volume Up
- Fn+F5 : Screen Lightness Down
- Fn+F6 : Screen Lightness Up
## kext/驱动
- Lilu
- VirtualSMC
- IntelBluetoothFirmware : Intel BT drivers
- VoodooInput
- VoodooPS2Controller
- WhateverGreen
- AppleALC : HD Audio Drivers
- HibernationFixup 
- SMCBatteryManager
- SMCLightSensor
- SMCSuperIO
- Airportitlwm : Intel Wifi Drivers 
    * SHOULD load IO80211Family.kext to use original WIFI panel / 需要强制加载IO80211Family以便使用原生wifi管理面板
- CPUFriend : CPU Frequence Fix
- RealtekCardReaderFriend
- ECEnabler : Read Embedded Controller fields over 1 byte
- USBPorts : USB fix
- CpuTscSync : CPU Sync Fix
- BlueToolFixup
- FakeAppleUSBMouse : 
    * You SHOULD Modify it with YOUR OWN MOUSE! / 需要自定义鼠标参数！
## ACPI SSDT
- SSDT-EC-USBX-LAPTOP
- SSDT-LANC
- SSDT-PLUG-DRTNIA
- SSDT-PNLF
- SSDT-XOSI
- SSDT-OCWork-TP
- SSDT-OCBAT0-TP_re80_tx70_x1c5th_s12017_p51
- SSDT-ThinkPad_ClickPad
- SSDT-GPRW
- SSDT-BrightKey
## Known Issues/已知问题
- ClickPad disable Randomly / 触控板随机失效
- Wakeup Randomly /睡眠随机自动唤醒
## Picture/图片
![image](https://user-images.githubusercontent.com/34964159/180008550-e4b2968a-17e3-41a3-88f0-5dad44318e0e.png)
![截屏2022-07-20 22 39 10](https://user-images.githubusercontent.com/34964159/180010623-6acf1e4c-fef6-4a15-bc48-64a40609af0b.png)
![截屏2022-07-20 22 40 38](https://user-images.githubusercontent.com/34964159/180010827-58618811-0a7e-4f2d-a68c-c8785108a664.png)

## Credit/致谢
Thanks to Everyone for providing Kexts/SSDT/Tools.
