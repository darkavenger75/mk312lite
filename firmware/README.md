# MK312-BT Firmware

1. Set fuses for external 8 MHz crystal:
   
   avrdude -c usbasp-clone -p m16 -U lfuse:w:0xFF:m -U hfuse:w:0xD9:m
   
2. Flash any of the two firmware files, e.g. by

   avrdude -c usbasp-clone -p m16 -U "flash:w:HelloFriend.bin"
