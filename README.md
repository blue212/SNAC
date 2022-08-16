# SNAC
Accessory converter for MiSTer


Serial Native Accessory Converter

SNAC is general purpose level shifter for use with MiSTer. It can be used to power 5v devices and it will safely convert any logic between the 3v3(MiSTer) and 5 device. It will be used mostly for 5v controllers and other peripherals.

The SNAC connects to the User port(formerly Serial I/O port) of the IO board on Mister. I recommend a male to female usb3 extension cable between them.

The SNAC is available in 2 versions the only difference being the connector on the controller side(USB3 or HDMI). Various adapters can then be plugged into that connector. I made various adapter PCBs for use with the USB3 verrsion.

Becasue the SNAC connects to the User port the peripheral connects to the GPIO of the MiSTer, this bypasses all layers the normal usb controllers use. So it's very much like having a controller port for the original system. One benefit of this is that most weird peripherals should work with their cores(like Lightguns etc) which most normal usb converters either don't or can't do. One downside to bypassing the layers is the you can't controle the OSD.

*A mod to the older IO boards is needed if you want to use SEGA peripherals. Analog IO board 6.1 and Digital 1.2 fix this issue and have a jumper near USER port that needs to be set to io6 .

-TODO detail the needed mod

-Updates

Changed the partslist to use a different part for the male USB connector.

Uxcell a19032000ux0260 instead of Wuerth 692112030100

Addded Mini version of the hdmi and USB3 snac boards.
