# Fortnite Settings Manager

Fortnite Settings Manager is a program written in Python by Nomadical that adds plenty of new functionallity to Fortnite's settings

**To install, just download the latest release and run `FortniteSettingsManager.exe`**

Source code is avaliable in the release and project code as FortniteSettingsManager.py

Here's a list of the features and how they work:

## Settings Profiles

Say you like the good looks of Fortnite at times, but at others you just need to squeeze out the maximum FPS possible; no worries!

With Fortnite Settings Manager you can create settings profiles that allow you to configure your settings in the Fortnite game and then save them to a profile

Then, you can name and switch between these profiles based on what settings you wish to use, meaning that you don't have to ruin all your careful settings tuning just to experience some good graphics.

## Sharing Settings

Did you find a set of settings that you think works well for you?

You can share your Fortnite Settings Manager profile with your friends in the form of a .fsm file by clicking the `Export Profile` button in the app

Then, they can click the `Import Profile` button to import your settings and click `Apply Profile To Game` to use them in their game.

## Hidden Settings

Most don't know this, but Fortnite actually has several hidden settings that the user can change via the Fortnite configuration file

Fortnite Settings Manager provides a nice and easy gui for changing two of these settings:
- Show Grass (Allows you to make grass dissapear when not on performance mode)
- Lobby FPS Cap (Allows you to cap or change the FPS limit in the Fortnite lobby screen)

You can also access the rest of the settings using the documented settings file included with the install, just click the ↪ button in the Fortnite Settings Manager app to open the directory where these files are located.

The Fortnite settings config file is titled `GameUserSettings.ini`, and the guide for this config file will appear next to the config file after you first run the app and is titled `GameUserSettingsDocumentation.txt`

## Other Features

You can change which Fortnite settings are included in your profiles by clicking the ↪ button in the app and opening the `FNsettingsmanager` folder, then opening `pgmconfig.txt`

After `SyncedSettings=` you will find a list of all the settings that are stored in profiles by Fortnite Settings Manager

These settings names are stored in the form of a list with comma seperated values `[Value1, Value2, Value3]`

The names of additional settings you can use is anything in `GameUserSettings.ini` that is followed by an `=` symbol

For example, `PreferredFullscreenMode=` is a value in `GameUserSettings.ini` that tells Fortnite whether to launch in fullscreen or windowed mode, and this value is not synced by Fortnite Settings Manager profiles.

You can add it manually by adding `PreferredFullscreenMode` to the end of the `SyncedSettings=` list in `pgmconfig.txt` and next time you save a profile in the app, it will sync this setting.

The default list of synced settings is:
```
SyncedSettings=[bMotionBlur, bShowFPS, LatencyTweak2, FortAntiAliasingMethod, TemporalSuperResolutionQuality, bRayTracing, RayTracingShadowsQuality, RayTracingReflectionsQuality, RayTracingAmbientOcclusionQuality, RayTracingAOQuality, RayTracingGIQuality, FrontendFrameRateLimit, DisplayGamma, UserInterfaceContrast, bUseHeadphoneMode, bDisableMouseAcceleration, bUseVSync, bUseDynamicResolution, ResolutionSizeX, ResolutionSizeY, AudioQualityLevel, FrameRateLimit, bUseNanite, DesiredGlobalIlluminationQuality, DesiredReflectionQuality, sg.ResolutionQuality, sg.ViewDistanceQuality, sg.AntiAliasingQuality, sg.ShadowQuality, sg.PostProcessQuality, sg.TextureQuality, sg.EffectsQuality, sg.FoliageQuality, sg.ShadingQuality, PreferredFeatureLevel, PreferredRHI, MeshQuality]
```
**Warning:** Some of the settings that aren't synced by Fortnite Settings Manager by defualt are account specific, and I have no idea what happens if you try to sync them to another account. The best bet is to only add custom synced settings that have a name that makes sense to you as something you would want to sync.
