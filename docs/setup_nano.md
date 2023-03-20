# Setup for Tang Nano 20K  :mushroom:

The main feature of 0.5 is standalone operation without tethering to a PC. To have a **standalone NESTang**, you need these,

* The Tang Nano 20K board.
* Two playstation 2 controllers, wired or wireless.
* A pair of Sipeed ps2 adapters.
* A MicroSD card for holding ROMS.

Once you have these, set your build up as follows,

* Connect the controller adapters to pin 15-20 of both sides of the board (see [schematics](https://dl.sipeed.com/shareURL/TANG/Nano_20K/2_Schematic) if you are not sure). Then connect the controllers.
* HDMI connection to a monitor or TV.
* Program [NESTang 0.5](https://github.com/nand2mario/nestang/releases) to the board with [openFPGALoader](https://github.com/trabucayre/openFPGALoader) or Gowin programmer.
* Use `tools/nes2img.py` python program to convert .nes ROM files to an .img file. This script requires Python >=3.7 and needs the Pillow package (install with `pip3 install pillow`).  Then burn that image to the sd card with any sd tool (e.g. [Balena Etcher](https://www.balena.io/etcher)) or `dd` under Linux or Mac.
* Insert MicroSD and power up the board, and enjoy your game!

