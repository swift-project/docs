<!--
    SPDX-FileCopyrightText: Copyright (C) swift Project Community / Contributors
    SPDX-License-Identifier: GFDL-1.3-only
-->

Here you find some high level tasks (besides open issues and fixes) you could work on

## as C++ programmer, swift pilot client

See [GitHub issues](https://github.com/swift-project/pilotclient/issues)

## swift pilot client UI design tasks

Requires less C++ skills than the above, but still installation of Qt Creator, more focused on the UI builder, stylesheets

* Improve the layout of the text message parts.
  Currently this is layouted via a CSS, and mostly shown as table view.
  This could somehow look cooler
* Also the popup error and warning messages look a bit crude and could be refined (more 3D looking).
  So this could be fine tuned as well.
  This screenshot shows what we mean
  ![](./../../img/popuperrormessage.jpg)

* CPDLC: create the UI for the CPDLC integration

## as PHP/JavaScript programmer

* allow to request (change request) new liveries
* allow to upload airline icons
* notification services (push messages) when relevant data change (e.g. from datastore to slack)

## no programming skills required

* help with the efforts to create mappings, see [Mapping hints](../../troubleshooting/model_mapping/mapping_hints.md)
* help us to complete the airline icons.
  Provide us with airline icons we can integrate, see [here](./airline_logos.md). Mind the copyright!
* ATC icons: We are using icons to represent the different ATC stations. Those icons currently have a low resolution.
  We could use them in higher resolutions and streamlined.

![](./../../img/atc_icons.jpg)
