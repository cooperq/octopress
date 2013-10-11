---
layout: post
title: "Drupal: Never Again, or, How I stopped worrying and learned to love markdown"
date: 2013-10-10 16:55
comments: true
categories: programming, security, web development
---
I have been a web developer for over 6 years now, I have hacked in Drupal,
Wordpress, Ruby on Rails and Django and more. Lately my favorite framework has 
been good ol' fashioned static HTML and Javascript. 

I switched my blog recently from a custom written Ruby on Rails CMS to this 
[Octopress](http://octopress.org) generated website and I couldn't be happier. In
fact, lately, I have been tempted to create every new site using a static generator.

Now obviously using a static site generator like Octopress or [Jekyll](http://jekyllrb.com/)
is not for everyone. You have to be reasonably comfortable with Ruby and with Markdown
to use Octopress; so I will probably not be rolling it out as a CMS for any of my clients 
any time soon. However, for the sites that I directly maintain it has been a fantastic tool.

*But Why?*

## Security
Using a static blog generator offers a level of security that can't be matched by Drupal, Wordpress
or RoR. Any framework is going to have the possibility of security problems: session hijacking, cross site
scripting, mysql injections and zero days.  A static site generator has none of these problems, this 
significantly decreases the attack surface for any website.

## Scalability
Static text scales better than anything else. With Drupal or RoR you need to cache the hell out of a site to get
it to scale to any reasonable site. With a static site you don't have any caching to worry about at all,
and if your site does somehow grow beyond the capabilities of your server it is easy to use varnish to increase 
your throughput, because it is static it can all be cached, and there is no database to be a pain in your side!

## Better Workflows
Now that I am using Octopress I don't have to worry about updates, caching, plugins, publishing or wysiwygs.
I just fire up vim and start writing my post in markdown. Then when I am done, I can publish and deploy with
one simple command: `# rake gen_deploy`. This is a workflow that is so easy for me it makes writing a joy.

Using octopress for blogging has so many benefits over other content management systems it makes me wonder how
I ever used them. I will certainly be using Octopress for every site I can from now on.

