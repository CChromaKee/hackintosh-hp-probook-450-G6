# HP Probook 450 G6 Hackintosh
My OpenCore config for the HP Probook 450 G6, Tested with Catalina and BigSur. 
![Screenshot](https://preview.redd.it/ef9zaiqjy4p71.png?width=1366&format=png&auto=webp&s=a4f4f0473a0866d5fccdd3be49b52b8eca415504)
# Hardware Info

- CPU: Intel Core i5-8265U (Coffee Lake)
- GPU: Intel UHD Graphics 620 (Whiskey Lake-U) 
- GPU: NVIDIA MX130 (Disabled)
- Audio Codec: ALC236
- Ethernet Card: RTL8111/8168/8411 PCI Express Gigabit Ethernet Controller
- WiFi/BT Card: Intel Dual Band Wireless-AC 9560 (With BT)
- Touchpad: Synaptics I2C touchpad
- BIOS Revision: R71
- OpenCore Version: 0.7.2

# What works

- Sound Output (Speakers, 3.5mm jack)
- Bluetooth
- Wi-Fi
- Ethernet
- Webcam
- Graphics

# What doesn't work (Not yet at least)

- HDMI
- Card Reader
- USB 3.0 Port #2 (Closest to the headphone jack)
- Fingerprint
- Brightness Keys (Currently bound to FN+C and FN+RSHIFT)

# Known Issues

- Lid switch internally mapped to brighness down (Only sometimes triggers though)
- Trackpad is a bit finicky
- Battery indicator displays percentage properly, but always reports as low when not on charge (Catalina only)
- Loading AirportItlwm on boot does not work (Catalina only)

# SMBIOS

- MacBookPro15,1

# Notes

- You will need to [generate your own smbios](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/coffee-lake.html#platforminfo), as well as replace [AirportItlwm](https://github.com/OpenIntelWireless/itlwm/releases/tag/v2.0.0) with the version that matches the version of MacOS you are trying to install.


