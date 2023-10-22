<!--
    SPDX-FileCopyrightText: Copyright (C) swift Project Community / Contributors
    SPDX-License-Identifier: GFDL-1.3-only
-->

!!! note

    Consolidation means your model data from the simulator will be merged with the DB data into a more detailed data set.

-   When you start the mapping tool and read the installed models the current DB data will be used
-   This also applies when you create the model set (the current DB data are used)
-   But other users (or yourself) can change the DB data at a later time to:
    -   Create new mappings
    -   Modify/correct existing mappings
-  Applying those changes requires consolidating your model data with the latest DB data.
   There are multiple ways to accomplish this
    -   Manually via the context menu: [Consolidation](./consolidation.md)
    -   Automatically in background: [Background Updater](./background_updater.md)
    -   During the model update for the client, see [Update model data](./../flying/update_model_data.md)
