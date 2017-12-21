# Git Ignore .DS_store files
## Remove those annoying Mac OS X `.DS_Store` files from a Git repository

### Method I
* Remove existing files from the repository:
```
find . -name .DS_Store -print0 | xargs -0 git rm -f --ignore-unmatch
```

* Add the following in `.gitignore` via `vim .gitignore`
```
.DS_Store
```


### Method II
* Globally ignore these files from all the git repository on your system..
  1. Creating a global gitignore file:
  ```
  vim ~/.gitignore_global
  ```

  2. Adding Rules for ignoring files
  ```
  # Compiled source #
  ###################
  *.com
  *.class
  *.dll
  *.exe
  *.o
  *.so

  # Packages #
  ############
  # it's better to unpack these files and commit the raw source
  # git has its own built in compression methods
  *.7z
  *.dmg
  *.gz
  *.iso
  *.jar
  *.rar
  *.tar
  *.zip

  # Logs and databases #
  ######################
  *.log
  *.sql
  *.sqlite

  # OS generated files #
  ###################
  .DS_Store
  .DS_Store?
  ._*
  .Spotlight-V100
  .Trashes
  ehthumbs.db
  Thumbs.db
  ```

  3. Add this file to global git config:
  ```
  git config --global core.excludesfile ~/.gitignore_global
  ```
