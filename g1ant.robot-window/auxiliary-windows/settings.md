# Settings

The command center of G1ANT.Robot is available from `Tools/Settings` menu. It offers all program settings, as well as other global options such as triggers and variables to be shared by all scripts.

The Settings window is a front-end to G1ANT.Robot.config XML file. Its path is displayed in the `File name` box.

![](https://github.com/G1ANT-Robot/G1ANT.Manual/blob/develop/-assets/settings.jpg)

| Item            | Description                                                  |
| --------------- | ------------------------------------------------------------ |
| **Credentials** | Shows items stored in the [Credential Container](../../g1ant.robot-window/auxiliary-windows/credential-container.md). This branch cannot be edited here, no new credentials can be added — to add or change credentials, use Credential Container window. |
| **Dashboard**   | Not used at the moment                                       |
| **Databases**   | Not used at the moment                                       |
| **Log**         | Not used at the moment                                       |
| **Main**        | Allows determining basic parameters for the program:&lt;br /&gt;**ShowStep** and **ShowStepTime** are not used&lt;br /&gt;**Startup** — if its value is set to true, G1ANT.Robot will start with Windows&lt;br /&gt;**StartMinimized** — if its value is set to true, G1ANT.Robot will start minimized&lt;br /&gt;**StopKey** defines the keyboard shortcut used to stop current process execution (**Ctrl+F12** by default) |
| **Studio**      | Controls workspace look and behavior:&lt;br /&gt;**Styling** — if its value is set to true, G1ANT.Robot will use G1ANT.Language syntax coloring for scripts&lt;br /&gt;**WordWrap** — if its value is set to true, the lines of code will wrap&lt;br /&gt;**Font** — lets choose font family and size for the script editor&lt;br /&gt;**Shortcut** — displays keyboard shortcuts changed by a user |
| **Triggers**    | This is the place for setting up new [triggers](../../g1ant-language/triggering/readme.md) or modifying existing ones. To add a new trigger, right-click **Triggers** item and choose `Add`. To delete a particular trigger, right-click it and choose `Remove`. |
| **Variables**   | Here you can declare global [variables](../../g1ant-language/variables/creating-new-variables.md) to be used by all scripts run by this G1ANT.Robot. To add a new trigger, right-click **Variables** item and choose `Add`. To delete a particular variable, right-click it and choose `Remove`. |

