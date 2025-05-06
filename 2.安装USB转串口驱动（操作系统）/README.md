Follow this tutorial to configure ESP32 to use your ESPhome.

本篇学习把esp32接入home assistant的全过程，不涉及配置文件的生成和固件的编译。
简单的让浏览器帮我们写入固件（via https://web.esphome.io/）。

# Connect your device to your PC

Plug in your ESP32 board to PC using a USB data cable, ensure your ESP32 board device is properly powered and detected by your computer.

## Key Points

查看是否已安装usb转串口驱动；

usb线是否连接在本机

usb线是否是数据线

esp32是否处于烧录模式

解决与brltty地址冲突问题 （非常高的可能性）

## step 1.安装USB转串口驱动

在做 UART 实验时，一般采用了电脑和ESP32单片机两台设备通信。ESP32单片机上有串口，但现在电脑上一般没有串口，需要外接 usb转串口小板，再拿线将串口小板和单片机串口连起来。但是，Ubuntu 不一定能够看到此串口。


### 安装USB驱动

You’ll need to have CP210x drivers（CP210x USB to UART Bridge VCP Drivers ） installed to flash the firmware.

如果你在电脑上USB正常插入 Arduino 板后，在 Arduino IDE 中看不到该板，那说明你还需要安装开发板的 USB 驱动程序。

目前主流的 Arduino 开发板一般使用以下两种驱动芯片：

cp2102 (原版)

ch340/ch341 (国产替代)



只要电脑上安装好 USB 驱动程序，即使使用了不同的 USB 芯片，这些开发板的用法没什么区别。

注意
为了方便，事实上以上两种驱动都可以装上。

如果你用的是 Linux 系统，特别是较新的 Ubuntu，如 ubuntu 22.04，它一般都是自带这两种驱动的。若在 IDE 中找不到相应的开发板，一般是因为端口被占用所致，进一步阅读后续章节。或者也在网上可以找到解决办法。

# No programming or other software required.

## step 2.Open https://web.esphome.io/

Automatic installation via Browser.Just press the Connect button below with your device connected via usb:

No programming or other software required.

Using this method, you can flash and configure your ESP32 directly from your browser without needing to install additional tools.

https://blog.matterxiaomi.com/blog/esphome-esp32-pir-hc-sr501-part1/


## step 3. project
Automatic installation via Browser.Just press the Connect button below with your device connected via usb:

No programming or other software required.

https://esphome.io/projects/index.html

Voice assistant

Bluetooth proxy

Media Player

ESPresense

https://espresense.com/firmware


## step 4. project