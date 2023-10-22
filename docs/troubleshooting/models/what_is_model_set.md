<!--
    SPDX-FileCopyrightText: Copyright (C) swift Project Community / Contributors
    SPDX-License-Identifier: GFDL-1.3-only
-->

The model set is a subset of all aircraft models you have installed / stored.
It represents the models you can use to display other users (i.e. other aircraft, the other pilots).
The model set is **needed for model matching**.

!!! danger

    No model set, no model matching, no working *swift* !


See also [this page](./../mapping_matching_model_set_theory_concepts.md)

## Why is *swift* using a model set, why is it needed?

From user perspective:

- the model set allows to define any combination of models for matching as you like it
- you can mix models from various distributors
- you can have multiple model sets suitable for special purposes (without installing/uninstalling models)
- easy testing: you can easily add or remove models to your set for testing purposes, without having to install/uninstall the physical models.

Technical reasons:

- *swift* is a multi simulator pilot client.
   By using a abstract model set (i.e. abstract from the physical models) we can use one matching concept for all simulators
-  *swift* can be used in [distributed mode](./../../documentation/distributed.md).
   The model set can be use on a remote computer without direct access (shared drive etc.) to your models folder.
