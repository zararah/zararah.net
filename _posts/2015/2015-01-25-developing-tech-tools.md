---
layout: post
title: "Developing effective technology tools: less shiny, more useful"
date: '2015-01-25'
category:
- data
- coding
- transparency
tags:
---

This week, I had the pleasure of joining a group of about 100 people working on topics around ['following the money'](http://tech.transparency-initiative.org/strategy-session/using-technology-to-follow-the-money/) at a two day workshop in Berlin. There was a mixture of people at this workshop; technologists, activists, journalists, and funders. One of the first 'spectogram' questions that was asked was regarding 'shiny tech tools, and whether they are useful or not. 

I found this statement, and the reactions that followed, particularly interesting - for the last year, I've been looking closely at how data is put online by international development organisations - normally, through "shiny" data portals, which seem to be used very rarely. The statement, and the rest of the workshop, got me thinking about what we makes an effective and useful technology tool.

<!--more-->

### What do we mean by "shiny" tech tools?

For background, let me explain the connotations associated with "shiny" tech tools; at least in this case, there usually seems to be an unsaid negative connotation with the word, implying that a "shiny" data portal or tech tool is inherently an unuseful or unused one. Essentially, something that looks good (especially to those with low levels of technical skills) - but does very little to solve the problem at hand, for any number of reasons.

Too often, these tech solutions are developed for the wrong reasons, for example to "match" competitors or similar organisations in the space, like the increasing trend of various UN agencies having their own, distinct and incompatible data portals. Or, to meet a standard or certain level; like organisations wanting to demonstrate their commitment to transparency for example. Or simply, to demonstrate that an organisation is up to date, modern, capable of employing the right buzzwords that people (funders?) are looking for, and using technology in their work, whether it is the correct solution or not.

I came across the latter solution a couple of times this week even; someone told me of a great idea that they had had - a portal, where they could put their budget or spending data online for everyone to see, and maybe even some automated visualisations. The way it was described made it sound almost exactly like [OpenSpending](http://openspending.org); but of course, using something that is already developed is a lot less interesting than coming up with your own version, which is another reason that "shiny" tech tools get developed; they didn't seem particularly interested or excited by the fact that their idea basically already existed.

This brings me to two main problems that I see in this space: the crucial aspects we miss out when developing new tech tools, and our lack of nuanced understanding and engagement with "open source".

### Overlooked steps in developing a new tech tool 

Firstly, from what I've seen, one of the most crucial roles in a tech tool is often left out; the users. As [I've written about before](http://zararah.net/blog/2014/09/18/the-road-to-hell-is-paved-with-brightly-coloured-bubble/), it's clear that many data portals and tools are not developed with the user in mind. Here, I feel like we could learn a lot from the private sector; thinking about UI or UX design ideas, or building out features based first on 'user stories' (as an example, [here are some I developed](https://docs.google.com/a/okfn.org/spreadsheets/d/1plrT-CZS0lFCOhWgL3OXF_yPpbq0nZoqK--TK8HWHSI/edit#gid=0) when building [my project website](http://opendevtoolkit.net)). At the stage of developing user stories, it might emerge that actually, a tech tool isn't the answer, and here, we need to be genuinely open to all sorts of possibilities.

Another aspect of effective tool development is being able to explain clearly and concisely what is needed from the tool to the people who are building it- here, people who act as 'tech translators' (hat tip to [Lucy Chambers](http://techtohuman.com/) for coining this term) are crucial. By this, I mean those who can bridge the gap between developers, and people with low levels of technical literacy but who came up with the concept or the project idea. This kind of mismatch happens a lot with data visualisation too - people start with the end product that they think will look great, but without thinking why they might need it, effectively starting the process backwards. I've seen it in both realms: people asking for an interactive map mainly because they've seen one and think it looks cool - or people wanting to emulate the latest trend in terms of tech tools, but with no idea how this matches to their needs.

We also need to realise that the tool development and launch isn't the end of the project, and build that into the wider project plan. I realised this especially sharply this week when running a session on OpenSpending together with [Friedrich](http://pudo.org): we came to the group to ask about new tech features that could be added to the platform, and realised that actually what was needed were better ways for people to engage with it. Technology wasn't the problem, but communications and marketing was; things like being notified when data you're interested in is added, or making it easier for people with topical interest to be able to follow and understand that particular topic. To quote the excellent site [Civic Patterns](http://civicpatterns.org) - "Build it, They Won't Come". 

We could also do with learning from other related areas: for example, the more national-level trend of civic technology. Again, I've mentioned this before- but [Civic Patterns](http://civicpatterns.org/) has a great collection of best practices around making a civic technology project succeed, that technology projects working on an international level could also follow and learn from. Or, from community-related journalism projects, for example via the articles on [Source](http://source.opennews.org/), a community of people working on code projects in journalism; their ethic of writing about and sharing ['learnings'](https://source.opennews.org/en-US/learning/) on their work is impressive, and contains some fascinating articles.

### Understanding and embracing open source

Far too often, tech-related solutions in this space end up being proprietary, closed source tools that can't be reused. Sadly, it seems that to many, the idea of being the one unique organisation or project to "fix" some niche is much more appealing than the idea of adapting what is already out there in the open source world, which might already perform the same function.

And, to make it harder, there's much more to making an **accessible** open source tool than simply open sourcing the code, too. To start, there's literally developing the code out in the open, for example using GitHub. There's documenting it well, so that a newcomer developer to the project can make sense of it, whether this be through thoughtful commit messages, or a detailed and up-to-date README document. And then, to encourage newcomers to the project, there's making a welcoming and inclusive community around it, whether this be through establishing a Code of Conduct for contributors to the code, or having an actively maintained and moderated mailing list, to name just a couple of methods.

Aside from the literal "code" side of the tool, too, there is the idea of being okay with - and actually welcoming- the fact that someone might take your idea or project, and remix it to be something else. And vice-versa, understanding that your great idea might already exist in some shape or form, and before starting anything else, actually looking out for projects that do similar things to what you want to do, and taking it and adapting it for your purpose. I tried to practise what I preach here last year when I was thinking about the development of the website for my project, the Open Development Toolkit. Instead of creating a whole new site, I took an already developed site - the Source one linked above- and forked it, to [create my own version.](https://github.com/zararah/source) Somewhat contrary to the point I'm making here, the people behind the site were totally on board with this, and gave me time and advice whenever I asked; I do wonder though, how many times this has happened? Other benefits aside, I also ended up [contributing once](https://github.com/mozilla/source/commit/8893206cbdcb04583c893ecd0ef4104466607bca) back to the original site, which brought benefits to both parties.

As a community of people working on engaging technology tools to solve social problems, I firmly believe that we need to both embrace open source, and develop these tools in a more thoughtful way. The guidelines and ideas behind the [Poplus Project](http://poplus.org/) are a great place to start learning about this. 

There are lots of communities and organisations who are already doing lots of these points, and much more besides, but I believe that more of us need to be aware of these issues, and address them head on. It's no mean feat, but from the energy and excitement I saw this week at the Follow the Money workshop, I do think it's possible. 
