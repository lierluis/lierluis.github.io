---
layout: post
title:  "Hello world!"
categories: blog
---

Welcome to my website!

I plan to use it as a blog/portfolio. This will be an ongoing project of mine.

I decided to use Jekyll to generate my website due to the site's static nature,
and of course for Jekyll's smooth integration with Github Pages to deploy the
site.

With Jekyll there's no need for databases, and therefore no complexity. I just
create pages in Markdown, push them to Github, and they're live!

Right now I'm just learning more of Jekyll's structure, which involves a bit of
Ruby, Sass, and Liquid.

If you'd like to learn more about me, visit my [About] page.
You can also check out my [Projects].

Thanks for stopping by!

[About]: {{ site.url }}{% link about.md %}
[Projects]: {{ site.url }}{% link projects/projects.md %}
