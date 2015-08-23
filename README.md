Secure Device Wipe

----------------------------------------------
Kenneth Thompson

Bash script to erase a device using three passes.

- Pass 1: zero out the device using /dev/zero
- Pass 2: write random numbers to the device using /dev/urandom
- Pass 3: zero out the drive again using /dev/zero
