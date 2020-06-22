# lovelace-xiaomi-purifier
Xiaomi Purifier lovelace card with css animation

## Extra Features
1. compact view to show temperature and humidity 
1. button to turn on/off buzzer
1. double click to swith led 
1. hold "Favorite" button to adjust fan speed


## HACS Installation
1. HACS -> Settings -> Add custom repository <-> Plugin
2. Find 'xiaomi purifier' in HACS Plugins
3. Install and add to Lovelace

## Manual Installation
1. Download `xiaomi-purifier.js` to `www/plugins/xiaomi-purifier.js`
1. Add to lovelace resources
   ``` yaml
   resources:
    - url: /local/plugins/xiaomi-purifier.js
      type: js
   ```
## Add lovelace card 
  ``` yaml
  type: 'custom:xiaomi-purifier'
  entity: fan.anyid
  title: name of the purifier device
  advanced: #optional (true for showing temperature and humidity in the middle, otherwise shows in green panel)
  ```
  
### Language 
Displays English texts by default, for Chinese language users, add 
```
language: chs
``` 
to card configuration for displaying texts in Chinese.

Add translations to get your own language support. 
``` 
translate: 
   'Good': '优',
   'Moderate': '良',
   'Mild Unhealthy':'轻度污染',
   'Unhealthy': '中度污染',
   'Very Unhealthy': '重度污染',
   'Hazardous': '严重污染',

   'Air Purifier': '空气净化器',

   'On': '开启',
   'Off': '关闭',

   'Set speed': '设置速度',
   'Device turned on': '开启设备',
   'Device turned off': '关闭设备',
   'Indoor AQ': '室内空气',

   'Auto': '自动',
   'Silent': '睡眠',
   'Favorite':'最爱',

   'Temperature': '温度',
   'Humidity': '湿度'

```


## Credits
[shaonianzhentan](https://github.com/shaonianzhentan/lovelace-air-filter) (Original Author)
