<!--
    SPDX-FileCopyrightText: Copyright (C) swift Project Community / Contributors
    SPDX-License-Identifier: GFDL-1.3-only
-->

Essentially, *swift***Core** contains all central pilot client functionality, such as:

* connect to the network (e.g. VATSIM, local FSD server etc.)
* connect to the simulator (via a plugin driver)
* doing the model matching
* voice connectivity

By default, *swift* pilot client will run as one executable together where *swift*GUI includes *swift*Core - we call this "Standalone Mode".
It is possible to run *swift*Core independently from *swift*GUI (2 separate executables) and *swift*GUI will then interact with *swift*Core via DBus.
This can be configured and initiated in *swift***Launcher**.
The only real use-case for the latter is when running swift in **Distributed Mode**, when your flight simulator software is located on a different computer from where *swift*GUI is active.
[More information on operating swift in Distributed Mode.](./distributed.md)
