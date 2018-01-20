# App Export

## Firmware (inbyggt program) för ESP8266, NodeMCU, BlynkBoard, etc.

#### Förbered utvecklingsmiljön (IDE)
1. Installera [Arduino IDE](https://www.arduino.cc/en/Main/Software)
2. Installera [Blynk bibliotek](https://github.com/blynkkk/blynk-library/releases/latest) och starta om Arduino IDE
3. Installera [ESP8266 core för Arduino](https://github.com/esp8266/Arduino#installing-with-boards-manager)
4. För Windows / OS X, kan du behöva installera extra drivrutiner för din programmerare
 - СP2102: https://www.silabs.com/products/mcu/Pages/USBtoUARTBridgeVCPDrivers.aspx 
 - FTDI (FT232, etc): http://www.ftdichip.com/Drivers/VCP.htm
 - *AttGöra: Länk Till drivers för CH340 and PL2303.*
5. Om ditt kort har en NeoPixel RGB LED, installera [Adafruit NeoPixel](https://github.com/adafruit/Adafruit_NeoPixel) biblioteket från Bibliotekshanterare

#### Bygg din Firmware (inbyggda program)
1. Öppna vårt exempel i Arduino IDE: ```File -> Examples -> Blynk -> Provisioning -> Blynk_ESP8266```
2. Öppna ```Settings.h``` tabben.
3. Konfigurera din Firmware:
  * ```BOARD_NAME``` - ...
  * ```BOARD_VENDOR``` - ...
  * ```PRODUCT_WIFI_SSID``` - ...
  
#### Ladda upp Firmware
1. Välj ditt kort:   ```Tools -> Board -> [Your Board]```
2. Välj rätt port:  ```Tools -> Port -> [...]```
3. Verifiera och ladda upp!

Observera att för Blynk Board, kan du välja kort-typ: ```NodeMCU 1.0```.
