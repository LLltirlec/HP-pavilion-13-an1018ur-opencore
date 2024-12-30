# HP-pavilion-13-an1018ur-opencore
 Opencore for HP Pavilion 13-an1018ur

![Снимок экрана 2023-02-15 в 02 35 14](https://user-images.githubusercontent.com/19612593/218887324-dfb17819-37a3-417c-9d6f-cc14cd797aa9.png)

 ## My Laptop
 | Specs         | Details                    
 | -----------   | ------------------------------- |
 | Laptop        | `HP Pavilion laptop 13-an1018ur`|
 | CPU           | `Intel Core i5-1035G1`          |
 | IGPU          | `Intel UHD Graphics G1`         |
 | WiFi+BT       | `Fenvi BCM94360NG`              |
 | SSD.          | `Intel 670p 512gb`              |
 | RAM           | `8 GB DDR4 SDRAM`               |
 | OC ver.       | `0.8.9`                         |
 | MacOC ver.    | `15.0 Sequoia`                  |

 ### Works
 - [x] Intel Integrated Graphics (IGPU)
 - [x] USB
 - [x] Webcam
 - [x] Brightness controls
 - [x] Speakers
 - [x] Integrated Microphone (you can talk to Siri)
 - [x] Apple Services (iCloud, Apple Music, Apple TV ...)
 - [x] Airdrop & Handoff
 - [x] WiFi & Bluetooth
 - [x] SD Card Reader
 - [x] TouchPad with Advanced Gestures
 - [x] Battery percentage
 - [x] Sleep
 - [x] Trim

 ### Doesn't work & Bugs
 - Synaptics touchpad twitches
 - Blackscreen after sleep with plugged in AC adapter 
 
 ### Terminal
  - sudo pmset -a hibernatemode 3
  - sudo trimforce enable
 
 ### Sleep

Remember that you are recommended to apply these settings once you booted macOS:

```
sudo pmset autopoweroff 0
sudo pmset powernap 0
sudo pmset standby 0
sudo pmset proximitywake 0
sudo pmset tcpkeepalive 0
```
You can keep `tcpkeepalive` on, but you might experience a litte bit more discharge than usual when putting your laptop to sleep overnight (7-8% instead of 3-5%) but you have the possibility to recieve notifications/updates every 2 hours since the laptop will wake to check them if `tcpkeepalive` is set to `1`
 
