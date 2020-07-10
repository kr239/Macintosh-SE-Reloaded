# Macintosh SE Reloaded

So many classic macs, starting with the SE, have died because of Apple's short sighted decision to add a battery to the board. This inevitably leaks and causes a horrific amount of damage. Luckily - most of the custom chips survive even this, so i decided to make a near 1:1 reproduction of the board, using Sprint Layout v6.0

Project inspired by Rob 'Peepo' Taylors work on the A500++ and the SixtyClone PCB's, which in turn were inspired by John 'Chucky' Hertell. 

# List of parts to save from the Macintosh SE Board

* **SIMM Sockets** - NEARLY IMPOSSIBLE TO GET. If you can get some from here: https://www.peconnectors.com/sockets-pga-cpu-and-memory/hws9229/ then do so! Re-using and cleaning up your old ones involves desoldering. These need a lot of heat as there are a lot of connections to the ground plane. Pre-heat the joints, maybe add a dab of proper Kester 63/37 eutectic LEADED solder (none of that RoHS crap), flood with flux. 
* **PDS Socket** - Amphenol/AMP/AVX DIN-41612 3-row, 96-pin connector (Style-C) - Available new, but still worth reclaiming as sifting through the minute variations of parts is an arse...
* **DB19 Connector** - NLA, only available as NoS or Reclaimed. These are a bastard to get out cause the lugs are soldered. I found that pre-heating the joint first, filled with flux, then pressing hard into the pad with the desoldering gun, waiting til you see the solder go molten, you can often schlorp out the majority of the solder and then tidy up with wick afterwards.
* **Main 14-pin Molex** - Molex P/N 39-28-1143 - Still available new - costs less than £2. Get a new one. 
* **Inductors** - probably easy enough to get new ones, but ehhh, they don't really break, and they fit fine. Reuse the big ones - buy new small axial ones.  
* **Passives** - **REPLACE ALL** - use high tolerance metal film resistors & nichicon or panasonic electrolytics. Maybe try and save the PLCC Socket if you can. remove it cleanly - sometimes the pins pull out but they can be put back in if you're careful. 
* **AM26LS30's** - NLA, only available as NoS or Reclaimed
* **AM26LS32's** - Available new, but still worth reclaiming
* **MC3488A** - NLA, only available as NoS or Reclaimed
* **Rockwell 338-6523 "VIA"** - NLA, only available as NoS or Reclaimed. Somewhat related to the 6522 Versatile Interface Adapter used in the Mac128k to Mac Plus. Compared to the 6522, the 6523 adds a third I/O port but does not include a timer, shift register or interrupt output.
* **RTC Chip** - Custom Chip - maybe possible to clone using pin-compatible ATTiny85
* **ADB Chip** - Apple branded PIC16CR54 - maybe possible to re-produce/clone
* **GLU Chip** - Apple branded PAL16L8 - maybe possible to re-produce/clone
* **BBU Chip** - Custom Chip
* **NCR5830/AM58C30 SCSI Chip** - NLA, only available as NoS or Reclaimed
* **WIM/SWIM Floppy Chip** - Custom Chip
* **Hi & Lo ROM Chips** - Toshiba TC531000CP MASK ROM's - Reclaim & reuse, but these are the same pinout as 27C512, but adds A16 in place of VPP pin - you can use 27C1001's on an adapter - doug brown made a similar setup with a built in ROM disk for the Mac Plus. 
* **74LS245** - Available new, but still worth reclaiming - replace with CY74FCT245ATPC or CD74FCT245E
* **74F257** - Available new, but still worth reclaiming - replace with CD74ACT257E

A full BOM is incoming. But for now, here, have a picture of the finished article...

![Finished Logic Board](/macse9.jpg)
