## Notes if you're going to 3840x2160 (4K) Mod

3840x2160 requires Extended memory layout for any emulator.

**For Ryujinx**: Go to `Options` and then click on `System`.

Enable the option of use Extend Memory Layout or if you're using GreemDev/Keaton's Build click on `DRAM Size` and set it to 8GB.

**For Yuzu**: Go to `Emulation` and then click on `Configure`

Click the `System Tab` and again click on `System`. Set the `Memory Layout` to 8GB.

## ExeFS vs RomFS

When I first uploaded the mods, I talked about ExeFS vs RomFS mods.

In this game we used the traditional methods for resolution mods as well as resolution cheats and we compared it with a mod made in `RomFS` format.

Thanks to NineKain, Fl4sh and I noticed the following:

- RomFS quality was higly superior. 

This is due to the Screen Percentage was superior on RomFS compared to ExeFS.

Therefore, Fl4sh started to investigate and we had to find another way to make the mods, bringing the result closer to RomFS.

Finally, it could be done. However applying this to all games is complicated and time consuming so depending on the game, opting for RomFS might be a better option if there is no other choice.

Below there's a comparison between ExeFS (left) before the fix vs RomFS (right)

![image](https://i.imgur.com/nuOgNIP.jpeg)

You can clearly see how one looks blurry and the other not ...

## If you're playing on Switch

You can use the 1080p mod. I uploaded the .IPS file converted.

If you want, you can compare a 1080p cheat vs this mod vs 1080p RomFS option.