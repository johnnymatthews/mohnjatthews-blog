---
title: "Disable Caps Lock in Manjaro"
description: "It's literally all in the title. This post shows you how to disable caps-lock in Manjaro, and possibly other Linux distros."
date: 2024-08-29
---

Right, this is crazy simple:

1. Open terminal.
2. Enter:
    
    ```shell
    setxkbmap -option ctrl:nocaps
    ```

3. That's it.
