+++
author = "Abdurrahman Rajab"
title = "Resetting Linux/Ubuntu password"
description = "Password resetting tips for ubuntu"
date = "2022-08-08"
tags = [
    "Learning",
    "Linux",
    "sysadmin",
]
categories = [
    "Learning",
    "Linux",
    "sysadmin",
]
aliases = ["linux_tips"]
+++

forgetting your system password could teach you a lot about how to handle this kind of situation and the system you are using. 
Thankfully, I use linux 😃, which helped me a lot to restart my personal account password. Here is the steps that I had to recover it: 

1. Go to recovery mode by pressing ESC when I booted my PC. 
2. Go to root mode 
3. use the command `passwd USERNAME`
4. Horay it's done! 

During this journey I set my root password by mistake which let me to learn that I can delete it with: 

```
sudo passwd -d `whoami`
```

The whoami command will get the current user.

After all of that the keyring will ask you for your old password which you need to either reset it as well or remove it. You can find the detailed answer in the last link in the resources.


Helpful resources: 

* [askubuntu lost admin password](https://askubuntu.com/questions/24006/how-do-i-reset-a-lost-administrative-password)
*  [Official resources](https://wiki.ubuntu.com/RecoveryMode)
*  [Listing users](https://linuxize.com/post/how-to-list-users-in-linux/)
*  [Delete password](https://askubuntu.com/questions/281074/can-i-set-my-user-account-to-have-no-password)
* [Remove Keyring password](https://askubuntu.com/questions/191190/i-continue-to-get-this-when-trying-to-log-into-ubuntu-one-from-the-ubuntu-deskto)