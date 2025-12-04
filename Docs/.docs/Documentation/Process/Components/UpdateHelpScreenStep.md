# Update Help Screen Step

To help the user during the process you can update the information in the floating help screen, this can be achieved using the `UpdateHelpScreenStep`.

![update-help-screen.png](.attachments/update-help-screen.png)

![help-screen.png](.attachments/help-screen.png)

> [!NOTE]
> Keep in mind that texts must be provided for each localization selected in the [SceneConfiguration](https://virooportal.virtualwareco.com/docs/3.0/viroo-studio/Environment-Customization/Localization/Setting-Localization.html) component.
> ![localization-scene-configuration.png](.attachments/localization-scene-configuration.png)

## Update Title

To update the screen title you can do it by enabling the `Update Title` section of the component, here you can configure the desired title in each localization configured in the `SceneConfiguration` component.

![update-help-screen-title.png](.attachments/update-help-screen-title.png)

This component allows you to change the title of the help screen:

![step-help-screen-title.png](.attachments/step-help-screen-title.png)

## Update Description

To update the screen title you can do it by enabling the `Update Description` section of the component, here you can configure the desired description for each localization.

A locution can also be added to each text in order to play an auditive feedback when updating this information.

![update-help-screen-description.png](.attachments/update-help-screen-description.png)

![step-help-screen-step-text.png](.attachments/step-help-screen-step-text.png)

## Move Help Screen

The help screen can be moved to desired position throughout the scene. Here you can configure the following:

- The position in the scene to move to.
- If the help screen will move to the assigned position in `Local` or `Global` mode.
- Whether to play an auditory feedback when moving the screen (this will only be played if the description does not have a locution).

![update-help-screen-movement.png](.attachments/update-help-screen-movement.png)
