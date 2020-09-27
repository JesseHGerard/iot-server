# IOT Server

### You will Need

- Raspbery Pi 4 (tested with 4gb ram model)
- SD card may be necessary for bootloader upgrade
- SSD drive (test with 120 gb sata SSD in a USB 3 case)

## Preparing the Device

Follow this tutorial to update bootloader and prepare boot files: https://medium.com/@zsmahi/make-ubuntu-server-20-04-boot-from-an-ssd-on-raspberry-pi-4-33f15c66acd4

Connect to wifi (optional if using ethernet):
https://ubuntu.com/tutorials/how-to-install-ubuntu-on-your-raspberry-pi#3-wifi-or-ethernet

- in ssd, add network to `network-config`
  ````yaml
  wifis:
    wlan0:
    dhcp4: true
      optional: true
      access-points:
        "<wifi network name>":
        password: "<wifi password>"
    ```
  ````
  Not exactly sure which thing worked:

* https://raspberrypi.stackexchange.com/questions/111722/rpi-4-running-ubuntu-server-20-04-cant-connect-to-wifi
* https://linuxconfig.org/ubuntu-20-04-connect-to-wifi-from-command-line
* https://medium.com/@huobur/how-to-setup-wifi-on-raspberry-pi-4-with-ubuntu-20-04-lts-64-bit-arm-server-ceb02303e49b
