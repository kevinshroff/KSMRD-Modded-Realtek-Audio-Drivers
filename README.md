# Kevin Shroff's Modded Realtek Audio Drivers (KSMRD)

KSMRD release notes:
- v3.0.2: added driver level support for XPS 13 9350 (needs testing)

As of KSMRD v3.0.2 pre-release, driver supports the following hardware:
- XPS 15 9570
- XPS 15 9560
- XPS 15 9550 (probably)
- XPS 13 9370 (probably)
- XPS 13 9360
- XPS 13 9350

This is the latest version of my KSMRD driver, based on the latest Realtek Audio drivers released by Dell. Currently has been verified to work on XPS 15 9560 and some other Dell laptops - support for other devices can be requested to be added OR verified that they are supported by the driver by doing the following:
1) Open an issue here on GitHub
2) Go to Device Manager - Sound, video and game controllers, and right click Realtek Audio.
3) Click properties, then click on tab "Details", and then under the Property drop-down list select Hardware IDs and copy and paste the second line to the GitHub issue, asking me to verify or add support for that device.

Installation instructions: 

Follow all instructions EXACTLY otherwise you WILL face problems.

1) Use the [same instructions as for the old KSMRD driver](https://www.reddit.com/r/Dell/comments/6nt3ch/kevin_shroffs_modded_realtek_audio_drivers_for/), (Note: in the KSMRD install instructions step 12, disable "Realtek HD Audio Universal Service" and "Waves MaxxAudio Service Application" in Task Manager's startup tab - the services have been renamed) 

2) **AND** also do the following registry tweak (after driver installation): 
- Change the values of ALL instances of ConservationIdleTime and PerformanceIdleTime to FF FF FF under HKEY_LOCAL_MACHINE\SYSTEM\ (use CTRL+F to search for ConservationIdleTime, etc.) within the registry.

> Developed by Kevin Shroff
