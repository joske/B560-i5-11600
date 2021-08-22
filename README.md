# B560-i5-11600

OpenCore config for my Rocket Lake desktop containing:

* ASUS prime B560-PLUS 
* i5 11600
* Samsung 980 pro NVMe drive (Linux)
* Samsung 850 EVO 500 GB (Linux)
* Samsung 850 EVO 250 GB (macOS)
* 32 GB corsair DDR4-3200 RAM

At the moment:
* the machine boots, and show both displays (but only mirrored - iGPU)
* sound works with alcid 69
* on board ethernet (intel) works
* some USB ports work, not all

What doesn't work:
* video acceleration (rocket lake iGPU not supported)
* sleep/resume

Initial config based on : https://www.tonymacx86.com/threads/utterdisbeliefs-comet-lake-itx-asrock-b560m-itx-ac-i3-10320-32gb-ddr4-gt710-2gb.312443/
