<!--
    SPDX-FileCopyrightText: Copyright (C) swift Project Community / Contributors
    SPDX-License-Identifier: GFDL-1.3-only
-->

*swift* can display airline logo icons in its menus.
Although optional, it's a nice eye-catcher.

If you wish to add missing icons please follow these rules:


## Image Format
* **use a 4:1 ratio**, such as 300:75px
* **maximum size** 300:75px (see hint about hires below)
* use **``png``** format

## File Naming Conventions
* **5-digit airline ID** + **airline ICAO code** (for Virtual Airlines also use their 3-letter ICAO code)
* you can research both the ID and the code in our [swift Datastore](https://datastore.swift-project.org/page/publicairlineicao.php)
  * **example:** you want to submit a new logo for "Lufthansa"
  * in [swift Datastore](https://datastore.swift-project.org/page/publicairlineicao.php) search in the field **''Name''** for "Lufthansa"
  * result: ID = 3221 and ICAO Code "DLH".
    Don't forget to add a leading zero to the airline ID to make it a 5-digit number!
  * correct airline logo file name to submit: **``03221_DLH.png``**

* we may use **higher resolutions** in the future, therefore you can also add a hires version like 1024:205 pixel.
  Such icons have to labelled additionally with **``hi``** => **``03221_DLH.hi.png``**
* dark optimized icons (for a black background) will be using **``.do``** in their name => **``03221_DLH.do.png``**

* Valid file names:
  ***``03221_DLH.png``** lowres version (approx 300:75)
  ***``03221_DLH.do.png``** lowres version, dark optimized (approx 300:75)
  ***``03221_DLH.hi.png``** hires version
  ***``03221_DLH.do.hi.png``** hires version, dark optimized
* if an airline or virtual airline is not listed in *swift* Datastore, [request to add the airline](https://datastore.swift-project.org/page/changerequestairlineicao.php?clear=true).
  More information [here](./../../documentation/swift_datastore/change_requests.md).

!!! danger

    **DO NOT use copyright protected icons!**
    Check Wikipedia, they will show you the copyright for each icon.
