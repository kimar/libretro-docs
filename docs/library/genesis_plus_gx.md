# Sega - MS/GG/MD/CD (Genesis Plus GX)

## Background

Genesis Plus GX is an open-source Sega 8/16 bit emulator developed by Eke-Eke which focuses on accuracy and portability. The source code, originally based on Genesis Plus 1.3 by Charles MacDonald, has been heavily modified & enhanced, with respect to initial goals and design, in order to improve the accuracy of emulation, implementing new [features](https://github.com/ekeeke/Genesis-Plus-GX/blob/master/wiki/Features.md) and adding support for [extra peripherals](https://github.com/ekeeke/Genesis-Plus-GX/blob/master/wiki/Features.md#support-for-various-peripherals), [cartridge & systems hardware](https://github.com/ekeeke/Genesis-Plus-GX/blob/master/wiki/Features.md#support-for-various-cartridges-extra-hardware) such as various lightguns, the FM Sound Unit and Lock-On cartridge technology.

Genesis Plus GX has [100% compatibility](https://github.com/ekeeke/Genesis-Plus-GX/blob/master/wiki/Compatibility.md) with Genesis / Mega Drive, Sega/Mega CD, Master System, Game Gear, SG-1000 & Pico released software (including all unlicensed or pirate known dumps), also emulating backwards compatibility modes when available. 

**Keep in mind that [32X games](https://segaretro.org/Sega_32X#List_of_games) are not supported.**

The Genesis Plus GX core has been authored by:

- Eke-Eke
- Charles McDonald

The Genesis Plus GX core is licensed under:

- [Non-commercial](https://github.com/libretro/Genesis-Plus-GX/blob/master/LICENSE.txt)

A summary of the licenses behind RetroArch and its cores can be found [here](../development/licenses.md).

## BIOS

Required or optional firmware files go in the frontend's system directory.

!!! warning ""
    Please note that BIOS choice isn't locked to any specific revisions.
!!! warning ""
    BIOS files that are labeled (bootrom) and (lock-on) must have their corresponding [core option](#core-options) (System bootrom core option or Cartridge lock-on core option) configured correctly in order for them to be loaded.

| Filename      | Description                                     | md5sum                           |
|:-------------:|:-----------------------------------------------:|:--------------------------------:|
| bios_MD.bin   | [MegaDrive TMSS startup ROM](https://segaretro.org/TradeMark_Security_System) (bootrom) - Optional | 45e298905a08f9cfb38fd504cd6dbc84 |
| bios_CD_E.bin | [MegaCD EU BIOS](https://segaretro.org/Sega_Mega-CD/Boot_ROM) - Required for MegaCD EU games   | e66fa1dc5820d254611fdcdba0662372 |
| bios_CD_U.bin | [SegaCD US BIOS](https://segaretro.org/Sega_Mega-CD/Boot_ROM) - Required for SegaCD US games   | 854b9150240a198070150e4566ae1290 |
| bios_CD_J.bin | [MegaCD JP BIOS](https://segaretro.org/Sega_Mega-CD/Boot_ROM) - Required for MegaCD JP games   | 278a9397d192149e84e820ac621a8edd |
| bios_E.sms    | [MasterSystem EU BIOS](https://segaretro.org/Sega_Master_System/Boot_ROM) (bootrom) - Optional       | 840481177270d5642a14ca71ee72844c |
| bios_U.sms    | [MasterSystem US BIOS](https://segaretro.org/Sega_Master_System/Boot_ROM) (bootrom) - Optional       | 840481177270d5642a14ca71ee72844c |
| bios_J.sms    | [MasterSystem JP BIOS](https://segaretro.org/Sega_Master_System/Boot_ROM) (bootrom) - Optional       | 24a519c53f67b00640d0048ef7089105 |
| bios.gg       | [GameGear BIOS](https://www.smspower.org/Development/BIOSes#GameGear) (bootrom) - Optional              | 672e104c3be3a238301aceffc3b23fd6 |
| sk.bin        | [Sonic & Knuckles ROM (lock-on)](https://segaretro.org/Sonic_%26_Knuckles/Technical_information) - Optional       | 4ea493ea4e9f6c9ebfccbdb15110367e |
| sk2chip.bin   | [Sonic & Knuckles UPMEM ROM](https://info.sonicretro.org/Knuckles_the_Echidna_in_Sonic_the_Hedgehog_2#Functioning) (lock-on) - Optional | b4e76e416b887f4e7413ba76fa735f16 |
| areplay.bin   | [Action Replay ROM](https://segaretro.org/Action_Replay) (lock-on) - Optional          | a0028b3043f9d59ceeb03da5b073b30d |
| ggenie.bin    | [Game Genie ROM (lock-on)](https://segaretro.org/Game_Genie_(Mega_Drive)) - Optional             | e8af7fe115a75c849f6aab3701e7799b |

## Extensions

Content that can be loaded by the Genesis Plus GX core have the following file extensions:

* .m3u
* .mdx
* .md
* .smd
* .gen
* .bin
* .cue
* .iso
* .chd
* .bms
* .sms
* .gg
* .sg
* .68k
* .sgd

RetroArch database(s) that are associated with the Genesis Plus GX core:

- [Sega - Game Gear](https://github.com/libretro/libretro-database/blob/master/rdb/Sega%20-%20Game%20Gear.rdb)
- [Sega - Master System - Mark III](https://github.com/libretro/libretro-database/blob/master/rdb/Sega%20-%20Master%20System%20-%20Mark%20III.rdb)
- [Sega - Mega-CD - Sega CD](https://github.com/libretro/libretro-database/blob/master/rdb/Sega%20-%20Mega-CD%20-%20Sega%20CD.rdb)
- [Sega - Mega Drive - Genesis](https://github.com/libretro/libretro-database/blob/master/rdb/Sega%20-%20Mega%20Drive%20-%20Genesis.rdb)
- [Sega - PICO](https://github.com/libretro/libretro-database/blob/master/rdb/Sega%20-%20PICO.rdb)
- [Sega - SG-1000](https://github.com/libretro/libretro-database/blob/master/rdb/Sega%20-%20SG-1000.rdb)

## Features

Frontend-level settings or features that the Genesis Plus GX core respects.

| Feature           | Supported |
|-------------------|:---------:|
| Restart           | ✔         |
| Saves             | ✔         |
| States            | ✔         |
| Rewind            | ✔         |
| Netplay           | ✔         |
| Core Options      | ✔         |
| RetroAchievements | ✔         |
| RetroArch Cheats  | ✔         |
| Native Cheats     | ✕         |
| Controls          | ✔         |
| Remapping         | ✔         |
| Multi-Mouse       | ✔         |
| Rumble            | ✕         |
| Sensors           | ✕         |
| Camera            | ✕         |
| Location          | ✕         |
| Subsystem         | ✕         |
| [Softpatching](../guides/softpatching.md) | ✕         |
| Disk Control      | ✔         |
| Username          | ✕         |
| Language          | ✔         |
| Crop Overscan     | ✕         |
| LEDs              | ✔         |

## Directories

The Genesis Plus GX core's library name is 'Genesis Plus GX'

The Genesis Plus GX core saves/loads to/from these directories.

**Frontend's Save directory**

| File         | Description                                                                          |
|:------------:|:------------------------------------------------------------------------------------:|
| *.srm        | MS/GG/MD/Pico/SG-1000 Cartridge backup save                                          |
| cart.brm     | Sega/Mega CD RAM Cart                                                                |
| scd_U.brm    | Sega CD US Backup RAM - When the CD System BRAM core option is set to Per-BIOS     |
| scd_E.brm    | Mega CD EU Backup RAM - When the CD System BRAM core option is set to Per-BIOS     |
| scd_J.brm    | Mega CD JP Backup RAM - When the CD System BRAM core option is set to Per-BIOS     |
| *.brm        | Sega CD/MegaCD Backup RAM - When the CD System BRAM core option is set to Per-Game |

**Frontend's State directory**

| File     | Description |
|:--------:|:-----------:|
| *.state# | State       |

## Geometry and timing

- The Genesis Plus GX core's core provided FPS is dependent on the loaded content.
- The Genesis Plus GX core's core provided sample rate is 44100 Hz
- The Genesis Plus GX core's base width is dependent on the loaded content.
- The Genesis Plus GX core's base height is dependent on the loaded content.
- The Genesis Plus GX core's max width is 720
- The Genesis Plus GX core's max height is 576
- The Genesis Plus GX core's core provided aspect ratio is dependent on the 'Core-provided aspect ratio' [core option](#core-options).

## Loading Sega CD games

When loading Sega CD games, Genesis Plus GX needs a cue-sheet that points to an image file. A cue sheet, or cue file, is a metadata file which describes how the tracks of a CD or DVD are laid out.

If you have e.g. `foo.bin`, you should create a text file and save it as `foo.cue`. If the Sega CD game is single-track, the cue file contents should look like this:

```
 FILE "foo.bin" BINARY
  TRACK 01 MODE1/2352
   INDEX 01 00:00:00
```

After that, you can load the `foo.cue` file in RetroArch with the Genesis Plus GX core.

!!! warning ""
    Certain Sega CD games are multi-track, so their .cue files might be more complicated.

Here's a cue file example done with Lunar - Eternal Blue (USA)

![](../image/core/genesis_plus_gx/cue.png)

!!! warning ""
	For Sega-CD games, ISO + WAV, BIN + CUE and ISO + OGG formats are supported; ISO + MP3 is not supported. Audio files must be in the 16-bit stereo 44100Hz format. If using a cue sheet, WAV or OGG tracks should be denoted as AUDIO.

When loading ISO + WAV or ISO + OGG format games, the core will attempt to load a cue named the same as the iso first. If one is not found, the following audio track naming formats are accepted for a data track of "game.iso":

- game02.ogg
- game 02.ogg
- game-02.ogg
- game - 02.ogg
- game_02.ogg

## Core options

The Genesis Plus GX core has the following option(s) that can be tweaked from the core options menu. The default setting is bolded.

Settings with (Restart) means that core has to be closed for the new setting to be applied on next launch.

### System

Configure base hardware selection / region / BIOS / Sega CD save file parameters.
_________________

- **System hardware** [genesis_plus_gx_system_hw] - Runs loaded content with a specific emulated console.

-- **Auto [auto]** - Loads the game with the most appropriate system based on the loaded [game's ROM information](https://raw.githubusercontent.com/ekeeke/Genesis-Plus-GX/master/core/loadrom.c) like its ROM type, product code/version, checksum, size and region code.
-- SG-1000 [sg-1000 II] - Loads game with the [SG-1000 console](https://segaretro.org/SG-1000).
-- SG-1000 II + RAM Ext. [sg-1000 II + ram ext.] - Loads game with the [SG-1000 II console](https://segaretro.org/SG-1000_II) with a [RAM extension adapter](https://segaretro.org/8kB_RAM_Adapter).
-- Mark III [mark-III] - Loads game with the [Mark III console](https://segaretro.org/Sega_Mark_III)
-- Master System [master system] - Loads game with the [Master System console](https://segaretro.org/Sega_Master_System#Master_System)
-- Master System II [master system II] - Loads game with the [Master System II console](https://segaretro.org/Sega_Master_System#Master_System_II)
-- Game Gear [game gear] - Loads game with the [Game Gear handheld console](https://segaretro.org/Sega_Game_Gear)
-- Mega Drive/Genesis [mega drive / genesis] - Loads game with the [Mega Drive/Genesis console](https://segaretro.org/Sega_Mega_Drive)

- **System region** [genesis_plus_gx_region_detect] - Specify which region the system is from. For consoles other than the Game Gear, 'PAL' is 50hz while 'NTSC' is 60hz. Games may run faster or slower than normal if the incorrect region is selected.

-- **Auto [auto]** - Changes the system's region to whatever is most appropriate for the game which is based on the loaded [game's ROM information](https://raw.githubusercontent.com/ekeeke/Genesis-Plus-GX/master/core/loadrom.c) like its ROM type, product code/version, checksum, size and region code.
-- NTSC-U [ntsc-u] - Changes the system's region to [NTSC-U](https://en.wikipedia.org/wiki/NTSC).
-- PAL [pal] - Changes the system's region to [PAL](https://en.wikipedia.org/wiki/PAL_region).
-- NTSC-J [ntsc-j] - Changes the system's region to [NTSC-J](https://en.wikipedia.org/wiki/NTSC-J).
 
- **System Boot ROM** [genesis_plus_gx_bios] (**disabled**/enabled) - Use official BIOS/bootloader for emulated hardware, if present in RetroArch's system directory. Displays console-specific start-up sequence/animation, then runs loaded content. Look above at the [BIOS section](#bios) for supported BIOS types/files.

-- **Off [disabled]** - Disables using the user supplied System Boot ROM.
-- On [enabled] - Enables using the user supplied System Boot ROM.

- **CD System BRAM** [genesis_plus_gx_system_bram] - When running Sega CD content, specifies whether to share a single save file between all games from a specific region (Per-BIOS) or to create a separate save file for each game (Per-Game). Note that the Sega CD has limited internal storage, sufficient only for a handful of titles. To avoid running out of space, the 'Per-Game' setting is recommended."

-- **Per-BIOS [per bios]** - All games from a specific region share a single save file.
-- Per-Game [per game] - Creates a separate save file for each game.

??? note "*CD System BRAM diagram*"
	![](../image/core/genesis_plus_gx/bram.png)

- **CD Backup Cart BRAM** [genesis_plus_gx_cart_bram] - When running Sega CD content, specifies whether to share a single backup ram cart for all games (Per-Cart) or to create a separate backup ram cart for each game (Per-Game).

-- **Per-Cart [per cart]** - All games share a single backup RAM cart.
-- Per-Game [per game] - Creates a seperate backrup RAM cart for each game.

- **CD add-on (MD mode) (Requires Restart)** [genesis_plus_gx_add_on] - Specify which add-on to use for CD audio playback with supported Mega Drive/Genesis games.

-- **Auto [auto]** - Loads a CD game with the most appropriate CD add-on based on the loaded [game's ROM information](https://raw.githubusercontent.com/ekeeke/Genesis-Plus-GX/master/core/loadrom.c) like its ROM type, product code/version, checksum, size and region code.
-- Sega/Mega CD [sega/mega cd] - Loads the game using the [Sega/Mega CD add-on](https://segaretro.org/Sega_Mega-CD).
-- MegaSD [megasd] - Loads the game using the [MegaSD FPGA cartridge](https://terraonion.com/en/producto/megasd/).
-- None [none] - Disables loading a CD game with any CD add-on.

- **Cartridge Lock-On** [genesis_plus_gx_lock_on] - Lock-On Technology is a Mega Drive/Genesis feature that allowed an older game to connect to the pass-through port of a special cartridge for extended or altered gameplay. This option specifies which type of special 'lock-on' cartridge to emulate. Look above at the [BIOS section](#bios) for supported BIOS types/files.

-- **Off [disabled]**
-- Game Genie [game genie] - Connects the loaded game to a [Gamie Genie](https://segaretro.org/Game_Genie_(Mega_Drive)).
-- Action Replay (Pro) [action replay (pro)] - Connects the loaded game to an [Action Replay (Pro)](https://segaretro.org/Action_Replay).
-- Sonic & Knuckles [sonic & knuckles)] - Connects the loaded game to [Sonic & Knuckles](https://info.sonicretro.org/Sonic_%26_Knuckles).

### Video

Configure aspect ratio / display cropping / video filter / frame skipping parameters.
_________________

- **Core-Provided Aspect Ratio** [genesis_plus_gx_aspect_ratio] - Choose the preferred content aspect ratio. This will only apply when RetroArch's aspect ratio is set to 'Core provided' in the Video settings.

-- **Auto [auto]** - Chooses the aspect ratio based on the loaded [game's ROM information](https://raw.githubusercontent.com/ekeeke/Genesis-Plus-GX/master/core/loadrom.c) like its ROM type, product code/version, checksum, size and region code.
-- NTSC PAR [NTSC PAR] - Sets the game's aspect ratio to NTSC PAR.
-- PAL PAR [PAL PAR] - Sets the game's aspect ratio to PAL PAR.

- **Borders** [genesis_plus_gx_overscan] - Enable this to display the overscan regions at the top/bottom and/or left/right of the screen. These would normally be hidden by the bezel around the edge of a standard-definition television.

-- **Off [disabled]** - Disables displaying the game's overscan regions.
-- Top/Bottom [top/bottom] - Enables displaying the game's Top and Bottom overscan regions.
-- Left/Right [left/right] - Enables displaying the game's Left and Right overscan regions.
-- Full [full] - Enables displaying the game's Top/Bottom and Left/Right overscan regions.

- **Hide Master System Side Borders** [genesis_plus_gx_left_border] - Cuts off 8 pixels from either the left side of the screen, or both left and right sides when running Master System games.

-- **Off [disabled]** - Disabling cutting off pixels from the screen of a Master System game.
-- Left Border Only [left border] - Cuts off 8 pixels from the left side of the screen of a Master System game.
-- Left & Right Borders [left & right borders] - Cuts off 8 pixels from the right side of the screen of a Master System game.

- **Game Gear Extended Screen** [genesis_plus_gx_gg_extra] - Forces Game Gear titles to run in 'SMS' mode, with an increased resolution of 256x192. May show additional content, but typically displays a border of corrupt/unwanted image data.

??? note "*Game Gear extended screen - Off [disabled]*"
    ![](../image/core/genesis_plus_gx/off.png)

??? note "*Game Gear extended screen - On [enabled]*"
    ![](../image/core/genesis_plus_gx/on.png)

- **Blargg NTSC Filter** [genesis_plus_gx_blargg_ntsc_filter] - Apply a video filter to mimic various NTSC TV signals.

??? note "*Blargg NTSC filter - Off [disabled]*"
    ![](../image/core/genesis_plus_gx/normal.png)

??? note "*Blargg NTSC filter  - Monochrome [monochrome]*"
    ![](../image/core/genesis_plus_gx/monochrome.png)

??? note "*Blargg NTSC filter - Composite [composite]*"
    ![](../image/core/genesis_plus_gx/composite.png)

??? note "*Blargg NTSC filter  - S-Video [svideo]*"
    ![](../image/core/genesis_plus_gx/svideo.png)

??? note "*Blargg NTSC filter - RGB [rgb]*"
    ![](../image/core/genesis_plus_gx/rgb.png)

- **LCD Ghosting Filter** [genesis_plus_gx_lcd_filter] - Apply an image 'ghosting' filter to mimic the display characteristics of the Game Gear and 'Genesis Nomad' LCD panels.

??? note "*LCD Ghosting filter - On [enabled]*"
    ![](../image/core/genesis_plus_gx/ghost.png)

- **Interlaced Mode 2 Output** [genesis_plus_gx_render] - Interlaced Mode 2 allows the Mega Drive/Genesis to output a double height (high resolution) 320x448 image by drawing alternate scanlines each frame (this is used by 'Sonic the Hedgehog 2' and 'Combat Cars' multiplayer modes). 'Single Field' mimics original hardware, producing each field (320x224) alternatively with flickering/interlacing artefacts. 'Double Field' simulates the interlaced display, which stabilises the image but causes mild blurring.

??? note "*Single Field [single field]*"
    ![](../image/core/genesis_plus_gx/single.png)

??? note "*Double Field [double field]*"
    ![](../image/core/genesis_plus_gx/double.png)

- **Frameskip** [genesis_plus_gx_frameskip] - Skip frames to avoid audio buffer under-run (crackling). Improves performance at the expense of visual smoothness. 'Auto' skips frames when advised by the frontend. 'Manual' utilises the 'Frameskip Threshold (%)' setting.

-- **Off [disabled]** - Disables frameskip.
-- Auto [auto] - Automatically skips frames to avoid audio crackling.
-- Manual [manual] - Allows the user to utilises the 'Frameskip Threshold' core option's set percentage to manually adjust frameskip.

- **Frameskip Threshold (%)** [genesis_plus_gx_frameskip_threshold] - When the 'Frameskip' core option is set to 'Manual', specifies the audio buffer occupancy threshold (percentage) below which frames will be skipped. Higher values reduce the risk of crackling by causing frames to be dropped more frequently.

-- 15% to 60% in increments of 3%, **33% is default**.

### Audio

Change audio device settings.
_________________

- **Master System FM (YM2413)** [genesis_plus_gx_ym2413] - Enable emulation of the [FM Sound Unit](http://segaretro.org/FM_Sound_Unit)) used by certain Sega Mark III/Master System games for enhanced audio output.

-- **Auto [auto]** - Automatically enables emulation of FM Sound Unit based on the loaded [game's ROM information](https://raw.githubusercontent.com/ekeeke/Genesis-Plus-GX/master/core/loadrom.c) like its ROM type, product code/version, checksum, size and region code.
-- Off [disabled] - Disables emulation of FM Sound Unit.
-- On [enabled] - Enables emulation of FM Sound Unit.

- **Master System FM (YM2413) Core** - [genesis_plus_gx_ym2413_core] - Select method used to emulate the FM Sound Unit of the Sega Mark III/Master System. 'MAME' option is fast, and runs full speed on most systems. 'Nuked' option is cycle accurate, very high quality, and has substantial CPU requirements. The 'Master System FM (YM2413) Core' core option only appears if the Genesis Plus GX libretro core was compiled with the [HAVE_OPLL_CORE flag](https://github.com/libretro/Genesis-Plus-GX/blob/master/Makefile.libretro).

-- **MAME [mame]** - Uses the MAME option for emulating the FM Sound Unit for Sega Mark III/Master System games which is fast and full speed for most games.
-- Nuked [nuked] - Uses the Nuked option for emulating the FM Sound Unit for Sega Mark III/Master System games which is high quality but has substantial CPU requirements.

- **Mega Drive/Genesis FM** [genesis_plus_gx_ym2612] - Select method used to emulate the FM synthesizer (main sound generator) of the Mega Drive/Genesis. 'MAME' options are fast, and run full speed on most systems. 'Nuked' options are cycle accurate, very high quality, and have substantial CPU requirements. The 'Nuked' core option settings only appear if the Genesis Plus GX libretro core was compiled with the [HAVE_YM3438_CORE flag](https://github.com/libretro/Genesis-Plus-GX/blob/master/Makefile.libretro). The 'YM2612' chip is used by the original Model 1 Mega Drive/Genesis. The 'YM3438' is used in later Mega Drive/Genesis revisions.

-- **MAME (YM2612) [mame (ym2612)]** - Selects MAME (YM2612) [original Model 1 Mega Drive/Genesis] as FM synthesizer method which is fast and fullspeed.
-- MAME (ASIC YM3438) [mame (asic ym3438)] - Selects MAME (ASIC YM3438 [later Mega Drive/Genesis revisions] as FM synthesizer method which is fast and fullspeed.
-- MAME (Enhanced YM3438) [mame (enhanced ym3438)] - Selects MAME (Enhanced YM3438) [later Mega Drive/Genesis revisions] as FM synthesizer method which is fast and fullspeed.
-- Nuked (YM2612) [nuked (ym2612)] - Selects Nuked (YM2612) [original Model 1 Mega Drive/Genesis] as FM synthesizer method which is high quality but has high CPU requirements.
-- Nuked (YM3438) [nuked (ym3438)] - Selects Nuked (YM3438) [later Mega Drive/Genesis revisions] FM synthesizer method which is fast but has high CPU requirements.

- **Sound Output** [genesis_plus_gx_sound_output] - Select stereo or mono sound reproduction.

-- **Stereo [stereo]** - Selects stereo output.
-- Mono (mono) - Selects mono output.

- **Audio Filter** [genesis_plus_gx_audio_filter] - Enable a low pass audio filter to better simulate the characteristic sound of a Model 1 Mega Drive/Genesis." The 'EQ' core option setting only appears when the Genesis Plus GX core was compiled with the [HAVE_EQ flag](https://github.com/libretro/Genesis-Plus-GX/blob/master/libretro/libretro.c).

-- **Off [disabled]** - Disables low pass audio filter.
-- Low-Pass [low-pass] - Enables low pass audio filter.
-- EQ [EQ] - Enables internal audio equalizer.

- **Low-Pass Filter %** [genesis_plus_gx_lowpass_range] - Specify the cut-off frequency of the low-pass audio filter. A higher value increases the perceived 'strength' of the filter, since a wider range of the high frequency spectrum is attenuated. This core option requires the 'Audio Filter' core option to be set to 'Low-Pass".

-- 5% to 95% in increments of 5. *60% is default**. 

- **PSG Preamp Level** [genesis_plus_gx_psg_preamp] - Set the audio preamplifier level of the emulated SN76496 4-channel Programmable Sound Generator found in the SG-1000, Sega Mark III, Master System, Game Gear and Mega Drive/Genesis.

-- 0 to 200 in increments of 5. **150 is default**.

- **FM Preamp Level** [genesis_plus_gx_fm_preamp] - Set the audio preamplifier level of the emulated Mega Drive/Genesis FM sound synthesizer or Sega Mark III/Master System FM Sound Unit

-- 0 to 200 in increments of 5. **100 is default**.

- **CD-DA Volume** [genesis_plus_gx_cdda_volume] - Adjust the mixing volume of the emulated CD audio playback output.

-- 0 to 100 in increments of 5. **100 is default**.

- **PCM Volume** [genesis_plus_gx_pcm_volume] - Adjust the mixing volume of the emulated Sega CD/Mega-CD RF5C164 PCM sound generator output.

-- 0 to 100 in increments of 5. **100 is default**.

- **EQ Low** [genesis_plus_gx_audio_eq_low] - Adjust the low range band of the internal audio equalizer.

-- 0 to 100 in increments of 5. **100 is default**.

- **EQ Mid** [genesis_plus_gx_audio_eq_mid] - Adjust the mid range band of the internal audio equalizer.

-- 0 to 100 in increments of 5. **100 is default**.

- **EQ High** [genesis_plus_gx_audio_eq_high] - Adjust the high range band of the internal audio equalizer.

-- 0 to 100 in increments of 5. **100 is default**.

### Input
_________________
Change light gun and/or mouse input settings.

- **Light Gun Input** [genesis_plus_gx_gun_input] - Use a mouse-controlled 'Light Gun' or 'Touchscreen' input.

-- **Light Gun [lightgun]** - Selects mouse-controlled 'Light Gun' input (devices will use RetroLightgun inputs).
-- Touchscreen [touchscreen] - Allows the MS Light Phaser, MD Menancer and MD Justifiers device types to be controlled via touchscreen input (devices will use RetroPointer inputs instead).

- **Show Light Gun Crosshair** [genesis_plus_gx_gun_cursor] - Display light gun crosshairs when using the MD Menacer, MD Justifiers and MS Light Phaser input device types.

??? note "*Lightgun crosshair - On [enabled]*"
    ![](../image/core/genesis_plus_gx/lightgun.png)

- **Invert Mouse Y-Axis** [genesis_plus_gx_invert_mouse] - Inverts the Y-axis of the 'MD Mouse' input device type.

-- **Off [disabled]** - Enables Y-Axis inversion.
-- On [enabled] - Disables Y-Axis inversion.

### Emulation Hacks
_________________
Change processor overclocking and emulation accuracy settings that affect low-level performance and compatibility.

- **Remove Per-Line Sprite Limit** [genesis_plus_gx_no_sprite_limit] - Removes the original sprite-per-scanline hardware limit. This reduces flickering but can cause visual glitches, as some games exploit the hardware limit to generate special effects.

-- **Off [disabled]** - Keeps the per-line sprite limit.
-- On [enabled] - Disables the per-line sprite limit.

- **Enhanced per-tile vertical scroll** [genesis_plus_gx_enhanced_vscroll] - Allows each individual cell to be scrolled vertically, instead of 16px 2-cell, by averaging out with the vscroll value of the neighbouring cell. This hack only applies to few games that use 2-cell vertical scroll mode.

-- **Off [disabled]** - Enables enhanced per-tile vertical scrolling.
-- On [enabled] - Disables enhanced per-tile vertical scrolling.

- **Enhanced per-tile vertical scroll limit** [genesis_plus_gx_enhanced_vscroll_limit] - Only when the Enhanced per-tile vertical scroll core option is enabled. Adjusts the limit of the vertical scroll enhancement. When the vscroll difference between neighbouring tiles is bigger than this limit, the enhancement is disabled.

-- 2 to 16 in increments of 1. **8 is default**

- **CPU Speed** [genesis_plus_gx_overclock] - Overclock the emulated CPU. Can reduce slowdown, but may cause glitches. The 'CPU Speed' core option only appears when the Genesis Plus GX core was compiled with the [HAVE_OVERCLOCK](https://github.com/libretro/Genesis-Plus-GX/blob/master/libretro/libretro.c) flag.

-- 100% to 500% in increments of 25%. **100% is default.**

- **System Locks-Ups** [genesis_plus_gx_force_dtack] - Emulate system lock-ups that occur on real hardware when performing illegal address access. This should only be disabled when playing certain demos and homebrew that rely on illegal behavior for correct operation.

-- **On [enabled]** - Enables emulation of system lock-ups.
-- Off [disabled] - Disables emulation of system lock-ups.

- **68K Address Error** [genesis_plus_gx_addr_error] - The [Mega Drive/Genesis main CPU (Motorola 68000)](http://segaretro.org/M68000) generates an Address Error exception (crash) when attempting to perform unaligned memory access. Enabling this will simulate this behavior. It should only be disabled when playing ROM hacks, since these are typically developed using less accurate emulators and may rely on invalid RAM access for correct operation.

-- **On [enabled]** - Enables simulation of 68K Address Error.
-- Off [disabled] - Disables simulation of 68K Address Error.

- **CD access time** [genesis_plus_gx_cd_latency] - Simulate [original CD hardware latency](https://segaretro.org/Sega_Mega-CD/Technical_specifications#Storage) when initiating a read or seeking to a specific location on loaded disc. This is required by a few CD games that crash if CD data is available too soon and also fixes CD audio desync issues in some games. Disabling this can be useful with [MSU-MD games](https://emulation.gametechwiki.com/index.php/Sega_Genesis_emulators#Mega_Drive_Plus_.2F_Genesis_Plus_.2F_MSU-MD_modes) as it makes CD audio tracks loops more seamless.

-- **On [enabled]** - Enables simulation of original CD hardware latency.
-- Off [disabled] - Disables simulation of original CD hardware latency.

### Advanced Channel Volume Settings
_________________
Change the volume of individual hardware audio channels.

- **Show Advanced Audio Volume Settings (Reopen menu)** [genesis_plus_gx_show_advanced_audio_settings] - Enable configuration of low-level audio channel parameters. NOTE: Quick Menu must be toggled for this setting to take effect.  The 'Show Advanced Audio Volume Settings' core option only appears when the Genesis Plus GX core was compiled with the [USE_PER_SOUND_CHANNELS_CONFIG flag being set to 1](https://github.com/libretro/Genesis-Plus-GX/blob/master/Makefile.libretro).

-- **On [enabled]** - Enables configuration of low-level audio channel parameters.
-- Off [disabled] - Disables configuration of low-level audio channel parameters.

- **PSG Tone Channel 0 Volume %** [genesis_plus_gx_psg_channel_0_volume] - Reduce the volume of the [PSG Tone Channel](https://segaretro.org/Sega_Mega_Drive/Technical_specifications#Audio) 0.

-- 0% to 100% in increments of 10%. **100% is default**.

- **PSG Tone Channel 1 Volume %** [genesis_plus_gx_psg_channel_1_volume] - Reduce the volume of the [PSG Tone Channel](https://segaretro.org/Sega_Mega_Drive/Technical_specifications#Audio) 1.

-- 0% to 100% in increments of 10%. **100% is default**.

- **PSG Tone Channel 2 Volume %** [genesis_plus_gx_psg_channel_2_volume] - Reduce the volume of the [PSG Tone Channel](https://segaretro.org/Sega_Mega_Drive/Technical_specifications#Audio) 2.

-- 0% to 100% in increments of 10%. **100% is default**.

- **PSG Tone Channel 3 Volume %** [genesis_plus_gx_psg_channel_3_volume] - Reduce the volume of the [PSG Tone Channel](https://segaretro.org/Sega_Mega_Drive/Technical_specifications#Audio) 3.

-- 0% to 100% in increments of 10%. **100% is default**.

- **Mega Drive/Genesis FM Channel 0 Volume %** [genesis_plus_gx_md_channel_0_volume] - Reduce the volume of the [Mega Drive/Genesis FM Channel](https://segaretro.org/Sega_Mega_Drive/Technical_specifications#Audio) 0. Only works with MAME FM emulators (Mega Drive/Genesis FM core option).

-- 0% to 100% in increments of 10%. **100% is default**.

- **Mega Drive/Genesis FM Channel 1 Volume %** [genesis_plus_gx_md_channel_1_volume] - Reduce the volume of the [Mega Drive/Genesis FM Channel](https://segaretro.org/Sega_Mega_Drive/Technical_specifications#Audio) 1. Only works with MAME FM emulators (Mega Drive/Genesis FM core option).

-- 0% to 100% in increments of 10%. **100% is default**.

- **Mega Drive/Genesis FM Channel 2 Volume %** [genesis_plus_gx_md_channel_2_volume] - Reduce the volume of the [Mega Drive/Genesis FM Channel](https://segaretro.org/Sega_Mega_Drive/Technical_specifications#Audio) 2. Only works with MAME FM emulators (Mega Drive/Genesis FM core option).

-- 0% to 100% in increments of 10%. **100% is default**.

- **Mega Drive/Genesis FM Channel 3 Volume %** [genesis_plus_gx_md_channel_3_volume] - Reduce the volume of the [Mega Drive/Genesis FM Channel](https://segaretro.org/Sega_Mega_Drive/Technical_specifications#Audio) 3. Only works with MAME FM emulators (Mega Drive/Genesis FM core option).

-- 0% to 100% in increments of 10%. **100% is default**.

- **Mega Drive/Genesis FM Channel 4 Volume %** [genesis_plus_gx_md_channel_4_volume] - Reduce the volume of the [Mega Drive/Genesis FM Channel](https://segaretro.org/Sega_Mega_Drive/Technical_specifications#Audio) 4. Only works with MAME FM emulators (Mega Drive/Genesis FM core option).

-- 0% to 100% in increments of 10%. **100% is default**.

- **Mega Drive/Genesis FM Channel 5 Volume %** [genesis_plus_gx_md_channel_5_volume] - Reduce the volume of the [Mega Drive/Genesis FM Channel](https://segaretro.org/Sega_Mega_Drive/Technical_specifications#Audio) 5. Only works with MAME FM emulators (Mega Drive/Genesis FM core option).

-- 0% to 100% in increments of 10%. **100% is default**.

- **Master System FM (YM2413) Channel 0 Volume %** [genesis_plus_gx_sms_fm_channel_0_volume] - Reduce the volume of the [Master System FM Channel](https://segaretro.org/Sega_Master_System/Technical_specifications#Audio) 0.

-- 0% to 100% in increments of 10%. **100% is default**.

- **Master System FM (YM2413) Channel 1 Volume %** [genesis_plus_gx_sms_fm_channel_1_volume] - Reduce the volume of the [Master System FM Channel](https://segaretro.org/Sega_Master_System/Technical_specifications#Audio) 1.

-- 0% to 100% in increments of 10%. **100% is default**.

- **Master System FM (YM2413) Channel 2 Volume %** [genesis_plus_gx_sms_fm_channel_2_volume] - Reduce the volume of the [Master System FM Channel](https://segaretro.org/Sega_Master_System/Technical_specifications#Audio) 2.

-- 0% to 100% in increments of 10%. **100% is default**.

- **Master System FM (YM2413) Channel 3 Volume %** [genesis_plus_gx_sms_fm_channel_3_volume] - Reduce the volume of the [Master System FM Channel](https://segaretro.org/Sega_Master_System/Technical_specifications#Audio) 3.

-- 0% to 100% in increments of 10%. **100% is default**.

- **Master System FM (YM2413) Channel 4 Volume %** [genesis_plus_gx_sms_fm_channel_4_volume] - Reduce the volume of the [Master System FM Channel](https://segaretro.org/Sega_Master_System/Technical_specifications#Audio) 4.

-- 0% to 100% in increments of 10%. **100% is default**.

- **Master System FM (YM2413) Channel 5 Volume %** [genesis_plus_gx_sms_fm_channel_5_volume] - Reduce the volume of the [Master System FM Channel](https://segaretro.org/Sega_Master_System/Technical_specifications#Audio) 5.

-- 0% to 100% in increments of 10%. **100% is default**.

- **Master System FM (YM2413) Channel 6 Volume %** [genesis_plus_gx_sms_fm_channel_6_volume] - Reduce the volume of the [Master System FM Channel](https://segaretro.org/Sega_Master_System/Technical_specifications#Audio) 6.

-- 0% to 100% in increments of 10%. **100% is default**.

- **Master System FM (YM2413) Channel 7 Volume %** [genesis_plus_gx_sms_fm_channel_7_volume] - Reduce the volume of the [Master System FM Channel](https://segaretro.org/Sega_Master_System/Technical_specifications#Audio) 7.

-- 0% to 100% in increments of 10%. **100% is default**.

- **Master System FM (YM2413) Channel 8 Volume %** [genesis_plus_gx_sms_fm_channel_8_volume] - Reduce the volume of the [Master System FM Channel](https://segaretro.org/Sega_Master_System/Technical_specifications#Audio) 8.

-- 0% to 100% in increments of 10%. **100% is default**.

## User 1 device types

The Genesis Plus GX core supports the following device type(s) in the controls menu, bolded device types are the default for the specified user(s):

- Joypad Port Empty - None - No device is connected; input is disabled.
- **Joypad Auto** - Joypad - Depending on the loaded [game's ROM information](https://raw.githubusercontent.com/ekeeke/Genesis-Plus-GX/master/core/loadrom.c), the core will automatically emulate a MD Joypad 3 Button controller, or a MD Joypad 6 Button controller or a MS Joypad 2 Button controller.
- [MD Joypad 3 Button](https://segaretro.org/Control_Pad_(Mega_Drive)) - Joypad
- [MD Joypad 6 Button](https://segaretro.org/Six_Button_Control_Pad_(Mega_Drive)) - Joypad
- [MS Joypad 2 Button](https://segaretro.org/Control_Pad_(Master_System)) - Joypad - Also used for Game Gear.
- [MD Joypad 3 Button + 4-WayPlay](https://segaretro.org/4_Way_Play) - Joypad - Enables multitap for 4-WayPlay games.
- [MD Joypad 6 Button + 4-WayPlay](https://segaretro.org/4_Way_Play) - Joypad - Enables multitap for 4-WayPlay games.
- [MD Joypad 3 Button + Teamplayer](https://segaretro.org/Team_Player) - Joypad - Enables multitap for Teamplayer games.
- [MD Joypad 6 Button + Teamplayer](https://segaretro.org/Team_Player) - Joypad - Enables multitap for Teamplayer games.
- MS Joypad 2 Button + Master Tap - Joypad - Enables [Furrtek's Master Tap](https://www.smspower.org/Homebrew/BOoM-SMS) (unofficial mulitap device).
- [MS Light Phaser](https://segaretro.org/Light_Phaser) - Lightgun
- [MS Paddle Control](https://segaretro.org/Paddle_Control) - Analog
- [MS Sports Pad](https://segaretro.org/Sports_Pad) - Analog
- [MS Graphic Board](https://segaretro.org/Sega_Graphic_Board) - Pointer
- [MD XE-1AP](https://segaretro.org/XE-1_AP) - Analog
- [MD Mouse](https://segaretro.org/Sega_Mouse) - Mouse

## User 2 device types

- Joypad Port Empty - None - No device is connected; input is disabled.
- **Joypad Auto** - Joypad - Depending on the loaded [game's ROM information](https://raw.githubusercontent.com/ekeeke/Genesis-Plus-GX/master/core/loadrom.c), the core will automatically emulate a MD Joypad 3 Button controller, or a MD Joypad 6 Button controller or a MS Joypad 2 Button controller.
- [MD Joypad 3 Button](https://segaretro.org/Control_Pad_(Mega_Drive)) - Joypad
- [MD Joypad 6 Button](https://segaretro.org/Six_Button_Control_Pad_(Mega_Drive)) - Joypad
- [MS Joypad 2 Button](https://segaretro.org/Control_Pad_(Master_System)) - Joypad - Also used for Game Gear.
- [MD Joypad 3 Button + 4-WayPlay](https://segaretro.org/4_Way_Play) - Joypad - Enables multitap for 4-WayPlay games.
- [MD Joypad 6 Button + 4-WayPlay](https://segaretro.org/4_Way_Play) - Joypad - Enables multitap for 4-WayPlay games.
- [MD Joypad 3 Button + Teamplayer](https://segaretro.org/Team_Player) - Joypad - Enables multitap for Teamplayer games.
- [MD Joypad 6 Button + Teamplayer](https://segaretro.org/Team_Player) - Joypad - Enables multitap for Teamplayer games.
- MS Joypad 2 Button + Master Tap - Joypad - Enables [Furrtek's Master Tap](https://www.smspower.org/Homebrew/BOoM-SMS) (unofficial mulitap device).
- [MD Menancer](https://segaretro.org/Menacer) - Lightgun
- [MD Justifiers](https://segaretro.org/The_Justifier)  - Lightgun
- [MS Light Phaser](https://segaretro.org/Light_Phaser) - Lightgun
- [MS Paddle Control](https://segaretro.org/Paddle_Control) - Analog
- [MS Sports Pad](https://segaretro.org/Sports_Pad) - Analog
- [MS Graphic Board](https://segaretro.org/Sega_Graphic_Board) - Pointer
- [MD XE-1AP](https://segaretro.org/XE-1_AP) - Analog
- [MD Mouse](https://segaretro.org/Sega_Mouse) - Mouse

## Other devices

- [PICO tablet](https://segaretro.org/Sega_Pico) - The Genesis Plus GX core can emulate PICO tablet inputs but this is done automatically, based on the loaded [game's ROM information](https://raw.githubusercontent.com/ekeeke/Genesis-Plus-GX/master/core/loadrom.c) and cannot be manually selected as a device type.
- [Terebi Oekaki tablet](https://segaretro.org/Terebi_Oekaki) - The Genesis Plus GX core can emulate Terebi Oekaki table inputs but this is done automatically, based on the loaded [game's ROM information](https://raw.githubusercontent.com/ekeeke/Genesis-Plus-GX/master/core/loadrom.c) and cannot be manually selected as a device type.

## Multitap

Activating multitap support in compatible games can be configured by the 4-WayPlay, Teamplayer, Master Tap device types for either the [User 1](#user-1-device-types) or [User 2](#user-2-device-types) ports.

## Joypad

| RetroPad Inputs                                | User 1 - 8 input descriptors | [MD Joypad 3 Button](https://segaretro.org/Control_Pad_(Mega_Drive)) | [MD Joypad 6 Button](https://segaretro.org/Six_Button_Control_Pad_(Mega_Drive)) | [MS Joypad 2 Button](https://segaretro.org/Control_Pad_(Master_System)) | [MS Paddle Control](https://segaretro.org/Paddle_Control) | [MS Sports Pad](https://segaretro.org/Sports_Pad) | [MD XE-1AP](https://segaretro.org/XE-1_AP)     |
|------------------------------------------------|------------------------------|--------------------|--------------------|--------------------|-------------------|---------------|---------------|
| ![](../image/retropad/retro_b.png)             | B                            | B                  | B                  | 1                  | 1                 | 1             | E2            |
| ![](../image/retropad/retro_y.png)             | A                            | A                  | A                  |                    |                   |               | E1            |
| ![](../image/retropad/retro_select.png)        | Mode                         |                    | Mode               |                    |                   |               | Select        |
| ![](../image/retropad/retro_start.png)         | Start                        | Start              | Start              | Start              | Start             | Start         | Start         |
| ![](../image/retropad/retro_dpad_up.png)       | D-Pad Up                     | D-Pad Up           | D-Pad Up           | D-Pad Up           |                   |               |               |
| ![](../image/retropad/retro_dpad_down.png)     | D-Pad Down                   | D-Pad Down         | D-Pad Down         | D-Pad Down         |                   |               |               |
| ![](../image/retropad/retro_dpad_left.png)     | D-Pad Left                   | D-Pad Left         | D-Pad Left         | D-Pad Left         |                   |               |               |
| ![](../image/retropad/retro_dpad_right.png)    | D-Pad Right                  | D-Pad Right        | D-Pad Right        | D-Pad Right        |                   |               |               |
| ![](../image/retropad/retro_a.png)             | C                            | C                  | C                  | 2                  |                   | 2             |               |
| ![](../image/retropad/retro_x.png)             | Y                            |                    | Y                  |                    |                   |               |               |
| ![](../image/retropad/retro_l1.png)            | X                            |                    | X                  |                    |                   |               | C             |
| ![](../image/retropad/retro_r1.png)            | Z                            |                    | Z                  |                    |                   |               | A             |
| ![](../image/retropad/retro_l2.png)            |                              |                    |                    |                    |                   |               | D             |
| ![](../image/retropad/retro_r2.png)            |                              |                    |                    |                    |                   |               | B             |
| ![](../image/retropad/retro_l3.png)            |                              |                    |                    |                    |                   |               |               |
| ![](../image/retropad/retro_r3.png)            |                              |                    |                    |                    |                   |               |               |
| ![](../image/retropad/retro_left_stick.png) X  |                              |                    |                    |                    | Paddle            | Trackball X   | Thumb-stick X |
| ![](../image/retropad/retro_left_stick.png) Y  |                              |                    |                    |                    |                   | Trackball Y   | Thumb-stick Y |
| ![](../image/retropad/retro_right_stick.png) X |                              |                    |                    |                    |                   |               | Slider Y      |
| ![](../image/retropad/retro_right_stick.png) Y |                              |                    |                    |                    |                   |               | Slider X      |

## Mouse

| RetroMouse Inputs                                     | [MD Mouse](https://segaretro.org/Sega_Mouse)        |
|-------------------------------------------------------|-----------------|
| ![](../image/retromouse/retro_mouse.png) Mouse Cursor | MD Mouse Cursor |
| ![](../image/retromouse/retro_left.png) Mouse 1       | MD Mouse Left   |
| ![](../image/retromouse/retro_right.png) Mouse 2      | MD Mouse Right  |
| ![](../image/retromouse/retro_middle.png) Mouse 3     | MD Mouse Start  |
| Wheel Down                                            | MD Mouse Center |

## Pointer

| RetroPointer Inputs                                                                                                    | [MS Graphic Board](https://segaretro.org/Sega_Graphic_Board)        |
|------------------------------------------------------------------------------------------------------------------------|-------------------------|
| ![](../image/retromouse/retro_mouse.png) or ![](../image/Button_Pack/Gestures/Gesture_Finger_Front.png) Pointer Position | MS Graphic Board Stylus |
| ![](../image/retromouse/retro_left.png) Mouse 1                                                                        | MS Graphic Board Pen    |
| ![](../image/retromouse/retro_right.png) Mouse 2                                                                       | MS Graphic Board Menu   |
| ![](../image/retromouse/retro_middle.png) Mouse 3                                                                      | MS Graphic Do           |

## Lightgun

| RetroLightgun Inputs                                   | [MD Menacer](https://segaretro.org/Menacer)           | [MD Justifier](https://segaretro.org/The_Justifier)           | [MS Light Phaser](https://segaretro.org/Light_Phaser)           |
|--------------------------------------------------------|----------------------|------------------------|---------------------------|
| ![](../image/retromouse/retro_mouse.png) Gun Crosshair | MD Menacer Crosshair | MD Justifier Crosshair | MS Light Phaser Crosshair |
| Gun Trigger                                            | MD Menacer A         | MD Justifier A         | MS Light Phaser A         |
| Gun Aux A                                              | MD Menacer B         | MD Justifer B          | MS Light Phaser B         |
| Gun Aux B                                              | MD Menacer C         | MD Justifer C          | MS Light Phaser C         |
| Gun Start                                              | MD Menacer Start     | MD Justifer Start      | MS Light Phaser Start     |

## Other

| Inputs                                                                                                                   | [PICO tablet](https://segaretro.org/Sega_Pico)               | [Terebi Oekaki tablet](https://segaretro.org/Terebi_Oekaki)      |
|--------------------------------------------------------------------------------------------------------------------------|---------------------------|---------------------------|
| ![](../image/retromouse/retro_mouse.png) or ![](../image/Button_Pack/Gestures/Gesture_Finger_Front.png) Pointer Position | PICO tablet Stylus        | Terebi Oeka tablet Stylus |
| ![](../image/retromouse/retro_left.png) Mouse 1                                                                          | PICO tablet Pen           | Terebi Oeka tablet Pen    |
| ![](../image/retromouse/retro_right.png) Mouse 2                                                                         | PICO tablet Red           |                           |
| ![](../image/retromouse/retro_middle.png) Mouse 3                                                                        |                           | Terebo Peka tablet Start  |
| Wheel Up                                                                                                                 | PICO tablet Previous page |                           |
| Wheel Down                                                                                                               | PICO tablet Next page     |                           |
| ![](../image/retropad/retro_dpad_up.png)                                                                                 | PICO tablet Up (White)    |                           |
| ![](../image/retropad/retro_dpad_down.png)                                                                               | PICO tablet Down (Orange) |                           |
| ![](../image/retropad/retro_dpad_left.png)                                                                               | PICO tablet Left (Purple) |                           |
| ![](../image/retropad/retro_dpad_right.png)                                                                              | PICO tablet Right (Green) |                           |

## External Links

- [Official Genesis Plus GX Github Repository](https://github.com/ekeeke/Genesis-Plus-GX)
- [Libretro Genesis Plus GX Core Info File](https://github.com/libretro/libretro-super/blob/master/dist/info/genesis_plus_gx_libretro.info)
- [Libretro Genesis Plus GX Github Repository](https://github.com/libretro/Genesis-Plus-GX)
- [Report Libretro Genesis Plus GX Core Issues Here](https://github.com/libretro/Genesis-Plus-GX/issues)
- [Gameplay Videos Playlist](https://www.youtube.com/playlist?list=PLRbgg4gk_0If0UWkhjPbRmWUBcGaRiPZt)

## Sega 16-bit

- [Sega - Master System (Emux SMS)](emux_sms.md)
- [Sega - MS/MD/CD/32X (PicoDrive)](picodrive.md)
- [Sega - MS/GG/SG-1000 (Gearsystem)](gearsystem.md)
- [MSX/SVI/ColecoVision/SG-1000 (blueMSX)](bluemsx.md)
