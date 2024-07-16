<!--
    SPDX-FileCopyrightText: Copyright (C) swift Project Community / Contributors
    SPDX-License-Identifier: GFDL-1.3-only
-->

In **General** you will find a list of things that are required regardless of your Operating System or flight simulator platforms used.
The rest of this chapter deals with items that are specific to OS and flight simulator platforms.

##  General
* Are there any **CSL or AI aircraft models installed**? Download Models.
* Have you **created a Model Set** with the help of the Configuration Wizard? [First Model Set](./install/configure_xp.md)
* If you don't mind, **[enable crashdump reports](./../troubleshooting/crash_reports.md)** to help developers analyze the cause of crashes
* **Close other pilot clients**, so the voice port is not blocked. **X-Plane** users need to make sure that **[plugins of other online flying clients](./../troubleshooting/faq/xp_landing_gear/index.md) are completely disabled**
* **Do not touch** the **gnd.flag** and **fast position settings** unless you know what you are doing!
* **Do not** run *swift*Core and *swift*GUI in **standalone mode** on the same computer.
  *swift*Core is **only** needed by users who want to run *swift* in [Distributed Mode (on a remote computer)](./../documentation/distributed.md).
* Do you get **model validation errors** on program startup?
  If there are **a lot** of validation error messages, something in your setup may be wrong: [Help Page](./../documentation/flying/why_validation_errors.md).
* Make sure malware protection allows *swift* to run.
  "Acronis TrueImage Active protection" and similar programs may be interfering


## OS specific

### macOS
* Enable the microphone for *swift*: [Help Page](./../troubleshooting/no_sound_macos.md)


### Windows
* make sure swift can access your microphone: [Help Page](./../troubleshooting/no_microphone_windows.md)

### Linux
* Hotkeys: We read keyboard and joystick stuff from ``/dev/input/event`` and ``js``.
  Those files have to be readable by your user: [Help Page](./../troubleshooting/linux_hotkeys.md)

## Flight Simulator specific

### X-Plane 11
*swift* is compatible with OpenGL and Vulkan/Metal.
X-Plane has seen significant internal changes, as a consequence you have to use specific verisons of *swift* to correctly display aircraft and to have an operational TCAS!
Until including **X-Plane 11.41** you have to use *swift* **version 0.9.4.389**. From **X-Plane 11.50** download and install *swift* **0.9.5.x or newer**.

* use the **64bit version** of *swift*
* make sure **xswiftbus** is installed and that its **version number is identical** with the one of *swift*GUI
* traffic plugins and other pilot clients for X-Plane will interfere with *xswiftbus* and need to be properly deactivated or removed from the plugins folder.
  [More info](./../troubleshooting/faq/xp_landing_gear/index.md)
* CSL models must be installed inside the folder of X-Plane, it is advisable to avoid spaces and special characters in the file paths.
  [More information and recommendations](./models/xplane/index.md#recommended-installation-practices)
* if your BlueBell Models are being displayed inside the ground or floating above it, download and install the latest version of them, it already contains a fix for this: [More information](./models/xplane/index.md#recommended-installation-practices)

### FSX & P3D

* use *swift* 32bit for FSX and P3D v1-v3, *swift* 64bit for P3D v4 and newer
* P3D: to use external model directories (not in ``SimObjects``) add this directory in your [simulator settings](./install//fsx_p3d/index.md#select-your-simulators)
* FSX & P3D v1-v3: make sure that the **terrain probe** is installed: [Help Page](./install/fsx_p3d/install_terrain_probe.md)
* enable [Simconnect Offsets](./../documentation/flying/settings/simconnect_sb4_offsets.md) in the driver settings if you want to use ATC Transponder updates from PMDG and other aircraft
* you **cannot connect** *swift* to P3D or FSX?
  If you run P3D/FSX **as Admin**, then run *swift* **as Admin** as well
* FSX and some P3D versions cannot handle all frequencies with **8.33 kHz spacing**.
  Such frequencies can only be tuned through the swift UI.
  In this case, your radio within the simulator might show a different frequency than selected within swift.
  However, the frequency used to receive and transmit voice is always the frequency shown within swift.

### FS9

* make sure **FSUIPC is installed**, *swift* needs FSUIPC to work properly
* if you run FS9/FSUIPC **as Admin**, run *swift* **as Admin** as well
* since Windows 10 Update 1909, the **automatic connect function** between *swift* and FS9 may **not** work anymore.
  You will have to **[connect FS9 manually](./../troubleshooting/connect_fs9_manually.md)**
* consider the **Ground Elevation** recording: [Help Page](./install/fs9/fs9_ground_elevation.md)
* The COM frequencies selected within FS9 are **not synchronized** with swift.
  You must tune the frequencies through the swift UI.
