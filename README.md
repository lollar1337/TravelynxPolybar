# TravelynxPolybar
a Module to view your Travelynx Status and notify about Delay/Next Stops


![Screenshot of the Module](https://github.com/thisjade/TravelynxPolybar/blob/a23dded24a06bc404cd4cc1612f4d148e369ce99/checked_in.png "Screenshot")


![Screenshot of the Module](https://github.com/thisjade/TravelynxPolybar/blob/a23dded24a06bc404cd4cc1612f4d148e369ce99/not_checked_in.png "Screenshot")


![Screenshot of the Module](https://github.com/thisjade/TravelynxPolybar/blob/a23dded24a06bc404cd4cc1612f4d148e369ce99/delay_notification.png "Screenshot")


## Dependencies

* You need curl installed and a API Key from your Travelynx.de Account.


## Module

```ini
[module/train]
type = custom/script
exec = ~/.config/polybar/train.sh
tail = true
```
