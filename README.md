Wipe Device

----------------------------------------------
Kenneth Thompson

Bash script to erase a device using three passes.

- Pass 1: zero out the device using /dev/zero
- Pass 2: write random numbers to the device using /dev/urandom
- Pass 3: zero out the drive again using /dev/zero

** I make no guarantee about the effectiveness of this utility! **

For the main device this script can be run from a Live Linux ISO.
The device will usually be /dev/sda

This should not be run on SSDs if you're planning on reusing the drive. Zeroing
out an SSD will degrade performance. Use [hdparm]("https://ata.wiki.kernel.org/index.php/ATA_Secure_Erase")
