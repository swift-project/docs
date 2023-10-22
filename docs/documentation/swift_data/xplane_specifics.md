<!--
    SPDX-FileCopyrightText: Copyright (C) swift Project Community / Contributors
    SPDX-License-Identifier: GFDL-1.3-only
-->

## CSL vs. .ACF-aircraft
* Like **XSquawkBox**, we render CSL models to represent the remote aircraft (other pilots)
* There is a distinction between CSL and the aircraft that the local user flies (the .ACF-aircraft)
* One cannot fly a CSL, and *swift* cannot render a .ACF in X-Plane
* We need both in the database, but we can not use .ACF to render remote aircraft in X-Plane
* For this reason .ACF-aircraft are ``X`` (**excluded**), which prevents them from being used for rendering
* .ACF-aircraft with ``X`` normally do not belong in the Active Model Set (do not confuse Active Model Set and Own Models)
* *swift* uses .ACF-files in the database so *swift* knows what plane the local user is flying, so we can pass that info to the other clients on the network
* See also [Excluded models](./excluded_models.md)
* Do we need mappings for .ACF-aircraft? Yes, see [Excluded models](./excluded_models.md)

## Model directories
* One can install CSL models wherever you want, as long as they are inside X-Plane's program directory
* In the mapping tool, simulator settings panel, you direct *swift* where to search for them, by adding to the list of model directories
* All subdirectories of your X-Plane directory are already selected
* For your own (non-CSL) models, ACF-aircraft and excluded should be automatically added by default when the mapping tool discovers the models
