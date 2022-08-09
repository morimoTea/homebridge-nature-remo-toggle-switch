# homebridge-nature-remo-toggle-switch
## About
Homebridge plugin to control toggle switches using Nature Remo.

## Installation
You can easily find this plugin by searching on "Plugins" tab of [Homebridge Config UI X](https://github.com/oznu/homebridge-config-ui-x).  
Or just run this command in terminal.
```bash
npm install -g homebridge-nature-remo-toggle-switch
```

## Example config.json
```json
  "accessories": [
    {
      "name": "Living Room's Light",
      "access_token": "[Your access_token]",
      "signal_ID": "xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
      "accessory": "NatureRemoToggleSwitch"
    }
  ]
```
- `name` can be set whatever you want
- To get `access_token`, visit https://home.nature.global/
- To get `signal_ID`, run `curl -X GET "https://api.nature.global/1/appliances" -H "Authorization: Bearer [access_token]"` and find `id` key
- `accessory` must be `NatureRemoToggleSwitch`