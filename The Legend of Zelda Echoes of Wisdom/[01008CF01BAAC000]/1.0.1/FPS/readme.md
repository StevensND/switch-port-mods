## About FPS Drops

First of all, **YOU MUST READ THE ENTIRE TEXT TO UNDERSTAND EVERYTHING. DON'T SKIP IT BECAUSE ALL THE INFO IS IMPORTANT**

The game runs natively at 60FPS on Switch. However the game is using double buffer.

So if you're facing FPS drops and your FPS drops to 30 is due to that + Switch GPU on Default is bottleneck to mantain stable FPS. 

If you have a potato device (PC with low specs, Steam Deck, Smartphone ...) you can try this mod to reach a few more FPS.

> [!TIP]
If you're playing on Switch you can try to OC your Switch and apply a good OC to stabilize the FPS. Also add this mod and see if something improves.

**I won't explain how to OC your Switch**. Read [THIS GUIDE](https://rentry.co/howtoget60fps) instead.

**Also you can try the Potato Version**. That mod decrease the resolution to 1024x576p so the GPU is not limited on Default.

I've been trying this resolution on my Switch and I think this is the closest resolution to achieving a stable 60FPS without having to OC.

> [!NOTE]
Despite this mod, I think a triple buffer patch or do a little more research could make the FPS improve. 

I'm not 100 % sure but I'm not entirely satisfied with this mod fix yet.

## What this mod does

Echoes Of Wisdom **already sets the present interval to 1**. However, there are situations in which the game changes this interval to 2.

This mod tries to force the game to set all the time the present interval to 1 and be able to reach 60FPS. 

I hope to make the explanation as basic as possible for you to understand.

To make the game runs at 60FPS, you need to set something called `Present Interval` to 1.

```
1 = 60FPS
2 = 30FPS
0 = Uncap FPS
````

**This would be enough in all games?: No.** 

Some games require more patches and you won't always unlock FPS by doing this.

Also add that sometimes you'd need to fix speedup, game breaking due to the game was not designed to play at those FPS ... which is really annoying and it can take hours.

I'm not going to focus on explaining that because it's more complicated than you think.

**However, despite this explanation there are people who still think that making a 60FPS mod that works correctly in all games is a matter of 2 minutes or less.**

## Why you don't do an 120FPS/ Uncap FPS version

If the game goes above 60FPS and you open the menu to see the inventory, map etc etc. **THE MENU IS SPEEDUP**

If you reach 120FPS higher, **you can't leave water caves and other areas** so it's preferably keep FPS locked to 120 and lower or just 60FPS.

I'm not focusing on release a 30FPS mod. **It's not my purpouse with this game.** 

## Fl4sh vs KeatonTheBot vs Stevens

> [!IMPORTANT]
If you're using Fl4sh option, sometimes you'll find a V2 version in the .pchtxt files. **YOU NEED BOTH .PCHTXT FILES. DON'T DELETE THEM**

All versions has the same perfomance on my tests. However, the methods we use are different.

So if one of them doesn't work for you due, try the other options.

> [!NOTE]
I did all my test on the Switch, not emulator. The purpouse was focus on the perfomance on Switch with no OC (default settings).

This way we could find fixes for both Switch and emulator.

My version is more similar to KeatonTheBot's mod. 

However, while Keaton would have to update his mod if the game releases a new update, I would not have to (If Nintendo doesn't change the files).

Fl4sh is using a different method than us, but as I said: **in the end the performance is the same on Switch (hardware).** 

**[GET FL4SH OPTION HERE](https://gamebanana.com/mods/545054)**

**[GET KEATON OPTION HERE](https://github.com/KeatonTheBot/switch-pchtxt-mods/tree/main/Legend%20of%20Zelda%2C%20The%20-%20Echoes%20of%20Wisdom/01008CF01BAAC000)**

## Default vs 1024x576p 

As I explained above, the Default mod would work with the default resolution of the game, while the other version would change this resolution to 576p for potatos devices.

1024x576p option will be called `Potato` to make it easy to distinguish.

> [!NOTE]
The Default Resolution on **Docked** is 1408x792p.