<!--
    SPDX-FileCopyrightText: Copyright (C) swift Project Community / Contributors
    SPDX-License-Identifier: GFDL-1.3-only
-->

!!! important

    Always save your stashing data (then you recover it in case of a crash)

-  Always check if the aircraft already has a mapping (DB icon)
    - If you see an existing mapping, which is wrong, we appreciate very much if you fix it.
    - Otherwise, create mappings for non existing aircraft entries.
    - see here, entries with and without icon

        ![](./../../img/WithAndWithoutMapping.jpg)

- New ICAO codes: [change request](./../../documentation/swift_datastore/change_requests.md)

-   [Effective creating mappings](./../../documentation/swift_data/effective_create_mapping.md)

## Which mappings do we need?

- We cannot tell you exactly what mappings to create, as we do not know which models you have installed
- However, it is always good to create mappings for payware aircraft (as we definitely can not buy all those).
- All Libraries we would like to have in the DB
    - VATSIM FLAI
    - World of AI: <http://www.world-of-ai.com/>
    - FAIB: <http://fsxaibureau.com/>
    - Juergen Baumbusch: <http://www.juergenbaumbusch.de>
    - Flying carpet: <http://www.flyingcarpet75.com>

## Q&A

- Should I use the `P3D` for P3D v1-3 or also for v4?
  We are currently evaluating P3D v4, for now use it for all P3D versions.
- I have the same model installed, but from another distributor, what should I do?
  This can happen, many models are part of multiple distributions.
  Normally there is not need to update the distributor.

- I have a model, but the distributor is missing?
  Request the distributor, you can already do the mapping and save your stash.
  Later you can fix the distributor.
  Or you can use `ZZZZ`, publish and later change/fix the distributor

- How can I efficiently create mappings?
    - If you place random models on the stash, it will be more work.
    - Try to assign multiple attributes at once, e.g. select all aircraft of an airline and assign those at once
    - You can filter your aircraft and stash the filtered only (example: Filter by aircraft, push result to stash, assign aircraft ICAO in one step)
- How do we set the distributor for FS, FSX, P3D standard models?
  See [this page](./mapping_fs9_fsx_p3d_standard_models.md)
- What are excluded models?
    See [this page](./../../documentation/swift_data/excluded_models.md)
- XPlane
    - Why are some models excluded (`CSL` vs `.acf` models)?
      See [this page](./../../documentation/swift_data/excluded_models.md)
    - Do we need mappings for `ACF` models?
      Yes, see [this page](./../../documentation/swift_data/excluded_models.md)

## Problems?

see [this page](./../../documentation/swift_data/problems.md)
