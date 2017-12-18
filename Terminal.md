
# Terminal
#### Tools for terminal

All command should be typed into Terminal

## Homebrew

[Homebrew](https://brew.sh/) installs the stuff you need that Apple didn’t. Homebrew installs packages to their own directory and then symlinks their files into `/usr/local`

Install:
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Check version:
```
brew --version
```


## Zsh
[ZSH](http://www.zsh.org/) is a shell designed for interactive use, although it is also a powerful scripting language.

Install:
```
brew install zsh
```

Check version:
```
zsh --version
```

Switch from bash to zsh:
```
sudo sh -c "echo $(which zsh) >> /etc/shells"

chsh -s $(which zsh)
```

Open new terminal and check (it is suppose to show `/bin/zsh`):
```
echo $SHELL
```

## Oh My Zsh
[Oh My Zsh](http://ohmyz.sh/) is an open source, community-driven framework for managing your ZSH configuration. It comes bundled with a ton of helpful functions, helpers, plugins, themes, and a few things that make you shout...

Install:
```
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```


## tmux
[tmux](https://github.com/tmux/tmux/wiki) is a terminal multiplexer. It lets you switch easily between several programs in one terminal, detach them (they keep running in the background) and reattach them to a different terminal.
```
brew install tmux
```

## ctags
[ctags](http://ctags.sourceforge.net/) generates an index (or tag) file of language objects found in source files that allows these items to be quickly and easily located by a text editor or other utility. A tag signifies a language object for which an index entry is available (or, alternatively, the index entry created for that object).
```
brew install ctags
```
