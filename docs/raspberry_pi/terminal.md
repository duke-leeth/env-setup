# Terminal

## Package manager `apt-get` update & upgrade

```bash
$ sudo apt-get update
$ sudo apt-get upgrade
```

---

## Python default version (system-wide)

Change the default python version system-wide ([reference](https://linuxconfig.org/how-to-change-from-default-to-alternative-python-version-on-debian-linux))


Run the following command to find out what python binary exexutables are available

```bash
$ ls /usr/bin/python*

/usr/bin/python            /usr/bin/python2-pbr       /usr/bin/python3.7m-config
/usr/bin/python2           /usr/bin/python3           /usr/bin/python3-config
/usr/bin/python2.7         /usr/bin/python3.7         /usr/bin/python3m
/usr/bin/python2.7-config  /usr/bin/python3.7-config  /usr/bin/python3m-config
/usr/bin/python2-config    /usr/bin/python3.7m        /usr/bin/python-config
```


Login as root user, and list all available python alternatives

```bash
$ update-alternatives --list python

update-alternatives: error: no alternatives for python
```

Update our alternatives table and include both `python2.7` and `python3.7`

```bash
$ sudo update-alternatives --install /usr/bin/python python /usr/bin/python2.7 1

update-alternatives: using /usr/bin/python2.7 to provide /usr/bin/python (python) in auto mode

$ sudo update-alternatives --install /usr/bin/python python /usr/bin/python3.7 2

update-alternatives: using /usr/bin/python3.7 to provide /usr/bin/python (python) in auto mode
````

The `--install` option take multiple arguments from which it will be able to create a symbolic link. The last argument specified it priority means, if no manual alternative selection is made the alternative with the highest priority number will be set. In our case we have set a priority 2 for 1/usr/bin/python3.7` and as a result the `/usr/bin/python3.7` was set as default python version automatically by update-alternatives command. 


Check the python version again

```bash
$ python --version

Python 3.7.3
```

List all python alternatives

```bash
$ update-alternatives --list python

/usr/bin/python2.7
/usr/bin/python3.7
```


```bash
$ Update-alternatives --config python

There are 2 choices for the alternative python (providing /usr/bin/python).

  Selection    Path                Priority   Status
------------------------------------------------------------
* 0            /usr/bin/python3.7   2         auto mode
  1            /usr/bin/python2.7   1         manual mode
  2            /usr/bin/python3.7   2         manual mode

Press <enter> to keep the current choice[*], or type selection number: 
```

---

## Vim

Check [Vim](../macbook/terminal.md#vim) for the instruction.

---

## Vundle

Check [Vundle](../macbook/terminal.md#vundle) for the instruction.

---

## Preserve your own `.vimrc` when `sudo`

Command pattern:

```bash
$ sudo -E vim <FILE_NAME>
```

Option explained:

```bash
-E    The -E (preserve environment) option indicates to the security policy that the user wishes to preserve their existing environment variables.  The
      security policy may return an error if the -E option is specified and the user does not have permission to preserve the environment.
```
