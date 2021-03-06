<!--
    SPDX-FileCopyrightText: Copyright (C) swift Project Community / Contributors
    SPDX-License-Identifier: GFDL-1.3-only
-->

## General

- *swift* has **no hot plug and play for all types yet,** some sound hardware needs to be plugged in/on before starting *swift*
- is the device correctly selected in the settings? [Audio page](./../documentation/swift_gui/audio_page.md)
- make sure the *swift* volume ist `100%` and voice not muted in *swift*
- **check your PTT button**
    - Is the PTT button defined, see [here](./../documentation/swift_gui/settings_page.md#hotkeys)
    - Does it work, If you press it, do you see the LED flashing?
    - If it is defined but does NOT work, remove it and add it again!
- on **MacOSX** [make sure mic privilege is granted](./no_sound_macos.md).
- **Linux**: We read keyboard and joystick stuff from `/dev/input/event*` and `js*`. Those files have to be readable by your user. See [this page](./linux_hotkeys.md)
- **Windows**: [Microphone not working on Windows](./no_microphone_windows.md)
- **Is loopback working**? If not, this would mean some issue of *swift* and your hardware.
   You would need to have RX2 enabled to hear loopback

    ![](./../img/loopback.jpg){: style="width:70%"}

- Make sure TX/RX (transmit/receive are enabled).
  If you sync. swift with your aircraft cockpit and your cockpit COM units are disabled, this can be your COM unit is "disabled".
  See [here](./../documentation/flying/integrated_com.md).
- **Check yourself on the AFV map**: <https://afv-map.vatsim.net/> Is your callsign shown, and your frequencies correct?

## Sample rate

*swift* uses the following values for output and tries to find the closest audio setup on your machine.
It might help to adjust your sample rates (Google for "Windows Audio sample rate").

```cpp
outputFormat.setSampleRate(48000);
outputFormat.setChannelCount(1);
outputFormat.setSampleSize(32);
outputFormat.setSampleType(QAudioFormat::Float);
outputFormat.setByteOrder(QAudioFormat::LittleEndian);
outputFormat.setCodec("audio/pcm");
```

```cpp
inputFormat.setSampleRate(m_sampleRate); // normally 48000
inputFormat.setChannelCount(1);
inputFormat.setSampleSize(16);
inputFormat.setSampleType(QAudioFormat::SignedInt);
inputFormat.setByteOrder(QAudioFormat::LittleEndian);
inputFormat.setCodec("audio/pcm");
```

## Changing the driver (Windows only, WASAPI)

*swift* for Windows comes with two audio plugins, WASAPI and a Windows plugin.
You can remove one of those and try which works better for you.
**Just move them to another directory** (outside swift), so you can copy them back if needed.

- Go into your swift installation bin path (e.g. `C:\Program Files\swift-0.9.3-64bit\bin`).
- Change to subfolder `audio`
- Since *swift* 0.9.4.206 we have disabled the WASAPI driver, you can find them here (just copy them in the directory, use the 32 or 64bit version as required by your installation).

    ![](./../img/wasapidriver.jpg){: style="width:70%"}

To remove:

- Find dlls containing "wasapi" or "windows"
- Move them to a backup directory outside swift
- So as a result, you SHALL have only the "wasapi" **OR** the "windows" ones in the `audio` subdir
