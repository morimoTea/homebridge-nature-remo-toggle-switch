# homebridge-nature-remo-toggle-switch
[Homebridge](https://github.com/homebridge/homebridge) plugin to control toggle switches using [Nature Remo](https://nature.global/nature-remo/).

## Installation
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
