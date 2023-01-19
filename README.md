# ComponentTester

[![forthebadge](https://forthebadge.com/images/badges/powered-by-electricity.svg)](https://forthebadge.com)
[![forthebadge](https://forthebadge.com/images/badges/0-percent-optimized.svg)](https://forthebadge.com)
[![forthebadge](https://forthebadge.com/images/badges/made-with-crayons.svg)](https://forthebadge.com)

My attempt to modify [Karl-Heinz Kübbeler's AVR Transistortester](https://www.mikrocontroller.net/articles/AVR_Transistortester) for more accurate and faster component measurements. In the future hopefully with the possibility of measuring, controlling and identifying ICs. For now I will use the Karl-Heinz Kübbeler design, scaled to 24 test points, with at least 12 bits sampling resolution.

You can also see the hardware related files (schematic, PCB layout...) at [https://cadlab.io](https://cadlab.io/projects/componenttester).

I will try to stick to the [CERN Open Hardware License Version 2 - Strongly Reciprocal User Guide](https://ohwr.org/project/cernohl/wikis/uploads/cf37727497ca2b5295a7ab83a40fcf5a/cern_ohl_s_v2_user_guide.pdf), but since I'm new to Open Hardware, that's not necessarily the rule. So please feel free to point out any deviations or errors to me.

## Repository Contents

* __/Hardware:__ The schematic and PCB layout can be found here. I will also add exported files (PDFs...) there. For now, this project uses `Autodesk EAGLE`, but I may switch to `KiCad` when I get familiar enough with it.  
* __/Firmware:__ The source code of the tester will be here. __WIP__  
* __/Documentation:__ Resources with hardware and software documentation can be found here.  
* __/Software:__ Hopefully one day it will be possible to connect this tester to a computer and use the software in this directory for more complex testing. __WIP__  

## Documentation Overview

[Hardware related](docs/Hardware.md)  
[Contribution guidelines for this project](docs/CONTRIBUTING.md)

---

### Software License

[GNU General Public License v3.0](LICENSE)

### Hardware License

[CERN Open Hardware Licence Version 2 - Strongly Reciprocal](LICENSE_HARDWARE)

### Documentation License

TODO: Add Docs license
