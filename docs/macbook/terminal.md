# Terminal

Tools for terminal

All command should be typed into Terminal

---

## Homebrew

[Homebrew](https://brew.sh/) installs the stuff you need that Apple didn’t. Homebrew installs packages to their own directory and then symlinks their files into `/usr/local`

Install:

```bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Check version:

```bash
brew --version
```

---

## Git

[Git](https://git-scm.com/) is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

```bash
brew install git
```

---

## tmux

[tmux](https://github.com/tmux/tmux/wiki) is a terminal multiplexer. It lets you switch easily between several programs in one terminal, detach them (they keep running in the background) and reattach them to a different terminal.

```
brew install tmux
```

---

## ctags

[ctags](http://ctags.sourceforge.net/) generates an index (or tag) file of language objects found in source files that allows these items to be quickly and easily located by a text editor or other utility. A tag signifies a language object for which an index entry is available (or, alternatively, the index entry created for that object).

```bash
brew install ctags
```

---

## Mercurial

[Mercurial](https://www.mercurial-scm.org/) is a free, distributed source control management tool. It efficiently handles projects of any size and offers an easy and intuitive interface.

```bash
brew install mercurial
```

---

## ZSH

[ZSH](http://www.zsh.org/) is a shell designed for interactive use, although it is also a powerful scripting language.

Install:

```bash
brew install zsh
```

Check version:

```bash
zsh --version
```

Switch from bash to zsh:

```bash
chsh -s $(which zsh)
```

Open new terminal and check (it is suppose to show `/usr/local/bin/zsh`):

```zsh
which zsh
```

### `.zshrc`

Please see the [`.zshrc`](https://github.com/duke-leeth/env-setup/blob/master/.zshrc).
If you like, put [`.zshrc`](https://github.com/duke-leeth/env-setup/blob/master/.zshrc) to `~` directory by cloning this repository.


```bash
git clone https://github.com/duke-leeth/env-setup.git

mv <PATH_TO_THIS_REPOSITORY>/.zshrc> ~
```

---

## Oh My Zsh

[Oh My Zsh](http://ohmyz.sh/) is an open source, community-driven framework for managing your ZSH configuration. It comes bundled with a ton of helpful functions, helpers, plugins, themes, and a few things that make you shout...

Install:

```zsh
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

---

## Vim

[Vim](http://www.vim.org/) is a highly configurable text editor built to make creating and changing any kind of text very efficient. It is included as "vi" with most UNIX systems and with Apple OS X.

```bash
brew install vim --with-luajit
```

---

## Vundle

[Vundle](https://github.com/VundleVim/Vundle.vim) is short for Vim bundle and is a Vim plugin manager.
* Setup

  ```bash
  git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
  ```

* Configure Plugins
  * Download this repository via

  ```bash
  git clone https://github.com/duke-leeth/env-setup.git
  ```

  * Put [`.vimrc`](https://github.com/duke-leeth/env-setup/blob/master/.vimrc) under `~` directory to use Vundle

  ```bash
  mv <PATH_TO_THIS_REPOSITORY>/.vimrc ~
  ```

* Install Plugins:
  * Launch `vim` and run `:PluginInstall`
  * To install from command line: `vim +PluginInstall +qall`

### [Onedark Theme](https://github.com/joshdick/onedark.vim)

  > Install the theme using your Vim plug-in manager of choice (or manually, by placing colors/onedark.vim in your ~/.vim/colors/ directory and autoload/onedark.vim in your ~/.vim/autoload/ directory.)

---
