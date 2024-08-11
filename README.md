# Command to flash the firmware

Run the following command to know serial port of that device is connected. Zigbee Dongle P will be /dev/ttyUSB0 (In most cases)
```
ls /dev/tty*
```

Format will be : -
```
sudo python3 cc2538-bsl.py -ewv -p /dev/ttyUSBx(Serial port that device is connected) --bootloader-sonoff-usb /home/pi/flash_router/CC1352P2_CC2652P_launchpad_router_20221102.hex(Location of the desir4ed firmware in the machine)
```

For instance ; To flash router firmware into Zigbee Dongle P

```
sudo python3 cc2538-bsl.py -ewv -p /dev/ttyUSB1 --bootloader-sonoff-usb /home/pi/flash_router/CC1352P2_CC2652P_launchpad_router_20221102.hex
```
