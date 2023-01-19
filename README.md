# ComponentTester

[![forthebadge](https://forthebadge.com/images/badges/powered-by-electricity.svg)](https://forthebadge.com)
[![forthebadge](https://forthebadge.com/images/badges/0-percent-optimized.svg)](https://forthebadge.com)
[![forthebadge](https://forthebadge.com/images/badges/made-with-crayons.svg)](https://forthebadge.com)

My attempt to modify [Karl-Heinz Kübbeler's AVR Transistortester](https://www.mikrocontroller.net/articles/AVR_Transistortester) for more accurate and faster component measurements. In the future hopefully with the possibility of measuring, controlling and identifying ICs. For now I will use the Karl-Heinz Kübbeler design, scaled to 24 test points, with at least 12 bits sampling resolution.

You can also see the hardware related files (schematic, PCB layout...) at [https://cadlab.io](https://cadlab.io/projects/componenttester).

I will try to stick to the [CERN Open Hardware License Version 2 - Strongly Reciprocal User Guide](https://ohwr.org/project/cernohl/wikis/uploads/cf37727497ca2b5295a7ab83a40fcf5a/cern_ohl_s_v2_user_guide.pdf), but since I'm new to Open Hardware, that's not necessarily the rule. So please feel free to point out any deviations or errors to me.

## Goals and Expectations

My main goal is to keep the simplicity of the original design but add speed and accuracy, along with additional capabilities such as automated testing of components and parts. I plan on having a computer environment capable of communicating with the tester to easily add components to the database, define their limits and normal operating values. I also want to keep the price as low as possible, which will be more difficult given my requirements for the unit itself.

* [ ] Higher resolution ADC
  * At least a 12-bit ADC
* [ ] Some DAC
  * I'm not sure if I'll add it, but I'd sure like to have at least a couple of analog outputs. Some sort of 8-bit DAC might do the trick, no need for such a precise output anyway.
* [ ] Measure a wide variety of components
  * [ ] Resistors
  * [ ] Capacitors
  * [ ] Inductors
  * [ ] Diodes
    * [ ] Standard
    * [ ] Shottky
    * [ ] Zener
  * [ ] Transistors
    * [ ] BJT
      * [ ] PNP
      * [ ] NPN
    * [ ] FET
      * [ ] JFET
        * [ ] N-Channel
        * [ ] P-Channel
      * [ ] MosFET
        * [ ] N-Channel
        * [ ] P-Channel
  * [ ] Various
    * [ ] IGBT
    * [ ] Tyristor
    * [ ] TRIAC
    * [ ] Maybe even vacuum tube?
  * [ ] Up to 24-pin ICs with 5V or 3.3V logic
* [ ] Computer software
  * [ ] Print detailed test results
  * [ ] Specify test cases
  * [ ] Add ICs to DB
    * [ ] Add schematics to DB
    * [ ] Add diagrams to DB
    * [ ] Add normal operating values and limits of parts

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

Copyright Daniel Židek 2023.  
This source describes Open Hardware and is licensed under the CERNOHL-S v2.  
You may redistribute and modify this source and make products using it
under the terms of the [CERN-OHL-S v2](https://ohwr.org/cern_ohl_s_v2.txt).  
This source is distributed WITHOUT ANY EXPRESS OR IMPLIED
WARRANTY, INCLUDING OF MERCHANTABILITY, SATISFACTORY
QUALITY AND FITNESS FOR A PARTICULAR PURPOSE. Please see
the [CERN-OHL-S v2](https://ohwr.org/cern_ohl_s_v2.txt) for applicable conditions.  
Source location: https://github.com/Just-Danuse/ComponentTester  
As per CERN-OHL-S v2 section 4, should You produce hardware based
on this source, You must where practicable maintain the Source Location
visible on the external case of the ComponentTester or other products you make using
this source.
