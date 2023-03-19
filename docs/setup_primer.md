# Setup for Tang Primer 20K

If you have Tang Primer 20K instead (get the nano if you don't have any board). Then here's what you need.

* Sipeed Tang Primer 20K (starting at $30).
* Muse-Lab HDMI PMod if you got the lite version of Tang: [aliexpress](https://www.aliexpress.com/item/3256804122775243.html) or [taobao](https://item.taobao.com/item.htm?id=671021594308). The dock version already has HDMI so you are fine. [Wiring instructions](/wiring) for lite version.

Here are the steps to set up NESTang，

* Download [NESTang 0.4](https://github.com/nand2mario/nestang/releases/tag/v0.4).
* Start **Gowin Programmer**, and program `nestang-lite.fs` or `nestang-dock.fs` depending on which board you have. If you see a colorful NES palette, then your setup is working. 
* Connect your game controller/controllers to your PC. I use a pair of old Xbox 360 controllers.
* Run `loader.exe -c COM4 games\rom.nes` (replace COM4 with your port number) to load the game `rom.nes` and run it. If it complains about missing DLLs, install [Microsoft Visual C++ Redistributable package](https://aka.ms/vs/17/release/vc_redist.x64.exe).
* Press the left button (LB) to call out the in-game OSD menu. There you can load other games in the `games` directory.
* If it didn't work, `loader.exe -r game.nes` will print messages from the core.

Now enjoy your game!

For 0.4, there's also a Linux loader program in addition to Windows. See [Linux loader](linux.md)
