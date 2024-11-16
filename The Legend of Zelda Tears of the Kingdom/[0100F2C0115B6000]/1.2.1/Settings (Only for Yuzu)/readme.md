## VIDEO GUIDE

[VIDEO SHOWING THE SETTINGS HERE](https://youtu.be/EUnyMMIWcZU?si=DLYLdqJFP5TeAxdd)

I did this video showing my settings in real time if you want to see it too.

## DISCLAIMER

If you don't understand something because you don't know English, translate the information using [Deepl](https://www.deepl.com/). It's a better translator compared to Google. Also keep in mind that I don't offer official support to solve your problems and I'm not a Yuzu developer. There are many people who think that by making a guide I must solve all your problems. This guide is totally voluntary. Remember to read [MaxLastBreath TOTK's Megathread](https://www.reddit.com/user/Maxlastbreath/comments/148o725/tears_of_the_kingdom_yuzu_setup_guide_60_fps_up/) as well as [MaxLastBreath's Bugs Megathread](https://www.reddit.com/user/Maxlastbreath/comments/148p4wh/yuzu_totk_bugmegathread/) instead.

I have based my settings on this [TOTK-Mods-collection guide](https://github.com/hoverbike1/TOTK-Mods-collection/blob/main/SETUP.md#recommended-yuzu-system-setting). MaxLastBreath has a [TOTK Optimizer tool](https://github.com/MaxLastBreath/TOTK-mods/releases) that setup everything for you automatically although I personally don't like his tool (Sorry Max) and I prefer to setup everything myself manually. 

**My PC Specs are**: CPU: Ryzen 5600 (6 cores, 12 threads), GPU: GTX 1080 (8GB), RAM: 16GB 3600Mhz

## 02/22/2024 Update

If I remember correctly, this is the only change that is new in Yuzu's UI after I have written this guide so **keep it mind**. Below you can read the changelog about it:

<ins>**Mainline 1723 @Updates - PC**</ins>

- Added toggle to decide how much vram is allowed for games. Setting can be found in Graphic Advanced. [#13001]

  - <ins>**Conservative**</ins>: Allow 7 GB of vram at native resolution and allow more vram depending on the scaling value, the higher the more allowed. This will prevent Yuzu from slowing down when used with third party programs that require vram.
 
  - <ins>**Aggressive**</ins>: Allow to use 7/8 of available vram for games. It reduce stutter from cleaning vram consistently on games. Recommended when user has no other program that requires running, while using resolution mod without scaler and using very high resolution scaling of emulator.

I set it on `Conservative`. I think this is the Default option.

## Global Settings

Go to `Emulation -> Configure` and then go to `System`. Here just select your Language, Region and Time Zone. **Leave the other options as default**.

Then go to `CPU` and **leave it on** `Auto`. If you ever need to change this for any game, make a custom settings for that game. **Don't change it in the global settings**.

Now go to `Graphics`. Here select `Vulkan`. Vulkan is preferable to `OpenGL` as it has better performance. OpenGL is a rather old technology and nowadays most games use Vulkan. **Only change to OpenGL if you have issues** (I still recommend doing this by creating custom settings for the specific game you have problems with).

`ASTC Decoding Method: GPU`

`Vsync Mode: Mailbox (Recommended)`. I think this option is only for Nvidia Users. If you have ADM leave it on FIFO (Vsync ON).

`NVDEC Emulation: GPU Video Decoding (Default)`

Leave the other options as default although I change the `Resolution: 2X (1440p/2160p)`, `Windows Adapting Filter: Bicubic` and `Anti-Aliasing Method: SMAA` due to my PC can handle these settings.

You'll find more info about Windows Adaptating Filter [here](https://web.archive.org/web/20240304181558/https://yuzu-emu.org/entry/yuzu-art/)

**I don't understand the resolution I am selecting, could you explain?**: The first number (1440p) will be the Resolution that you will use if you're playing on Handheld. 2160p will be the Resolution that you will use if you're playing on Docked. I'm playing on Docked.

![imagen](https://i.imgur.com/YsxQNSl.png)

## Advanced Global Graphics Settings

![imagen](https://i.imgur.com/8U80pew.png)

## Custom TOTK Settings

We setup this by Right Click on the game and then click on Properties

![imagen](https://i.imgur.com/3XQ8e8B.png)

![imagen](https://i.imgur.com/A1uQXEH.png)

You can leave Memory Layout on 4GB DRAM (Default) too. Just test it. I wouldn't use a higher option at 4GB or 6GB. For 1440p you might want to use 6GB to avoid crashes. If you go above 4K, use 8GB.

![imagen](https://i.imgur.com/ZOoJMUH.png)

![imagen](https://i.imgur.com/Bvyd8G9.png)

In this section you can make some modifications and adapt them according to your needs:

`Accuracy Level`: You can leave it on High if you are having a lot of flickering.

`Anisotropic Filtering`: You can change it if you want. I leave it on Auto.

`ASTC Recompression Method`: Change this if your weapons, shields etc etc menu is lagging. This mighht help that. I set it on BC3 based on my GPU VRAM (8GB). Check [this section of the TOTK-Mods-Collection guide](https://github.com/hoverbike1/TOTK-Mods-collection/blob/main/SETUP.md#recommended-yuzu-advanced-graphics-1) to know what you should use.

`Use asynchronous shader building (Hack)`: Untick (Disable) this only if you're having issues with missing weapon menu image. You have [more info about this here](https://web.archive.org/web/20240227232543/https://github.com/yuzu-emu/yuzu/pull/10464)

Also after doing the disable Asynchronous shader building step I would recommend clearing your shader cache and rebuilding it. We do this by Right Click on the game and following the image below:

![imagen](https://i.imgur.com/dZEIrdj.png)

Next we will continue with the [mods that I'm using](https://github.com/StevensND/switch-port-mods/tree/main/The%20Legend%20of%20Zelda%20Tears%20of%20the%20Kingdom/%5B0100F2C0115B6000%5D/1.2.1/Mods).