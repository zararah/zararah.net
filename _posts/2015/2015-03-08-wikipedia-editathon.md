---
layout: post
title: "What I learned at the Art and Feminism Wikipedia editathon"
date: '2015-03-08'
category:
- data
- technology
- global-dev
- feminism
tags:
- technology
---

This weekend was the [Art and Feminism](https://en.wikipedia.org/wiki/Wikipedia:Meetup/ArtAndFeminism) Wikipedia Editathon- a campaign to improve coverage of women and the arts on Wikipedia.

I joined the Berlin group today, and I did two main things: created a page for the feminist artist [Dilara Begum Jolly](https://en.wikipedia.org/wiki/Dilara_Begum_Jolly), whose work looks at social injustices in Bangladesh and globally, focusing on the role of women; and I improved the page of [Kanak Chanpa Chakma](https://en.wikipedia.org/wiki/Kanak_Chanpa_Chakma), a Bengali artist who focuses on the lives of ethnic minorities in Bangladesh.

I found both of them via this pretty enormous page, [Women Artists of Bangladesh](https://en.wikipedia.org/wiki/Women_Artists_of_Bangladesh). I wasn't sure where to start on cleaning it up purely because it is so unwieldy - that is to say, long, without many references or structure, and with a very unusual style of writing. So, I focused on the two of them instead. 

It is a lot more rewarding than I had thought to create a page and to see the improvements on Kanak Chanpa Chakma's page, too! To my surprise, just 4 hours after creating Dilara Begum Jolly's page, it's now in the top 5 hits when you search for her name on Google, too. 

Here are some things I learned today: 

<!--more-->

### Structuring a new page 

Though I've made some small edits before, and tried (!) to edit Hedy Lamarr's page (you can read about that tale of woe [here](http://zararah.net/blog/2014/11/09/happy-100th-birthday-hedy-lamarr/)) I've never created a page myself.

I know enough about Wikipedia to know that there are rules and guidelines around structure, so I wasn't sure quite how to start the page - but then I came across this [Biography template](https://en.wikipedia.org/wiki/Template:Biography). Just by writing:

{% raw %}
```{{subst:Biography}}```
{% endraw %}

a set of default headings get automatically created: just type it, then click 'save', and come back to to the page- they should all be there, with information about Socrates in there as a sample! Going through this page and deleting the irrelevant sections was a lot easier for me than creating new ones from scratch. 

I also discovered afterwards that a [biography template specifically for artists](https://en.wikipedia.org/wiki/Wikipedia:Artist_biography_article_template) is currently being made - this will be really useful for next year's event, I imagine!

### Page under construction 

While I was making the new page, it was in varying stages of readability - so, just in case anybody had come across it and thought it was in terrible quality, I put a notice at the top of the page, using the ["template: under construction"](https://en.wikipedia.org/wiki/Template:Under_construction)

By writing:

{% raw %}
 ```{{under construction}}```
{% endraw %}

this comes up at the top of the page:

<img src="{{ site.url }}/assets/blog/2015/under-construction.png" alt="under construction warning">

...which I think is brilliant; it lets visitors know that the page is still undergoing work, and it puts less pressure on the editor to get it done quickly. There's a few different variations of that template too, depending on what you want to indicate - ['new page'](https://en.wikipedia.org/wiki/Template:New_page) (which I probably should have used), for example.

### Creating references the easy way

I had quite a lot of experience using a MediaWiki platform back in 2011 and 2012, and one of the things that took the longest time was manually creating references. Today, I was super happy to discover the 'cite' option in the editor, which makes it a lot more simple to reference sources. In the editing window, just click 'Cite', then go to the 'Template' drop down menu, and select what kind of source you're citing, to get this pop up box that you need to fill in:

<img src="{{ site.url }}/assets/blog/2015/cite-popup.png" alt="citation pop up box">

Even easier than that though, is the new [Visual Editor](https://en.wikipedia.org/wiki/Wikipedia:VisualEditor), which is currently in beta mode. If you click on Preferences at the top of the screen, there is an option for 'Beta Features' which includes the Visual Editor. If you check the Visual Editor box, then a new tab should come up at the top of each new page - Edit (beta), and when you click on this, the page should appear just like it does when you normally view it, but now you can click and add things to it! 

As I'm not so accustomed to the regular wikitext editor, I'm not at all opposed to this change: it makes it a lot easier to see where things need to be changed, and I imagine for totally new Wikipedia editors, it lowers the barrier to entry quite significantly. I'll be using the Visual Editor for the foreseeable future, at least! 

### Openly licensed photos are SO IMPORTANT

For both of the women whose pages I worked on today, I have been unable to find an explicitly openly licensed photo of them, and of their work. It's so frustrating: they both have photos online, and there are lots and lots of photos of their work - but, because none of them have a Creative Commons license on them, I can't put them in their Wikipedia pages.

I can't really see any benefits to this for anyone- for viewers of the page, people who want to appreciate their art, or them personally. I can see a photo of them if I search for it separately, and I can see their art if I search for it separately, but I just can't see information about them **and** these photos at the same time. Not being able to put any photos in the pages makes them a lot less interesting than they could be - having descriptions of an exhibition next to a picture from the exhibition would, for example, make a lot more sense. 

I never really realised how much of a problem this would be, but I've learned my lesson: I am going to make a concerted effort in the future to put (with permission) any photos of notable people that I might take, online, and CC-licensed so that they can be used. Please do the same! 

## Conclusion

Having the visual editor and more of a grasp of where to find useful templates will, I hope, encourage me to edit Wikipedia more often. Given the incredibly important role that Wikipedia plays in giving people information, it's so vital that [women are represented fairly](http://observer.com/2015/02/moma-to-host-wikipedia-edit-a-thon-to-repair-art-world-gender-imbalance/).

If you've never edited Wikipedia before but you think this sounds kind of fun (it is!) - check out the [Meetups](https://en.wikipedia.org/wiki/Wikipedia:Meetup) page to see if there are any upcoming events in your area. I would really recommend popping along! 


