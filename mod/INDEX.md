# GTBikeV 0.3.0.2 - Documentation <!-- omit in toc -->

The latest version of this document is available on github: [https://github.com/gtbikev/docs/blob/master/mod/INDEX.md](https://github.com/gtbikev/docs/blob/master/mod/INDEX.md)

**About**

`GTBikeV` is a mod for GTA V that turns a Smart Bike Trainer, or cycling power meter, into the game controller, making your game time actual training time. You'll have a cycling workout immersed in the `GTA V` world environment. `GTBikeV` mod is developed by Nestor Matas (Makinolo) and the project is hosted on [gta5-mods.com](https://www.gta5-mods.com/scripts/gt-bike-v).

**Document Information**

This document is a collection of information found on [Grand Theft Auto Bike](https://www.facebook.com/groups/1089053124812221) facebook group, YouTube and other sources on the internet. This documentation supports the following GTBikeV release:

| GTBikeV Mod | Release Date  |
| :---------- | :------------ |
| 0.3.0.2     | June 22, 2020 |

**Important Notice / Warning**

GTBikeV mod is only supported in GTA V `Story Mode`. If you play the mod in GTA V `Online` then you will be immediatly blocked from accessing the game.

This mod requires actual `PHYSICAL EXCERSISE` to be meaningful.

---

**Table of Contents**

- [1. Installation](#1-installation)
  - [1.1 Hardware requirements](#11-hardware-requirements)
  - [1.2 Software requirements](#12-software-requirements)
  - [1.3 Installation guide](#13-installation-guide)
    - [1.3.1 Part I: Install GTA](#131-part-i-install-gta)
    - [1.3.2 Part II: Install Mod](#132-part-ii-install-mod)
    - [1.3.3 Additional Resources](#133-additional-resources)
- [2. Upgrade](#2-upgrade)
- [3. User guide](#3-user-guide)
  - [3.1 Start ride](#31-start-ride)
  - [3.2 End ride](#32-end-ride)
  - [3.2 Configuration](#32-configuration)
  - [3.3 Courses](#33-courses)
    - [3.3.1 About courses](#331-about-courses)
    - [3.3.2 Install courses](#332-install-courses)
- [4. Shortcuts](#4-shortcuts)
  - [4.1 Function keys](#41-function-keys)
  - [4.2 Keyboard keys](#42-keyboard-keys)
  - [4.3 Numpad keys](#43-numpad-keys)
- [5. Troubleshooting](#5-troubleshooting)
  - [5.1 Connection Issue](#51-connection-issue)
- [6. Credits](#6-credits)
- [7. Contributors](#7-contributors)


## 1. Installation

### 1.1 Hardware requirements

* Windows PC. System Requirements: https://support.rockstargames.com/articles/203428177/Grand-Theft-Auto-V-PC-System-Requirements
* ANT+ dongle for your PC to communicate with the trainer
* Smart trainer ANT+ FE-C compatible or ANT+ Cycling Power Meter
* A bicycle compatible with your smart trainer
* Optional: keyboard with NumPad

### 1.2 Software requirements

The following software is required:

* Most recent version of GTA V (Windows PC version) from [Steam](https://store.steampowered.com/) or [Epic Games](https://www.epicgames.com/)
* [ScripthookV](http://www.dev-c.com/gtav/scripthookv/)
* [ScripHooktVDotnet](https://github.com/crosire/scripthookvdotnet/releases)
* [GT Bike V Mod](https://de.gta5-mods.com/scripts/gt-bike-v)

Optional (if you don't have them already):
* [Microsoft .Net Framework 4.5.2 or above](http://www.microsoft.com/en-us/download/details.aspx?id=42643)
* [Visual C++ Redistributable Packages](https://www.microsoft.com/en-us/download/details.aspx?id=53840)

### 1.3 Installation guide

#### 1.3.1 Part I: Install GTA

Perform the following steps to install GTA:

1. Buy GTA V (Windows PC version) from [Steam](https://store.steampowered.com/) or [Epic Games](https://www.epicgames.com/)
2. Install GTA V
3. Play in GTA V in `Story Mode` and complete all missions of the `Prologue`. The prologue contains four missions: `The Robbery`, `The Threat-Assessment`, `The Escape`, `The Getaway`. There are several tutorials on the internet and on YouTube about how to finish the prologue. You find a walkthrough link in [chapter 1.3.3](#133-additional-resources).

#### 1.3.2 Part II: Install Mod

Perform the following steps to install mod:

1. Download [ScriptHookV](http://www.dev-c.com/gtav/scripthookv/)
2. Download [ScripHooktVDotnet](https://github.com/crosire/scripthookvdotnet/releases)
3. Download [GT Bike V Mod](https://de.gta5-mods.com/scripts/gt-bike-v)
4. Unzip `ScriptHookV` file; navigate to bin folder; copy `dinput8.dll`, `NativeTrainer.asi`, `ScriptHookV.dll` to GTA V installation directory
5. Unzip `ScriptHookVDotnet` file; copy all ScriptHookVDotNet.* files to GTA V installation directory
6. Unzip `GTBikeV` file: copy folder `Scripts` to GTA V installation directory; copy folder `ModSettings` to user data directory located at `My Documents\Rockstar Games\GTA V`

> Important note: folder `Rockstar Games\GTA V` will be created after you have launched GTA V.

#### 1.3.3 Additional Resources

* GTBikeV Mod page: [https://www.gta5-mods.com/scripts/gt-bike-v](https://www.gta5-mods.com/scripts/gt-bike-v) (Makinolo)
* Prologue Walkthrough: [https://www.ign.com/wikis/gta-5/Prologue](https://www.ign.com/wikis/gta-5/Prologue) (IGN)
* Tutorial: [https://www.youtube.com/watch?v=dbMh9LEGMBg](https://www.youtube.com/watch?v=dbMh9LEGMBg) (Chris Pritchard Cycling News)
* Setup, How-To Guide: [https://www.youtube.com/watch?v=Bl17P_mpHI0](https://www.youtube.com/watch?v=Bl17P_mpHI0) (GPLama)


## 2. Upgrade

Perform the following steps to upgrade mod:

1. Download [GT Bike V Mod](https://de.gta5-mods.com/scripts/gt-bike-v)
2. Unzip `GTBikeV` file: copy folder `Scripts` to GTA V installation directory; copy folder `ModSettings` to user data directory located at `My Documents\Rockstar Games\GTA V`


## 3. User guide

### 3.1 Start ride

Perform the following steps to start a ride: 

1. Start `GTA V`
2. Select `Story Mode`
3. Open mod menu using `F5` key
4. Select `Activate mod` to activate the mod and initialize comunication with the trainer
5. If you want to use autodrive feature then select checkbox `Auto drive`
6. If you want to avoid bstacles then select checkbox `Avoid obstacles`
7. If you want to ride a pre-defined route then select `Courses` and choose a route
8. If not done in the configuration file, specify user weight
9. Start riding!

### 3.2 End ride

Perform the following steps to end a ride:

1. Wait until the virtual bike computer shows zero speed
2. Open mod menu using `F5` key
3. Select option `End and save current activity`

This will save the ride data to a fit file to user data directory located at `My Documents\Rockstar Games\GTA V`

### 3.2 Configuration

The following options can be set in the `GTBikeVConfig.ini` in the user data directory located at `My Documents\Rockstar Games\GTA V\ModSettings`:

|Key|Value|Description|
|:---|:---|:---|
|SelectedBike|SCORCHER, TRIBIKE, TRIBIKE2, TRIBIKE3, FIXTER, CRUISER, BMX|Bike used by the avatar during the ride. The game does not feature any other bike models.|
|SlopeScale|0.0-2.0|Scales the inclines in the game, ranges from 0.0 to 2.0. The first one will remove any slope change and the latter will multiply slopes by 2. Default value is 0.5 which is the more realistic one. This settings affects the incline value sent to your trainer as well as the one used to calculate virtual speed.|
|DebugWindow|True / False|Activates the debug view showing internal data in 3 panels, Activity panel, general panel and Simulation data / trainer data panel.|
|InitialGPSPointLat InitialGPSPointLong||Initial GPS coordinates corresponding to the 0,0 coordinates in Los Santos map. The defaultInitial GPS coordinates corresponding to the 0,0 coordinates in Los Santos map. The default value maps to a small island in the pacific but you can change it to wherever in the world you want your FIT files to be located at.|
|FECDeviceId PWRDeviceId HRDeviceId CADDeviceId ControlsDeviceId||Sets the mod to listen to a specific ANT device id for every of the ANT+ supported profiles so in case you have more than one device you can select the one you will be using. The special value 0 means it will pair the first device ot finds which is usually fine if you only have one. The special value 65535 is used when you want to deactivate the reception of a particular device, which can help with mod performance when you don't own that kind of sensor. FEC is an ANT+ smart trainer. PWR is an ANT+ power sensor. HR is an ANT+ heart rate strap. CAD is an ANT+ cadence sensor. Controls is an ANT+ remote control (experimental).|
|Imperial|True / False|Toggles the unit system used in the bike display to show distance, speed, etc.|
|UserWeightKg||User weight for the simulation. In Kilograms. This value changes if you change the weight in the mod menu.|
|RoadFeel|True / False|Toggles the road feel simulation for Tacx Neo line of trainers and indoor bikes.|
|WayPointDefaultColor|FFADFF2F|Configures the color of the waypoints shown while following one of the predefined routes. If there is a specific configuration in the course file, it has precedence over this one Colors are specified in AARRGGBB format.|
|WayPointDefaultRadius|0-40|Configures the radius of the waypoints shown while following one of the predefined routes. If radius is zero the waypoints are not shown. If there is a specific configuration in the course file, it has precedence over this one.|
|AlwaysUseVirtualSpeed|True / False|Allows you to always use the virtual speed calculations regardles if you have a smart trainer broadcasting its own speed. If you only have a power meter this setting does not apply, speed will be always virtual.|

### 3.3 Courses

#### 3.3.1 About courses

`GT Bike V` mod features a course reader which auto drives you around Los Santos following different routes of various difficulty levels. Course files (.json) are storing the starting point, start banner, waypoints and end banner with X, Y and Z coordinates.

#### 3.3.2 Install courses

Courses are stored in the folder `ModSettings` in the user data directory located at `My Documents\Rockstar Games\GTA V`. Courses are stored in a [repository](https://github.com/gtbikev/courses) and a preview is available on a [route database](https://www.gtbikevroutes.fun). Community members are also sharing often routes on [Grand Theft Auto Bike](https://www.facebook.com/groups/1089053124812221) facebook group. Install courses by copy the course file (.json) to `My Documents\Rockstar Games\GTA V\ModSettings`.


## 4. Shortcuts

### 4.1 Function keys

| Shortcut | Description  | Action                                |
| :------- | :----------- | :------------------------------------ |
| F5       | GTBikeV menu | Open GTBikeV menu                     |
| F11      | Debug menu   | Display debug information for GTBikeV |

### 4.2 Keyboard keys

| Shortcut | Description       | Action                |
| :------- | :---------------- | :-------------------- |
| S        | Brake             | Use breaks            |
| V        | First person view | Toggles between views |

### 4.3 Numpad keys

| Shortcut | Description                         | Action                                                    |
| :------- | :---------------------------------- | :-------------------------------------------------------- |
| 1        | Auto Steering On/Off                | Toggles autosteering without needing to get into the menu |
| 4        | Smooth Steering Left                | Smooth steering with keys Numpad 4 and Numpad 6           |
| 6        | Smooth Steering Right               | Smooth steering with keys Numpad 4 and Numpad 6           |
| 7        | Activate Radio / Skip Radio Station | Activate radio resp. skip radio station when turned on    |


## 5. Troubleshooting

### 5.1 Connection Issue

Please use the following steps as guideline for troubleshooting connection issue:

1. Verify [hardware requirements](#21-hardware-requirements)
2. Verify [software requirements](#22-software-requirements)
3. Run GTA V in `Story Mode` and complete `The Prologue`
4. Press key `F5` and verify if `GTBikeV` mod menu is shown
5. Press key `F11` and verify (in top right window) that your smart bike trainer is connected


## 6. Credits

Credits go to the following people (in no order):

* Nestor Matas for developing GT Bike V
* Alexander Blade for developing ScripthookV
* Crosire for developing ScripHooktVDotnet
* Guad for developing NativeUI
* All others who have helped build this into a vibrant, active community


## 7. Contributors

This documentation would not be possible without the people who are contributing (in alphabetical order):

* Matthias Urech
* Nestor Matas
