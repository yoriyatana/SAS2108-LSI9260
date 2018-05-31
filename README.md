# SAS2108-LSI9260
SAS2108 (LSI 9260) based firmware files

LSI 9260 based controller Firmware page.

Here all the latest LSI SAS2108 based FW can be found.

It includes FW from LSI, IBM, Dell, Oracle, SuperMicro, Fujitsu and Intel.

[sas2108](https://drive.google.com/open?id=1gmBCkyYrGQbInOof3BMi3aROA9zU7o9r "Google Drive")

How to flash the SAS2108 based cards:

Make a bootable DOS USB disk (Google it)

Place the above files on the USB

Boot to USB

Megarec -cleanflash 0 (0 = if only one LSI card in computer, you'll need to work out which number to flash if more than one)

Reboot to USB

Megarec -m0flash 0 0xxx_yyy.rom (xxx= version number, yyy= OEM version)

Megarec -writesbr 0 sbrzzzzz.bin (zzzzz= Card type you are trying to flash to, only really needed with M5014/5015)

Reboot

Done

Latest BIOS from Firmware Package 12.12.0-0124

[BIOS 3.25.00_4.12.05.00_0x05180000.00 7/25/20](https://github.com/yoriyatana/SAS2108-LSI9260/blob/master/0124_bio.rom)



Use Megarec or Megacli or MSM to flash to controller, nothing else will be updated only BIOS


## Source

* https://forums.laptopvideo2go.com/topic/29166-sas2108-lsi-9260-based-firmware-files/
