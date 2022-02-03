# Script: battery-combined-ramp-udev

A shell script that shows the battery status. This is an extended version of [battery-combined-udev](https://github.com/polybar/polybar-scripts/tree/master/polybar-scripts/battery-combined-udev).

It supports two rechargeable batteries and changing icons. It works even if only one battery is used.

This script is able to display power supply changes in real time. For this udev is being used.

I added a loop that shows a set of differnt icons when charging your device.


## Configuration

Copy `95-battery.rules` to `/etc/udev/rules.d/95-battery.rules`. Make sure that the paths in the file have been modified properly.


## Module

```ini
[module/battery-combined-udev]
type = custom/script
exec = ~/polybar-scripts/battery-combined-ramp-udev.sh
tail = true
```

