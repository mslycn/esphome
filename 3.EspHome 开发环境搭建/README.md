本篇学习把esp32接入home assistant的全过程，涉及配置文件的生成和固件的编译。
然后简单的让浏览器帮我们写入已生成的固件（via https://web.esphome.io/）。

key points
1. 搭建开发环境( install esphome addon)

2. 生成配置文件（new devie）

3. 生成fireware（Install）

4. 保存fireware (Mode)

5. 上传固件到esp32（）


Install the ESPHome addon to HA.
Buy an esp8266 or esp32 board. You can also buy a smaller esp D1 mini.
Buy the BH1750 sensor.
You will need a USB cable to connect esp and HA to be able to upload yaml to esp.
Then look here

## step 1. Install the ESPHome addon to HA.


## step 2.New device


## step 3. get fireware

To get the factory file of your ESPHome project:
~~~
Open your ESPHome dashboard
Find your device card click on menu (more_vert)
Click on Install
Click on Manual Download
Click on Modern Format
~~~


## step4. upload fireware to esp32 via ttps://web.esphome.io/

Open https://web.esphome.io/

https://blog.matterxiaomi.com/blog/esphome-esp32-pir-hc-sr501-part2/

https://blog.matterxiaomi.com/blog/esphome-esp32-pir-hc-sr501-part1/

在从github上克隆ESP8266_RTOS_SDK时会经常超时失败，很耽误时间，现在乐鑫有了国内镜像：https://gitee.com/EspressifSystems