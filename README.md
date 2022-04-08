## Introduction
Let's be honest: **Linux is harder to master than Windows.** Sometimes it's not user-friendly, and following an outdated tutorial may break your Linux4Tegra System.  
There is no centralized software repository, except for the `apt` repositories which lack many desktop applications.  
Surely there is a better way! **There is.**  
Introducing L4T-Apps, a well-maintained collection of app installation-scripts that you can run with **one click**.  

## Install L4T-Apps
Open a terminal and run this command:
```bash
wget -qO- https://raw.githubusercontent.com/Dark98/l4t-apps/master/install | bash
```
<img src="icons/screenshots/main%20window.png?raw=true" align="right" height="270px"/>

#### Supported systems:

- [Ubuntu 18.04(Linux4Tegra)](https://www.switchroot.org/) (64-bit): fully supported.
- Android, ChromeOS, non-ARM, non-Ubuntu(18.04) operating systems: Not supported. Your mileage may vary.

<details>
<summary><b>To install L4T-Apps manually</b> if you prefer to see what happens under the hood</summary>
 
```
git clone https://github.com/Dark98/l4t-apps
~/l4t-apps/install
```
</details>

<details>
<summary><b>To uninstall L4T-Apps</b></summary>
This will not uninstall any apps that you installed through L4T-Apps.

```
~/l4t-apps/uninstall
```
</details>

## To run L4T-Apps
- From the start menu: Accessories -> L4T Apps
- Use the terminal-command: `l4t-apps`
- Run L4T-Apps from its directory: `~/l4t-apps/gui`

## To Update L4T-Apps
- L4T-apps will automatically check for updates on boot and display a notification to update.
- To manually run the updater, use this command: `~/l4t-apps/updater gui`
- It also supports a cli interface: `~/l4t-apps/updater cli`

## Basic usage
L4T-Apps is very easy to use.  
- This is the **main window**.  
![main window](icons/screenshots/main%20window.png?raw=true)  
  - ![icon](icons/screenshots/buttons/search.png?raw=true) Search for apps.
  - ![icon](icons/screenshots/buttons/info.png?raw=true) Open the selected category. (you can also double-click on the category)
    
- Opening a category will reveal a **list of apps**:  
![app list](icons/screenshots/app%20list.png?raw=true)  
  - ![icon](icons/screenshots/buttons/back.png?raw=true) Go back to the main list of categories.
  - ![icon](icons/screenshots/buttons/install.png?raw=true) Install the selected app.
  - ![icon](icons/screenshots/buttons/uninstall.png?raw=true) Uninstall the selected app.
  - ![icon](icons/screenshots/buttons/info.png?raw=true) See more details about the app. (see **details window** below)

- This is the **details window**:  
![details](icons/screenshots/details%20window.png?raw=true)  
  - ![icon](icons/screenshots/buttons/back2.png?raw=true) Go back to the list of apps.
  - ![icon](icons/screenshots/buttons/scripts.png?raw=true) View the shell-scripts responsible for installing or uninstalling the selected app.
  - ![icon](icons/screenshots/buttons/edit.png?raw=true) Modify the app's description, icons, or scripts. (This button is hidden unless you enable it in Settings)
  - ![icon](icons/screenshots/buttons/install.png?raw=true) Install the selected app.
  - ![icon](icons/screenshots/buttons/uninstall.png?raw=true) Uninstall the selected app.
  - ![icon](icons/screenshots/buttons/credits.png?raw=true) See who played a part in adding the app.
  - ![icon](icons/screenshots/buttons/errors.png?raw=true) If the selected app failed to install, this button will allow you to see its error log.
    
- L4T-Apps Settings can be configured by launching Menu -> Preferences -> L4T-Apps Settings.  
![settings](icons/screenshots/settings.png?raw=true)  
In addition to changeable settings, this window also gives access to these tools:
  - ![icon](icons/screenshots/buttons/categories.png?raw=true) Does that one app seem to be in the wrong category? With this button, you can change it.
  - ![icon](icons/screenshots/buttons/new%20app.png?raw=true) Create a new app with a wizard-style set of dialogs. We recommend reading [the tutorial](https://github.com/Dark98/l4t-apps/wiki/Creating-an-app).
  - ![icon](icons/screenshots/buttons/log%20files.png?raw=true) View the past weeks-worth of installation logs. This is useful if you ever encounter an app that won't install and want to see the terminal output after you closed the terminal.
  - ![icon](icons/screenshots/buttons/import%20app.png?raw=true) This allows you to easily import a 3rd-party app from elsewhere. It helps L4T-Apps developers test upcoming apps for reliability on a variety of systems.

To learn more about L4T-Apps, read [the documentation](https://github.com/Dark98/L4T-apps/blob/master/DOCUMENTATION.md) and the [wiki](https://github.com/Dark98/l4t-apps/wiki).

