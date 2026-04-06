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

http://192.168.2.126:6052



~~~
http://192.168.2.138:6052/
esphome
esphome
~~~

cd /data/docker/esphome/config

debian:/data/docker/esphome/config# ls -ls
~~~
total 36
4 drwxr-xr-x 2 root root 4096 Jun 23 12:00 archive
4 -rw-r--r-- 1 root root  545 Jun 24 17:29 c3.yaml
4 -rw-r--r-- 1 root root 2274 Mar  5 15:01 esp32-bluetooth-proxy-58d270.yaml
4 -rw-r--r-- 1 root root  428 Aug 23 21:55 esp32-devkitv1-no2.yaml
4 -rw-r--r-- 1 root root 3630 Aug 21 16:46 esp32no2.yaml
4 -rw-r--r-- 1 root root  504 Feb 27 07:33 esp32-s3-box-3-2d954c.yaml
4 -rw-r--r-- 1 root root 3060 May  1 11:11 esp32s.yaml
4 -rw-r--r-- 1 root root  533 Feb 27 07:33 esp8266-12f.yaml
4 -rw-r--r-- 1 root root   86 Mar  2 10:55 secrets.yaml

~~~



other

docker run --rm -v "${PWD}":/config -it ghcr.io/esphome/esphome


useful links

Installing Docker ESPHome and configuring ESPHome with ESP8266 and ESP32

https://chelmiki.com/posts/installing-and-configuring-esphome/

https://docs.sunfounder.com/projects/raspad3-cn/zh/latest/iot/homeassistant/install_and_configure_esphome.html



## docker-compose.yaml
~~~
cd /data/docker/esphome

docker-compose up -d

docker-compose down
docker-compose up -d
~~~





http://192.168.2.138:6052


source code in here:

/data/docker/esphome/config


log

~~~

~~~




useful links

ESPHome Command Line

https://esphome.io/guides/getting_started_command_line.html#installation
  


