# TravelynxPolybar
a Module to view your Travelynx Status and notify about Delay/Next Stops


![Screenshot of the Module](https://github.com/thisjade/TravelynxPolybar/blob/a23dded24a06bc404cd4cc1612f4d148e369ce99/checked_in.png "Screenshot")


![Screenshot of the Module](https://github.com/thisjade/TravelynxPolybar/blob/a23dded24a06bc404cd4cc1612f4d148e369ce99/not_checked_in.png "Screenshot")


![Screenshot of the Module](https://github.com/thisjade/TravelynxPolybar/blob/a23dded24a06bc404cd4cc1612f4d148e369ce99/delay_notification.png "Screenshot")


## Dependencies

* You need ```curl``` and ```jq```.

* Your API Key from [Travelynx](https://travelynx.de/).


## Module

```ini
[module/train]
type = custom/script
exec = ~/.config/polybar/train.sh
tail = true
```

## Options in train.sh

![Screenshot of the Module](https://github.com/thisjade/TravelynxPolybar/blob/8d8d950e8b6b1cdb807aebd3549ccb4b88596d8d/travelynx_needed_things.png "Screenshot")

Generate a API Key on the "Generieren/Generate" Button and then Copy the Part that is currently blurred out on my end.

```ini
API_KEY=
```
Set to "true" to receive Next Stop Notifications on every Step on your Journey, "false" will disable that.

```ini
NOTIFICATIONS_NEXT_STOP="true"
```

Set to "true" to receive Notifications about current Delays on your Journey, "false" will disable that.

```ini
NOTIFICATIONS_DELAY="true"
```

Set to "DE" to have the Module output everything in German, set to "EN" to have the Module output everything in English.

```ini
LANGUAGE="DE"
```

Set your Symbol for infront of the Text in Polybar, set "" for no Symbol. (Standard uses a Train Symbol from Googles Material Icons)

```ini
SYMBOL=""
```
