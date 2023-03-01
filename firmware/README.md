# MK312-BT Firmware

1. We are using an external 8mhz crystal instead of the internal RC
   oscillator that the original uses. We need to set the fuses to
   enable this. 
   - LOW FUSE: 0xFF 
   - HIGH FUSE: 0xDC
