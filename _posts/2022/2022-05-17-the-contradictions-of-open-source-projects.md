---
layout: post
title: "The contradictions of open source communities and projects"
date: '2022-05-17'
category:
- bookworm
- technology
- diversity
---

One of my first consultancy projects is looking at strengthening the open source ecosystem, and as part of it, I've been catching up on research that might help inform next steps - such as Nadia Eghbal's 2020 book, ['Working in Public: The Making and Maintenance of Open Source Software'](https://app.thestorygraph.com/books/2505f748-ac12-41fb-a411-0868cbe3694c).

<!--more-->


It's a great read, and articulates well some inconsistencies and struggles that I've anecdotally heard of and wondered about - such as the contradictions inherent in how we think about the health of open source projects and contributors. For example, the role of creating an open source project - that is, coming up with an idea (usually to meet a specific need) and writing the code for it - is significantly different to other roles that are also necessary for that project to get lots of contributions, such as documentation, onboarding new contributors, reviewing their contributions, and maintaining that project. However, those other roles may be far less interesting to the initiator of the project - and the way in which the contributions graph on Github is structured means that pushing code is more valued than responding to pull requests (though there are some interesting projects and approaches to countering that, such as [All Contributors](https://allcontributors.org/)).

At a time when I feel like many in the spaces I'm in are valuing the role of maintenance, I found this description particularly illustrative:

*An open source maintainer... is expected to maintain the code they published for as long as people use it. In some cases, this could be literally decades, unless the maintainer formally steps away from the project. This is the equivalent of a writer being asked to edit and make changes to the same book every day, into perpetuity, long after they’ve reaped the initial financial and reputational rewards from its creation. (p96)*

I feel like that description makes it really clear how the structures around maintenance of open source projects are so unique and actually make little sense. She draws a distinction between two often-conflated parts of open source, too:

*I’d like to... argue that managing open source code requires separating its production from consumption: treating them as not one but two types of economic goods. Anyone can consume code, but only a limited number of people can produce it.*

So the issue really, when it comes to strengthening the open source ecosystem, seems to be less about supporting consumers of code and more about introducing more nuance into how we consider 'producers' of the code. It's startling to consider that the way in which we consider 'success' of an open source project (eg. lots of contributors, lots of users, been going for a long time) is actually often not what the author of that project wants, because that means they have to do a lot more work that is very far removed from their original role of writing the code for that project.

Eghbal describes how in the case of open source projects, which can be used over and over again at no cost to the author, the real problem comes with how the open source producer's attention is used:

**"A tragedy of the commons occurs not from consumers over-appropriating the content itself, but from consumers over-appropriating a creator’s attention"** - noting that every pull request, every new person who wants to join the project, every request for a new feature, every maintenance update - requires attention and time, and that those roles and tasks might just not be that interesting for the person who made the project (often in their spare time, and often for fun or to meet their own specific need). 

In fact, increasing the diversity of contributors to a project (eg. by lowering the barrier to entry) may well create too much work (too many new people to onboard, many pull requests that need a close review or back-and-forth on) for the maintainer(s), which means that it might actually be in the best interest of whoever's project it is to just keep the contributors to a minimum. That feels counterintuitive to me in many ways, especially recognising the value of a diverse group of collaborators, but as Eghbal describes it in practical terms, and noting the ways in which open source contributions are valued and rewarded (or not), I can see why this may be the case. Especially when a project is just run by one person, without community infrastructure, there are a lot of roles and tasks that can suddenly pop up when a project gains in popularity, and as illustrated with the quote above about the longevity of maintenance, these don't go away over time.

So how, in the long run, can we both incentivise healthy (resilient, sustainable) communities around projects, while recognising that many different types of people need to contribute to make that happen; and also that the attention of producers of open source code is limited and sometimes people need to step away? It seems like having an easier sunsetting process (or retirement, if specific people want to step away from projects) might help subvert the expectations that people will stay with projects for as long as they're going. Or, better metrics or ways of recognising non-code contributions (noting that we measure what we care about) on platforms like Github (to flag, [Gitlab already recognises more contributions than just code](https://docs.gitlab.com/ee/user/group/contribution_analytics/)).

Anyway. I'll be reading more on this in the coming weeks, and would love any suggestions for where to look or who to talk to!

















