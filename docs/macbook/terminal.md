# Terminal

Tools for terminal

All command should be typed into Terminal

---

## Homebrew

[Homebrew](https://brew.sh/) installs the stuff you need that Apple didn’t. Homebrew installs packages to their own directory and then symlinks their files.

Install:

Follow the [instruction](https://brew.sh) to install homebrew

Check version:

```bash
brew --version
```

Check brew location:

```bash
which brew
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

Open new terminal and check (it is suppose to show `/opt/homebrew/bin/zsh`):

```zsh
which zsh
```

### `.zshrc`

Please see the [`.zshrc`](https://github.com/duke-leeth/env-setup/blob/master/.zshrc).
If you like, download [`.zshrc`](https://github.com/duke-leeth/env-setup/blob/master/.zshrc) and put it under `~` (or `$HOME`) directory by 


```bash
curl -o $HOME/.zshrc https://raw.githubusercontent.com/duke-leeth/env-setup/master/.zshrc
```

---

## Oh My Zsh

[Oh My Zsh](http://ohmyz.sh/) is an open source, community-driven framework for managing your ZSH configuration. It comes bundled with a ton of helpful functions, helpers, plugins, themes, and a few things that make you shout...

Install:

Follow the [instructions](https://ohmyz.sh/#install)

---

## Vim

[Vim](http://www.vim.org/) is a highly configurable text editor built to make creating and changing any kind of text very efficient. It is included as "vi" with most UNIX systems and with Apple OS X.

Follow the instruction to [install vim via homebrew](https://formulae.brew.sh/formula/vim)

---

## Vundle

[Vundle](https://github.com/VundleVim/Vundle.vim) is short for Vim bundle and is a Vim plugin manager.
* Setup

  ```bash
  git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
  ```

* Configure Plugins

  * Download [`.vimrc`](https://github.com/duke-leeth/env-setup/blob/master/.vimrc) and put it under `~` (or `$HOME`) directory to use Vundle

  ```bash
  curl -o $HOME/.vimrc https://raw.githubusercontent.com/duke-leeth/env-setup/master/.vimrc
  ```

* Install Plugins:

  * Option 1: Launch `vim` and run `:PluginInstall`
  * Option 2: Install from command line: `vim +PluginInstall +qall`

### [Onedark Theme](https://github.com/joshdick/onedark.vim)

  > Install the theme using your Vim plug-in manager of choice (or manually, by placing colors/onedark.vim in your ~/.vim/colors/ directory and autoload/onedark.vim in your ~/.vim/autoload/ directory.)

---
