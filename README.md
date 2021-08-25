# B560-i5-11600

OpenCore config for my Rocket Lake desktop containing:

* ASUS prime B560-PLUS 
* i5 11600
* radeon rx 460
* Samsung 980 pro NVMe drive (Linux)
* Samsung 850 EVO 500 GB (Linux)
* Samsung 850 EVO 250 GB (macOS)
* 32 GB corsair DDR4-3200 RAM

Working:
* the machine boots, and show both displays
* accelerated graphics with native AMD driver
* sound works with alcid 69
* on board ethernet (intel) works
* some USB ports work, not all
* video acceleration (rocket lake iGPU not supported)
* sleep/resume with following pmset options:
```
➜  ~ sudo pmset -g
System-wide power settings:
Currently in use:
 standby              0
 Sleep On Power Button 1
 womp                 1
 hibernatefile        /var/vm/sleepimage
 proximitywake        0
 powernap             0
 networkoversleep     0
 disksleep            10
 standbydelayhigh     86400
 sleep                1 (sleep prevented by UserEventAgent)
 autopoweroffdelay    259200
 hibernatemode        0
 autopoweroff         0
 ttyskeepawake        1
 displaysleep         10
 tcpkeepalive         0
 highstandbythreshold 50
 standbydelaylow      86400
```

What doesn't work:
* some USB ports

Initial config based on : https://www.tonymacx86.com/threads/utterdisbeliefs-comet-lake-itx-asrock-b560m-itx-ac-i3-10320-32gb-ddr4-gt710-2gb.312443/
