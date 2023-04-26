---
layout: home
title: The Sustainable Donation License
---

# Funding Open-Source Software with a better license

Software licensing is a pretty boring topic for most engineers.
If you're typical, you make a repo on GitHub and agree to the "use Apache 2 and/or MIT" convention that everyone else does, and then never think about it again.
After all, you just want to start writing some sweet code and become a rockstar.

However, Open Source is in trouble. As usual, Randall Munroe has summed it up for us neatly:

![https://xkcd.com/2347](https://imgs.xkcd.com/comics/dependency.png) <https://xkcd.com/2347>

You can see some specific examples of this:

- SBOM (tracking a "bill of materials" used in your supply-chain). How many maintainers are jumping on the [npm provenance public beta](https://github.blog/changelog/2023-04-19-npm-provenance-public-beta/)? That doesn't sound fun for them, and only BigCorps really need this.
- Entitled users vs. depressed maintainers. Read the [heartbreaking story of the core.js guy](https://github.com/zloirock/core-js/blob/master/docs/2023-02-14-so-whats-next.md). I come away from that feeling that he made a lot of poor financial decisions, but why was he prevented from making a living from wildly successful OSS?
- Suspicion of corporate motivations, for example Turbopack is the new Webpack but people claim "Vercel is evil why are they taking our OSS". I don't know the story, but I can imagine Tobias would like to afford food and clothing and not just toil on Webpack for free.

We have a fundamental disconnect between the economic engine that pays engineers at big companies, and the indispensible value these companies get from software that no one funds. Nadia Eghbal wrote a terrific book, and if you care about Open Source I recommend reading it: [Working in Public: The Making and Maintenance of Open Source Software](https://press.stripe.com/working-in-public).

## Existing solutions

At first I was disappointed that _Working in Public _ doesn't go into the problem of funding. However, the author has helpfully given away the answer for free :bow: on GitHub: [nayafia/lemonade-stand](https://github.com/nayafia/lemonade-stand). It lists the traditional options to fund OSS projects.

One kind of solution requires building a "sidecar" business around your OSS (like my company [Aspect](https://aspect.build) has done).
In this model, all your time spent on your OSS project is just the "marketing budget" for getting engineers to consider using your other, paid work.
It's exhausting, and also pulls you away from the OSS passion work to build something else.

Accepting donations is the other way to go. You can already do them a few ways.
I'm using [OpenCollective](https://opencollective.com/) on a few projects, and have spent a bunch of time hounding users to donate.
It feels a bit gross to answer someone's legit bug report with "no one pays me for that, would you like to?"

Even with a lot of "sales" effort, donations are not enough. Big companies that rely on OSS for critical business operations introduce burden but not funding.

## Modelling the problem as an "OSS outage"

Let's think of this from a "what if" perspective. It's like a Disaster Recovery simulation that companies do. They don't really know what "load bearing" edges they depend on, like that XKCD. So you just kick out a wall and see what happens. If the roof starts to cave in, then you needed that wall. You then do some structural engineering to make your building more resilient. Imagine this for OSS. What if some software you rely on was unavailable for a day?

We can do this with a license that includes "outages" as a feature. 364 days a year, the software is dual-licensed Apache2/MIT. One day a year (yes leap days thank you) a big company ought to pay.

HOWEVER, in practice a typical sequence of events:

1. Product engineer is trying to deliver on-schedule.
    
2. An OSS library/tool helps them do that quickly, they grab it and ship.
    
3. Lawyercats from Legal ask what licenses are in use and discover a "non-standard" one.
    
4. Laywercat tells the engineer "you can't use this"
    
5. Engineer can't justify the distraction required to escalate this to their manager and incur extra billing hours from their expensive legal team and go through some "enterprise sales" process, just to continue using this library
    
6. Engineer has to back out the feature and everyone hates the project that chose a non-standard license.
    
So, what we need is a way for that engineer to make the "compliance problem" just magically "go away" right there at step 3. Let's re-write the narrative:

3. Lawyercats from Legal ask what licenses are in use and discover a "non-standard" one.
    
4. Engineer figures it's worth a few dollars to keep using the library. They ask their manager to expense it. Even if the manager says no, the engineer figures they'll just pay $100 out-of-pocket for their 100-person company to use it, since it's totally worth it to them.
    
It might seem strange for an engineer to pay for software that their company uses rather than make the company pay. But, the engineer is the one who gets value from this library - they were able to ship and meet their manager's expectations and get career growth by "standing on the shoulders" of OSS authors who already solved part of the problem.

Any non-standard license will cause a decrease in adoption. Our goal here is to minimize that decrease, although it means we will not collect as much revenue as we might if we were more aggressive in terms and enforcement.

## Introducing the "Sustainable Donation License"

1. If you use the software for personal use, at a non-profit or university, or in a company with fewer than X employees, this software is dual-licensed for use under both Apache 2 and MIT.
    
2. If you use the software on days that aren't the outage day (April 1 of each year, say) then this software is dual-licensed for use under both Apache 2 and MIT.
    
3. Legal entities in the following list are granted a perpetual, royalty-free, etc. license to use the software at any time, including on the outage day:
    
    * \[empty list\]
        
4. This project exists only thanks to funding from its users. Anyone may donate to the project under \[OpenCollective or something\].
    
5. A donation may be accompanied with a nomination for any legal entity to be added to this license under section 3. The suggested donation is $1 USD per employee of the entity or its subsidiaries.
    

## Enforcement

Usually software licenses must be enforced in some way. We leave this up to each project to decide, however the intent of this license is that you only enforce it to the extent legally required for the license to be valid. If a bunch of companies don't have lawyers checking their licenses, and violate the terms, you could just let them do that.

By choosing to have an "outage day", many companies might just accept the risk of being non-compliant on one day of the year. Since our goal above was to minimize the adoption drop-off from a non-standard license, this is intentional.