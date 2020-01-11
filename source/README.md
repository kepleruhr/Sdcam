This directory contains the source- and configuration-files running the Raspi (Zero, V3, V4), Cam, and T-sensors.

## Preconditions for proper usage of these Python scripts:

### Once here there will be hints about the tested Raspian OS
### Python3, picamera- and PIL-libraries
```
  sudo apt-get install python3-picamera
  sudo apt-get install python3-pil
```
### Imply W1Terhmosens
```
sudo apt-get install python3-w1thermsensor
```
### Imply a RAM-disk
make a new directory
```
sudo mkdir /mnt/ramdisk
```
edit fstab-table at the end:
```
sudo nano /etc/fstab
  tmpfs /mnt/ramdisk tmpfs nodev,nosuid,size=50M 0 0
```
reboot and check for success
```
sudo reboot
df -h
```

## Store the scripts to the working directory
```
e.g. /home/pi/Sdcam
sundial.py, sdfun.py, sdfun2.py
```
