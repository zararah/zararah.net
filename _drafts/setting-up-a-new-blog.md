---
layout: post
title: 'Setting up a new blog: part 1'
date: '2014-10-26T'
category:
- coding
tags:
- jekyll
- github
---

I’ve been meaning to migrate my blog off Tumblr for a while now, and on to Github pages. Why? I don’t like the writing/editing interface for text in Tumblr (the window is too small to be able to see much text) - certain bits of html disappear between the visual editor and the html editor - it’s difficult to use images or put code snippets in, and I want to be able to write in Markdown, to name just a few reasons. I also like the idea of creating lists or resources that other people can contribute to - ie. via Github - that can live on my site, and I want to be able to customise it a little more easily than Tumblr offers.

So, here goes. 

First, I set up a new repository on Github: I followed [these instructions](http://learn.andrewmunsell.com/learn/jekyll-by-example/tutorial) up until Step 3. 

Then, on my machine I created a folder where I want the blog to live - imaginatively, called ‘blog’. 

In the terminal, I [changed directory](https://github.com/0nn0/terminal-mac-cheatsheet/wiki/Terminal-Cheatsheet-for-Mac-(-basics-)) to be in /blog - so that everything I then do happens in the right place. 

then ran 

{% highlight ruby %}
git clone https://github.com/zararah/zararah.github.io
{% endhighlight %}

Next, as I knew that I wanted my new page to run on Jekyll, I checked out the documentation [from here.](http://jekyllrb.com/docs/installation/)

This told me to run: 

{% highlight ruby %}
gem install jekyll
{% endhighlight %}

(bearing in mind I’ve already worked with ruby and Jekyll before, so I had all the [requirements already](http://jekyllrb.com/docs/installation/#requirements)

But, for some reason, I got the following error: 

{% highlight ruby %}
ERROR:  While executing gem ... (Gem::FilePermissionError)
    You don't have write permissions for the /Library/Ruby/Gems/2.0.0 directory.
{% endhighlight %}

I have no idea why I didn’t have the write permissions, so I used [sudo](https://www.xkcd.com/149/) instead, and ran:

{% highlight ruby %}
sudo gem install jekyll
{% endhighlight %}

and then 

{% highlight ruby %}
sudo gem install github-pages
{% endhighlight %}

 to make sure [everything else was up to date.](https://github.com/github/pages-gem)  - 

Both seemed to do make something happen in the Terminal - a good sign, I think! 

Next, I thought it might be time to think about what kind of theme I wanted to use. I found [this page](http://jekyllthemes.org/) with a variety of Jekyll themes that I could fork. I liked [this one](http://mademistakes.com/) - but it’s more focused on pictures, rather than writing. Or [this one](http://jekyll.gtat.me/), but it looks a lot like [Medium.](https://medium.com/) I thought [this one was nice, too](http://jekyllthemes.org/themes/exemplar/) - but at the risk of sounding like Goldilocks, nothing was quite right. 

So, as [Friedrich](http://pudo.org/) pointed out, why not take this opportunity to make my own? A challenge, but a good learning opportunity, too. 

Perhaps a decision I’ll regret, but here goes: 

I was very happy to find this [excellent tutorial on building a Jekyll blog from scratch](http://learn.andrewmunsell.com/learn/jekyll-by-example/tutorial), which I pretty much followed word for word. There were a few things that are now out of date though, which I’ve noted down here in case others have the same problem.

If you open the link above to the tutorial - everything seems to work until I tried running

{% highlight ruby %}
jekyll --auto --server
{% endhighlight %}

It turns out that there’s been a deprecation of this command: I got

{% highlight ruby %}
zaras-air:zararah.github.io zararahman$ jekyll --auto --server
       Deprecation: Jekyll now uses subcommands instead of just switches. Run `jekyll --help' to find out more.
       Deprecation: The --server command has been replaced by the 'serve' subcommand.
       Deprecation: The switch '--auto' has been replaced with '--watch'.
{% endhighlight %}

so, instead I ran:

{% highlight ruby %}
jekyll serve -w
{% endhighlight %}

to get the local server running, instead - the -w means that it updates automatically, without needing to update changes. 

And it worked! I can see…

{{ site.url }}/assets/site1.png

So on to the next step of building the theme, and installing Twitter Bootstrap - (see section Building the Theme in Andrew’s tutorial) 

Now I can see: 

{{ site.url }}/assets/site2.png

To set up a sidebar though, I ran into a couple of issues as I’m using bootstrap v. 3.2.0 - which is newer than the tutorial.

So instead of the recommended sidebar.html, I put 

{% highlight ruby %}

{% include header.html %}
  <div class="row">
  	 <div class="col-md-8">
    {{ content }}
  </div>
  <div class="col-md-4">
    {% include sidebar.html %}
  </div>
</div>
{% include footer.html %}

{% endhighlight %}

after referring to the [new bootstrap documentation.](http://bootstrapdocs.com/v3.2.0/docs/css/)

(Incidentally, correcting:

{% highlight ruby %}
<div class="row-fluid">
  <div class="span12">
{% endhighlight %}

to 

{% highlight ruby %}
<div class=”row”>
  <div class=”col-md-12”>
    {% endhighlight %}

(or whatever number you want) is something that you’ll have to do throughout the tutorial, if you’re using the newer version of Bootstrap. 

Also, within the code there for post.html I found something that didn’t seem to work - the date_to_long_string here: 
{% highlight ruby %}
  {% include header.html %}

<div class="row-fluid">
  <div class="span8">
    <h1>{{ page.title }}</h1>
    <p class="muted">{{ page.date | date_to_long_string }}</p>

    {{ content }}
  </div>
  <div class="span4">
    {% include sidebar.html %}
  </div>
</div>

{% include footer.html %}

{% endhighlight %}

...so I deleted the date_to_long_string 

and I changed it to 

{% highlight ruby %}
  	<p class="muted">{{ page.date | date: "%-d %B %Y" }}</p>
{% endhighlight %}

following advice [from here.](http://alanwsmith.com/jekyll-liquid-date-formatting-examples)

And, everything else in the tutorial worked splendidly - so I now have a super basic skeleton of a blog set up! 

It looks like this:

{{ site.url }}/assets/site2.png
