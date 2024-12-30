---
title: "Backdoors don't work"
description: "The cybersecurity situation in North America is becoming more and more dire as leaders fail to understand the basics of infosec, and as external threats continue to abuse this misunderstanding. One common knowledge-gap held by North American leaders is _\" Why can't we build a secure backdoor that only we can use, but the bad guys can't?/"_."
date: 2024-12-30
---

<!--Explain what backdoors are.-->

A _backdoor_ refers to any method that bypasses normal authentication or security controls to gain access to a computer system, network, or app. It's like a secret entrance that lets someone get into an area while avoiding the normal security _front door_. Backdoors can be created in a few different ways:

1. Deliberately installed by developers for maintenance or troubleshooting. While this is **super bad** security practice, it's fairly common since it makes the developer's job way easier.
1. Maliciously inserted by attackers who have already compromised a system. This often happens when hackers compromise developer machines and/or workflows.
1. Created through vulnerabilities in software or hardware, often through a supply-chain attack.

These types of backdoors are particularly prickly and can be hard to remove or even spot. But the type of backdoor we're going to discuss in the rest of this post is one that is **covertly installed by developers of a product or service at the behest of law enforcement**.

<!--Some historical examples of backdoors and how they got abused.-->
## Notable historical backdoors

I thought it'd be fun to run through a few backdoors that have been found in the past few years.

### The Dual_EC_DRGB debacle

The [Dual_EC_DRBG cryptographic algorithm](https://en.wikipedia.org/wiki/RSA_Security#NSA_Dual_EC_DRBG_backdoor) is fairly notable for having a sophisticated backdoor. The algorithm was standardized by the National Institute of Standards and Technology (NIST), but later revelations from the Snowden documents indicated that the National Security Agency (NSA) inserted a deliberate weakness that could be exploited to predict encryption keys. RSA Security made this algorithm the default in their BSafe products, reportedly after receiving $10 million from the NSA.

### Juniper Networks

The [Juniper Networks](https://en.wikipedia.org/wiki/Juniper_Networks#ScreenOS_Backdoor) case (2015) revealed unauthorized code in their NetScreen firewalls that persisted for several years. This backdoor allowed anyone knowing the hardcoded password to remotely access these devices, potentially compromising numerous corporate and government networks that used them.

### Salt Typhoon hack of US telecom services

This one is a doozy. The Salt Typhoon breach is an _ongoing_ cyberattack targeting major US internet service providers and telecommunications services. The attack involved exploiting vulnerabilities in the companies' networks, raising concerns about the security of critical infrastructure and the need for enhanced cybersecurity measures. The attackers were observed abusing backdoors placed into telecom services by law enforcement agencies.

## Why backdoors are bad

Ok, so now we know that backdoors are a thing and that they've been seen in the wild. But the biggest problem that the previous three examples outline is that backdoors placed into products by leaders and law enforcement _always_, **always** get abused at some point down the line. There's a common belief within leadership circles that we, developers and security professionals, should be able to just make the backdoor super secure while still allowing authorized users instant access to whatever service they're connected to.

Imagine you have a really strong lock on your front door. You think it's so strong that no one could ever break in. But just in case, you leave a spare key hidden under the welcome mat. You think it's safe because only you know about it. The problem is that anyone who knows about spare keys under welcome mats could come along and use them to get into your house. It's like leaving a secret backdoor open – you think it's safe, but it's really just waiting for someone to find it and use it for bad things.

> Ok, but what if you monitored the key super closely to make sure unauthorized people don't use it?

Constantly checking the key to make sure no one is tampering with it might seem safer, but there's a whole host of other problems that go along with this kind of baby-sitting:

Even the most vigilant person can make mistakes. Someone might accidentally bump the key, or you might get distracted and not notice someone trying to use it. The key itself might have flaws that someone could exploit, even if you're watching it closely. What if the person watching the key decides to use it for their own purposes? Maybe they want to let their friends in without your permission, or even worse; they could sell the key to someone else who might cause harm.

## The only real solution

Backdoors are always proposed using the same argument -- to enable the _good guys_ to do their work and catch the _bad guys_. But as we've just seen, this clearly doesn't work. The only real solution to avoiding huge security flaws like this is to utilize open-source software (OSS) as much as possible.

Transparency is a core tenet of OSS, with the idea being that anyone can examine the source code. This _many-eyes_ approach increases the likelihood of identifying and fixing vulnerabilities. Security researchers, independent developers, and everyday users can and do scrutinize the code for weaknesses, backdoors, or other malicious code.

When a vulnerability is discovered in open-source software, it's often quickly addressed -- unlike in closed-source programs where the maintainers can sweep the vulnerability under the rug and hope no one notices.

However, it's important to note that OSS is not inherently immune to security issues. Open-source projects rely on a vast ecosystem of dependencies. If a vulnerability exists in one of these dependencies, it can impact the security of the entire project -- often called a _supply chain attack_. Also, the effectiveness of community-driven security relies on the expertise and dedication of the community members.

So, we've covered the serious problems with backdoors in cybersecurity, especially how many leaders misunderstand them. A backdoor lets someone sneak into a system without going through normal security, often set up by developers or through security holes that hackers exploit. In the end, the best way to keep things secure is to completely get rid of backdoors.
