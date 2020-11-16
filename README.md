# Jriver_LCD_Smartie_Plugin_Fix

The Jriver Media Center LCDSmartie 32-bit and 64-bit plugin installers are written for a specific Media Center version. The plugin can be installed on more recent Media Center versions by changing the default installation path to point to the latest installation directory. However, the plugin will not be recognized by MC, even though the installation appears to have been successful. This is because certain registry entries are hard-coded within the installer to a fixed version registry hierarchy.

A workaround is  to install the plugin, pointing it to the latest Media Center installation directory, then run the appropriate .reg file from this repository to create the needed registry key. Once run, the plugin magically appears when Media Center is relaunched.

One caveat, if you use the plugin uninstaller from the latest plugin, it will leave behind the registry entries created by the workaround files. It will also disable the plugin from the older version of Media Center, if you have it installed, as it will delete the needed hard-coded registry values!
