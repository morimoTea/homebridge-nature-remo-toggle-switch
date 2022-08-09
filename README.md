# homebridge-nature-remo-toggle-switch
## About
Homebridge plugin to control toggle switches using Nature Remo.

## Example config.json
```json
  "accessories": [
    {
      "name": "[Name of Switch]",
      "access_token": "[Your access token of Nature Remo Cloud API]",
      "signal_ID": "[ID of switch's signal]",
      "accessory": "NatureRemoToggleSwitch"
    }
  ]
```