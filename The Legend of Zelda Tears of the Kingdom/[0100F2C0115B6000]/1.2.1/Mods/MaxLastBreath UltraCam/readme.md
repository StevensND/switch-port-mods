## DISCLAIMER. Update December 2023

Thanks to Masagrator's help, MaxLastBreath has been able to add a Triple Buffering option to UltraCam so **the Gamebanana download is outdated**.

Triple buffer is so your game won't drop immediately to 30 FPS when it drops even one frame.

So ... I have added a new folder called `UltraCam TOTK Optimizer 1.5.3` where you can find a [.zip file](https://github.com/StevensND/switch-port-mods/tree/main/The%20Legend%20of%20Zelda%20Tears%20of%20the%20Kingdom/%5B0100F2C0115B6000%5D/1.2.1/Mods/MaxLastBreath%20UltraCam/UltraCam%20TOTK%20Optimizer%201.5.3) inside this folder with the new update. 

I have extracted the updated UltraCam mod from his [TOTK-Optimizer](https://github.com/MaxLastBreath/TOTK-mods/releases) for those of you who would like to have this mod separately.

Here is the changelog of this update:

```
- UltraCam now uses Triple Buffer. Should improve game stability and performance.
- UltraCam now reads the config file more consistently.
- UltraCam now uses proper parameters for FOV and etc. when a config file isn't present.
- UltraCam base rotation speed has been increased.
```
Also the folders inside `RomFS` have changed and now have another name, so I have also updated the MaxLastBreath README.TXT section.

Finally remind that despite this update, the UltraCam mod can be found in his [Gamebanana Original Post Link](https://gamebanana.com/mods/480138) as well as the TOTK-Optimizer.

## MaxLastBreath README.TXT:

[Full English INI here](https://github.com/StevensND/switch-port-mods/blob/main/The%20Legend%20of%20Zelda%20Tears%20of%20the%20Kingdom/%5B0100F2C0115B6000%5D/1.2.1/Mods/MaxLastBreath%20UltraCam/UltraCam%20TOTK%20Optimizer%201.5.3/INI%20File%20Info/English.md)

[Full Spanish INI here](https://github.com/StevensND/switch-port-mods/blob/main/The%20Legend%20of%20Zelda%20Tears%20of%20the%20Kingdom/%5B0100F2C0115B6000%5D/1.2.1/Mods/MaxLastBreath%20UltraCam/UltraCam%20TOTK%20Optimizer%201.5.3/INI%20File%20Info/Spanish%20(Espa%C3%B1ol).md)

Please open the `RomFS` folder and then go to the `UltraCam` folder and **open the maxlastbreath.ini config file** using NotePad or [NotePad++](https://notepad-plus-plus.org/downloads/).

I suggest use NotePad++. We will edit the .ini file to setup the mod based on your desired outcome.

Most importantly make sure you match your emulator's upscaling settings to the upscaling settings inside of the config file.

DON'T USE THIS MOD WITH OTHER DFPS MODS, IT MAY BREAK THINGS!. USE AT YOUR OWN RISK.

WARNING!

FOR KEYBOARD ENABLE VIRTUAL KEYBOARD IN YUZU/RYUJINX.

Ryujinx needs to be installed in ATMOSPHERE FOLDER or keyboard won't work.

Support this mod at https://ko-fi.com/maxlastbreath

## StevensND's maxlastbreath.ini Personal Settings:

![image](https://i.imgur.com/ygZPN8S.png)

## Things that you need to know to modify the .ini file:

`MaxFrameRate`: Here you can indicate whether you want your MaxFrameRate to be: 20, 30 or 60. If your PC is unable to exceed 30fps, leave it at 30. If you don't reach 30 stable try leaving it at 20. Set 60fps if your frames are between 35-50fps. **Keep in mind that even the most powerful CPU can't handle 60fps stable**. This is a game that requires a good high CPU (above 8 cores) for good performance.

`Fov`: You can edit this and set it to your liking. I leave it as default.

`ResolutionScale`: This section is important. If you use 0 it will Disable all Resolution Quality Optimization. So if your PC can't handle 1080p Docked & 720p Handheld and you try to decrease it and set 0, it won't work. Keep that in mind.

**How Emu Resolution  Scale works**:

![image](https://i.imgur.com/n4BlNHz.png)

I'm using 2X (1440p/2160p). So that will be 1440p on Handheld mode and 2160p on Docked Mode. And this will be 2 in the .ini file.

To use this mod you cannot use resolutions lower than 1x. Also don't use 1.5x because it's buggy. So if you're using 1x here, set the ResolutionScale to 1. If you're using 2X, set 2, 3X set 3 etc etc.

`ShadowResolution`: I'm using 1024. You can use 512 if you're having issues. Decrease it to 206 if 512 and 1024 doesn't work properly for you although I'd use 512 or 1024. I won't go higher.

`DisableFog`: This is personal preference. You like FOG?: Keep it (Off). You don't like FOG: Disable it (On).