LedClock-Resized
As its name tells, this is a resized and an easier to make version of @imeszaros ledclock project.

Main differences are:

all PCBs are under 100mm height so you can order them for like $5 + shipping.
3D printed parts can be printed on smaller printers because the base is split in half (you have to assemble it with some M3 screws and nuts). I printed my parts on an Ender3 V2, so I guess anyone can print them.
3D printed parts can be printed without supports. Please check 3mf folder to see orientation if you can't figure it out.
controller board, led 7segments and dots now uses only 0805 SMD components for easier soldering. I don't have a reflow hot-plate so I made the assembly by hand.
controller board now uses an "off the shelf" ESP32 D1 Mini [link for reference] for more convenience. By using an embedded ESP32 you will have to overcomplicate the board. Another reason for using a dedicated ESP32 D1 Mini was because some of the components required in the original design are impossible to solder by hand (CP2102). Just upload the firmware on the ESP32 Mini board and then plug it into the main controller board.
