ESP32 WiFi Marauder Device

DISCLAIMER
This project is intended strictly for educational and research purposes only.
Use this device only on networks you own or have explicit permission to test.
Unauthorized use on networks you do not own is illegal.
The author is not responsible for any misuse.


PROJECT DESCRIPTION
This project documents how to create a WiFi testing device using an ESP32 WROOM-32
and the ESP32 Marauder firmware. The device uses an SD card module, display, and
external antenna, and is controlled using a serial terminal such as PuTTY.


HARDWARE REQUIREMENTS
- ESP32 WROOM-32
- Micro SD Card Adapter
- Micro SD Card
- Display (OLED / TFT compatible with ESP32)
- External Antenna
- Jumper Wires


HARDWARE CONNECTIONS
Micro SD Card Adapter to ESP32

VCC  -> 5V
GND  -> GND
CS   -> GPIO 12
SCK  -> GPIO 18
MOSI -> GPIO 23
MISO -> GPIO 19


INSTALLING ESP32 MARAUDER FIRMWARE

Step 1: Firmware Documentation
https://github.com/justcallmekoko/ESP32Marauder/wiki/update-firmware

Step 2: ESP32 Web Flasher
https://esptool.spacehuhn.com/

Step 3: Flash Required Binaries
- Bootloader
- Partition Table
- Boot App
- Firmware

Firmware file:
esp32_marauder_v1_9_0_20251213_v6.bin


INSTALL USB TO UART DRIVER (WINDOWS)
https://www.silabs.com/software-and-tools/usb-to-uart-bridge-vcp-drivers

Driver installation steps:
1. Press Windows + X
2. Open Device Manager
3. Expand Ports (COM & LPT)
4. Right-click ESP32 device
5. Click Update Driver
6. Install downloaded driver


FLASHING STEPS
1. Open the web flasher
2. Click Connect
3. Select the correct COM port
4. Reset ESP32 if prompted
5. Flash all binaries
6. Unplug and reconnect ESP32


USING SERIAL TERMINAL (PUTTY)

Download PuTTY:
https://the.earth.li/~sgtatham/putty/latest/w64/putty.exe

PuTTY Settings:
Connection Type: Serial
COM Port: ESP32 COM Port
Speed (Baud Rate): 115200


PROJECT STATUS
Platform: ESP32 WROOM-32
Firmware: ESP32 Marauder
Storage: Micro SD Card
Interface: Serial (PuTTY)
