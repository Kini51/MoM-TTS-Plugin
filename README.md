# MoM TTS Plugin

**MoM TTS** is an unofficial TTS audio plugin for the PC version of **Mansions of Madness: Second Edition**.

The plugin adds pre-rendered voice audio to the game by playing prepared sound files when matching in-game text events appear. It is designed for the official PC version of the game and supports the official scenarios/adventures included in the app.

This project does **not** generate speech in real time.
All voice lines are pre-baked and distributed as packaged audio files.

## Features

* TTS-style voice playback for in-game text events
* Pre-rendered audio files for supported official scenarios
* Language-based audio package structure
* Packed audio files instead of loose WAV files
* BepInEx-based plugin for the Windows PC version

## Current Language Support

Currently available:

* German (`_de`)

Planned:

* English (`_en`) is planned to follow later, most likely around Q4 2026.

Other languages are currently not planned. If active development of this project stops at some point, the source code and/or required project information may be made available so that others can continue the work or add additional languages.

Tested with:

* **Mansions of Madness: Second Edition**
* Official PC version
* **BepInEx 5.4.23.4**
* Unity runtime shown by the game log: **Unity 2022.3.62**
* Windows 64-bit

The plugin is made for the official app and the official scenarios/adventures. It is not guaranteed to work with modified versions of the game.

## Valkyrie Mod Support

Support for the **Valkyrie** mod/tool may be investigated in the future.

At the moment, there is no guarantee that this plugin will work with Valkyrie or that Valkyrie support will be added.

## How to Use

### 1. Install Mansions of Madness

Install the official PC version of **Mansions of Madness: Second Edition**, for example through Steam.

Start the game once before installing the plugin, then close it again.

### 2. Download BepInEx

Download **BepInEx 5.4.23.4 or newer BepInEx 5.x x86** from the official BepInEx release page:

[Download BepInEx releases](https://github.com/BepInEx/BepInEx/releases)

Use the Windows x86 version, x64 won't work!

Do **not** use BepInEx 6 unless this plugin explicitly states support for it.

```text
Mansions of Madness/
├─ BepInEx/
│  ├─ config/
│  ├─ plugins/
│  └─ LogOutput.log
├─ Mansions of Madness.exe
└─ ...
```

### 3. Download the Plugin and Language Package

Download the latest plugin release from the GitHub **Releases** section.

You need:

* the plugin package
* at least one language package, for example German (`_de`)

The release packages already contain the correct folder structure.

### 4. Copy the Plugin and Sound Files

Copy the downloaded files into the BepInEx plugin folder.

The final structure should look like this:

```text
Mansions of Madness/
└─ BepInEx/
   └─ plugins/
      └─ MoMTTS/
         ├─ MoMTTS.dll
         └─ tts/
            └─ _de/
               ├─ localization_de.momtts
               ├─ scenario_escape_from_innsmouth_mad20_de.momtts
               ├─ scenario_cycle_of_eternity_mad20_de.momtts
               ├─ scenario_shattered_bonds_mad20_de.momtts
               ├─ scenario_rising_tide_mad20_de.momtts
               └─ ...
```

### 5. Start the Game

Start Mansions of Madness normally.

If everything is installed correctly, the plugin should load automatically and play the matching voice lines during the game.


## Audio Package Protection

The sound files are not distributed as loose audio files.

They are packaged and protected so that they are only intended to work with this plugin and the official Mansions of Madness PC application. This is meant to prevent direct casual extraction, redistribution, or reuse of the individual sound files outside the intended plugin environment.

The goal of this protection is also to avoid making game-related content available as a standalone audio archive. The audio packages are not meant to be used outside this plugin and are only useful together with the official Mansions of Madness PC application.

## Notes

This is an unofficial fan-made project.

It is not affiliated with, endorsed by, sponsored by, or approved by Fantasy Flight Games, Asmodee, or any other rights holder of Mansions of Madness.

Mansions of Madness and all related names, scenarios, texts, trademarks, and assets belong to their respective owners.

This plugin requires the official PC application to be useful and does not replace the original game.
