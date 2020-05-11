# lovelace-xiaomi-purifier
Xiaomi Purifier lovelace card with css animation


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
  

## Credits
[shaonianzhentan](https://github.com/shaonianzhentan/lovelace-air-filter) (Original Author)
