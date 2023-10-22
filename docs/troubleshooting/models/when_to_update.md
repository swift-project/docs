<!--
    SPDX-FileCopyrightText: Copyright (C) swift Project Community / Contributors
    SPDX-License-Identifier: GFDL-1.3-only
-->

Do I have to update my model set if I update my models (like
downloaded a new FLAI, BB, or X-IVAP version)?

Short answer, most likely "yes"

Details:

- *swift* uses the models you have specified in the model set
- If an update contains new models and you want to use those, you need to add them to your model set
- If models have been deleted, you need to delete those from your set
- It can happen new models are available but those data are not in the *swift* DB yet.
  You can help to provide those data or wait until those are available.
- It is a good idea to use model validation to detect inconsistencies / errors in your model set, see [this page](./../../documentation/flying/model_set_validation.md).

Other reasons when you have to update your model set

- you have moved or deleted a model directory
- you have manually deleted models from your model directory
