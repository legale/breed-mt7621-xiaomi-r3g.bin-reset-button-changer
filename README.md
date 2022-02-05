# Breed bootloader breed-mt7621-xiaomi-r3g.bin reset button patcher
## Description
This script purpose is to change the GPIO number of the reset button in the bootloader file BREED compiled for xiaomi mi router 3g.
Tested with breed versions r1338, r1286.

## Smartbox devices 
Reset Button - Device's
GPIO 7  - Beeline SmartBox PRO/WiFire S1500.NBN
GPIO 14 - Beeline SmartBox TURBO+/Beeline SmartBox TURBO/Etisalat Sercomm S3
GPIO 4  - Beeline SmartBox GIGA
GPIO 3  - Beeline SmartBox Flash/MTS WG430223

## Usage
To change reset GPIO number to 5:
```./breed_magic --src breed.bin --dst breed_mod.bin -r 5```

## Passed tests
This script was tested with breed-mt7621-xiaomi-r3g.bin versions: r1286, r1338
Patched binary for smartbox flash/giga/turbo/pro was tested on smartbox flash with boot breed from RAM.
```boot breed 0x80001000```
### Patching and testing video
Screen recording with the script patching demo and testing its launch on a real device 
https://raw.githubusercontent.com/legale/breed-mt7621-xiaomi-r3g.bin-reset-button-changer/main/demo.mp4


