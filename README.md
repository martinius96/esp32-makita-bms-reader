# ESP32 MAKITA BMS Reader

Ported **esp32-makita-bms-reader** project from [@Belik1982](https://github.com/Belik1982) to Arduino IDE from the original PlatformIO project.  
Licensed under the **MIT License**.

* **Original project:** [Belik1982/esp32-makita-bms-reader](https://github.com/Belik1982/esp32-makita-bms-reader)

---

## 🛠 Instructions (Arduino IDE)

### 1. File Preparation
* **MAKITA folder:** Move this directory to your Arduino projects folder (e.g., `Documents/Arduino`).
* **libraries:** Copy all contents from this folder into your `Arduino/libraries` directory.
* **ESP32FS Tool:** Copy the `ESP32FS` directory to `Arduino/tools`.
    > ⚠️ **Note for Arduino IDE 2.0+:** You need to install the [LittleFS/SPIFFS Upload tool](https://github.com/earlephilhower/arduino-esp8266littlefs-plugin) manually, as the old tool structure has changed.

<p align="center">
  <img src="https://github.com/user-attachments/assets/5a6ea867-09d2-4785-b27b-e61921a0360a" width="750" alt="File structure setup" />
</p>

### 2. Uploading Data to ESP32
1.  Open the **MAKITA** project in Arduino IDE.
2.  Connect your ESP32 and select the correct **COM port**.
3.  Go to **Tools** --> **ESP32 Sketch Data Uploader**. 
    * *This uploads the HTML files from the `/data` directory into the SPIFFS/LittleFS sector of the ESP32.*

<p align="center">
    <img width="638" height="244" alt="image" src="https://github.com/user-attachments/assets/da7e0cf3-082f-4f67-b2e8-cde86b128ae4" />
<br>
  <img src="https://github.com/user-attachments/assets/ca5b0a9e-64b6-4ca1-a3e1-ccf11531e540" width="600" alt="Data Uploader Tool" />
</p>

### 3. Uploading Firmware
1.  Click the **Upload** button in Arduino IDE to flash the firmware.
2.  Once finished, you can monitor the process via the **Serial Monitor**.

<p align="center">
  <img src="https://github.com/user-attachments/assets/1b1f5461-8381-4de2-ac87-e267c6fb4c3a" width="700" alt="Compiling" />
  <br>
  <img src="https://github.com/user-attachments/assets/1301cdb1-ad29-4b3e-b9fe-56f85176b302" width="600" alt="Uploading process" />
</p>

---

## 📱 Usage
1.  After a successful flash, ESP32 will create a WiFi Access Point named: `Makita_BMS_Tool`.
2.  Connect to this WiFi.
3.  Open your browser and go to: **`192.168.4.1`**

<p align="center">
  <img src="https://github.com/user-attachments/assets/46ca90a5-1ffa-4050-9de3-28d0a1b1dc6b" width="400" alt="WiFi Connection" />
</p>

### Final Result
Now you can connect the battery and monitor real-time data like voltage, cell status, etc.

![Working app](https://github.com/user-attachments/assets/45af2cf9-c011-4930-86fd-fba5e2e5f132)
