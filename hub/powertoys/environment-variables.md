---
title: PowerToys Environment Variables for Windows
description: Environment Variables is a convenient way to manage environment variables.
ms.date: 10/24/2023
ms.topic: article
no-loc: [PowerToys, Windows, Environment Variables, Win]
---

# Environment Variables

Environment Variables app offers a nice and easy way to manage environment variables. Also, you can create profiles and manage multiple variables at once. Profile variables have precedence over User and System variables. In the background, applying the profile adds variables to User environment variables. When profile is applied, if there is an existing User variable with the same name, backup variable is created in User variables which will be reverted to original one on profile un-apply.

Applied variables list shows the current state of the environment, respecting the order of evaluation of environment variables (Profile -> User -> System). Evaluated Path variable value is shown at the top of the list. 

![PowerToys Environment Variables screenshot.](../images/powertoys-environment-variables.png)

## Edit/Remove variable

To edit or remove a variable (profile, User or System) for specific variable select more options button (**•••**):

![PowerToys Environment Variables: Edit/Remove variable](../images/powertoys-environment-variables-edit-variable.gif)

## Add profile

To add new profile:

 - Select **New profile**
 - Enter profile name
 - Set Enabled toggle to On to apply the profile right after creaton
 - Select **Add variable** to add variables to profile (either new variable or existing User/System variables).
 - Select **Save**

![PowerToys Environment Variables: Add profile](../images/powertoys-environment-variables-add-profile.gif)

To edit or remove the profile, select profile more options button (**•••**).

## Apply profile

To apply profile, set profile toggle to On. Only one profile can be applied at the time. Applied variables list will show applied profile variables at the top (below Path variable):

![PowerToys Environment Variables: Apply profile](../images/powertoys-environment-variables-apply-profile.gif)

## Settings

From the Settings menu, the following options can be configured:

| Setting | Description |
| :--- | :--- |
| Launch as administrator | Launch as administrator to be able to manage System variables. If disabled, only profile and User variables can be modified. Environment Variables is started as administrator by default. |