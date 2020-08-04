A complete image of a *ready to go Raspi* can be downloaded this week - at first for a Raspberry Pi 4 (will support the link here - hopefully latest Aug 8, 2020), secondly for a Raspberry Pi Zero.

The (shrinked) size of the image is 7.9 GB (the compressed .gz size is 3.7 GB) which goes to a 16 GB SD-card (e.g. using the SW balanEtcher). On booting the Raspi the system will expand automatically for making full usage of the SD-card.

It contains an OS with all necessary uploads, file structures, a ramdisk, and a startup procedure for automatically entering into full operation.

Preconditions for the Raspi (Pi 4 and Pi Zero):
* Raspi-Cam V1 or V2 (or similiar) attached - Sdcam operation stops if there is no camera,
* two 1Wire-Temperature sensors (e.g. DS 1822) attached - Sdcam operation continues if there are no sensors, but there will be no Temperatur readings.

By using this image you:
1) prepare your 16 GB SD-card and boot the Raspi with it,
2) either operate headless - Raspi is awaiting the standard-WLAN (see docu), or operate with keyboard/HDMI monitor attached,
3) enter your SSID/password (WLAN),
4) adjust your parameter/info to the .cfg files (Partner station parameters as delivered by the organizers),
5) activate Sdcam launch on boot by uncomment last line of launcher.sh,
5) reboot and let the Raspi do the rest.
