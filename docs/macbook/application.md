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
* [TeamViewer](https://www.teamviewer.us/)

---

## Messenger

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


### [pyenv](https://github.com/pyenv/pyenv)

* On macOS, update `homebrew` and install `pyenv`

  ```bash
  brew update
  brew install pyenv
  ```

  | Command            | Description |
  | ------------------ | ----------- |
  | **Create a new env** |
  | `pyenv install <PYTHON_VERSION>` | Create a new `PYTHON_VERSION` with pyenv |
  | `pyenv install 3.13.13` | Ceate an environment with python version `3.13.13` installed |
  |  |  |
  | **Remove a new env** |
  | `pyenv uninstall <PYTHON_VERSION>` | Remove a new `PYTHON_VERSION` |
  |  |  |
  | **List envs** |
  | `pyenv install --list` | List available Python envs to be installed |
  | `pyenv versions` | To see what is already installed on the machine |
  |  |  |
  | **Activate a specific Python version env** |
  | `pyenv local <PYTHON_VERSION>` | For a project folder  |
  | `pyenv shell <PYTHON_VERSION>` | For just the current shell session |
  |  |  |
  | **Deactivate the current env** |
  | `pyenv shell --unset` | Unset a shell-selected version |
  |  |  |
  | **Sets the default Python version globally** |
  | `pyenv global <PYTHON_VERSION>` | Set Python `PYTHON_VERSION` the default env |
  |  |  |

* Note:
  * `pyenv global` sets the default Python version for the user account, and pyenv stores that choice in `~/.pyenv/version`. That version is used in every shell unless a project-level `.python-version` file or a temporary shell override takes priority
  * Priority order
    * `pyenv` checks versions in this order: a shell override > a local project version > the global version > the system Python if no pyenv setting applies. So `pyenv global` is the broad default, but it is not the highest priority setting.
    * **IMPORTANT!!!** If you don't see the command `pyenv global <PYTHON_VERSION>` working, make sure there is no `.python-version` in the directory. Otherwise, the local project version has higher priority than the global one. 


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
