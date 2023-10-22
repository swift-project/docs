<!--
    SPDX-FileCopyrightText: Copyright (C) swift Project Community / Contributors
    SPDX-License-Identifier: GFDL-1.3-only
-->

## Fundamentals

- [Understanding the fundamentals](./../mapping_matching_model_set_theory_concepts.md)
- Matching depends on the settings: [Matching script](./matching_script.md)
-   Without model set model matching is not possible. So check that you have created a model set:

    - Model set in swift pilot client

        ![](./../../img/swift_pilot_client_aircraft_models.jpg){: style="width:70%"}

    - Model set in swift mapping tool

        ![](./../../img/swift_datastore_model_set.jpg){: style="width:70%"}

## Analyze your models and matching

-   Use the matching messages to understand how a particular aircraft is matched.

    ![](./../../img/swift_pilot_client_matching_messages.jpg){: style="width:70%"}

- You can also see some mapping details in the models view.
  You can see how the ICAO code of the aircraft is mapped or how the livery is mapped `from -> to` or `[=]` (same code).

    ![](./../../img/Models_view_see_mapping.jpg){: style="width:70%"}

- In the statistics view you can check if you have a model for a particular ICAO code combination installed

    ![](./../../img/swift_pilot_client_statistics.jpg){: style="width:70%"}

- In the mapping tool you can check the coverage of your model set:

    - Create matrix

        ![](./../../img/swift_mapping_tool_matrix.jpg)

    - Example matrix

        ![](./../../img/Model_set_example_matrix.jpg)
