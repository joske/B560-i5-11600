# B560-i5-11600

OpenCore config for my Rocket Lake desktop containing:

* ASUS prime B560-PLUS 
* i5 11600 + be quiet! Shadow Rock 3 cooler
* be quiet! Pure Power 11 500W
* AMD Radeon rx 460
* Samsung 980 pro NVMe drive (Linux)
* Samsung 850 EVO 500 GB (GhostBSD)
* Samsung 850 EVO 250 GB (macOS)
* Kingston 128 GB (win 10)
* 32 GB corsair DDR4-3200 RAM
* ASUS DRW-24D5MT
* be quiet! PURE BASE 600 case

Working:
* the machine boots, and show both displays
* accelerated graphics with native AMD driver (with the rx460 - rocket lake iGPU not supported)
* external sound works with alcid 69 (USB audio, HDMI/DP audio). Sees the internal audio device, but does not seem to output any sound and all apps using sound with that device selected are getting stuck
* on board ethernet (intel) works
* all USB ports work
* appletv+ playback with shikigva=128
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

Quirk:
* DVD player clicks every 7 minutes or so - seems to be known issue

What doesn't work:
* audio out of internal jack - does not matter, using USB audio directly to my Kanto TUK speakers

Initial config based on : https://www.tonymacx86.com/threads/utterdisbeliefs-comet-lake-itx-asrock-b560m-itx-ac-i3-10320-32gb-ddr4-gt710-2gb.312443/
