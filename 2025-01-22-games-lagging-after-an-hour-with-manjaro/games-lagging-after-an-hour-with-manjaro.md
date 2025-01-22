---
title: "Games lagging after an hour with Manjaro"
description: "I've having a problem with Manjaro at the moment where games will start to stutter after about an hour of play. Before then, everything's running super smoothly with no issues. I found a potential solution."
date: 2025-01-22
---

This solution isn't mine, I'll admit. I found it on some random Reddit thread that I can't find anymore. Anyway, here's what you need to do:

1. Open Steam.
1. Find the game you're having trouble with in your library, right click and select **Properties...**.
1. Under **Launch Options**, add:

    ```plaintext
    LD_PRELOAD="" %command%
    ```

1. Close that window and launch your game.

Hopefully this fixes the issue. It _seems_ to have solved things in Chivarly 2 and Space Marine 2; for me at least.
