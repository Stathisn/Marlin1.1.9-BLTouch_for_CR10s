# Marlin1.1.9-BLTouch_for_CR10s

Note: This is not my code, full credit goes to the developers at http://marlinfw.org/. I have merely configured and optimised this version for use with the Creality CR-10s printer with BLTouch ABL.

For wiring for the Creality v2.1 board, see image "CR-10s v2.1.jpg"

You will need to set probe offset for your printer. It is currently configured for BLTouch mounted on a Petsfang "Bullseye". If you have mounted yours in the same way, you will still need to calibrate your z-offset.

There are some minor modifications you will need to make in the Configuration.h file, see below:

780 #define X_PROBE_OFFSET_FROM_EXTRUDER -42  // X offset: -left  +right  [of the nozzle]
781 #define Y_PROBE_OFFSET_FROM_EXTRUDER -5  // Y offset: -front +behind [the nozzle]
782 #define Z_PROBE_OFFSET_FROM_EXTRUDER 0   // Z offset: -below +above  [the nozzle]

You may also want to update your printer name:
139 #define CUSTOM_MACHINE_NAME "CR-10s + BLTouch"


Happy printing!
