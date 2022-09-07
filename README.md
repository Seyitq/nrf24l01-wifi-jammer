<h1 align="center">Wifi Jammer</h1>
<h3 align="center">This module is a transceiver, meaning it does both send and receive. These modules are very cheap on price with small size, the operating voltage of this module is from 1.9 to 3.6 volts, MOSI, MISO and SCK pins are the SPI pins of the module. Must be connected to SPI protocol pins in Arduino. The CSN and CE pins are for setting the module to active mode and switching between command mode and data transfer. These two pins can be attached to any digital pin on the Arduino. The IRQ pin is an interrupt pin and does not need to be connected.</h3>

<p align="center">Some of the specifications of these modules are as follows:

- Power consumption when sending data is about 12 mA.
- Range, if used outdoors with antenna, can reach up to 1000 meters
- Each module can communicate with up to 6 other modules.
- Use the 2.4 GHz band.
- You can send 1 to 25 bytes of raw data at a speed of 1 MB.
- Interference in the 2.4 GHz network band
There are many devices that operate in the 2.4GHz range, such as; Telephone, Bluetooth, WiFi, car alarm, microwave are all in this range that with this project we will be able to measure and display these values. It is not usually very difficult to find interference. Products are coming to market that act as spectrum analyzers and use a standard USB interface to a laptop, meaning that the interference source can be easily used with an antenna to find interference.</p>

Project working method
The activity of the nRF24 RF radio board is transmitted to the Arduino board via the serial interface and displays any type of activity in ASCII code. Domains are displayed in different channels with the help of a simple mapping. In this project, the 2.4GHz network scanner even shows the interference of microwaves and wireless cameras. Of course, you may be wondering what is the difference between this scanner and packet monitors ?! In response, I have to mention that in the monitor pack, it only monitors the 14 channels available for WiFi networks, but in this project, we can detect and actually see any frequency in the 2.4 range. In the second part, we will deal with this issue more. In the following, we will display these values in the form of graphs using the OLED display. The graph values are based on the nRF power consumption at the moment of scanning, which in this scenario is directly related to the input data.

Items needed:
- Arduino
- NRF24L01
- Oled 0.96
- Library installation required

First, we will install the required library in Arduino IDE software. Follow these steps:

- Follow this path Sketch> Include Library> Manage Libraries
- Search for Adafruit SSD1306.
- Install the library.
- Then search for the word “GFX” and install it.
