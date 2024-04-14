---
title: "Semantic pull request titles for documentation"
description: "Using these rules when creating a pull request title _won't_ make you a better person, but it might improve your Git repository. I based this post on a GitHub gist from [joshbuchea's](https://gist.github.com/joshbuchea) called [`semantic-commit-messages.md`](https://gist.github.com/joshbuchea/6f47e86d2510bce28f8e7f42ae84c716)."
date: 2024-04-14
---

I'm sure we've all seen Git repos with a shocking amount of branches. Without a decent naming convention, things can get messy real quick. The idea here is that adding the tags below to the start of your branch makes it easier for folks to quickly figure out what your trying to do.

## Types

These are the available types:

| Type | Description | Example |
| ---- | ----------- | ------- |
| `feat` | Adds a **new** section or page. New paragraphs to existing documentation are not a feature. | `feat/desktop-install` |
| `add` | Adds a **new** paragraph, sentence, or image to existing documentation. | `add/desktop-install-screenshots` |
| `remove` | Removes **existing** paragraphs, sentences, or images from existing documentation | `remove/browser-disclaimer` |
| `fix` | Fixes an **existing** typo, spelling, grammar, or formatting mistake. | `feat/desktop-broken-repo-link` |
| `refactor` | Completely changes an **existing** section or page while keeping the original narrative/purpose. Refactors are changes to documentation that do not result from a platform/package/software release. | `refactor/simplifies-dht-explanation` |
| `update` | Changes to **existing** documentation due to platform/package/software releases. Updates to documentation as a direct result of updates to platforms/packages/software releases. | `update/install-section-go-ipfs-0-7` |
| `chore` | Updates automation, CircleCI tasks, linting rules, etc. Chores do not fix documentation. | `chore/redirects-for-concepts-section` |

## Example

```plaintext
feat/ipfs-desktop-install
^--^  ^------------^
|     |
|     +-> Summary of your changes
|
+-------> Type: feat, add, remove, fix, refactor, update, or chore.
```
