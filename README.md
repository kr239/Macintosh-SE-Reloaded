# Macintosh SE Reloaded

![Finished Logic Board](/macseboard-final-rev16b-release.jpg)
![Finished Logic Board - Bottom](/macseboard-final-rev16b-release-rear.jpg)

**Latest version, v1.6 adds an A17 address pin next to **U2E**, a 74F257 to allow for potential ROM upgrades as the standard ROM sockets only allow A0 to A16 address lines.**

So many classic macs, starting with the SE, have died because of Apple's short sighted decision to add a battery to the board. This inevitably leaks and causes a horrific amount of damage. Luckily - most of the custom chips survive even this, so I decided to make a near 1:1 reproduction of the board, using Sprint Layout v6.0

Project inspired by Rob 'Peepo' Taylors work on the A500++ and the SixtyClone PCB's, which in turn were inspired by John 'Chucky' Hertell. 

Please note - this project is licensed under CC-BY-NC-SA - it is NOT for commercial use.

Only two vendors are licensed for commercial production. Maceffects (US) and Recapamac (Australia). 

If you wish to purchase a single, ready made board, I recommend purchasing from them direct. 

https://maceffects.com/products/macintosh-se-reloaded-logic-board

https://recapamac.com.au/shop/

# List of parts to save from the Macintosh SE Board

* **SIMM Sockets** - If you can get some from here: https://www.peconnectors.com/sockets-pga-cpu-and-memory/hws9229/ then do so! 
 
  Re-using and cleaning up your old ones involves desoldering. These need a lot of heat as there are a lot of connections to the ground plane. Pre-heat the joints, maybe add a dab of proper Kester 63/37 eutectic LEADED solder (none of that RoHS crap), flood with flux. 
* **PDS Socket** - Amphenol/AMP/AVX DIN-41612 3-row, 96-pin connector (Style-C) - Available new, but still worth reclaiming as sifting through the minute variations of parts is an arse...
* **DB19 Connector** - Almost NLA, only really available as NoS or Reclaimed. These are a bastard to get out cause the lugs are soldered. I found that pre-heating the joint first, filled with flux, then pressing hard into the pad with the desoldering gun, waiting til you see the solder go molten, you can often schlorp out the majority of the solder and then tidy up with wick afterwards. 
 
  NoS ones available from https://www.exxoshost.co.uk/atari/store2/ - search for **DB19F ASCI PCB RA POST**
* **Main 14-pin Molex** - Molex P/N 39-28-1143 - Still available new - costs less than £2. Get a new one. 
* **Inductors** - probably easy enough to get new ones, but ehhh, they don't really break, and they fit fine. Reuse the big ones - buy new small axial ones.  
* **Passives** - **REPLACE ALL** - use high tolerance metal film resistors & nichicon or panasonic electrolytics. Maybe try and save the PLCC Socket if you can. remove it cleanly - sometimes the pins pull out but they can be put back in if you're careful. 
* **AM26LS30's** - NLA, only available as NoS or Reclaimed
* **AM26LS32's** - Available new, but still worth reclaiming
* **MC3488A** - NLA - replace with Texas Instruments SN75150
* **Rockwell 338-6523** - This is identical to the 65C22N VIA, still available new
* **RTC Chip** - Custom Chip - this has been reverse engineered, see project here: https://github.com/pgreenland/attinyrtcmodule
* **ADB Chip** - Apple branded PIC16CR54 - this has been reverse engineered for the PIC16F88 by Tashtari: https://github.com/lampmerchant/macseadb88
* **GLU Chip** - Apple branded HAL16L8 - this has been reverse engineered for both GAL16V8 and discrete logic!
* **BBU Chip** - Custom Chip
* **SCC Chip** - Standard 85C30 Serial Communications controller - **NO LONGER AVAILABLE NEW AS OF 2024-06-01, officially discontinued by ZiLOG**
* **NCR5830/AM58C30 SCSI Chip** - NLA, only available as NoS or Reclaimed from UTSource
* **IWM/SWIM Floppy Chip** - Custom Chip - available NoS from UTSource
* **Hi & Lo ROM Chips** - Toshiba TC531000CP MASK ROM's - Reclaim & reuse, but these are the same pinout as 27C512, but adds A16 in place of VPP pin - you can use 27C010's on an adapter - doug brown made a similar setup with a built in ROM disk for the Mac Plus. 
* **74LS245** - Available new, but still worth reclaiming - replace with CY74FCT245ATPC or CD74FCT245E
* **74F257** - Available new, but still worth reclaiming - replace with CD74ACT257E

A full BOM is now available. 
