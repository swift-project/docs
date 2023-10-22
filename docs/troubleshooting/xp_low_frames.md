<!--
    SPDX-FileCopyrightText: Copyright (C) swift Project Community / Contributors
    SPDX-License-Identifier: GFDL-1.3-only
-->

If your frame rate in X-Plane drops below 20 FPS (frames per second) then you are at risk of being automatically disconnected from the network.
This is because below 20 FPS X-Plane will slow down the simulation time to compensate for the lack of frames, which would cause your actual speed (as observed by other users on the network) to be slower than what is reported by your aircraft instruments, and this could cause disruption for other users. (Loss of separation, etc.).

*swift* will automatically disconnect from the network if your low framerate causes you to be more than two nautical miles behind where you are supposed to be.
You will receive an automatic warning when you are one nautical mile behind where you are supposed to be:

[TODO: screenshot of disconnect message]

To avoid being disconnected, adjust your X-Plane rendering settings so that you can maintain a consistent framerate above 20 FPS.
