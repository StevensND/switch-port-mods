## [Hardware Requirements](https://i.imgur.com/sqsL5CD.png)

I have decided to add the Hardware Requirements link due to this is a very important section that many people ignore, especially new users emulating games.

You can check Ryujinx's Hardware Requeriments **[HERE](https://github.com/Ryujinx/Ryujinx/wiki/Ryujinx-Setup-&-Configuration-Guide#system-requirements)**

**Nintendo Switch was released on March 3, 2017** so if there is any component of your PC prior to this date (CPU, GPU ...) you should upgrade it for better performance or **just don't emulate Nintendo Switch**

Don't pretend/expect that a **2nd gen Intel i3** like [this one](https://www.intel.la/content/www/xl/es/products/sku/53426/intel-core-i32120-processor-3m-cache-3-30-ghz/specifications.html) which has 2-core, 4-thread run Zelda TOTK at 30/60fps in 720p/1080p stable because that's not the case. You might not even get the game to boot or you might not get more than 5-10fps.

With this in mind, let's continue. If you are going to upgrade your PC or you plan to buy a new PC for Nintendo Switch Emulation, **Yuzu's own website suggests that this CPU be a 6-core, 12-thread CPU at least**. I personally would choose the current generation if I can afford it or the previous generation. I would not choose older ones like an AMD Ryzen 2600/3600. The most current CPUs improve their performance, so if you have a CPU like the previous mentioned performance may not be as expected.

Also keep in mind that **Zelda TOTK is a CPU demanding game** so no matter how much you have a 3070, 3080, 4070, 4090 etc etc: if you don't have a good CPU to go with your graphics card, you won't get good performance either.

**GPUs must support OpenGL 4.6 & OpenGL Compatibility profile, or Vulkan 1.1 (or higher).**

To find out if your GPU meets these requirements, visit https://opengl.gpuinfo.org or https://vulkan.gpuinfo.org/ and check your GPU details.

Finally if we talk about RAM, IMO any RAM below 16GB is not enough (including 8GB). When you start opening Discord, Chrome/Firefox/Opera GX or any other browser you use, the emulator and some other program (Spotify, OBS ...) you will start noticing that your 8GB RAM is not enough. RIP 2GB/4GB RAM users. I would recommend 16 and if you can afford it, 32.

## CEMU vs Yuzu

Many people believe that CEMU and Yuzu are 2 equal emulators and that they have the same years of development. 

