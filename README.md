![alt text](https://github.com/Johnler/Wi-Ploit/blob/master/WifiExploit.jpg)
# Wi-Ploit 1.0.1
Wi-Ploit is a library of Wi-Fi exploitation tools.  
* Base code script of deltaflux Fluxion old version.
* For old Kali/ParrotOs version.

# (New Update)Wi-Ploit 2.0.0
Wi-Ploit is a library of Wi-Fi exploitation tools.
* Removes Python2 and dependecies.
** Pryit (disabled, waiting for python3 release).
* Updated Scripts.
* Tested on Kali (2020-05-12)

# Attacks:
1. Rogue Access Point (hostapd).  
2. Rogue Access Point (hostapd-mana).  
3. WPS attack (Reaver) * Upcoming.  

## Rogue Access Point (hostapd)
* Scan the networks.
* Capture a handshake (can't be used without a valid handshake, it's necessary to verify the password)
* Use WEB Interface *
* Launch a FakeAP instance to imitate the original access point
* Spawns a MDK3 process, which deauthenticates all users connected to the target network, so they can be lured to connect to the FakeAP and enter the WPA password.
* A fake DNS server is launched in order to capture all DNS requests and redirect them to the host running the script
* A captive portal is launched in order to serve a page, which prompts the user to enter their WPA password
* Each submitted password is verified by the handshake captured earlier
* The attack will automatically terminate, as soon as a correct password is submitted

## Rogue Access Point (hostapd-mana)
### attracting as many devices as possible to connect to perform MitM attacks.
* Scan the networks.
* Capture a handshake (can't be used without a valid handshake, it's necessary to verify the password)
* Use WEB Interface *
* Launch a FakeAP instance to imitate the original access point AND VICTIMS AUTOMATICALLY CONNECTS TO CREATED FAKEAP
* Spawns a MDK3 process, which deauthenticates all users connected to the target network, so they can be lured to connect to the FakeAP and enter the WPA password.
* A fake DNS server is launched in order to capture all DNS requests and redirect them to the host running the script
* A captive portal is launched in order to serve a page, which prompts the user to enter their WPA password
* Each submitted password is verified by the handshake captured earlier
* The attack will automatically terminate, as soon as a correct password is submitted

# Requirements
* Kali Linux OS or Ubuntu 18.04 OS
* External Wireless Adapters

## Recommended Wireless Adapters Chipsets
*Atheros:
ATH9KHTC (AR9271, AR7010)  
Tested: AR9271 (AWUS036NHA)

*Ralink:
RT3070

*Realtek:
RTL8192CU

# Installation
1. git clone https://github.com/Johnler/Wi-Ploit.git
2. cd Wi-Ploit/
3. chmod +x Installer
4. ./Installer
5. chmod +x wiploit
6. ./wiploit

# Versioning
1.b.c  
b = major release  
c = minor release

# Credits
1. vk496 - developer(s) of linset
2. deltaxflux - developer(s) of fluxion
3. SensePost - developer(s) of hostapd-mana



# Disclaimer
This is not responsibility of the developer(s) of any destructions, broken pc, illegal activities and nuclear war.
