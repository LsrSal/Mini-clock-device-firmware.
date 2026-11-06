## Modified to support that cute little "mini Smart Wifi Weather Clock". To purchase - search usual places: Ali, eBay, Amazon.
It is ESP8266 + ST7789 based + 4MB flash, perfect for Arduinot project.
It took me some time to figure out implementation specific pins. Unfortunately Adafruit examples do not work out of the box, in addition to pins, it need to use "SPI_MODE3". See example folder. 
![mini Smart Wifi Weather Clock](https://raw.githubusercontent.com/LsrSal/Adafruit-ST7735-Library/master/image.png) Only .ino is edited.


This is a library for Adafruit displays based on ST77* drivers.

Check out the links above for our tutorials and wiring diagrams.
These displays use SPI to communicate, 4 or 5 pins are required to
interface (RST is optional).

Adafruit invests time and resources providing this open source code,
please support Adafruit and open-source hardware by purchasing
products from Adafruit!

Written by Limor Fried/Ladyada for Adafruit Industries.
MIT license, all text above must be included in any redistribution.

Recent Arduino IDE releases include the Library Manager for easy installation. Otherwise, to download, click the DOWNLOAD ZIP button, uncompress and rename the uncompressed folder Adafruit_ST7735. Confirm that the Adafruit_ST7735 folder contains Adafruit_ST7735.cpp, Adafruit_ST7735.h and related source files. Place the Adafruit_ST7735 library folder your ArduinoSketchFolder/Libraries/ folder. You may need to create the Libraries subfolder if its your first library. Restart the IDE.

Also requires the Adafruit_GFX library for Arduino.

## Flip clock

One of long nights I've decided to code a flip clock for this device. Of course it is NTP synchronized.
Flip Page images stored in [LittleFS](https://github.com/earlephilhower/arduino-esp8266littlefs-plugin/releases) and related library (use library manager to install).

Bitmaps in File System can be easily be edited to your liking. 1MB FS is enough for this set.

You also will need TFT_eSPI library, configuration for this device is attached and must be placed in library directory (backup the original for other projects).

All settings are through USB/Serial terminal, just type "?" for help.
