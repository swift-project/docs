<!--
    SPDX-FileCopyrightText: Copyright (C) swift Project Community / Contributors
    SPDX-License-Identifier: GFDL-1.3-only
-->

Make sure you have the MIC (microphone) enabled for *swift*.

![](./../img/macsound.jpg){: style="width:70%"}

- There is a bug currently being investigated.
- macOS seems to be very picky about app bundle info.plist.
  No matter what we add to it, it just won't work without any warning.
- Workaround: Open the swiftguistd application bundle content and drag the internal binary into console.
  That should work

![](./../img/workaround_mac1.jpg){: style="width:70%"}

![](./../img/workaround_mac2.jpg){: style="width:70%"}

![](./../img/workaround_mac3.jpg){: style="width:70%"}
