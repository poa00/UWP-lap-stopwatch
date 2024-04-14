

# Work timer   ![app-logo](https://camo.githubusercontent.com/137100898759510dbb06006fa8b5062fc8a8874bc925c8e4c564bbe65d2d289c/68747470733a2f2f692e6c6f6c692e6e65742f323032302f30372f30382f68424e4c57354837596c4a66715a462e706e67 "logo")

The app was supposed to be made for my actual work needs, and when I made it, I found that it wasn't as good as I thought it would be, but it helped others because I didn't think of it.

So when I was sorting out the old project, I redesigned the UI and functionality of the app, removed the parts that tied to my work, and made it more versatile, so that it could continue to shine as a positive timer.

## Screenshot of the app

![](https://camo.githubusercontent.com/32e43ba2965e2a8876c44ec540e1b379f3d26cf568e7ffb7c090c8de684a71a2/68747470733a2f2f692e6c6f6c692e6e65742f323032302f30372f31312f354471736d7841587032527a68666c2e706e67 "main page")

## How to install

The app is available in the Microsoft Store, and you can download it by visiting the [Microsoft Store](https://www.microsoft.com/store/productId/9N71W9G714RK).

The app requires your system to be: **Windows 10 ver.1809** and above.

You can also clone the repository locally and run it through Visual Studio 2019.

After cloning, you need to open the files in the project, change the certificate to a self-signed certificate under the Packaging tab, and then rebuild the application and deploy it.`package.appxmanifest`

## Directions for use

### Timer

The app doesn't have many features, and the core is just a timer.

The timer is a forward timer rather than a countdown, meaning you can use it to keep track of how long it took you to complete something, rather than completing it within a set time.

The timer can only exist one at a time, and its ideal use case is a single-threaded mode of operation, where only one thing is done before moving on to the next.

The timer doesn't pause _(you can watch the time go by, but you can't stop it),_ and when you stop the timer, it means that the work corresponding to the timer has been completed. This timing record is saved.

You can click on the text below the timer button (the background color and cursor will change when you hover over it) to change its content to describe what you're currently doing. It will be saved as the title of the timer.

There is also a button below the title, click this button to switch the app to small window mode, that is, hover to the top of the screen in the upper right corner, click again to exit small window mode.

### History

Considering that there may be a need for inclusion, the app has added grouping and history features after the remaster.

#### Groups

Groups are used to divide timers based on custom categories e.g., date, usage scenarios, scope, or whatever the user's preference. To group timers, click the button in the bottom left corner to display the grouping information. The currently selected group is highlighted.

![](https://camo.githubusercontent.com/c08a48094ccfbbfb0c07bcec014bc245a1862c718e34b9c4738dfff9a7948a43/68747470733a2f2f692e6c6f6c692e6e65742f323032302f30372f30382f377a6434656d68505553564d7643392e706e67 "groups")

#### Records

When the timer stops timer, the timing record is saved to the currently selected group, forming a historical record.

![](https://camo.githubusercontent.com/8e9289e7ebcfa5ca50ce3e5462f5d22bf84259d0245a86e14864ad9dac47ebb4/68747470733a2f2f692e6c6f6c692e6e65742f323032302f30372f30382f6a4a736c59544c7064664e484461682e706e67 "record")

The historical record mainly includes: 
1. `Timer Title`,
2. `Start Time`,
3. `Time Elapsed`  

If you want to move the record to another group, you can do so by clicking the more button (three dots) on the card.

### Aggregate total

The app tracks the total time elapsed of all timers cumulatively, and an upper limit can be set. The default is 6 hours (360 minutes), which can be adjusted it in the settings. After configuration, every time an additional timer instance is added, the app will automatically count the total tracked time, displaying the figure at the bottom of the app interface.

### App settings

The app provides four basic settings:

1.  Theme settings

Optional, and follow the system to synchronize with the current system theme settings.`Light``Dark``System Default`

2.  Font settings

The app supports global font adjustment, and you can choose your favorite font to display.

3.  Language settings

The app supports Chinese and English, and can be accessed on demand.

4.  Preset duration

It is used to configure the number of hours to be worked per day for statistical purposes.

_Since the application is already open source, there is an additional open source address button in the settings that leads to the repository_

## Tool references

-   [Windows Community Toolkit](https://github.com/windows-toolkit/WindowsCommunityToolkit)
-   [Richasy.Helper.UWP](https://github.com/Richasy/Richasy-Helper-UWP)
-   [Richasy.Font.UWP](https://github.com/Richasy/Richasy-Font-UWP)
-   [Richasy.Controls.UWP](https://github.com/Richasy/Richasy-Controls-UWP)
