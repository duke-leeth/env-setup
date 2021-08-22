# Macbook Env Setup

Initialize new Macbook with the following:

1. [Application](application.md)
2. [Terminal](terminal.md)

Additional useful setting:
1. [Git Ignore .DS_store files](git_ignore_.DS_store.md)

# Troubleshoot

## When camera is not working

Open terminal and input the following command

```bash
sudo killall VDCAssistant
```

**Note**: In case that it does not solve the problem, use the following command instead

```bash
sudo killall AppleCameraAssistant
```
