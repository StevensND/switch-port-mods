### DISCLAIMER:

If you don't understand something because you don't know English, translate the information using [Deepl](https://www.deepl.com/). It's a better translator compared to Google. Also keep in mind that I don't offer official support to solve your problems and I'm not a Yuzu developer. There are many people who think that by making a guide I must solve all your problems. This guide is totally voluntary. Remember to read [MaxLastBreath TOTK's Megathread](https://www.reddit.com/user/Maxlastbreath/comments/148o725/tears_of_the_kingdom_yuzu_setup_guide_60_fps_up/) as well as [MaxLastBreath's Bugs Megathread](https://www.reddit.com/user/Maxlastbreath/comments/148p4wh/yuzu_totk_bugmegathread/) instead.

### Hardware Requeriments:

Before you continue and waste your time or asking me or asking "X" person why the game doesn't run well, crashes etc etc I recommend you to check the [Yuzu FAQs](https://yuzu-emu.org/wiki/faq/) and the [hardware requeriments](https://yuzu-emu.org/help/quickstart/#hardware-requirements) just to see if your PC/laptop is compatible with Yuzu. This is something no one does and **you should bother to do it**. 

If you don't meet these requirements because your PC is old and you have bad specs (2 cores in your processor, 4GB RAM, integrated graphics, etc etc), **please don't continue**. Your PC is not powerful enough to emulate Nintendo Switch and you will be playing between 5-10 fps or even between 0 and 2 fps. Neither the Yuzu developers nor a better settings can work miracles in this case.

### Get Yuzu:

So ... The first thing we will do is to download Yuzu Mainline from [their Github](https://github.com/yuzu-emu/yuzu-mainline/releases) and not from their official website. Yuzu Mainline is the stable version of Yuzu. You'll see Yuzu Early Access (EA). This version it's the "beta version" of Yuzu Mainline. New features and updates will come first on Yuzu EA and once they're tested and working without issues they will be merged into Yuzu Mainline. So if you use Yuzu EA you may have stability issues.

This is a personal preference and I do it basically because sometimes Yuzu makes mistakes causing bugs and making some features of the emulator not to work as it should (as of today 11/22/2023 Yuzu Mainline 1627 and 1628 have bugs and don't save the settings properly). If you want to download a new version you will have to do it manually or look for an updater that is not the official from Yuzu and allows you to select which version you want to use since the installer on the official Yuzu website always forces you to update to the latest version.

Also by default Yuzu installs everything on your main hard drive in the Appdata folder, so if you don't have enough space this is a problem.

**For this guide I'm using [version 1626](https://github.com/yuzu-emu/yuzu-mainline/releases/tag/mainline-0-1626)** which doesn't have these problems. Download the next file: `yuzu-windows-msvc-20231119-197fc9df6.zip`

Once you have downloaded the Yuzu .zip file, create a folder wherever you want and extract the zip file into that folder. You should have something like the image below:

![imagen](https://i.imgur.com/orVDeBq.png)

### Making a portable Yuzu:

Now create a folder inside this path and name it `user` (In the image you will see that I have already created that folder). Run Yuzu.exe and the first thing you're going to do is go to: `File -> Open Yuzu Folder`.

The `user` folder will open and there will be some files inside. If this is the first time you are using Yuzu ignore the following steps:

**If you have already installed Yuzu using the installer from the official website**, press Windows R on your keyboard and type `%appdata%`.

This will open the `AppData\Roaming` folder. Locate the Yuzu folder and open it. Locate the [following folders](https://i.imgur.com/NYP0DCp.png). Delete the previous folders from `user` folder. Now copy and paste the folders from Appdata into the `user` folder that you created before.

By creating the `user` folder we will be making a portable Yuzu installation (this will avoid the above mentioned issues and will allow us to have more than 1 version of Yuzu).

### Installing Yuzu for the first time: 

Now ... if you are installing Yuzu for the first time, go to: `File -> Open Yuzu Folder` and open the `keys` folder and paste your `prod.keys` there. **Don't ask me where to get them**. Here is a [guide on how you can dump them](https://yuzu-emu.org/help/quickstart/#dumping-decryption-keys). If you don't have a Switch/a jailbreak Switch I'm sorry, you'll have to figure out how to get them yourself.  

The following step is not necessary but we will do it for games in which we are asked to have a Mii (like Mario Kart 8 Deluxe). We will go to `nand\system\Contents\registered` and we will paste there the .nca files of our firmware (I'm using Firmware 17.0.0). Again, I can't tell you where to get it.

Finally we will restart Yuzu and add our game directory (You will see a green cross with a text that says: Add New Game Directory). Click there, find the folder where you have your games and select it. **Don't ask where to get games**.

If some of your games don't appear, do the following: Right click on the path you have added and then click on `Scan subfolders`. If they still don't appear your prod.keys are wrong and you need to change them. Also, **make sure your games are in .nsp or .xci format**. Yuzu doesn't recognize any format other than these.

![imagen](https://i.imgur.com/xClcIjH.png)

### About DLCs + Update Install:

If you want to install a DLC or any update: Go to `File -> Install Files to NAND` and select the DLC or update that you want to install.

We will now continue with my personal settings.