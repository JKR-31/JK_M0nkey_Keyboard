Here are all the files needed to make the PCB of my Keyboard. In the newest version with all bugfixes added.
(Fixed issues 24.09.21: missing trace at encoder, pull-up instead off pull-down at USB chip, wrong holewidth for 6,25 stab)

Also there is the .zip file that I used for upload at my PCB manufacturer of choise: JLCPCB and a picture of the options I choose on there website.
I like JLC-PCB because you can get good quality PCBs for cheap (5x for ~30EUR).

For soldering i did everything by hand. For the USB- & ATMEL-Controller and the USB-C Connector i used a hot-air-gun with solderpaste. So that i have a good connection of the groundpads.
Everything else was soldered using a soldering iron with a small tip.
It's a lot of work and it took me 3 evenings to complete.
After you finish check for any brigged connections, in particular at the USB-C port (i had that problem and nothing worked)

Also soldering and testing in steps makes sense here. So first do the USB-Hub --> test it. Than do the microcontroller --> test it.

The USB-Hub-Controller should work after everything is soldered on. It doesn't need any programming. It should show up automatically on your PC.
This controller has to work, so that we can access the USB-Bootloader of the AT90USB646.

When the USB-HUB is recognised by your PC, look in the device manager if you see the USB-Bootloader show up.
Now you just need to upload the keyboard code as described on the QMK website for any other mechanical keyboard.

