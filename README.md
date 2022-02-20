# TravelynxPolybar
a Module to view your Travelynx Status and notify about Delay/Next Stops


![Screenshot of the Module](https://github.com/thisjade/TravelynxPolybar/blob/a23dded24a06bc404cd4cc1612f4d148e369ce99/checked_in.png "Screenshot")


![Screenshot of the Module](https://github.com/thisjade/TravelynxPolybar/blob/a23dded24a06bc404cd4cc1612f4d148e369ce99/not_checked_in.png "Screenshot")


![Screenshot of the Module](https://github.com/thisjade/TravelynxPolybar/blob/a23dded24a06bc404cd4cc1612f4d148e369ce99/delay_notification.png "Screenshot")


## Dependencies

* You need curl installed and a API Key from your Travelynx.de Account.

* You also need Googles Material Design Icons for the Train Symbol

[AUR](https://aur.archlinux.org/packages/ttf-material-design-icons-git)
```ini
https://aur.archlinux.org/packages/ttf-material-design-icons-git
```

[FREEBSD](https://pkg.freebsd.org/FreeBSD:13:amd64/latest/All/material-icons-ttf-5.0.1.pkg)
```ini
https://pkg.freebsd.org/FreeBSD:13:amd64/latest/All/material-icons-ttf-5.0.1.pkg
```

[UBUNTU](http://archive.ubuntu.com/ubuntu/pool/universe/f/fonts-material-design-icons-iconfont/fonts-material-design-icons-iconfont_5.0.1-2_all.deb)
```ini
http://archive.ubuntu.com/ubuntu/pool/universe/f/fonts-material-design-icons-iconfont/fonts-material-design-icons-iconfont_5.0.1-2_all.deb
```

[FEDORA](https://download-ib01.fedoraproject.org/pub/fedora/linux/development/rawhide/Everything/x86_64/os/Packages/m/material-icons-fonts-4.0.0-6.fc36.noarch.rpm)
```ini
https://download-ib01.fedoraproject.org/pub/fedora/linux/development/rawhide/Everything/x86_64/os/Packages/m/material-icons-fonts-4.0.0-6.fc36.noarch.rpm
```  
  

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

Set to "DE" to have the Module output everything in German, set to "EN" to have the Module output everything in English

```ini
LANGUAGE="DE"
```
