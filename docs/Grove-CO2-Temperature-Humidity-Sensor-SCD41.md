---
name: Grove - CO2 & Temperature & Humidity Sensor - SCD41
category: 
bzurl: 
oldwikiname: 
prodimagename: 
surveyurl: 
sku: 101020952
tags: grove_i2c, io_3v3, io_5v, plat_duino, plat_bbg, plat_pi, plat_wio, plat_linkit
---



![](https://files.seeedstudio.com/wiki/Grove-CO2&Temperature&HumiditySensor-SCD4/img/101020952_Preview-07.png)



The Grove - CO2 & Temperature & Humidity Sensor - SCD41 is a small but powerful module which made by Sensirion. It is a multiple function sensor which can measure temperature, pressure, humidity and CO2 at the same time. It is based on the SCD4 module and you can use this sensor in your GPS, IoT devices or other device which needs those four parameters.

<p style=":center"><a href="https://www.seeedstudio.com/Grove-CO2-Temperature-Humidity-Sensor-SCD41-p-5025.html" target="_blank"><img src="https://files.seeedstudio.com/wiki/Seeed-WiKi/docs/images/300px-Get_One_Now_Banner-ragular.png" /></a></p>

## Features

- 3-in-1 for multiple measurement
- low power consumption
- Wide measurement range
- I2C Interface
- Wide power supply range





## Specification

|Item|Value|
|---|---|
|Working voltage|2.4V~5V|
|Operating range|-10~+60℃; 0-100% r.H.; 0-40,000ppm|
| I2C Address | 0x62 |







## Hardware Overview


### Pin Map

![](https://files.seeedstudio.com/wiki/Grove-CO2&Temperature&HumiditySensor-SCD4/img/1111.jpg)


## Platforms Supported


| Arduino                                                                                             | Raspberry Pi                                                                                             |                                                                                                 |                                                                                                          |                                                                                                    |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://files.seeedstudio.com/wiki/wiki_english/docs/images/arduino_logo.jpg) | ![](https://files.seeedstudio.com/wiki/wiki_english/docs/images/raspberry_pi_logo.jpg) | ![](https://files.seeedstudio.com/wiki/wiki_english/docs/images/bbg_logo_n.jpg) | ![](https://files.seeedstudio.com/wiki/wiki_english/docs/images/wio_logo_n.jpg) | ![](https://files.seeedstudio.com/wiki/wiki_english/docs/images/linkit_logo_n.jpg) |

!!!Caution
    The platforms mentioned above as supported is/are an indication of the module's software or theoritical compatibility. We only provide software library or code examples for Arduino platform in most cases. It is not possible to provide software library / demo code for all possible MCU platforms. Hence, users have to write their own software library.




## Getting Started


### Play With Arduino

#### Hardware

**Materials required**

| Seeeduino V4.2 | Base Shield| CO2 & Temperature & Humidity Sensor - SCD41 |
|--------------|-------------|-----------------|
|![enter image description here](https://files.seeedstudio.com/wiki/Grove_Light_Sensor/images/gs_1.jpg)|![enter image description here](https://files.seeedstudio.com/wiki/Grove_Light_Sensor/images/gs_4.jpg)|![enter image description here](https://files.seeedstudio.com/wiki/Grove-CO2&Temperature&HumiditySensor-SCD4/img/thumbnail.png)|
|<a href="https://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html" target="_blank">Get One Now</a>|<a href="https://www.seeedstudio.com/Base-Shield-V2-p-1378.html" target="_blank">Get One Now</a>|<a href="https://www.seeedstudio.com/Grove-CO2-Temperature-Humidity-Sensor-SCD41-p-5025.html" target="_blank">Get One Now</a>|


!!!note
    **1** Please plug the USB cable gently, otherwise you may damage the port. Please use the USB cable with 4 wires inside, the 2 wires cable can't transfer data. If you are not sure about the wire you have, you can click [here](https://www.seeedstudio.com/Micro-USB-Cable-48cm-p-1475.html) to buy
    
    **2** Each Grove module comes with a Grove cable when you buy. In case you lose the Grove cable, you can click [here](https://www.seeedstudio.com/Grove-Universal-4-Pin-Buckled-20cm-Cable-%285-PCs-pack%29-p-936.html) to buy.



- **Step 1.** Connect the Grove - CO2 & Temperature & Humidity Sensor - SCD41 to port **I^2^C** of Grove-Base Shield.

- **Step 2.** Plug Grove - Base Shield into Seeeduino.

- **Step 3.** Connect Seeeduino to PC via a USB cable.


![](https://files.seeedstudio.com/wiki/Grove-CO2&Temperature&HumiditySensor-SCD4/img/2222.jpg)


!!!Note
        If we don't have Grove Base Shield, We also can directly connect this module to Seeeduino as below.


| Seeeduino     |  Grove - CO2 & Temperature & Humidity Sensor - SCD41           |
|---------------|-------------------------|
| 5V            | Red                     |
| GND           | Black                   |
| SDA           | White                   |
| SCL           | Yellow                  |




#### Software

!!!Note
        If this is the first time you work with Arduino, we strongly recommend you to see [Getting Started with Arduino](https://wiki.seeedstudio.com/Getting_Started_with_Arduino/) before the start.




- **Step 1.** Download the [arduino-i2c-scd4x](https://github.com/Sensirion/arduino-i2c-scd4x) library and [arduino-core](https://github.com/Sensirion/arduino-core) dependency from Github.

- **Step 2.** Refer to [How to install library](https://wiki.seeedstudio.com/How_to_install_Arduino_Library) to install library for Arduino.

- **Step 3.** Restart the Arduino IDE. Open **Sensirion I2c SCD4x** example via the path: **File --> Examples --> Sensirion I2c SCD4x --> exampleUsage**. 


![](https://files.seeedstudio.com/wiki/Grove-CO2&Temperature&HumiditySensor-SCD4/img/6267778524616.png)

- **Step 4.** Upload the demo. If you do not know how to upload the code, please check [How to upload code](https://wiki.seeedstudio.com/Upload_Code/).

- **Step 5.** Open the **Serial Monitor** of Arduino IDE by click **Tool-> Serial Monitor**. Or tap the ++ctrl+shift+m++ key at the same time. if every thing goes well, you will get the result.


The result should be like:


```c
Serial: 0x6A565F073B88
Waiting for first measurement... (5 sec)
Co2:868	Temperature:33.08	Humidity:49.40
Co2:845	Temperature:32.72	Humidity:50.13
Co2:852	Temperature:32.28	Humidity:51.54
```


!!!bug
         - To get the stable and accurate value, you need to let the arduino run the code for about 2 hours. The result is much more reliable then. 

## Play on RaspberryPi

**Materials required**


| Raspberry pi | Grove Base Hat for Raspberry Pi | Grove - CO2 & Temperature & Humidity Sensor - SCD41 |
|--------------|-------------|-----------------|
|![enter image description here](https://files.seeedstudio.com/wiki/wiki_english/docs/images/rasp.jpg)|![enter image description here](https://files.seeedstudio.com/wiki/Grove_Base_Hat_for_Raspberry_Pi/img/thumbnail.jpg)|![enter image description here](https://files.seeedstudio.com/wiki/Grove-CO2&Temperature&HumiditySensor-SCD4/img/thumbnail.png)
|[Get One Now](https://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Base-Hat-for-Raspberry-Pi.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-CO2-Temperature-Humidity-Sensor-SCD41-p-5025.html)|

### Get ready for RaspberryPi

#### I2C Connection

- **Step 1.** Plug Grove - CO2 & Temperature & Humidity Sensor - SCD41 to **I2C** port of Grove - Base Hat.

- **Step 2.** Plug Grove - Base Hat into RaspberryPi.

- **Step 3.** Connect RaspberryPi to a PC via Serial or SSH.

![](https://files.seeedstudio.com/wiki/Grove-CO2&Temperature&HumiditySensor-SCD4/img/9dfb870f961902feae92f4bde5bdeaf.jpg)

![](https://files.seeedstudio.com/wiki/Grove-CO2&Temperature&HumiditySensor-SCD4/img/GPIO-Pinout-Diagram.png)

#### Software

- **Step 1.**  Enable I2C on RaspberryPi

```shell
sudo apt-get install -y i2c-tools
sudo raspi-config
```

Follow the pictures to enable I2C and SPI on your RaspberryPi.

![](https://files.seeedstudio.com/wiki/Grove-OLED-Yellow&Blue-Display-0.96-(SSD1315)_V1.0/img/rpicon.png)

![](https://files.seeedstudio.com/wiki/Grove-OLED-Yellow&Blue-Display-0.96-(SSD1315)_V1.0/img/rpicon1.png)

![](https://files.seeedstudio.com/wiki/Grove-OLED-Yellow&Blue-Display-0.96-(SSD1315)_V1.0/img/rpicon2.png)

And then reboot your RaspberryPi

```shell
sudo reboot
```

- **Step 2.** Install necessary libraries

```shell
sudo apt-get install wget gcc make unzip -y
```

Install WiringPi Library

*If you use WiringPi, you need to update WiringPi to version 2.52. This library may not be updated. Other libraries are recommended*
```shell
cd
sudo apt-get install wiringpi
wget https://project-downloads.drogon.net/wiringpi-latest.deb
sudo dpkg -i wiringpi-latest.deb
gpio -v
```

Install bcm2835

```shell
cd
wget http://www.airspayce.com/mikem/bcm2835/bcm2835-1.60.tar.gz
tar zxvf bcm2835-1.60.tar.gz 
cd bcm2835-1.60/
sudo ./configure
sudo make && sudo make check && sudo make install
```

For further information and the newest libraries please refer to website：[bcm2835](http://www.airspayce.com/mikem/bcm2835/)

- **Step 3.** Download the driver from the [Sensirion GitHub Page](https://github.com/Sensirion/raspberry-pi-i2c-scd4x/tags) and extract the `.zip` on your Raspberry Pi

- **Step 4.** Compile the driver

**1**.Open a terminal

**2**.Navigate to the driver directory. E.g. cd ~/raspberry-pi-i2c-scd4x

**3**.Run the make command to compile the driver


Output:

```shell
rm -f scd4x_i2c_example_usage
cc -Os -Wall -fstrict-aliasing -Wstrict-aliasing=1 -Wsign-conversion -fPIC -I. -o scd4x_i2c_example_usage  scd4x_i2c.h scd4x_i2c.c sensirion_i2c_hal.h sensirion_i2c.h sensirion_i2c.c \
	sensirion_i2c_hal.c sensirion_config.h sensirion_common.h sensirion_common.c scd4x_i2c_example_usage.c
```

- **Step 5.** Test your connected sensor

Run `./scd4x_i2c_example_usage` in the same directory you used to compile the driver.

Output:

```c
serial: 0xbff79f073b51
CO2: 799
Temperature: 20.92
Humidity: 35.95
CO2: 900
Temperature: 20.92
Humidity: 36.47
CO2: 926
Temperature: 20.81
Humidity: 36.85
...
```

For further infomation, please check [Sensirion/raspberry-pi-i2c-scd4x on GitHub](https://github.com/Sensirion/raspberry-pi-i2c-scd4x).

## Have fun learning with Micro:bit

Micro:bit is a powerful microcomputer development board designed by BBC (British Broadcasting Corporation) for programming education for young people and even primary students can use it to program. 

Although the board is amazingly only half the size of a credit card, the onboard electronic modules are so plentiful: 5x5 LED display, two programmable buttons, accelerometer, electronic compass, temperature light sensor, and Bluetooth low energy consumption, etc. It can also connect computing devices including Raspberry Pi and Arduino to realize various functions. 

You can click [makecode-extension-scd41](https://github.com/Sensirion/makecode-extension-scd41) to access the files and use it to connect [Grove - CO2 & Temperature & Humidity Sensor](https://www.seeedstudio.com/Grove-CO2-Temperature-Humidity-Sensor-SCD41-p-5025.html).

## Schematic Online Viewer

<div class="altium-ecad-viewer" data-project-src="https://files.seeedstudio.com/wiki/Grove-CO2&Temperature&HumiditySensor-SCD4/res/SCH&PCB.zip" style="border-radius: 0px 0px 4px 4px; height: 500px; border-style: solid; border-width: 1px; border-color: rgb(241, 241, 241); overflow: hidden; max-width: 1280px; max-height: 700px; box-sizing: border-box;">
</div>



## Resources

- **[PDF]** [Sensirion CO2 Sensors SCD4x Datasheet](https://files.seeedstudio.com/wiki/Grove-CO2&Temperature&HumiditySensor-SCD4/res/Sensirion_CO2_Sensors_SCD4x_Datasheet.pdf)
- **[STEP]** [STEP of Sensirion CO2 Sensors SCD4x](https://files.seeedstudio.com/wiki/Grove-CO2&Temperature&HumiditySensor-SCD4/res/Sensirion_CO2_Sensors_SCD4x_STEP_file.step)
- **[ZIP]** [Grove - CO2 & Temperature & Humidity Sensor - SCD41 Board File](https://files.seeedstudio.com/wiki/Grove-CO2&Temperature&HumiditySensor-SCD4/res/SCH&PCB.zip)

## Tech Support
Please do not hesitate to submit the issue into our [forum](https://forum.seeedstudio.com/).<br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://files.seeedstudio.com/wiki/Wiki_Banner/new_product.jpg" /></a></p>