# Visual Studio Code - Remote Development Setup

Assume using **macOS** to SSH into a Raspberry Pi

## Advantage of remote development
In this document, we will leverage our powerful computer/nice keyboard/magic mouse to develop, but saving/running/debugging codes in Raspberry Pi. As a result, we neither have to `scp` our code from this powerful computer to Raspberry Pi, nor `git push` from powerful computer and `git pull` from Raspberry Pi, before running that program from Raspberry Pi terminal.

General advantage of remote development mentioned in VS Code offical doc:

*The **Visual Studio Code Remote - SSH extension** allows you to open a remote folder on any remote machine, virtual machine, or container with a running SSH server and take full advantage of VS Code's feature set. Once connected to a server, you can interact with files and folders anywhere on the remote filesystem.*

*No source code needs to be on your local machine to gain these benefits since the extension runs commands and other extensions directly on the remote machine.*

---

## How-to Steps
### Installation
- Install [Visual Studio Code](https://code.visualstudio.com/)
- Install [Remote Development extension pack](https://aka.ms/vscode-remote/download/extension) 

### SSH Connect to Raspberry Pi
- Make sure both Raspberry Pi and your computer connect to the same wifi SSID
- Open terminal in Raspberry Pi and find IP address by running

    ```bash
    hostname -I
    ```

- Open terminal in your computer and verify SSH connection

    ```bash
    ssh pi@<RaspberryPi_IP_Address>
    ```

### Using SSH keys
- You have successfully finished the steps above
- Create your local SSH key pair

    ```bash
    ssh-keygen -t rsa -b 4096 -f "$HOME/.ssh/id_rsa-raspberrypi"
    ```
    
- Copy the generated public key to Raspberry Pi

    ```bash
    export USER_AT_RASPBERRYPI="pi@<RaspberryPi_IP_Address>"
    export PUBKEYPATH="$HOME/.ssh/id_rsa-raspberrypi.pub"

    ssh-copy-id -i "$PUBKEYPATH" "$USER_AT_RASPBERRYPI"
    ```

- Open terminal in Raspberry Pi to validate that the `authorized_key` file is in the `.ssh` folder

- In VS Code, run `Remote-SSH: Open Configuration File...` in the Command Palette (**F1**), select an SSH config file, and add (or modify) a host entry as follows:

    ```bash
    Host <HOST_NAME>
        HostName <RaspberryPi_IP_Address>
        User pi
        IdentityFile ~/.ssh/id_rsa-raspberrypi
    ```
    
    `<HOST_NAME>` can be anything you want. In this doc, we use `raspberrypi`


- In VS Code, run `Remote-SSH: Connect to Host...` from the Command Palette (**F1**) and select `raspberrypi` or `<HOST_NAME>` that you set in the last step

- Now you should have remote development on Raspberry Pi via ssh!


## Reference & Troubleshoot
- [Remote Development using SSH](https://code.visualstudio.com/docs/remote/ssh)
- [Remote Development Tips and Tricks](https://code.visualstudio.com/docs/remote/troubleshooting#_configuring-key-based-authentication)