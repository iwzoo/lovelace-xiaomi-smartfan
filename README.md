# Xiaomi Fan Lovelace Card
[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg)](https://github.com/custom-components/hacs)

Xiaomi Smartmi Fan Lovelace card for HASS/Home Assistant.

+  Supports [HACS](https://github.com/custom-components/hacs) installation
+  Works seamlessly with the [iwzoo/xiaomi_fan](https://github.com/iwzoo/xiaomi_fan) integration
+  Animations of the fan are made purely with CSS
+  Hold to adjust fan speed 
+  Hold to adjust oscillating angle (30, 60, 90, 120, 140) degrees
+  Translation for titles

## HACS Installation
Search for `Xiaomi Smartfan Card (Smartmi Fan 1x)`

## Manual Installation
1. Download `smartfan-xiaomi.js`
1. Copy to `www/plugins/lovelace-xiaomi-smartfan/xiaomi-smartfan.js`
1. Add the following to your Lovelace resources
    ``` yaml
    resources:
    - url: /local/lovelace-xiaomi-smartfan/xiaomi-smartfan.js
      type: js
    ```
1. Add the following to your Lovelace config `views.cards` key
    ```yaml
    - entity: fan.entity_id
      name: Fan Name
      type: 'custom:smartfan-xiaomi'
      translate: #optional for titles in any language
        Angle: 
        Child Lock:
        Natrual:
        Off:
        On:
        Oscillate:
        Speed Level:
        Timer:
    ```
    Replace `fan.entity_id` with your fan's entity_id and `Fan Name` with any name you'd like to name your fan with

## Preview
![](preview.gif)

## Credits
[fineemb](https://github.com/fineemb) (Original author)

[ikaruswill](https://github.com/ikaruswill/) (forked from)

[shaonianzhentan](https://github.com/shaonianzhentan/)

[花神](https://github.com/yaming116)
