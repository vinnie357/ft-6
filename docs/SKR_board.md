STEP 1:
INSTALLING THE STEPPER DRIVERS

Change jumpers under each stepper to look like the picture below:

![alt text][jumpers]

STEP 2 :
Install the MARLIN COM DRIVERS:
Driver: https://www.dropbox.com/s/a0k5idjmf4fn82f/lpc176x_usb_driver.inf?dl=0

STEP 3:
Install firmware
Place the firmware.bin file on the SD from the gdive for the kit and options you have:
https://drive.google.com/drive/folders/1ViILUwMNMFPJrsxo1Kwb7sst_un7l3P6?usp=sharing
Insert the SD card back into the SKR board, and cycle the power.
Note: the SKR board comes up as a mass storage drive and the firmware.bin can also be moved to the SD that way.

After the board is power cycled you will notice the file has been renamed to firmware.cur, this means the firmware has been uploaded successfully.

There is no need to compile the firmware yourself to get you printer going, but when you are ready to start tweaking and making mods this guide will help you:
https://www.dropbox.com/s/ppjfflhf3j5yzh2/MarlinV2.0%20SKRV1.1%20instruction.docx?dl=0




[jumpers]: ./images/skr_V1_3_jumpers.png "skr Jumpers"
