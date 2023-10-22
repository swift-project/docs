<!--
    SPDX-FileCopyrightText: Copyright (C) swift Project Community / Contributors
    SPDX-License-Identifier: GFDL-1.3-only
-->

Some models are marked as x **excluded** (meaning in that context here, that the model shall not be used for matching).
Typical reasons for that are:

- XPlane `.acf` models (flyable aircraft) cannot be used for matching.
- Some AI models for FSX/P3D do not show valid aircraft and are therefore excluded.
- Legal reasons might lead to excluded models.
- Some models exists, but are known to be buggy/malfunctional or consume too many resources
- **It is still useful to create mappings for such models!** see [Reverse lookup](./../../troubleshooting/model_matching/reverse_lookup.md).
    -   for automatic flight plan information
    -   for the login ICAO data
    -   for reverse lookup between swift clients (more detailed info used for matching)

!!! warning

    Normally **excluded** models are not used in a model set, but there might be exceptions (we cannot verify all cases)

