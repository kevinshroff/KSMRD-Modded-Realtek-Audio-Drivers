# Kevin Shroff's Modded Realtek Audio Drivers (KSMRD)

#### KSMRD release notes:
- v3.0.2: added driver level support for XPS 13 9350

As of KSMRD v3.0.2 pre-release, driver supports the following hardware:
- XPS 15 9570
- XPS 15 9560
- XPS 15 9550 (probably)
- XPS 13 9370
- XPS 13 9360
- XPS 13 9350
- Inspiron 15 Gaming 7577
- probably other recent Dell Windows devices

## Advantages of KSMRD:
1) Completely flat & clean audio experience: no post-processing

2) No extra, unalterable Waves MaxxAudio bloatware

3) Reduced power consumption compared to stock Dell Realtek Audio drivers - as there is no post-processing constantly going on with all audio, this may lead to increased battery life

4) No stupid GUI popups for Input/Output switcher (The prompt "What did you just plugin: Headphone/Speaker/Microphone" does not popup anymore)

5) Can prevent laptop speaker damage - some people had concerns that the Waves MaxxAudio software was pushing the XPS laptop speakers too hard, causing early speaker damage. As Waves MaxxAudio and its sound effects are removed, this concern should not be an issue with this driver.

#### About 
This modded Realtek Audio driver disables the heavy post-processing sound effects from the stock Dell driver to allow for a clean, neutral, and flat audio experience. This is achieved by disabling Waves MaxxAudio throughout the driver, thus leaving intact only the essential core Realtek audio software.

Waves Maxxaudio is immutable bloatware that is shipped with all modern Dell XPS systems. It is inherently flawed as it heavily manipulates any and all audio output, making it impossible to accurately produce or listen to music, and overall degrades the entire aural experience on any machine that it is present on.

As Waves MaxxAudio is part of the Audio driver of Dell XPS systems, it was otherwise impossible to disable just MaxxAudio and its processing effects - even when MaxxAudio is turned off in its application's GUI, post-processing STILL occurs on any and all audio output. The only other alternative was to use the Microsoft default Windows High Definition Audio driver, but this driver has many problems on Dell XPS machines - it causes random loud pops and crackles, especially during usage with ASIO software (in my experience).

My modded driver solves these problems as it disables all post-processing and provides flat, clean audio playback just like the Windows High Definition Audio driver, but without its bugs.

[DOWNLOADS & INSTALL INSTRUCTIONS](https://github.com/kevinshroff/KSMRD-Modded-Realtek-Audio-Drivers/releases "DOWNLOADS")
---
> Developed by Kevin Shroff | [Donate with Paypal](http://www.paypal.me/kevinshroff "donate") | Would greatly appreciate if you could support my driver work by following my social media: [My YouTube channel](https://www.youtube.com/c/KevinShroff "YouTube") | [My Soundcloud](https://soundcloud.com/nivekfforhs "Soundcloud")
