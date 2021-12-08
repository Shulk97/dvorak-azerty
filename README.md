Dvorak-azerty on Linux
------

This repository is an Azerty version of the project dvorak-qwerty (https://github.com/ZeptByteS/dvorak-qwerty).
The project contains two layouts that replace Qwerty by Azerty and Dvorak by programmer dDvorak from by Roland Kaufmann (https://www.kaufmann.no/roland/dvorak/).

------

In this layout, you can input Dvorak layout symbols while Capslock is on. And turn it off to switch back to Azerty layout.  Any key will always work as Azerty when pressed with Control, Alt or Super regardless of the state of the Capslock. For that, Caps lock can't be used for input uppercase.  

Installation
------

\#./install.sh

It will save your xkb configuration in archive named xkb-backup.tar.gz located in your working directory and will install the new configuration files.

After reboot, you can choose the Dvorak-Qwerty layout from text entry setting:




Issues with Gnome
------

Gnome may override some keys in some cases that existed in other levels that did not interfere in previous configurations.

You can clear these bindings with the help of dconf-editor.

Steps:

1. Install dconf-editor for your distro

2. Open dconf-editor

3. Browse through /org/gnome/desktop/input-sources and find xkb-options.

4. Remove from the string the record that overrides your keymap
