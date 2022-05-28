# i3blocks-apcups
i3blocks block script that displays APC UPS status

## Pre-requisites
You need to have apcupsd running. It does not have to be on your machine as long as the network port is available.
Configure it here (edit the script):
```
HOST = "127.0.0.1"
PORT = 3551
```

The symbols/icons are a mixture of emojis and Nerd Font glyphs.

## Config
```
[i3blocks-apcups]
markup=pango
interval=10
```

If you'd like, I also use the following i3 config for i3blocks:
```
bar {
    position top
    status_command i3blocks
    font pango:Sarasa Term SC Nerd Semibold 9
}
```

## Screenshots
Normal:
![alt text](https://github.com/amyeo/i3blocks-apcups/blob/master/normal.png?raw=true)

On Battery:
![alt text](https://github.com/amyeo/i3blocks-apcups/blob/master/batt.png?raw=true)

Short status output is also available.

## Keys
If you'd like you can edit the script to use any of the other available keys:
```
APC
DATE
MODEL
LINEV
LOADPCT
BCHARGE
TIMELEFT
MBATTCHG
MINTIMEL
MAXTIME
MAXLINEV
MINLINEV
OUTPUTV
DWAKE
DSHUTD
DLOWBATT
LOTRANS
HITRANS
RETPCT
ITEMP
ALARMDEL
BATTV
LINEFREQ
NUMXFERS
XONBATT
TONBATT
XOFFBATT
STESTI
STATFLAG
MANDATE
SERIALNO
BATTDATE
NOMOUTV
NOMBATTV
EXTBATTS
FIRMWARE
APC
```
