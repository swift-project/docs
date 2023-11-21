<!--
SPDX-FileCopyrightText: Copyright (C) swift Project Community / Contributors
SPDX-License-Identifier: GFDL-1.3-only
-->

# X-Plane landing gear missing/no animations

!!! note

    This issue is specific to X-Plane</note>

## Issue description

**All** CSL models have their **landing gears retracted/missing** and/or **animations** of parts **do not work** (e.g. landing gear never retracts, flaps never move etc.)

**Or** Aircraft are not drawn on TCAS

![](./../../../img/xpgearup.jpg){: style="width:70%"}


## Solution 1

**Another plugin is conflicting with xswiftbus**

One of the functions of *xswiftbus* is to inject CSL model data into X-Plane to render (display) the aircraft of other pilots near you, including model animation.
If another plugin with similar functions is **active at the same time**, it will interfere with the rendering process of those CSL models their animations will be broken or you won't be seeing any models at all.

Check the plugins-directory of X-Plane for other plugins that are related to injecting CSL model data.
Plugins for X-Plane 11 are saved in ``\X-Plane 11\Resources\Plugins\``.

The following plugins are known to interfere with xswiftbus:

* **XSquawkbox**
* **xPilot**
* **X-IvAp**
* **PilotEdge**
* **LiveTraffic**
* **World Traffic**

**You have to deactivate** any of those plugins for as long as you wish to use *swift*.
The default plugin manager of X-Plane does **not** prevent this from happening, because the way it "deactivates" plugins will not stop X-Plane from initializing them at startup.

**There are only 2 ways to reliably achieve this:**

- **move plugin-folder(s):** move the folders of conflicting plugins to another directory **outside** ``\X-Plane 11\Resources\Plugins\``
- **rename plugin-file(s):** when you rename a plugin-file, then X-Plane will not load it, this will completely deactivate it.
  Open the folder of an affected plugin and look for a file with a ``.xpl``-extension - that's the actual plugin.
  Rename the extension to ``.xpl.off``, or similar.
  When you wish to use the plugin again, just change the file-extension to read ``.xpl``

**For Windows users only:** a more comfortable solution to reliably manage plugins may be **xOrganizer**.
Further information about it can be found on this **[dedicated page](./deactivate_plugins_xorganizer.md)**.

## Solution 2

If **only a few CSL models are affected** by these problems then the reason may be other pilot clients sending wrong information about parts.
There's not much that you can do about this.
