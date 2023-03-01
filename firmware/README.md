# MK312-BT Firmware

1. We are using an external 8mhz crystal instead of the internal RC
   oscillator that the original uses. We need to set the fuses to
   enable this. 
   - LOW FUSE: 0xFF 
   - HIGH FUSE: 0xDC
   
   avrdude -c usbasp-clone -p m16 -U lfuse:w:0xFF:m -U hfuse:w:0xDC:m
   
2. Flash any of the two firmware files, e.g. by

   avrdude -c usbasp-clone -p m16 -U "flash:w:HelloFriend.bin"
