# The opencore EFI for Asrock deskmini H470

## Gears
CPU: Intel core i9 10900es QTB1
RAM: Corsair DDR4-3000 16GBx2
SSD: Western Digital SN550 1T
WIFI/BT: BCM94360CS2
CPU cooler: NOCTUA NH L9i Fan

## Hackintosh
1. HDMI has no audio output.
2. wifi and bluetooth is fine.
3. AirDrop is fine.
4. Audio output from front headphone port is fine.
5. Microphone is not tested.
4. DP output not tested.
7. USB ports are customized.
5. Sleep/Wake is working after change below
    * add boot-args: igfxonln=1 (if hdmi can not wake)
    * sudo pmset -a hibernatemode 0
    * sudo pmset autopoweroff 0
    * sudo pmset powernap 0
    * sudo pmset standby 0
    * sudo pmset proximitywake 0
6. SMBIOS iMac20,2 will hide the bluetooth, so changed to iMac20,1

## Warning
⚠️Change the SMBIOS in config.list-PlatformInfo-SerialNumber,UUID,MLB,etc., or iService will not be working.

## Next
Save money to buy MacBook M1.
