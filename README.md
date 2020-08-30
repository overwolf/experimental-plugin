### HAGS Overview

The WINDOWS 10 HARDWARE-ACCELERATED GPU SCHEDULING (HAGS) feature is currently supported on Windows 2004 and Nvidia's latest GPU driver (451.49).  
When set to On, it might cause captured videos to be laggy/choppy.

This is a quick experimental plugin with a simple way of detecting if it is on or not.

### Sample app

1. Download this sample app and load it as an unpacked extension.
2. The app contains a single-window without any controls. Just open the dev tools for this window.
3. The plugin will print to the console `isHAGSEnabled = false` or true. 

### Check if HAGS enabled in your app

In the same way, you can integrate this plugin in your app to detect if the HAGS Enabled or not.  
If you detect it is on, you can give a warning to the user with a link to change this setting:

You may open the relevant Windows Graphics settings by calling:  [overwolf.utils.openUrlInDefaultBrowser('ms-settings:display-advancedgraphics')](https://overwolf.github.io/docs//api/overwolf-utils#openurlindefaultbrowserurl).

