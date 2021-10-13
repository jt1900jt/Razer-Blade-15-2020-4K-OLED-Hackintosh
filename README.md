<b><h1>Razer Blade 15 2020 4K OLED Hackintosh</h1></b>

<img src="https://i.imgur.com/Pf1KxTt.png" />
<img src="https://i.imgur.com/KFpYw0c.jpeg" />
## Introduction
  
Configuration for getting macOS Big Sur to run on a Razer Blade 15 2020 using OpenCore 0.7.4. If you would like to get started with creating a Hackintosh on your Razer Blade but have no experience, I would highly reccomend following Dortania's fantastic [Opencore Install guide][1] and then returning here for troubleshooting.
  
I replaced my wifi card with a DW1560 so I am using the BCM kexts. If you would like to use your built in intel wifi it is possible but not recommended as it does not fully support contunity features such as handoff and apple watch unlock. If those features are not important to you then you can checkout the project here: https://github.com/OpenIntelWireless/itlwm. 

## Specs

| Key                    | Value                                                        |
| ---------------------- | ------------------------------------------------------------ |
| CPU                    | Intel Core i7-10750H                                         |
| GPU                    | Intel UHD Graphics 630                                       |
| Screen                 | 15" 4K/UHD Display                                           |
| Camera                 | HD webcam (720p)                                             |
| RAM                    | 16 DDR4 2,933MHz (2x8GB)                                     |
| Internal SSD           | Samsung SSD 970 EVO (MacOS) + SAMSUNG MZVLB512HBJQ (Windows) |
| Audio                  | ALC298                                                       |
| Wireless               | BCM94352Z - AKA DW1560                                       |

Quick Note: My serial number, MLB, and UUID have been removed from the config.plist. Please use CorpNewt's [GenSMBIOS][2] to create your own

<img src="https://i.imgur.com/HFMsSFR.png" />

## Pre-Install

You'll need to use a hardware programmer to unlock DVMT Options. Follow the instructions on https://git.io/JkuFs for how to mod your BIOS.

## What works

- iGPU
- Audio
- Battery
- Touchpad
- Touchscreen (if supported)
- USB Ports
- CPU Freq
- Intel Bluetooth / Wifi

## Credits:

- @steelbrain for his work on the BIOS modding
- OpenCore Team
- CorpNewt
[1]:https://dortania.github.io/OpenCore-Install-Guide/
[2]:https://github.com/corpnewt/GenSMBIOS
