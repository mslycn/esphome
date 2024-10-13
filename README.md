
## Project Information

local:F:\developer_Xiaomi\EspHome

remote:https://github.com/mslycn/esphome

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


Git Bash

cd f:
cd F:/developer_Xiaomi/EspHome

$ git init

$ git config user.email "36*@mail.com"


$ git config user.name "mslycn"


$ git add .



git commit -m "first commit"

 git add set-url origin https://mslycn:9W@github.com/mslycn/HEspHome.git

git remote set-url origin https://mslycn:9W@github.com/mslycn/HEspHome.git

git branch -M main

git push -u origin main







