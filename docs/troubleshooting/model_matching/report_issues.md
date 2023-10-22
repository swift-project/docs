<!--
    SPDX-FileCopyrightText: Copyright (C) swift Project Community / Contributors
    SPDX-License-Identifier: GFDL-1.3-only
-->

If you are unhappy with a matching result it is possible to investigate what is going on.
But please understand that model matching depends on many factors

- your model set
- the login data of the other party
- your model matching settings

So we have seen many cases where fantasy ICAO codes are used, or user login under mismatching credentials (like using `DLH123` as callsign, but login as `BAW `)

To investigate of what is going on we need a matching log.
swift can show en detail what happens during matching we need a [matching log](./matching_log.md)

Only this will tell us what has happend.
Discussions without a log are NOT productive.

Some hints:

- If you are just unhappy with a matching during a flight just change it manually, see [this page](./../../documentation/swift_gui/models/manually_changing_models.md)
- You can add more models to your set to cover more cases.
  But just adding models is pointless, you have to add models missing.
  Use the statistics to see your coverage.
- Validate your model set to see if there are issues, see [this page](./../../documentation/flying/model_set_validation.md) and [this page](./../../documentation/flying/model_set_validation_example.md)
