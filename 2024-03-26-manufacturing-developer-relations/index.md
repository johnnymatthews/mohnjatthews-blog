---
title: "Manufacturing developer relations"
description: "Developer relations, or devrel, is essentially a programmers version of a customer success team. It's all about building relationships between a tech company, and the developers who use that company's stuff. Setting up a devrel team or strategy can be tricky, and there's one huge pitfall I see companies fall into again and again."
date: 2024-03-26
---

## Devrel for beginners

There are five primary responsibilities of a devrel team:

1. **Advertise**: Hype and shill the company's products and services to external developers.
1. **Build a community**: Create an active community around the company's offerings. Generally speaking, this involves: 
    - Organizing events like hackathons, conferences, and meetups.
    - Providing resources like project templates, boilerplate code, and environment setup scripts.
    - Setting up communication channels for external developers to connect with each other.
1. **Provide support**: Give external developers the help they need through technical support, documentation, tutorials, and other resources to use the company's products effectively.
1. **Give feedback**: Listen to what developers have to say, get their insights and wish lists to help improve products down the line, and feed that to the internal engineering teams.
1. **Advocate**: Be the voice for external developers _inside_ the company and make sure their needs and concerns are heard.

If you've ever worked in or heard of a customer success team, you might recognize some similarities here. Customer success teams make sure that a company's customers have an easy time working with the company's product and have an avenue to express their thoughts/fears/concerns. Similarly, developer relations teams try to enable external developers to make really cool stuff.

Let's say, for example, that a company called _Massive Corp_ has a product called _massive.js_. The main use case for Massive.js is to allow developers to handle requests from millions of users at once. In this case, a devrel team would focus on creating examples of how to use Massive.js, fostering startups and small projects that need something like Massive.js, and going to events promoting the use of Massive.js. It's essential that the world has as many `.js` projects as possible; otherwise, GitHub will grind to a halt.

## The Pitfall

Now that we've covered the basics of what a devrel team does, we can get into the juicy side of where devrel strategies fall apart. It all comes down to one question:

**_Do you let the community grow organically, or do you try to stimulate growth artificially?_**

    
## Let's talk about video games

_Organic or artificial growth_ is a weird question, and to understand the answer, we need to turn to the world of competitive video games.

### Dota and Blizzard

Back in the early 2000s, there was this wildly popular custom map for Warcraft 3 called _Defense of the Ancients_ (eventually just shortened to Dota). The basic premise was that you had two teams of players controlling powerful heroes trying to push through waves of enemies and destroy the other team's base. This type of game became known as a _massive online battle arena_ (MOBA). It was great, and it inspired a bunch of spinoff games like League of Legends and Heroes of Newerth. Eventually, Valve bought the rights to Dota and created _Dota 2_ in 2013.

This whole situation really upset Blizzard because they felt that _they_ owned Dota, and thus, Dota 2. See, the Blizzard lawyers reckoned that because the game was created in a tool created by Blizzard, then it was _owned_ by Blizzard. This was a silly notion that caused Blizzard and Valve to go to court and file a suit in which Blizzard lost a lot of money and even more respect from the gaming community.

So, Blizzard decided to create a new game.

Like all MOBAs, [Heroes of the Storm](https://en.wikipedia.org/wiki/Heroes_of_the_Storm) (HotS) is a direct copy of Dota. Two teams, two bases, a bunch of mobs, some neutral creeps, and lots of heroes for the players to choose from. Simple. But Blizzard wanted more than just a game. It wanted money.

### The competitive scene

It's fair to say that most online games have a competitive scene: a community of players who battle out to be _the best_. Dota's competitive scene is pretty big. According to [escharts.com](https://escharts.com/games/dota2), Dota 2 ranks #6 for _all-time peak viewership_, and #1 in _total prize pool_ with a massive $313 million in available. This huge competitive scene spans many, _many_ years, with the first known Dota [competition happening in March 2006](https://dota2.fandom.com/wiki/History_of_Competitive_DotA_(The_First_Light_of_Dawn:_The_6.2x_Era)).

Blizzard, in an attempt to claim some market share from Dota, span up its own competition alongside the launch of Heroes of the Storm. The first major Heroes of the Storm tournament was the 2015 Heroes Global Championship, which featured a $500,000 prize pool. This set the stage for the game's burgeoning esports scene. In the following years, Blizzard continued to invest heavily in the Heroes esports ecosystem, hosting numerous regional and global championship events. Some of the most prominent Heroes of the Storm tournaments and leagues over the years included:

- Heroes of the Dorm (2015-2018): An annual college esports tournament.
- Heroes of the Storm Global Championship (2015-2018): Blizzard's premier global championship series.
- Dreamhack Heroes of the Storm tournaments (2016-2018).

However, in 2018, Blizzard made the surprise decision to discontinue its support for the esports scene. This led to the collapse of the game's professional ecosystem, with many top teams and players leaving the game. So, why the collapse?

Blizzard threw a ton of money at it, but it never came close to pulling in the kind of viewers and sponsorship cash that games like League of Legends and Dota 2 were bringing in. At the end of the day, the numbers just didn't add up - the costs of running a full global esports league for Heroes were way higher than the revenues they were seeing.

### Back to devrel

Much like Blizzard's investment in the HotS esports ecosystem, companies often jump into devrel with grand ambitions but without a true strategic commitment or deep understanding of the product and developer community. It becomes a box to check off rather than a genuine effort to foster organic growth and engagement.

Just as Blizzard poured resources into tournaments and leagues that failed to gain traction, companies can easily get caught up in hosting flashy hackathons, conferences, and other events that generate some short-term buzz but don't translate into long-term developer adoption or evangelism. The costs can quickly spiral out of control without a clear plan for sustainable value creation.

Additionally, companies may be overly focused on landing big-name sponsors, vendors, or high-profile projects to validate their devrel program, much like Blizzard likely wanted to attract the biggest esports organizations and viewerships. But true developer trust and loyalty has to be earned through consistent, authentic engagement over time - it can't be forced or bought.

It's not enough to just throw resources at the problem and hope for the best. Companies need a nuanced strategy, patience, and a laser focus on driving real value for developers rather than just chasing vanity metrics or short-term wins. Lessons learned from Blizzard's missteps in the HotS esports can help others avoid similar pitfalls in their own devrel journeys.

## Run stuff properly

First things first, **docs**. You need documentation that walks developers through how to use your product effectively. Get that foundation laid out super clearly before moving on to anything else.

Next up, **examples**. Give devs tons of sample code, tutorials, all that good stuff. Make it fairly simple for them to dive in and start playing around with your product.

Lastly, **community stuff**. It's cool if you've already got folks who are pumped about your project. But don't try to force-grow that community or anything before you've actually got the self-serve elements in place. Let that community develop naturally. Recreate the Dota 2 scene, not the HotS scene. Focus on empowering developers to succeed on their own before you start trying to supercharge things with events and contests and all that. Organic growth is where it's at.
