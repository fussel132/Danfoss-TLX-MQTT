# Danfoss-TLX
**RS485 Communication with Danfoss TLX solar inverter and MQTT publishing.**

I was very happy with AMajland's REST version but to get some more relevant data (like live power) pushed to HomeAssistant more frequently, I introduced "priorities" and switched from REST to MQTT so the ESP does not need to handle an entire webserver and thus slow down the communication with the inverter.

>The communication with the inverter is based on [TorbenNor](https://github.com/TorbenNor)'s `TLX-simple.ino` which can be found [here](https://github.com/TorbenNor/Danfoss-TLX).
Some error-handling and quality-checks are forked from [AMajland](https://github.com/AMajland), so thanks a lot to you two!

## Hardware Setup

TODO

Board LOLIN D32                                        
https://www.aliexpress.com/item/32808551116.htm
  Pin 16  :RXD2 Seriel in
  Pin 17  :TXD2 Seriel out
R411A01 mini 3.3V Auto RS485 to TTL232 Converter Board  
https://www.aliexpress.com/item/32782552104.html

## Configure and Install Software

TODO

MQTT Broker (like Mosquitto)

Used Libraries - output from verbose compile
Multiple libraries were found for "WiFi.h" Used:       ...\packages\esp32\hardware\esp32\2.0.3\libraries\WiFi
Using library WiFi at version 2.0.0 in folder:         ...\packages\esp32\hardware\esp32\2.0.3\libraries\WiFi 
Using library WebServer at version 2.0.0 in folder:    ...\packages\esp32\hardware\esp32\2.0.3\libraries\WebServer 
Using library ArduinoJson at version 6.19.4 in folder: ...\libraries\ArduinoJson 
Using library FS at version 2.0.0 in folder:           ...\packages\esp32\hardware\esp32\2.0.3\libraries\FS 

## Home Assistant Integration

TODO