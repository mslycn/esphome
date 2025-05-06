Install ESPhome via Docker 

ESPHome can be easily installed through docker.


# Install the Docker ESPHome  to HA.

## Instll Docker ESPHome via Command Line

Getting Started with the ESPHome Command Line.Installing ESPHome Manually.

~~~
docker pull ghcr.io/esphome/esphome:stable
~~~

run ok
~~~
sudo docker run -d --name="esphome" --restart=unless-stopped -p 6052:6052 -p 6123:6123 -v /home/finity/docker/esphome:/config esphome/esphome 
~~~

docker run -d --name="ESPHome" -e TZ=Asia/Shanghai -v /home/esphome:/config -v /run/udev:/run/udev --privileged --restart=always -p 6052:6052 esphome/esphome

goto

http://192.168.1.3:6052

other

docker run --rm -v "${PWD}":/config -it ghcr.io/esphome/esphome


useful links

Installing Docker ESPHome and configuring ESPHome with ESP8266 and ESP32

https://chelmiki.com/posts/installing-and-configuring-esphome/

https://docs.sunfounder.com/projects/raspad3-cn/zh/latest/iot/homeassistant/install_and_configure_esphome.html



## docker-compose.yaml

cd /data/docker/esphome

docker-compose up -d


docker-compose up -d

docker-compose down




http://192.168.1.3:6052

useful links

ESPHome Command Line
https://esphome.io/guides/getting_started_command_line.html#installation
  


