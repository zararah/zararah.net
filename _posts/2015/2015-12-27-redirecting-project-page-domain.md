---
layout: post
title: "Redirecting Github project pages to a custom domain"
date: '2015-12-27'
category:
- coding
---

Recently, Julia set up [this site](https://github.com/juliakloiber/superrr), and I purchased the domain [superrr.ninja](https://superrr.ninja) for it to live at. Finding how to redirect it - as it was a [project page](https://help.github.com/articles/user-organization-and-project-pages/) rather than a [user page](https://help.github.com/articles/user-organization-and-project-pages/) - was a little counter-intuitive at times, so in case anyone else wonders in the future, here's what I did: 

<!--more-->

(Before following these instructions, you'll probably have followed [these instructions](https://pages.github.com/) to set up a project page)

1. As [this Github documentation says](https://help.github.com/articles/adding-a-cname-file-to-your-repository/), set up a CNAME file to the project repository with just the domain name that you want to use - in our case, it looks like this:

{% highlight ruby %}
superrr.ninja
{% endhighlight %}

2. I found [these instructions from Github](https://help.github.com/articles/tips-for-configuring-a-cname-record-with-your-dns-provider/) on how to configure the DNS settings with your provider, but I wasn't so sure what to actually do after reading them- [the answers from Stack Overflow](https://stackoverflow.com/questions/9082499/custom-domain-for-github-project-pages) also helped. In short, though: on whatever service you used to buy your domain, you need to add two A Records in 'Settings', with the following details. In my case using Namecheap, I found this option in 'Advanced DNS settings', and added two 'A Records' which point to

{% highlight ruby %}
192.30.252.154
192.30.252.153
{% endhighlight %}

so it looks like this: (this is a screenshot from Namecheap)

<img src="{{ site.url }}/assets/blog/2015/namecheap-screenshot.png" alt="namecheap-screenshot">

and, in the same settings, modify the CNAME record so it reads as

{% highlight ruby %}
username.github.io.
{% endhighlight %}

...where 'username' is your username. Note the "." at the end, too.

*This is the part I found counterintuitive - at no point in the DNS records do you write what the project name is, just having the CNAME in the project repository is apparently enough.*

After a few minutes, your custom domain should work!



