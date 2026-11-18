# MHGU Recomp for iOS

A fork of [morerokk/MHGURecomp](https://github.com/morerokk/MHGURecomp) for iPad and iPhone. It renders at the screen's
real resolution and keeps the whole HUD visible on an iPad's 4:3 screen. New upstream releases are merged and built
automatically. Also works on iPhone.

No game data is included. You need your own dump of MHGU 1.4.0.

1. Get `MHGURecomp-iOS.<version>.ipa` from [Releases](https://github.com/cerroverb/MHGURecomp-iOS/releases).
2. Sideload it with a tool such as [iloader](https://github.com/nab138/iloader).
3. Start the app once, then put `exefs` and `romfs` in `MHGURecomp/data` with the Files app.

A controller is recommended. Plus + Minus opens the settings menu. Everything else works
as in [upstream's README](https://github.com/morerokk/MHGURecomp#readme).

# FAQ

### Will you add touch controls?

No. If you want that, request it upstream, as morerokk maintains an Android build, and they should build in this one if they are added. I'm not interested in supporting them myself. For phones, I recommend telescopic controllers. Otherwise, any dinput or Switch controllers should work via direct USB connection on all iOS devices, others with Bluetooth. 

# Known issues

-App can sometimes crash on returning from multitasking or simply exiting the app to the home menu. Fix is coming at some point, but for now, be sure you save before exiting the app for any reason. 

## Credits and license

All credit for MHGU Recomp goes to morerokk and its contributors. The iOS layer builds on
[WiseManChris/MHGURecomp-iOS](https://github.com/WiseManChris/MHGURecomp-iOS),
[Kamisorara/MHGURecomp-iOS](https://github.com/Kamisorara/MHGURecomp-iOS) and mhvuze's macOS port. MIT license, as
upstream. LLM assistance was used to port and maintain the iOS build.
