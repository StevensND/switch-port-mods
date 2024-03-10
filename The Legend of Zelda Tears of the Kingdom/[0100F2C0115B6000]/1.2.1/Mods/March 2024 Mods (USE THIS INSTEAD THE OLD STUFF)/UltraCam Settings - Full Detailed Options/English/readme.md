If you can't read the full instructions properly, download the .zip file instead.

```
# (NEW) CameraSpeed: is Rotational speed for the freecam.
# (NEW) Speed: The speed at which the freecam moves.
# (NEW)AutoHideUI: automatically FULLY hides the ui in freecam.
# (NEW) AnimationSmoothing: Smoothens the sequencer between key frames, it makes an arc between each keyframe basically.
# (NEW) AnimationFadeout: It makes the last Keyframe move slower until it reaches a complete stop.

[UltraCam]
TriggerWithController = On
AutoHideUI = On
CameraSpeed = 30
Speed = 5
AnimationSmoothing = 0.25
AnimationFadeout = On



# (NEW) FOV: Changes the fov for the entire game, including bow, zoom in, zoom out and more.
# (NEW) MenuFPSLock: Locks ingame menus to anything you desire.
# (NEW) MovieFPS: Locks the Movie FPS to 30, 60 or 120. ONLY USE WITH OTHER MODS. OR MOVIES WILL BE FASTER.
# (NEW) IsTimeSlower: When On Time will be slowed down by the float number of Time Speed.
# (New) TimeSpeed at 0.0 pauses ingame time. And at 1.0 is default, 2.0 is 2x faster/slower etc.
# (OLD) DisableFog: Removes the haziness of the game.

[Features]
Fov = 50
MenuFPSLock = 30
MovieFPS = 30
DisableFog = On
TimeSpeed = 1.0
IsTimeSlower = Off


# (NEW) Resolution now also inherits Aspect Ratio Automatically (UI is still stretched) <-- Just google your resolution with your desired aspect ratio.
# Keep 1920x1080 as the max for Switch. (1600x900) is the default.
# (NEW) Any FPS cap, feel free to adjust to your liking, 20-480 and anything in between! :).
# (NEW) Triple Buffer, previously On by default now an option, found out that TRIPLEBUFFER was causing issues with switch launching, (WIP) to investigate. KEEP OFF ON SWITCH.
# (NEW) QualityImprovements: Removes FSR and Dynamic Resolution.
# (NEW) RemoveDepthOfField: RemoveLensflare - Pretty self explanatory.
# (NEW) EmuScale = Match with Emulator scale, should be left to 1 and ideally 1x in Emulator for best Quality, This setting fixes skyisland and other issues caused by EMU scale...
# (NEW) ShadowResolution: Up to 8k SHADOWS. KEEP AT 1024 MAX on switch. Ryujinx doesn't like this setting very much 2048 is the max.
# (NEW) DisableFXAA: Removes internal FXAA.

# (IMPORTANT) SHADOW RESOLUTION AND RESOLUTION REQUIRE EXTENDED MEMORY HEAP. THE MAX RESOLUTION I HAVE TRIED AND IS WORKING IS 8K with 8K SHADOWS.

[Resolution]
MaxFramerate = 60
Width = 1920
Height = 1080
EmuScale = 1.0
ShadowResolution = 1024
RenderDistance = 25000
QualityImprovements = On
TripleBuffer = Off
RemoveDepthOfField = On
DisableFXAA = On
RemoveLensflare = On



# (NEW) OverrideHandheld_Resolution - Instead of 720p it will use the global Width and Height set in the RESOLUTION section.
# (NEW) Set Handheld resolution here.

[Handheld]
OverrideHandheld_Resolution = Off
Width = 1280
Height = 720



# (NEW) Coresponds to the rotational speed of the PLAYER camera. (MULTIPLIER), be careful with vertical it goes too fast past 1.5

[Gameplay]
Stick_Vertical_Speed = 1.0
Stick_Horizontal_Speed = 1.0



# Benchmark Index
# 0 - Kakariko
# 1 - Great Sky Island
# 2 - Lookout Landing
# 3 - Goron City
# 4 - Korok Forest (Only use when Korok Forest is COMPLETED)

[Benchmark]
Benchmark = 1



# (NEW) This allows for manual tweaking of certain memory allocations
# The main purpose of this is to allow easier merging of ROMFS mods.
# This is a direct multiplier of certain heaps.
# Graphical Heaps are done automatically by UltraCam.
# Please Ensure you don't have a romfs/System/Heap File that may interfere with UC.

[Heaps]
RSDB = 1.0
GameTextures = 1.0
```