# :desktop_computer: What to do after building a pc in 2020

I have been using laptops for ages, Dell Latitude D600 from 2003, Acer Aspire 4820 from 2010 and HPs for work. Finally built one for myself.

Main parts: AMD R5 3600 + MSI Mortar MAX + Nvidia 1660 super.

Record the steps for my first PC build, hopefully, to be of some help for the next one.

[TOC]

## Pre-Building

### Specifications

- Size of motherboard.

- Height of CPU cooler.

- Length of GPU card.

- Length of power supply.

- Wattage of power supply.



### Shopping list

- PH2 screwdriver (for removing the default CPU bracket on the motherboard).

- HDMI or DisplayPort cable.

- USB disk as [Windows 10 installation media](https://www.microsoft.com/en-us/software-download/windows10).

- USB keyboard (comment from a Bluetooth keyboarder).

- Wireless USB Adapter.

- Bluetooth USB Adapter.



### Checklist

- Memory slots for dual-channel setup.

- Test power via fans before screwing into the case.

- Orientation of the fans.



### OS part (15min)

1. Power on: lights on, screen on, welcome to the BIOS.
2. BIOS setting: Change the boot order to recognise USB disk.
3. Reboot to install Win10.
4. Reboot to setup Win10 (no network, no activation and turn off privacy).



## Fisrt-of-all-after-building

### Turn off optimisation

Do NOT defragment SSD .This is a windows bug and was fixed recently.


<img src="./screenshots/disk_management.png" align="left" width="600"/>





### Cancel indexing

Use other tools for global searching, so cancel the indexing on the disk.


<img src="screenshots/indexing.png" align="left"/>





### Cancel disk protection

Control Panel\System and Security\BitLocker Drive Encryption

Turn off the BitLocker.



### Activate Windows

Plug wireless USB adapter on and activate Windows.



### Update Windows

Update Windows with several reboot until see the message "Up to date".



### Update GPU driver

Update video card driver: https://www.nvidia.com/en-us/geforce/drivers/

Latest version: [451.67](https://www.nvidia.com/en-us/drivers/results/162105/)



Install the driver without GF experience.

Open NVIDIA control panel:

> Set "Power management mode" to max.
>
> Set "Texture filtering - Quality" to High performance.
>
> -- <cite>JayzTwoCents [video](https://youtu.be/RYYoCXh2gtw?t=1055)</cite>

<img src="./screenshots/nvidia_settings.png" align="left" width="400"/>



### Update BIOS driver

Check BIOS version in CMD/Powershell by:

```
systeminfo
```

Latest version: [7B89v1E](https://www.msi.com/Motherboard/support/B450M-MORTAR#down-bios)

Download the file into USB disk, plug in and update it.



## Windows settings

### Apps

#### Apps & features

**Uninstall**

feedback hub
Groove Music
Mail and Calendar
MS Solitaire Collection
MS Edge
MR portal
Skype
Spotify
Tips
Voice Recorder
Weather

**Advanced options - Off and Terminate**

Cortana
Get help
Maps
Movies TV
People

**Optional features - Remove**
Windows Fax and Scan
IE11
Windows Hello Face
Windows Media Player
Math Recognizer



<img src="./screenshots/apps_features_cortana.png" align="left" width="400"/>




<img src="./screenshots/cortana_advanced_options.png" align="left" width="400"/>





### System

#### About

Activate Windows.

Name your baby.



### Privacy

#### Windows permissions

offffffff (allofthem)

#### App permissions

offffff   (mostofthem)			



## More Settings

#### Display

Refresh rate: 144Hz



#### Chrome

Relocate the temp folder:


```
cd C:\Users\Shaw\AppData\Local\Google\Chrome
mklink /D "C:\Users\Shaw\AppData\Local\Google\Chrome\User Data" "E:\Temp\ChromeUserData"
```



#### Win Library

Remove unused ones.

Move user library location



#### Win

Set theme.

Set night light.



#### Backup

Disk++



#### Mileage

C disk: 35.4G used.

All disks: 253034 objects.



## Software

### System

Chocolatey: ```choco install list.config ```

MSI light



### Coding

VS

VS Code

#### extensions



### Entertainment

Game launcher set: Battle.net, Epic, Origin, Steam, Uplay



### Win Store

xodo pdf
eartrumpet



## License

CC-BY-4.0