>[!NOTE]
The proper way to use these mods on emulator is to **Set the Resolution Scale to 1x (Native 720p/1080p)**.

This will make these mods native. Otherwise, if you set 2x, 3x etc etc, you will increase the resolution and FPS drops/bad perfomance might happen.

![image](https://i.gyazo.com/9bc4441face99be41cde9b3fdb4423f5.png)

![image](https://i.gyazo.com/068939ee1b1b4e6cbafae8205a962539.png)

## Notes if you're going to use 3840x2160 (4K) Mod

3840x2160 requires Extended memory layout for any emulator.

**For Ryujinx**: Go to `Options` and then click on `System`.

Enable the option of `Expand DRAM to 8GiB` or if you're using GreemDev/Keaton's Build click on `DRAM Size` and set it to 8GB.

![image](https://i.gyazo.com/91aa18b6f0c20ec163861c01ff037fd1.png)

**For Yuzu**: Go to `Emulation` and then click on `Configure`

Click the `System Tab` and again click on `System`. Set the `Memory Layout` to 8GB.

![image](https://i.gyazo.com/afee192dd95a19c18fccfb33d5027caf.png)

## ExeFS vs RomFS

When I first uploaded the mods, I talked about ExeFS vs RomFS mods.

In this game we used the traditional methods for resolution mods as well as resolution cheats and we compared it with a mod made in `RomFS` format.

Thanks to NineKain, Fl4sh and I noticed the following:

- RomFS quality was higly superior. 

This is due to the Screen Percentage was superior on RomFS compared to ExeFS.

Therefore, Fl4sh started to investigate and we had to find another way to make the mods, bringing the result closer to RomFS.

Finally, it could be done. However applying this to all games is complicated and time consuming (Fl4sh had to fix the HUD overlay ...) so depending on the game, opting for RomFS might be a better option if there is no other choice.

Below there's a comparison between old ExeFS mod / 1080p resolution cheat (left) before the fix vs RomFS (right)

![image](https://i.imgur.com/nuOgNIP.jpeg)

You can clearly see how one looks blurry and the other not ...

## If you're playing on Switch

You can use the 1080p mod. I uploaded the .IPS file converted.

If you want, you can compare a 1080p cheat vs this mod vs 1080p RomFS option.