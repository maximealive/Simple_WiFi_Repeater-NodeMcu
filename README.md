# Simple Wi-Fi Repeater - NodeMcu
It's not properly equal to a repeater because of limited NodeMcu range and speed so "simple Wi-Fi repeater".

In case of issue -> erase & upload stock firmware(bin folder, guide in *'References/Codes'*).

Prerequirements:
Arduino IDE
Flash..

## Tutorial
- Install driver __*CH341SER_win.zip*__
- Connect NodeMcu and check com port (*Control Panel >> Device Manager >> Ports*)
- Open 'flash_download_tools_v3.6.8.exe' -> for me was *ESP8266*
- Put the same settings as in picture(BAUD, FLASH-SIZE, etc):


![esp_tool](https://user-images.githubusercontent.com/12975980/73595374-33deea00-4518-11ea-855e-0eae4022df18.jpeg)


- Open Arduino IDE -> *Tools* -> *Serial Monitor* and select *Both NL&CR* and *115200* as picture below:


![serial_monitor](https://user-images.githubusercontent.com/12975980/73595501-bb792880-4519-11ea-9f5d-42184f2b0752.PNG)

- Press *'RST'* on NodeMcu and in serial monitor:
1. set ssid 'xxxx'(in windows to show SSID in terminal `netsh wlan show profiles`)
2. set password 'xxxx'
3. set ap_ssid 'xxxx'
4. set ap_password 'xxxx'
5. set ap_open 0
6. save
7. quit

## References/Codes
- https://www.instructables.com/id/ESP-12F-Flashing-AT-Firmware/
- https://github.com/martin-ger/esp_wifi_repeater
- https://www.instructables.com/id/POWERFUL-Wi-Fi-REPEATER-NODE-MCU/



