# WinMM Patch

This guide will help you install OmniMIDI and patch PFA.

## Downloading OmniMIDI

> TODO: Move OmniMIDI set up to its own guide

To download OmniMIDI, click [here](https://github.com/KeppySoftware/OmniMIDI/releases/download/14.8.5.0/OmniMIDISetup.exe) to download the latest setup as of 1/10/2024.

## Adding soundfonts

After installing OmniMIDI and opening the configurator, its time to add a soundfont so the synth has audio.

First, click the + in the configurator window.

![Configurator window](https://github.com/GreenWeegeeCantCode/Black-MIDI-Guides/blob/main/docs/Piano%20From%20Above/images/AddingSFs.png)

Next, select the soundfont you want and press open. Now you have a soundfont that will be used in applications that use the synth!

## Patching PFA

In the configurator window, go to "extensions" and select "Windows Multimedia Wrapper"
Select "Patch an application" below the standard performance improvement patch.
Then, go to where your PFA exe is, select it and it should be patched.

??? note "Why can't I patch it?"

    If it says you dont have the permissions to do this, press OK and run the configurator as an administrator. (The configurator should automatically run it as an admin after clicking OK)
