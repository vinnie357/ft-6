# ENV
I used a blank Hyper-V windows 10 machine

## software
- vscode
- chrome
- marlin2 (skr1_3)

## VS code
Plugins:
- ### PlatformIO IDE
requires python2.7


## base instructions:
https://www.dropbox.com/s/ppjfflhf3j5yzh2/MarlinV2.0%20SKRV1.1%20instruction.docx?dl=0

## skip the removal of the SD card, use SCP
- scp firmware.bin pi@orangepi:/media/sda1/firmware.bin
- scp -i ~/keys/ssh_pub_key firmware.bin user@orangepi:/media/sda1/firmware.bin

## reload/flash firmware after copy
https://github.com/MarlinFirmware/Marlin/pull/15209
M997

## addtional options:
- Servo Direction
  - INVERT_[x,y,x]_DIR
- End stops direction
  - [x,y,z]_HOME_DIR
- End Stops sensor
  - [x,y,z]_MIN_ENDSTOP_INVERTING
- Extruder servo direction
  - INVERT_E[1-5]_DIR
- Print area
  - [X,Y]_BED_SIZE
  - Z_MAX_POS
- Auto bed leveling
  - AUTO_BED_LEVELING_UBL
  - RESTORE_LEVELING_AFTER_G28
  - EEPROM_SETTINGS 
- inductive probe
  - FIX_MOUNTED_PROBE
  - Z_SAFE_HOMING