**This is totally incorrect**. CEMU was released around 2015 and Yuzu around 2018. CEMU is a Wii U emulator while Yuzu is a Switch emulator (some people think that the 2 emulate the same thing, it's funny to see people asking: How can I play TOTK on CEMU).

On the other hand there are people who think that BOTW and TOTK are the same for the same reason mentioned previously. Even though BOTW is playable on Switch,  **BOTW was originally released on Wii U**. That's why you get a better perfomance playing BOTW on CEMU rather than on Yuzu (Yes ... There are strange people playing BOTW on Yuzu instead).

CEMU is more optimized than Yuzu because it has more years of development. Also the Wii U emulation is not the same as the Switch emulation.

FYI: When CEMU came out, it could barely run BOTW at a stable 30fps. Vulkan wasn't even an option, you had to play in OpenGL. There were barely any mods to improve performance like there are today, you can search for [BSOD Gaming videos](https://www.youtube.com/@BSoDGaming/videos) to know more about this. So if you intend to play TOTK at 120-140fps stable ... come back to reality. Yuzu is not as optimized as CEMU and TOTK has barely been on the market for 1 year.

## Shaders

There are always a lot of people arguing about this topic. I sincerely recommend you to **ignore these comments and try things for yourselves**.

In my personal tests, sharing shaders doesn't work as you might expect. You may get the feeling that it's working but I would say it's a bit more placebo. Here are 2 tests I did using shaders shared by other users. Judge for yourselves.

- [Test 1](https://youtu.be/JypO8UBHApk?si=AYgdoCwmF9aGoLxA)
- [Test 2](https://www.youtube.com/watch?v=u3x4ZfvptlM)

**How to test this**: Simple. Get an overlay to see your stats ([MSI Afterburner + RivaTurner for instance](https://www.msi.com/Landing/afterburner/graphics-cards)) and record a gameplay using OBS. Record 1 gameplay using your own shaders and record another one using shared shaders and do comparisons. Then do the same using cleaning shaders vs shared shaders. Finally record another one using clean shaders vs your previous built shaders.

Once you have all the gameplays recorded, make your notes, compare gameplays, take notes about if FPS were stable and better or not, if you noticed stuttering etc etc and finally draw your conclusions.

My personal opinion is that it's not worth it. Despite this there will always be people who say that sharing shaders works.

These shared shaders are built on another PC with totally different specs than yours and on a version of the game that is probably not the one you are using.

Also when you update the game and change version or when you want to move from a newer update to an older one, I would always advise to clean the shaders and rebuild them.

Finally always clean your shaders if you notice any stuttering. This might help.

## Drivers

A Yuzu developer discovered that the **545.84 Nvidia Drivers solves low VRAM stability** so you might want to give them a try.

Anyway, always keep your drivers up to date. For some older graphics cards it may be recommended to use older drivers but these are very specific and special cases. I have no idea about AMD but I recommend using the most up to date ones as well. I'm not a fan of AMD GPUs and their software.

Finally go to your Nvidia Control Panel Settings and set this (sorry for the Spanish Translation):

![image](https://i.imgur.com/xENj0XR.png)

Most people have this option on: Let the app decide and IMO this is a mistake.

## Integrated Graphics + Dedicated GPU

Some of you may have a dedicated and an integrated graphics card. When this happens it's possible that you are not using the dedicated graphics card, but the integrated one.

Go to the Windows menu and type: Graphics Settings. You will see a window like the one in the image below (Sorry for the Spanish translation). Click on the Yuzu button, find the `yuzu.exe` file and add it. Then click on Options, select High Performance and save it. Make sure that this option indicates your dedicated graphics card and not the integrated one. You can also try disabling the drivers for your integrated graphics card in the device manager (Google how to do this).

![image](https://i.imgur.com/SRVvJzo.png)
![image](https://i.imgur.com/zAoeFcT.png)

## Remove Background Tasks

**I'm not responsible for any misuse of the following recommendations**.

Sometimes we have apps running in the background that we don't need. I recommend using Task Manager and checking that we don't have things we don't need running in the background.

One program I recommend is [Autoruns](https://learn.microsoft.com/en-us/sysinternals/downloads/autoruns). Run it as Administrator. Then click on Logon and untick everything you don't use except: cmd.exe and any n/a box.

Do the same for Services and maybe Scheduled Task. Search on Google what you should untick. This will avoid these apps running at the background when you boot Windows. Also try to avoid bloatware (search on Google if you don't know what bloatware is).

Finally I did my PC optimizations using some videos from [this YouTube channel](https://www.youtube.com/@FR33THY/videos) so maybe you want to check it out.

## Nvidia/AMD Control Panel Optimization

If you are not an experienced PC user, please, don't continue and if you still decide to do it: **I'm not responsible if you make a mistake and damage your PC**, you have been previously warned.

Here are some videos about optimize your Nvidia/AMD Control Panel:

- [Nvidia (English)](https://www.youtube.com/watch?v=uNUyF-d0oa4) | [Nvidia (Spanish)](https://youtu.be/BNKC7U6OHfo?si=KCsVgSZ7XEMFD0vd)
- [AMD (English)](https://youtu.be/wQE5neY1Xlc?si=kYhMrEQrnoqT9KP7) | [AMD (Spanish)](https://youtu.be/B_Kb-AjLu5g?si=GWi7CpVm7etACA3X)

### End of the guide

That's all. I think this is all you'll need to know about setup Yuzu, settings, mods and possible optimizations.

Remember that if you want to support this work and keep a track of my mods + updates, here's my main [Github Mods Link](https://github.com/StevensND/switch-port-mods) and [my Ko-Fi](https://ko-fi.com/stevenss) as well as the rest of my [social media](https://linktr.ee/stevenssv2)

I hope this guide has been useful to you and that you will support it.