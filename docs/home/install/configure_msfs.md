<!--
    SPDX-FileCopyrightText: Copyright (C) swift Project Community / Contributors
    SPDX-License-Identifier: GFDL-1.3-only
-->

!!! note

    This chapter is for users who have installed *swift* **for the very first time** or who are making **a clean installation** and do not have previous configurations to copy their settings from.
    If you are an existing user and if you have copied all settings during installation of *swift* pilot client, then you don't need to run the Configuration Wizard!
    You can manage all your settings through *swift*GUI.

Check out our **[Tutorial Video](https://youtu.be/RdWmn-4c3XQ)** :simple-youtube: that is specific to Microsoft Flight Simulator 2020.

After the installation has completed, **swiftlauncher** will start automatically.
If, from there, the **Configuration Wizard** did not launch by itself, start it manually:

![](./../../img/swift_installation_configwizard.jpg){: style="width:70%"}


!!! note

    Should you have de-selected the option to launch *swift* Configuration Wizard during the program installation, it is possible to run the same initialization mode any time later by using the command line arguments ``swiftlauncher -i --bootstrapurl %%https://datastore.swift-project.org/shared/%%``


## Legal Wizard

The first wizard page deals with the necessary legal bits.

![](./../../img/configwizard_legal.jpg){: style="width:80%"}

* **accept** license and data protection policy. **Required item**.
* this page also asks for your **agreement to submit crash reports** to our crash report collection server. **Voluntary item**.

**About sending crash reports:** In case that any *swift* application crashes, a report will be generated with information about which line of code caused this.
With your agreement, the report will be uploaded to our server and helps the developers to diagnose and fix the cause.
This agreement can be changed anytime later in the **advanced settings** dialogue in ***swift*GUI**.

## Data Loading Wizard

The next wizard will download all data form the database of *swift* **automatically**.
You may continue to the next configuration page - data loading will continue in the background.
This data is required by *swift* to be fully functional.
**It is not necessary to click any of the load buttons**.

![](./../../img/configwizard_dataloading.jpg){: style="width:80%"}

## Copy Models Wizard

!!! note

    This page can be skipped, should you have no previous copies of *swift* installed on your computer.

If you had a previous version of *swift* installed already, then this wizard will help you migrate your existing aircraft model cache and model set to the new version of *swift*:

* select the older version you want to migrate from the list
* select whether you want to migrate the model set and/or model cache and for which simulators
* click the button ``start copy``

## Copy Settings Wizard

!!! note

    This page can be skipped, should you have no previous copies of *swift* installed on your computer.

If you had a previous version of *swift* installed already, then this wizard will help you migrate your settings:

* select the older version you want to migrate from the list
* select the settings to copy from the older version: either one by one or use the button **select all** on the bottom
* greyed out items mean that no user setting is available and the default setting is in use. They cannot be selected
* click on the button ``copy``

## Simulator Wizard

This page allows you to configure which flight simulator programs you want *swift* to work with and what model directories will be used or excluded.
For MSFS you need to choose "FSX"!

![](./../../img/configwizard_simulatorsetup_fs2020.jpg){: style="width:70%"}

### Select your simulator(s)
If you have multiple simulators installed and use them regularly, select all of them at the top of the page.
Otherwise just select the one flight simulator platform, that you are using.
For MSFS choose FSX.

![](./../../img/select_simulators_fs2020.jpg){: style="width:70%"}

### Setup of each individual simulator

In this you are able to configure the simulator path and any additional model directories.

* **Simulator**: select the flight simulator platform that you want configure the paths for. Even if you have only one flight simulator platform installed, make sure that the correct one has been selected!

    ![](./../../img/select_simulators_fs2020.jpg){: style="width:70%"}

* **Simulator directory**:
  If you don't know the exact drive and path where your MSFS has been installed to, activate the developer mode in MSFS:

      ![](./../../img/dev_mode.jpg){: style="width:70%"}

    A new menu will appear at the top and you can easily find the directory there:

      ![](./../../img/fs2020_find_folder1.jpg){: style="width:40%"}

      ![](./../../img/fs2020_find_folder2.jpg){: style="width:50%"}

    As simulator directory choose the **main directory** (in this case J:/FS2020):

      ![](./../../img/configwizard_simulatorsetup_simdirectory_fs2020.jpg)

* **Model directories**
  At this point in time there are no third party model packages available for MSFS, so you have to use the standard models.
  These models are in the Official/OneStore directory of your main MSFS path (look above).
  You should also add the community path (in this case J:/FS2020/Community) to include installed 3rd party liveries and future model packages.

    * to select the directory, use the ``...`` button
    * after you have made changes, you have to select **``save``**, or your change to the path will be lost

![](./../../img/configwizard_simulatorsetup_modeldirectories_fs2020.jpg){: style="width:70%"}

## First Model Set Wizard
This wizard will help you create your **first, basic model set to get you started**.
Each of the flight simulator platforms that you want to use with *swift* has to have its own model set.

![](./../../img/1stmodelset_wizard_fs2020.jpg){: style="width:70%"}

!!! note

    There will be **no** fine-tuning, **no** filtering: you will just **add all aircraft models** that *swift* can find **inside the paths that you have defined** in the previous section.
    If you want to perform some more elaborate work on your model set, you will need to use the **Mapping Tool** (*swift*Data app).
    Visit the **section about the Mapping Tool** and check out our **[YouTube Video Tutorial: Working with the Mapping Tool](https://youtu.be/hqOsjmV7wus)** :simple-youtube:

A model set consists of AI (Artificial Intelligence) aircraft that **have to be installed** on your computer.
For MSFS2020 they can be installed in your ``Community`` folder or in another folder and then linking them to the ``Community`` folder.
Without any models installed and without any model set defined, *swift* will not run properly, because it won't have anything to create and render the aircraft of other pilots around you with.

### Simulator & Selection

![](./../../img/1stmodelset_simulator_fs2020.jpg){: style="width:30%"}

* select the flight simulator platform, that you want to create a first model set for: choose ``FSX`` for MSFS.
* keep the check mark activated at ``with DB data only``

### Models

Now it's time to actually search for existing AI aircraft models, list them as your **Stored Own Models** and then add them to your **Active Model Set**.

![](./../../img/1stmodelset_modelselection_fs2020.jpg){: style="width:70%"}

- **Model dir.:** check the model directory/directories and if necessary change it/them - go back to the previous page and do it in the ([Simulator Wizard](./configure_msfs.md#simulator-wizard))
- **Models:** (in the **swift Mapping Tool** this is labelled as **Stored Own Models**)
    * click on ``reload`` to scan your model directory/directories.
      The result will be a pop-up message window, listing all AI aircraft that *swift* was able to find.
      In case that you get a **few error messages only**, close the error message pop-up window ``x``
- **Model Set:** (in the **swift Mapping Tool** this is labelled as **Active Model Set**)
    * click on ``create``
      This will extract all valid AI aircraft from **Models** (Stored Own Models) and insert them into your **Model Set**.
      A window with a list of these models will pop up
    * select ``save``' to **save your Active Model Set**.
      Failing to do so will result in losing your changes to the model set

    ![](./../../img/1stmodelset_saveactivemodelset_fs2020.jpg){: style="width:70%"}

Believe it or not, but you just created your first model set for *swift*, well done!

## Hotkey Wizard

The **Hotkeys Wizard** allows you to configure hotkeys.

![](./../../img/hotkeys_wizard.jpg){: style="width:70%"}

You have to define at least one joystick button or keyboard key as **Push-To-Talk (PTT)**, otherwise you won't be able to talk to Air Traffic Controllers.

![](./../../img/hotkeys_ptt.jpg){: style="width:40%"}

* you can assign **multiple keys or buttons** to **one single** function
* you can ``add``, ``edit`` and ``remove`` hotkeys

### Adding a new Hotkey
* select ``add``
* **Action**: select a function, ``Voice`` ==> ``Activate push-to-talk``
* **Combination**: click on ``[Select]`` and then **press the button/key** that you want to use as PTT


!!! tip

    The Config Wizard presents you only with a reduced selection of hotkey-functions to get you started with a PTT key.
    You can find **many more hotkey-functions** in the **[hotkey settings](./../../documentation/swift_gui/settings_page.md)** in the *swift***GUI application**

      ![](./../../img/hotkeys_guiexpanded.jpg){: style="width:40%"}


## MSFS activation

As long as MSFS is not supported natively, users have to check that MSFS has been activated correctly.
For this, start *swift*GUI, select the ``Settings`` wizard and in there click on ``Simulator``.
On this page make sure that the checkmark is active in the line of ``Flight Simulator 2020``.
When this is assured, close *swift*GUI.
While doing so this change will be saved.
Should *swift*GUI not remember this setting, try run *swift*GUI "as administrator" before making this change and save it.

![](./../../img/configwizard_simulatorsetup_activate_fs2020.jpg){: style="width:70%"}

## Congratulations
**You are now done configuring** *swift*!

Go ahead and start *swiftGUI*.
You can do this through *swiftLauncher* by clicking on the blue *swift* icon ![swift GUI icon](https://raw.githubusercontent.com/swift-project/pilotclient/main/src/blackmisc/icons/own/swift3D/sw3DBlue-32.png) or through the *swiftGUI* shortcut.

!!! tip

    you can configure your *swiftGUI* shortcut to start the client in **frameless** mode by adding ``-w f`` to it.
    Your "target" should then look like this ``YourDrive:\YourDirectory\swift-x.x.x-64bit\bin\swiftguistd.exe -w f``

Before your **first flight** check out this **[Tutorial Video](https://youtu.be/7HTrfqXy4nU)** :simple-youtube: to take our program tour of *swift*GUI and show you further setup options.

You can find more tutorial videos on this **[dedicated page](./../video_tutorials.md)**.
