# Application

A list of recommended applications

## Browser

* [Edge](https://www.microsoft.com/en-us/edge?r=1)

---

## Cloud Space

* [Dropbox](https://www.dropbox.com/)
* [OneDrive](https://onedrive.live.com/)
* [Pocket](https://getpocket.com/)

---

## Remote Tool

* [ZOOM](https://zoom.us/)
* [Skype](https://www.skype.com/)
* [TeamViewer](https://www.teamviewer.us/)

---

## Messenger

* [Telegram](https://telegram.org/)
* [Line](https://line.me/)

---

## System Tool

* [Rectangle](https://rectangleapp.com/)
* [Battery Health 2](https://itunes.apple.com/us/app/battery-health-2-monitor-battery-stats-and-usage/id1120214373?mt=12)
* [The Unarchiver](https://theunarchiver.com/)
* [OmniDiskSweeper](https://www.omnigroup.com/more)
* [AppCleaner](https://freemacsoft.net/appcleaner/)
* [Dr. Cleaner](https://itunes.apple.com/us/app/dr-cleaner-disk-mem-clean/id921458519?mt=12)
* [Android File Transfer](https://www.android.com/filetransfer/)

---

## Media - Sound / Music / Video

* [Audacity](http://www.audacityteam.org/)
* [VOX](https://vox.rocks/mac-music-player)
* [VOX Preferences](https://vox.rocks/mac-music-player/control-extension-download)
* [Free Mac Media Player](https://www.macblurayplayer.com/mac-media-player.htm)
* [Cisdem Video Player](https://www.cisdem.com/video-player-mac.html)

---

## Office

* Microsoft Word / Powerpoint / Excel / OneNote

---

## Programming

### [Miniconda](https://docs.conda.io/en/latest/miniconda.html)

* [Miniconda macOS installers](https://docs.conda.io/en/latest/miniconda.html#macos-installers) and download the `Miniconda3 macOS 64-bit pkg`


  | Command            | Description |
  | ------------------ | ----------- |
  | `conda create -n <ENV_NAME> python=<VERSION>` | create an environment named as `ENV_NAME` with python `VERSION` |
  | `conda create -n py39 python=3.9` | create an environment named as `py39` with python3.9 installed |
  | `conda create -n py27 python=2.7` | create an environment named as `py27` with python2.7 installed |
  | `conda create -n py39 python=3.9 anaconda` | create an environment named as `py39` with python3.9 and anaconda packages installed |
  | `conda create -n py39 python=3.9 notebook` | create an environment named as `py39` with python3.9 and `Jupyter Notebook` installed. For more info: [Installing Jupyter](https://jupyter.org/install#jupyter-notebook). |
  |  |  |
  | `conda env list` | view a list of conda environment |
  |  |  |
  | `conda list -n <ENV_NAME>` |  view a list of packages in `ENV_NAME` environment |
  | `conda list -n py39` |  view a list of packages in `py39` environment |
  |  |  |
  | `conda activate <ENV_NAME>` | activate environment named as `ENV_NAME` |
  | `conda activate py39` | activate environment named as `py39` |
  |  |  |
  | `conda deactivate` | deactivate environment and switch to base environment |
  |  |  |
  | `conda install -n <ENV_NAME> <PACKAGE_1> <PACKAGE_2>` | install specific packages, i.e. `PACKAGE_1` `PACKAGE_2`  to `ENV_NAME` |

* Reference: [Use conda to manage environments](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html)

### [Visual Studio Code (VS Code)](https://code.visualstudio.com/)

  * Install `code` command to terminal
    * Open Visual Studio Code Application
    * Type `⇧ ⌘ P` to open `Command Palette` 
    * Type command `install code` and press `Enter`
    * You will see a pop up message in Visual Studio Application window as

      `Shell command 'code' successfully installed in PATH.`
    * Open `Terminal` and type in the command to see if the `code` works properly 

      ```bash
      $ which code

      /usr/local/bin/code
      ```

  * Extensions
    * Programming languages

      For more languages: [supported programming languages](https://code.visualstudio.com/docs/languages/overview) 

      * [Java Extension Pack](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-pack)
      * [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
      * [C++](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools)
      * [JavaScript](https://code.visualstudio.com/docs/languages/javascript)

  * Useful shortcuts:

    | Shortcut          | Description |
    | ----------------- | ----------- |
    |  |  |
    |  Terminal  |
    | ``^ ` ``          | toggle integrated terminal |
    |  |  |
    |  Editor management |
    | `⌘ \`             | split the editor |
    | `⌘ NUMBER`        | witch between views e.g. `⌘ + 1`, `⌘ + 2` |
    |  |  |
    | Navigation |
    | `⌃ g`             | go to line |
    | `⌘ ↑`             | go to the beginning of a file |
    | `⌘ ↓`             | go to the end of a file |
    | `⌘ ←`             | go to the start of the line |
    | `⌘ →`             | go to the end of the line |
    | `home`            | go to the start of the line |
    | `end`             | go to the end of the line |
    | `⌘ ⇧ o`           | go to entity (e.g. variables, functions, etc) |
    |  |  |
    | Editing |
    | `⌥ ↑`             | move line up |
    | `⌥ ↓`             | move line down |
    | `⌥ ⇧ ↑`           | copy the line and paste it above |
    | `⌥ ⇧ ↓`           | copy the line and paste it below |
    | `⇧ ⌘ k`           | remove the line |
    | `⌘ enter`         | insert a line below |
    | `⇧ ⌘ enter`       | insert a line above |
    | `⌘ ⇧ \`           | jump to matching bracket |
    | `⇧ ⌥ a`           | add block comment |
    | `⇧ ANY_DIRECTION` | hightlight code |
    | `⇧ d`             | select next match |
    | `⌘ u`             | takes the cursor back to where it was prior to the jump |
    | `⌥ CLICK`         | add cursor |
    | `⌘ ⌃ ⇧ ←`         | select pieces of code based on scope |
    | `⌘ ⌃ ⇧ →`         | select pieces of code based on scope |
    | `⌘ t`             | search the whole project for a given piece of code |
    |  |  |
    | File management |
    | `⌘ 0`             | focus the explorer panel  |
    | `⌘ b `            | toggle sidebar |
    | `⌘ ⇧ e`           | sidebar focus |
    | `⌘ ↓`             | open file/folder in the sidebar |
    | `⌘ tab`           | change file tabs |
    | `⌘ p`             | select files by opening a search bar, and type in either a filename or a full path |
    | `⌘ ⇧ t`           | reopen closed editor |
    | `⌘ enter`         | open file onto the side |
    | `⌘ +`             | zoom in |
    | `⌘ -`             | zoom out |
    |  |  |

    * [Keyboard shortcuts for macOS](https://code.visualstudio.com/shortcuts/keyboard-shortcuts-macos.pdf)
    * [Key Bindings for Visual Studio Code](https://code.visualstudio.com/docs/getstarted/keybindings)
    * [Learn these keyboard shortcuts to become a VS Code ninja](https://blog.logrocket.com/learn-these-keyboard-shortcuts-to-become-a-vs-code-ninja/)

### [Atom](https://atom.io/)

  * useful plugins:
    * [platformio-ide-terminal](https://atom.io/packages/platformio-ide-terminal)
    * [Script](https://atom.io/packages/script)
    * [Hydrogen](https://atom.io/packages/hydrogen)

### [JetBrains](https://www.jetbrains.com/products.html)

  * [IntelliJ IDEA](https://www.jetbrains.com/idea/)
  * [PyCharm](https://www.jetbrains.com/pycharm/)
  * [CLion](https://www.jetbrains.com/clion/)
  * [WebStorm](https://www.jetbrains.com/webstorm/)

### [Xcode](https://developer.apple.com/xcode/)

### [Matlab](https://www.mathworks.com/products/matlab.html)

---

## Ptt

* [Welly](https://github.com/clyang/welly)

---

## 3D Printer

* [PrusaSlicer](https://www.prusa3d.com/drivers8)
* [Fusion 360](https://www.autodesk.com/products/fusion-360/overview)

---
