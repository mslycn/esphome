Integrate your own sensors using ESPHome.These steps will prepare your computer to deploy the sensor board and integrate into Home-Asssistant.

ESPHome is a system to control your ESP8266/ESP32 by simple yet powerful configuration files and control them remotely through Home Automation systems. It allows to define your sensor-board in terms of a yaml file and will generate and upload code to the ESP8266/ESP32 board.


## Project Information

local:F:\developer_Xiaomi\EspHome

remote:https://github.com/mslycn/esphome

通过XESP32S3  通过 ESPHome 与 Home Assistant 连接，

我们可以让ESP32作为主心骨，接下来就是学习其他外设有机衔接从而完成功能，进而丰富我们的生活

## ESPHome - Hardware
~~~
 ESP32
 ESP32 IDF
 ESP8266
 RP2040
 BK72xx
 RTL87xx

~~~




Esp32

Esp32 Expansion board

PCB打板


TOF10120激光测距模块

## Esp32 bluetooth proxy

Esp32 ESPHome Bluetooth Proxy ->Bluetooth integration ->xiaomi BLE integration

This is because an ESPHome Bluetooth Proxy is forwarding its data to the official Bluetooth integration in Home Assistant. The Bluetooth integration is forwarding the data to a brand specific integration(for example xiaomi BLE integration).

source:https://custom-components.github.io/ble_monitor/parse_data#extend-bluetooth-range-with-esphome-ble-gateway

## Passive BLE Monitor integration

Esp32 ESPHome BLE Gateway -> Passive BLE Monitor integration

Passive BLE Monitor integration is using its own Bluetooth collecting mechanism based on aioblescan which is working at a lower level (HCI). BLE monitor is not using the Bluetooth integration to receive its data, and is therefore not able to receive data from ESPHome Bluetooth Proxies. You can use ESPHome BLE Gateway instead, which is forwarding the data to to Passive BLE Monitor integration.


step 1.Configure the integration

To add a device, add the following to your configuration.yaml

detail:https://custom-components.github.io/ble_monitor/configuration_params#configuration-in-yaml

配置使用哪个蓝牙适配器
1.build-in adater
2.usb adapter
3.eps32 ble gateway



#### step 3.Extend Bluetooth range with ESPHome BLE Gateway

https://custom-components.github.io/ble_monitor/parse_data#extend-bluetooth-range-with-esphome-ble-gateway



## Private BLE Device integration

可以直接跟踪iPhone等各种蓝牙设备，离家回家检测更简单

## basic

https://blog.matterxiaomi.com/blog/esphome-esp32-pir-hc-sr501-part1/

https://blog.matterxiaomi.com/blog/esphome-esp32-pir-hc-sr501-part2/

## git

Git Bash

cd f:
cd F:/developer_Xiaomi/EspHome

$ git init

$ git config user.email "****@mail.com"


$ git config user.name "mslycn"


$ git add .



git commit -m "first commit"

 git add set-url origin https://mslycn:9W@github.com/mslycn/HEspHome.git

git remote set-url origin https://mslycn:9W@github.com/mslycn/HEspHome.git

git branch -M main

git push -u origin main

~~~
Micropython and ESP32
Arduino and ESP32


~~~

## Projects List



Useful links

可充电HC-SR501人体感应传感器
https://mp.weixin.qq.com/s/vA-lqT7bzfF5ig_a6ZA54Q?poc_token=HHmXB2ejIjsO150y6rWY9G5oKqkfbEhuJ_oTVfQx

ESP8266 NodeMCU V3 Multi Sensor with Home Assistant (ESPHome)
ESP8266 NodeMCU V3 with Multisensor

IR Flame Detector Sensor
LDR Light Sensor
RCWL-0516 Microwave Radar Motion Sensor
DS18B20 Temperature Sensor

https://www.elec-cafe.com/esp8266-nodemcu-v3-multi-sensor-with-home-assistant-esphome/


https://esp32io.com/tutorials/esp32-tm1637-4-digit-7-segment-display


各种芯片指南

https://eeworld-1304436219.cos.ap-nanjing.myqcloud.com/html/Peripheral/Peripheral-docs/arduino-boards/install-usb-driver.html


useful links

github 中的各种开发板安装包文件过大，网速又不好，造成 Arduino IDE 在线自动安装 ESP32 等开发板的软件包不易成功。

本文介绍离线安装方法。该方法同时适用于 Windows 和 Linux

source:https://eeworld-1304436219.cos.ap-nanjing.myqcloud.com/html/Peripheral/Peripheral-docs/Esp32/install-esp32-arduino.html







