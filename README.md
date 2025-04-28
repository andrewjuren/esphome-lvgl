Modified from: https://github.com/jtenniswood/esphome-lvgl/
Add this code to esphome to install

```
# ESP32-S3-Touch-LCD-7
substitutions:
  name: "main-panel"
  friendly_name: "Main Panel"
  room: "Main Entrance"

# Wifi Setup
wifi:
  ssid: !secret wifi_ssid
  password: !secret wifi_password

# Packages
packages:
  setup:
    url: https://github.com/andrewjuren/esphome-lvgl/
    files: [device/esp32-s3-touch-lcd-7.yaml,
            addon/time.yaml,
            addon/backlight.yaml,
            addon/network.yaml,
            assets/fonts.yaml,
            assets/icons.yaml,
            assets/images.yaml,
            theme/button.yaml,
            office/sensors.yaml,
            office/lvgl.yaml]
    refresh: 1sec
```
