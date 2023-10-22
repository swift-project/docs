<!--
    SPDX-FileCopyrightText: Copyright (C) swift Project Community / Contributors
    SPDX-License-Identifier: GFDL-1.3-only
-->

On top of *swift*GUI you will find a **status bar** that is comprised of a number of **virtual LEDs** (=status lights).

![](./../../img/manual_swiftgui_statusbar.jpg){: style="width:70%"}

## Transponder
On the far left you can verify the current status of your **ATC Transponder**


|||
|-|-|
| ![](./../../img/manual_swiftgui_statusbar_xpdr_stby.jpg){: style="width:20%"} | **STBY** = standby, transponder is not transmitting data |
| ![](./../../img/manual_swiftgui_statusbar_xpdr_on.jpg){: style="width:20%"} | **CHARLIE** = ON, transponder is transmitting data |
| ![](./../../img/manual_swiftgui_statusbar_xpdr_ident.jpg){: style="width:20%"} | **IDENT** = ident-mode is activated temporarily |


Preferably you will **operate the transponder panel in the cockpit of your flight simulator platform**.
*swift* is synchronized to it and code and mode changes should occur accordingly.

Should the transponder panel of your virtual aircraft not be compatible with *swift*, then you can toggle between STBY and ON modes manually by clicking on the transponder light in in the status bar or in the Cockpit Widget of *swift*GUI.
If you need to change your transponder code or select IDENT, then this can be done in the Cockpit Widget, too.
There's a quick access IDENT button as well.

![](./../../img/manual_swiftgui_statusbar_xpdr_cockpit.jpg){: style="width:25%"}

|||
|-|-|
| ![](./../../img/manual_swiftgui_statusbar_network.jpg) |The network status light indicates whether you are connected to a server or not (= offline). The screenshot features the LED being OFF. |
| ![](./../../img/manual_swiftgui_statusbar_simulator.jpg) |This LED will only light up, when *swift*GUI is connected to your flight simulator platform. |
| ![](./../../img/manual_swiftgui_statusbar_mapperready.jpg) |This just means that the aircraft model mapper is active. |
| ![](./../../img/manual_swiftgui_statusbar_dbus.jpg) |when you run *swift* in [Distributed Mode](./../distributed.md), this should be lit, because DBus must be active for it to work. |
| ![](./../../img/manual_swiftgui_statusbar_ptt.jpg) |**PTT** is "**PushToTalk**" and its status light will be active for as long as you are pressing a PTT key. |
| ![](./../../img/manual_swiftgui_statusbar_audio.jpg) |This status light indicates that your Audio codec was initialized successfully. |
