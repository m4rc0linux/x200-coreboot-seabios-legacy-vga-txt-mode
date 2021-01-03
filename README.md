# x200-coreboot-seabios-legacy-vga-txt-mode

coreboot 4.13 rom for thinkpad x200 featuring seabios v. 1.14.0 https://seabios.org/Releases#SeaBIOS_1.14.0
commit 5c186c6777c9438ff4681929c9c25c98dee28bef

it has been compiled to use libgfixnit graphics initialization with legacy vga txt-mode

ISSUE - descriptor and gbe present, however ethernet port is not recognized

Rom is 8mb, I could compile the 4 and 16mb as well for this model but
I own just a laptop and it has a 8mb chip so I will not be able to 
test roms for 4 or 16 mb chips

gbe.bin has been added with a random MAC address 00:11:22:33:44:55

No support to intel wifi and bluetooth

./cbfstool x200m4rc0.rom add-int -i 1000 -n etc/boot-menu-wait has been already applied to reduce the waiting time

added flashregion_0_flashdescriptor.bin from libreboot

ich9fdgbe_8m.bin with 00:11:22:33:44:55 mac address

No secondary payloads added

ISSUE - descriptor and gbe present, however ethernet port is not recognized
