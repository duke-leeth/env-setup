# Mac Setup
## Mac environment setup
Date: 2020.04.18

Author: Duke Lee


Initialize new Macbook with the following:

1. [Application](Application.md)
2. [Terminal](Terminal.md)

Additional useful setting:
1. [Git Ignore .DS_store files](Git_Ignore_.DS_store.md)

# Troubleshoot
## When camera is not working
Open terminal and input the following command
```
sudo killall VDCAssistant
```

**Note**: In case that it does not solve the problem, use the following command instead
```
sudo killall AppleCameraAssistant
```
