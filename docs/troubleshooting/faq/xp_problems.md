<!--
    SPDX-FileCopyrightText: Copyright (C) swift Project Community / Contributors
    SPDX-License-Identifier: GFDL-1.3-only
-->

# Top 4 XPlane problems

There are 4 top problems using *swift* and XPlane

* no models are shown / no other aircraft, in most of the cases the aircraft folder is in the wrong place. see [here](./../aircraft_not_rendered.md) or you did not create a model set
* landing gear not visible or always visible: conflict with other pilot client, remove any other pilot client or AI traffic plugin you have installed, e.g. XSquawkBox, X-IvAp, PilotEdge, WorldTraffic.
* aircraft are too high or low: IVAO Vertical Offset Fix not installed for BlueBell CSL models.
  As of August 2020, a new version of BlueBell CSL models is available that already incorporate these vertical offsets.
  Visit [CSL models for X-Plane](./../../home/models/xplane/index.md).
* If you **move your model folder you need to reload your models in the mapping tool and recreate the model set**
