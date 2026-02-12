# ESP32 MAKITA BMS Reader
Ported esp32-makita-bms-reader project from @Belik1982 to Arduino IDE from Platformio project
Original project link: https://github.com/Belik1982/esp32-makita-bms-reader

# Instructions (valid for Arduino IDE < 2.0)
* MAKITA - upload directory to your Arduino projects directory (e.g. Documents)
* libraries - everything from libraries copy into Arduino/libraries directory (whole directories)
* ESP32FS - upload whole directory to Arduino/tools location (for 2.0 Arduino IDE and above, you need to install LittleFS Upload yourself)
#
* Open Project MAKITA in Arduino IDE, connect ESP32 to your PC, set COM port
* Click on Tools --> ESP32 Sketch Data Uploader (that will upload HTML files from data directory into SPIFFS sector of ESP32)
* Click on Upload to upload firmware
* You can see Serial output on start of ESP32, or you will see open WiFi network "Makita_BMS_Tool"
* Connect to it and open 192.168.4.1
* You can connect to the battery and see its voltage, etc.
