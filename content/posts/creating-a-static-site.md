---
title: How to build your own static site
draft: true
showtoc : true
showreadingtime : true
date : 2024-12-30
cover:
    image: '/img/brot-dev/cover.jpg'
author: Alex Kellermann
summary: How to build your static site on either GitHub Pages or Cloudflare Pages. By going with these platforms you can host your website entirely for free, even on a custom domain if you have your own! Build your own personal brand or just host a website for a project you're working on.
tags: [GitHub Pages, Cloudflare Pages, AWS S3, Hugo]
---

Building a static site is an easy way to take control of your content and find your own corner of the internet. The recent TikTok ban and subsequent overturn was a good reminder that on those platforms you're at the mercy of the platform provider!

# 

# Using GitHub Pages
[GitHub Pages](https://pages.github.com) is the standard for deploying static pages for free.

# Using Cloudflare Pages
[Cloudflare Pages]() and the [docs](https://developers.cloudflare.com/pages/)

# Using Hugo

## Some things to remember

- [Remember to generate a robot.txt file for your site](https://gohugo.io/templates/robots/). Bing and duckduckgo will still go ahead and crawl your website without one, but Google won't. I accidentally didn't do this for the first year my site was active and wasn't crawled unless I manually submitted a new sitemap.
- You can just add the `enableRobotsTXT = true` to your hugo.toml and Hugo will auto generate one for you. You can also write your own `robots.txt` and place it in your `static` directory and it'll be copied over when your site is built.
