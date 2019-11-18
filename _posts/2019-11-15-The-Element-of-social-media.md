---
layout: post
title: The Element of Social Media
date: 2019-11-15 11:43:27 -0600
categories: 1dv022
comments: true
---

![Thought bubbles]({{ site.url }}/assets/bubbles.png)

### Adding the ability to comment on posts

As you might have noticed there is a small logo saying "Disqus" at the bottom right of the area for commenting on my blog posts. Thats because I am using a tool to make it possible for you to comment, respond and see realtime comments from other users. Disqus is logging over 50 million comments from users worldwide _every_ month! Thats crazy! It also makes it possible for you to get tracking data of user interaction and statistics for how well your blog posts are doing. In this day and age that is digital gold!

Using this tool is super easy. I just had to make a free user, go through the guided steps in their webpage to create a new connection to my site and thats pretty mush it on that end. This gave me something they call a short-name that I needed to include in my \_config.yml file. Something that wasn't very clear was that I needed to enter the url to my published site to make it work. Then I also had to configure the frontmatter with "comments: true". After setting up the user on Disqus, providing the short-name and url in the \_config.yml file and configuring the individual posts I was good to go!

### The Power of Open Graph

Open Graph is something the Facebook developed around 2010. They created Open Graph because they wanted an easier integration with the webb on their social media platform. If you copy an address to a page and paste it in a timeline-post or a private message you automatically get a small preview with a picture and/or some short information about the page. If you think about how Facebook gets that information it should be quite apparent that it would be hard for Facebook to get the right image and information for every possible link. Thats why they created this standard to make it possible for web developers to decide what information should be used if someone tries to share a link to their web page.

The way I use Open Graph is by entering meta tags in the <head> section of my page. The information I provide is title, url, type and image. Here below you can see how this all is used in practice.

```
<head>
<meta content="_SITE_NAME_GOES_HERE_" property="og:site_name" />
<meta content="_URL_/assets/IMAGE.png" property="og:image" />
<meta content="article" property="og:type" />
</head>
```
