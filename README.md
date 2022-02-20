# TravelynxPolybar
a Module to view your Travelynx Status and notify about Delay/Next Stops

## Dependencies

* You need curl installed and a API Key from your Travelynx.de Account.


## Module

```ini
[module/train]
type = custom/script
exec = ~/.config/polybar/train.sh
tail = true
```
