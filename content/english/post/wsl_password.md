+++
author = "Abdurrahman Rajab"
title = "Resetting WSL password"
description = "Password resetting tips for WSL"
date = "2023-04-15"
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
aliases = ["WSL_tips"]
+++
Working on WSL after leaving it for a while, could be such a great lesson for you! I recently forgot my password and found out that there is a way to recover it easily.

Here is the solution:

1. Change user to root.

    ```bash
    ubuntu config --default-user root
    ```

    For this, you might have a different run command for Ubuntu. which you can find in the reference but it's like the next:
    - Kali for Kali
    - ubuntu 2004 for Ubuntu 20.04
    - and so on

1. Set user password.

    here you need to open your WSL and set the password like Linux:

    ```bash
    passwd username
    ```
1. Change back to the default user.

    ```bash
    ubuntu config --default-user USERNAME
    ```
1. Horay!


Helpful resources:

* [intsfoss](https://itsfoss.com/reset-linux-password-wsl/)
