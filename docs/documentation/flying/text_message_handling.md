<!--
    SPDX-FileCopyrightText: Copyright (C) swift Project Community / Contributors
    SPDX-License-Identifier: GFDL-1.3-only
-->

## Detached message window

You can detach the `message window` (like any other window)

![](./../../img/Detached_message_window.jpg){: style="width:70%"}

## Overlay messages

From the ATC and cockpit view you can use overlay text messages directly in the window

![](./../../img/ATC_overlay_window.jpg){: style="width:50%"}

![](./../../img/Overlay_text_messages.jpg){: style="width:50%"}

## Private message buttons

You can use the `private message buttons` to send private messages to the closest ATC stations

![](./../../img/Private_message_buttons.jpg){: style="width:50%"}

## Configure text messages

- Defining which text messages are relayed to the simulator

![](./../../img/Text_messages_to_simulator.jpg){: style="width:50%"}

- Defining which text messages are shown as overlay in the client

![](./../../img/messagesoverlaysettings.jpg){: style="width:50%"}


- Set focus as wanted

## Disable overlay messages

Disable all checkboxes for overlay messages

![](./../../img/disableoverlay.jpg){: style="width:50%"}

## Text message views

Normally you have text views for each radio channel and/or private text messages.
The UNICOM and COM1/2 channels are permanent while the private channels can be closed.

![](./../../img/textmessages.jpg){: style="width:70%"}

That leads us to the role of the `ALL` view.
This is a sortable table view (and no HTML text view as the other ones).
It's role is different:
It can help you to find a message again if you have already closed the private message tab or you do not know where it was.

!!! tip

    You can use the tooltip to see longer messages .. image::
    ![](./../../img/longmessage.jpg){: style="width:70%"}

## Relay messages to simulator
see [this article](./settings/simulator_messages.md).
