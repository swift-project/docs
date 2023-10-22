<!--
    SPDX-FileCopyrightText: Copyright (C) swift Project Community / Contributors
    SPDX-License-Identifier: GFDL-1.3-only
-->

# Download and Installation of X-CSL models

Watch our **[YouTube Video Tutorial: X-CSL Model Set Installation](https://youtu.be/cc2Be3_OQRY)** :simple-youtube: and follow these steps:

**A short introduction, please read!**

The X-CSL Updater will later on be used to update your existing set of CSL models.
You need to keep one "master copy" of all X-CSL models that will **not** be converted or altered in any way.
Otherwise the X-CSL Updater will think that all files are "new" and you will have to download of the files everytime you wish to update X-CSL!
Therefore create a new directory in a place of your choice where you wish to permanently keep a "master copy" of all X-CSL models, e.g. ``YourDrive:\X-CSL Master\``.


!!! danger

    For the master set, do **not** choose a path inside X-Plane's program directory!

## Initial Installation of X-CSL models

- **Proceed to the homepage of X-CSL** and download the X-CSL Updater.
  Use **version 1.2.0** for xIvAp
- install the **X-CSL Updater** in a directory of your choice
- should you already have X-CSL models inside X-Plane's program directory, **delete** them all
- as explained in the introduction, **create** a directory where you will install and maintain your **master copy** of X-CSL models.
  It can be at a place of your choice, the only condition for it to be **outside** X-Plane's program directory.
  Choose a meaningful name, e.g. ``X-CSL Master``. Make sure there's enough disc space, you'll need at least 2.5 GB!
- now **create another folder** **inside** X-Plane's program folder, where you want to copy those CSL model sets to.
  We recommend using the ``Custom Data`` directory, e.g. ``X-Plane 11\Custom Data\CSL\X-CSL``
- **start the X-CSL Updater** application
- **open File-menu** and select **Set X-Plane location** => browse to your X-Plane 11 program directory, select ``X-Plane.exe``
- **open File-menu again**, select option **Set custom path** and confirm the warning with ``OK``.
  Then browse to and select the directory of **X-CSL's Master Copy** that you created in **step 4)**
- in the X-CSL Updater program **click on Index** on the bottom right.
  This will check the current status of your X-CSL Master Copy against the database on their server
- **select the model sets** from the list that require installation or updating.
  Should this be your first installation of X-CSL, you will have to select all of them and then click on **Update**.
  It may take quite a while to finish this process.
  Should you just be updating your existing X-CSL model set, this will be much faster - make sure you only select the aircraft types that are flagged "outdated"
- when you are done with downloading all models, close the X-CSL Updater program
- **copy** all X-CSL models from your Master Copy (e.g. ``YourDrive:\X-CSL Master\``) to the designated CSL directory (e.g. ``X-Plane 11\Custom Data\CSL\X-CSL``)
- to make X-CSL models work in **X-Plane's Vulkan graphics** driver, it is imperative to **convert them**.
  How it's done is shown on our **[CSL2XSB Model Converter Page](./csl2xsb_converter.md)**.
  **You MUST run the CSL2XSB converter every time you update X-CSL models** or they won't be available to add to your model set!
- start *swift***Data** app (Mapping Editor)
    * **reload** your **Own** Models (*Force reload*)
    * **re-create** your **Active** Model Set (*New set*)
    * visit the **section about the Mapping Tool** and check out our **[YouTube Video Tutorial: Working with the Mapping Tool](https://youtu.be/hqOsjmV7wus)** :simple-youtube:

## Updating X-CSL models

- **delete** all your existing X-CSL models inside X-Plane, e.g. in ``X-Plane 11\Custom Data\CSL\X-CSL``
- **start the X-CSL Updater** application
- in the X-CSL Updater program **click on Index** on the bottom right.
  This will check the current status of your X-CSL Master Copy against the database on their server
- **select the model sets** from the list that require updating.
  Make sure you only select the aircraft types that are flagged "outdated"
- when you are done with downloading all outdated models, close the X-CSL Updater program
- **copy** all X-CSL models from your Master Copy (e.g. ``YourDrive:\X-CSL Master\``) to the designated CSL directory (e.g. ``X-Plane 11\Custom Data\CSL\X-CSL``)
- to make X-CSL models work in **X-Plane's Vulkan graphics** driver, it is imperative to **convert them**.
  How it's done is shown on our **[CSL2XSB Model Converter Page](./csl2xsb_converter.md)**.
  **You MUST run the CSL2XSB converter every time you update X-CSL models** or they won't be available to add to your model set!
- start *swift***Data** app (Mapping Editor)
    * **reload** your **Own** Models (*Force reload*)
    * **re-create** your **Active** Model Set (*New set*)
    * visit the **section about the Mapping Tool** and check out our **[YouTube Video Tutorial: Working with the Mapping Tool](https://youtu.be/hqOsjmV7wus)** :simple-youtube:
