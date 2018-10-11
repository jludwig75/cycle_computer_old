# cycle_computer
ESP-32 GPS Cycling Computer with BLE HRM

This project is for a GPS cycling computer using an ESP-32. It will support BLE for connecting to a Bluetooth heart rate monitor.

Componenent List
- ESP32 MCU
- MTK3329 GPS with PPS output
- MPL3115A2 baramoter/thermometer - Provides refined altitude data and temperature
- MPU9250 accelerometer/magnetometer - Will use compass for possible navigation and could use accelerometer as INS
- OLDE (st7735R) - Display
- P-channel MOSFETs as switches for GPS, barometer, accerlerometer and display
- LiOn Charging circuit

Power
-----
The device will always be connected to the battery. When powered down, all devices will be powered down and the ESP-32 will enter its deepest sleep mode from which it can be awakened via an interrupt through a button push.

