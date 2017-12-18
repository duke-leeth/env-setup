# MacSetup
## Mac environment setup
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
szzsh --version
```

Switch to zsh from bash:
```
chsh -s $(which zsh)
```

Check success (it is suppose to show `/bin/zsh`):
```
echo $SHELL
```

## Oh My Zsh
[Oh My Zsh](http://ohmyz.sh/) is an open source, community-driven framework for managing your ZSH configuration. It comes bundled with a ton of helpful functions, helpers, plugins, themes, and a few things that make you shout...

Install:
```
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

Change theme:
In `~/.zshrc`, replace line `ZSH_THEME=”…”` with `ZSH_THEME="agnoster"`.
