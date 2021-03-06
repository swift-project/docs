<!--
    SPDX-FileCopyrightText: Copyright (C) swift Project Community / Contributors
    SPDX-License-Identifier: GFDL-1.3-only
-->

*swift* saves the screen size in order to restore size and location of its window.
If you need to reset to a default location and size you can use

* select ``reset window`` in the launcher

![](./../../../img/wizard.jpg){: style="width:50%"}

* alternatively press ``SHIFT + ALT`` during startup (you can try this first, it is the *easiest* solution)
* alternatively use the command line ``--resetsize`` or ``-r``, like `swiftguistd.exe --resetsize`
* or delete the GUI settings.
To find those check out for a line like ``GUI settings are here`` in the log.
On Windows OS you find them here:
    `\HKEY_CURRENT_USER\Software\swift-project.org\swift pilot client GUI`
- You can also delete all registry entries from the launcher tools:

![](./../../../img/registrydelete.jpg){: style="width:50%"}
