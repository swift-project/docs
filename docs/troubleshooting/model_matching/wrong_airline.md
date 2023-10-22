<!--
    SPDX-FileCopyrightText: Copyright (C) swift Project Community / Contributors
    SPDX-License-Identifier: GFDL-1.3-only
-->

Matching means to find the most suitable model for another pilot in your model set.
If the other pilot flies a `DLH B744` and you have `DLH B744` in your model set, then the process is straight forward, we just take that one.

**If NOT**, then guessing starts and the opinion of what should happen varies.

- some want to see a neutral (all white) aircraft
- some want to see a `B744`, but accept that from another airline
- some prefer to see a `DLH` livery but accept another aircraft type

So there is not "best" solution, it depends on multiple factors.
The result in swift depends on

- the models you have in your *swift* model set
- your model matching settings, see [matching script](./matching_script.md)
- your own matching script (if you have written any)

This means the result for *swift* users can be (very) different depending on the mentioned points.
If you want to understand your matching result, just create a [matching log](./matching_log.md).

To improve your matching check [this page](./tips.md).
But there are things you can check by yourself.

- Do you use models without swift DB entry?
  Those might be unreliable because not enough information are available.
- Check your settings
- Check the matching log, in many cases this is already self-explanatory
- If you want to see airline `FOO`, do you have models for `FOO`?
  Check your coverage with the model matrix.
- You could use your own logic, see [matching script](./matching_script.md) and [matching script technical](./matching_script_technical.md)
