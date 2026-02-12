# ESP32 MAKITA BMS Reader
Ported esp32-makita-bms-reader project from @Belik1982 to Arduino IDE from Platformio project
Original project link: https://github.com/Belik1982/esp32-makita-bms-reader

# Instructions (valid for Arduino IDE < 2.0)
* MAKITA - upload directory to your Arduino projects directory (e.g. Documents)
* libraries - everything from libraries copy into Arduino/libraries directory (whole directories)
* ESP32FS - upload whole directory to Arduino/tools location (**for 2.0 Arduino IDE and above, you need to install LittleFS Upload yourself**)


#
* Open Project MAKITA in Arduino IDE, connect ESP32 to your PC, set COM port
* Click on Tools --> ESP32 Sketch Data Uploader (that will upload HTML files from data directory into SPIFFS sector of ESP32)
<img width="710" height="444" alt="image" src="https://github.com/user-attachments/assets/ca5b0a9e-64b6-4ca1-a3e1-ccf11531e540" />

* Click on Upload to upload firmware
<img width="927" height="361" alt="image" src="https://github.com/user-attachments/assets/1b1f5461-8381-4de2-ac87-e267c6fb4c3a" />
<img width="698" height="331" alt="image" src="https://github.com/user-attachments/assets/1301cdb1-ad29-4b3e-b9fe-56f85176b302" />
* You can see Serial output on start of ESP32, or you will see open WiFi network "Makita_BMS_Tool"
<img width="412" height="215" alt="image" src="https://github.com/user-attachments/assets/46ca90a5-1ffa-4050-9de3-28d0a1b1dc6b" />
* Connect to it and open 192.168.4.1
* You can connect to the battery and see its voltage, etc.
![Working app](https://github.com/user-attachments/assets/45af2cf9-c011-4930-86fd-fba5e2e5f132)

