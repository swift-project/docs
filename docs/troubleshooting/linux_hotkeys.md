<!--
    SPDX-FileCopyrightText: Copyright (C) swift Project Community / Contributors
    SPDX-License-Identifier: GFDL-1.3-only
-->

swift reads events directly from raw input devices (``/dev/input/event*``) for the hotkeys.
This is required because hotkeys like Push-to-Talk should also work when the swift window is not focused, for example when the flight simulator is active.
The ``/dev/input/event*`` device files are protected because access to them allows direct interaction with devices like the keyboard.
This could be misused by keyloggers or other users on the machine.

For some devices, it is not critical that every user can read its input, such as devices that are not used to input sensitive data like joysticks.
Access to these might be granted automatically (often with udev rules and the ``uaccess`` tag, as described below), depending on how your system is configured.

!!! note

    If the hotkeys are working for you, you do not need to read any further.

## Granting access to ``/dev/input/event*`` device files

Two ways to grant access to ``/dev/input/event*`` devices are described below, both of which require systemd and udev (included with systemd).
systemd is used by most Linux distributions nowadays like Ubuntu, Debian, Arch Linux, and many more.
If your distribution does not use systemd, you must find some other way to grant your user account (or specifically swift) access to the required ``/dev/input/event*`` devices files.

### Using udev rules with ``uaccess`` tag (recommended)
The following information is based on https://wiki.archlinux.org/title/udev section 4.2 (Allowing regular users to use devices).

One could use udev rules and the udev ``uaccess`` tag.
This way, only the active user is granted access to the specified device.
First, you need to find the vendor ID and product ID of your device that you want to use for the hotkey.
If the device is a USB device, you can find this by using the ``lsusb`` command.

With a line like the following, ``046d`` is the vendor ID and ``c336`` is the product ID.

```
Bus 003 Device 002: ID 046d:c336 Logitech, Inc. G213 Prodigy Gaming Keyboard
```

Afterwards you need to create a udev rule (file) like ``/etc/udev/rules.d/71-keyboard.rules`` with the following contents:

```
SUBSYSTEMS=="usb", ATTRS{idVendor}=="<YOUR VENDOR ID>", ATTRS{idProduct}=="<YOUR PRODUCT ID>", MODE="0660", TAG+="uaccess"
```

After rebooting, you should have access to the required ``/dev/input/event*`` files of the specified device.

Be aware, that the ``TAG+="uaccess"`` method could also be misused my malicious software because every application running under your user account is now able to access the device!

For now, this is the recommented way, but we are planning to work on an easier and more secure way in upcoming swift versions.


### Adding user to ``input`` Group (discouraged)
The easiest and discouraged way is by adding the own user to the ``input`` group.
After adding the user to the group, you might have to log-out and log-in again to get access.

This group automatically has access to all ``/dev/input/event*`` device files since systemd version 215.
Using this approach, the user has access to all events, which might not be necessary and should be avoided for security.
Further, these device files can also be accessed by the user while the user session is not active, for example because another user is logged in as well.


