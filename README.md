# IoT enabled dust sensor
Final project for second microcontrollers course at AGH, Cracow. The sensor platform is build around powerful ARM Crotex M0+ microcontroler. It's main purposes are monitoring the environtment, displaying the data to user and sending them to thingspeak account. It is achieved using Sharp GP2Y1010AU analog dust sensor, Bosh BMP180 i2c temperature and pressure sensor and ESP8266 WiFi module for internet comunication. 

![](https://cloud.githubusercontent.com/assets/25593055/22663203/0d1d30ce-ecac-11e6-8479-7e0b9328e5e0.jpg)

## Description
Sensor platform uses Nextion NX4832K035 display for presenting collected infromation. Both i2c and UART libraries were written for this project. Freescale KL46 family microcontroler acquires the data from sensors, averages them and sends to display. Every 20 seconds samples are sent to thingspeak channel.

![](https://cloud.githubusercontent.com/assets/25593055/22663204/0d1d9aaa-ecac-11e6-9044-d8223159bb86.png)

To eliminate messy wiring and make the project more elegant, an add-on shield board was made. It's purpose is providing power for the display and microcontroler as well as interfacing with WiFi module and dust sensor.

![](https://cloud.githubusercontent.com/assets/25593055/22663205/0d1ee23e-ecac-11e6-8c8e-f9a42bbcb6a5.png)

###BOM
 - FRDM-KL46Z board
 - BMP180 digital preassure sensor
 - GP2Y1010AU dust sensor
 - NX4832K035 HMI display
 - ESP8266 module
 - 5V and 3.3V regulators
