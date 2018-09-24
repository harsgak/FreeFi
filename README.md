# FreeFi
A little application for sharing internet connection over WiFi.

## How it works?
This little app uses windows 'netsh wlan' commands to identify support for hosted networks (hotspots) and
create + control state of hosted network (hotspot).

Prior to `Windows 10 version 1607` hotspot feature was not made available for use directly in `Windows`. Without resorting to the command line, setting up a hotspot for sharing internet was not possible in these earlier versions of Windows 10 and for Windows 7,8. This application was created to address this lack of an easy hotspot setting.    




## Usage

### First time Setting up

1. Run **FreeFi.exe** and if UAC window pops up select allow.
2. Follow instructions on screen to set wifi *name* and *password*.

3. In lan/ethernet settings turn on internet sharing for ethernet/your internet source network.  
  See [Troubleshooting - Error 3](#troubleshooting)

### REGULAR USE

* Use **Hotspot_on_off.exe** as on/off switch.

About  *Hotspot_on_off.exe*
* It is a toggle (on/off) switch. 
* If hotspot is currently ***on*** it will turn wifi sharing(hotspot) ***off***.
* If hotspot is currently ***off*** it will turn wifi sharing(hotspot) ***on***.



^Tricks:
Pin it to the taskbar for one click access.

## Troubleshooting


**Error 1-** "The wireless local area network interface is powered down and doesn't support the requested operation"  
**Cause**    : Self explanatory  
**Solution** : Switch on your damn wifi. How else you gonna share?!


**Error 2-** "The wireless local area network interface is currently not in a state to perform that operation"  
**Cause**    : Its state most probably is OFF.  
**Solution** : Switch on your damn wifi. How else you gonna share?


**Error 3-**  Connected to FreeFi but no internet on mobile.  
**Cause 1**  : Havent followed step 3 in [Setting Up](#first-time-setting-up)  
**Solution** : (For --Windows 8/8.1/10--)  
  1. Switch Hotspot onn
  2. Goto "Network Connections"
  3. Right click on Ethernet and click on Properties
  4. Under Sharing tab click "Allow other network users to connect" checkbox (to tick it)
  5. Set Home networking connection to "Local Area Connection* xx" (The one corresponding to your Hotspot name)
    If it is already set ,repeat 4,5.

**Cause 2**  :Your Antivirus' firewall is not letting mobile devices to connect to internet through PC. Some antivirus or firewall software may do this by default.  
**Solution** :Toggle "Block internet sharing"  off. Exact wording depends on the firewall software.

## Status
[![Project Status: Inactive – The project has reached a stable, usable state but is no longer being actively developed; support/maintenance will be provided as time allows.](https://www.repostatus.org/badges/latest/inactive.svg)](https://www.repostatus.org/#inactive)

Project Status: Inactive – The project has reached a stable, usable state but is no longer being actively developed; support/maintenance will be provided as time allows
