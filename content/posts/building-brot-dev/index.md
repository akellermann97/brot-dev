---
title: Building brot.dev
draft: false
showtoc : true
ShowReadingTime : true
date : 2024-04-23
env: production
summary: What decisions go into building brot.dev 0.1.0, how it's setup, and the deployment pipeline.
cover:
    image: '/img/brot-dev/cover.jpg'
tags: [Blog, Tech, GitHub, How-To]
---
[^1]

# Building brot.dev
*Editors Note:* This is an accurate reflection of the website as of April 24th, 2024. If you're reading this in the future, things may have changed!


There's a lot that goes into building a website, even a simple one! When deciding to build a personal site, there were a couple things I was looking to have.

- Easy to Build
- Easy to Maintain
- Low or Zero Cost

So when looking around, there are lots of options to choose from, ranging from something as simple as setting up a Wix site, where they give you a free domain to use, and you can use their templating engine, or going for something more complex, like self-hosting an EC2 instance running ngnix and handwriting html, jss, and js.

Running through some sensible choices left me with some options:
- Use some basic HTML templates from online with FOSS licenses
- Start from scratch and build a site using flexbox and something like [orbitcss.com](https://orbitcss.com)
- Use Wix or Squarespace and use a UI to build my site
- Use a static website creator like Hugo or Jekyll

HTML templates are fun, but they're not easy to use, a pain to update when technology changes and you need to go through and update things like mediaqueries and worry about responsiveness and all the things web designers get paid good money to update. I don't want this site to be a major time investment, and I'm not a designer or webdev, so making something that is responsive, looks good, and only needs minimal maintainance on my part meant I wasn't going to do something from scratch. 

Wix and Squarespace are great tools, and those companies have made major strides in the past decade to where I would feel happy to use them to build a site, but ultimately didn't want to spend any money on the site when this is really going to be a hobby and I won't be generating any money or running any ads on it.

So I decided using a static site generator would be my best bet. As for why I chose Hugo over Jekyll comes down to Hugo's choice to use golang. I don't know any Ruby, so if I need to make some crazy changes or quickly need to debug how Hugo works it'll be easier if it's in a language I already understand well. Otherwise Jekyll looks like it would've been equally as good. Both services function similarly, where you choose a template, or make your own, and write content in the form of Markdown. You can kick it up a notch and do more advance things, and write lots of HTML directly with Hugo as well, but I'm sticking with the simplest option. 

## Building a static site
So, now you know you want to build a static site, and you're going to use Hugo. The question now is how are you going to get those beautiful pages that Hugo generates online?

- Run `nginx`/`apache`/`lighttpd`
- Dump it into a S3 bucket or Google Storage and use their native solutions to host it right out of there
- [GitHub Pages](https://pages.github.com)

*If* I wanted to run my own nginx server, I would probably use [Hetzner](https://hetzner.com) to buy a VPS since you can get good compute capacity for ~30 bucks a month, assuming you get low traffic. Would then look to have Cloudflare serve as my CDN and WAF and rely on their free tier. All in all you could get this running for around 30 bucks a month if you just wanted to run a static site, and this gives you a lot of room to grow. If you want to host dynamic content this would be a really good option, and you could buy a better tier of VPS and run multiple things on it, use it as an Exit Node in a Tailnet, etc. This option has the most upfront investment, both timewise and money wise.

{{< figure src="/img/brot-dev/hetzner.png" caption="~5 Euros a Month for 20TB of traffic!" class="normal" >}}

Many big name companies actually host their own websites using s3 static sites! You get a good balance of security, ease of use, and flexibility with that. But bucket-based hosting does require a lot of setup. You'll need to make sure your bucket permissions are correct, give AWS/GCP/Azure a credit card, set up things like TLS certificates, get a CDN up and running so you get better performance and maybe save a bit of \$\$\$. This is a lot of upfront work, but once it's all setup it's fairly effortless to keep running. Cloud providers handle a lot of the headache for you in terms of rotating certs and running a CDN (at least with AWS) and a static website is fairly one-click. If I were a business I would go for this route unless I had the willingness to staff an inhouse team to manage nginx directly.

Lastly, we have GitHub pages. To me this was always going to be my first choice, because GitHub does so much to make this incredibly easy. You don't even need to have a registrar for this to work, GitHub will host it directly on their github.io subdomain if you need them to. You don't have to even think about how CDN operates on your content, worrying about DDOS protection, or even give them a credit card.

## GitHub Pages Setup
[GitHub Pages](https://pages.github.com) is a great service provided by GitHub themselves. Don't pay any mind to the fact that the landing page hasn't been updated since the iPhone 6 came out, all that matters is that it's still supported and FREE! Yes, it relies on the fact that your respository is public, but since you want your website to be on the internet anyway, doesn't seem like a big tradeoff. If you were really secretive about the stack you were using to build your website, you could have a private repo host the actual Bread and Butter and use GitHub actions to push the final published pages to the public repo.

{{< figure src="/img/brot-dev/pages.png" caption="This websites actual repo! For now..." class="normal" >}}

With GitHub pages you also get the ability to use GitHub actions, build from branches other than main/master, and you don't have to think about Bandwidth costs, CDN setup, or a CI/CD pipeline. If you're using a Hugo project like me, you can really just follow the Hugo Quickstart guide and put that in a Git Repo and push that and it'll be your new website. If you're using GitHub actions I would add `public` to your .gitignore since the vanilla GitHub action will build your website on deploy.

### Setting the domain
This is probably the trickiest part, since every registrar will have a slightly different UI, but basically you need to set the `A` and `AAAA` records of your site to the IPs owned by GitHub. You can find the instructions [here](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site#configuring-an-apex-domain). Depending on DNS propagation it might take a couple seconds to a couple hours for all DNS servers to pick up on the changes. While that's happening make sure that your domain name is also set in the `settings` page in your Repo under code/automation. Once DNS propagation is finished your site's set up! Just gotta worry about what you're going to put on there now.

## Hugo Setup
There's nothing too fancy about the Hugo setup. The website uses the theme [papermod](https://github.com/adityatelange/hugo-PaperMod), which is a great, FOSS theme. Once I have some time and more articles up, I'll likely revisit this decision to have some nicer formatting, especially regarding images. Other than that this is barebones Hugo with two custom shortcodes. Full toml for Hugo is available on GitHub (https://github.com/akellermann97/brot-dev/blob/main/hugo.toml)

### Shortcodes
This is the only custom piece in the site. I use two shortcodes to get some extra features in Hugo without having to resort to writing HTML pages directly

- rawhtml
- exif

[rawhtml](https://anaulin.org/blog/hugo-raw-html-shortcode/) is a simple shortcode you can include when you do want to include some HTML in a page without turning the whole page into an HTML document for Hugo to then template out. As stated in the blogpost "...sometimes, markdown is not enough"

**exif** is a mixture of shortcodes I've cobbled together. It basically is just the included `figure` shortcode, but it will automatically fetch the EXIF data in the picture and include them as a caption in the image.

### brot.dev's actual setup

- DNS:
    - CNAME Points to brot.dev
    - A/AAAA records on registrar point to GitHub Pages
- GitHub:
    - Repo located at [akellermann97/brot-dev](https://github.com/akellermann97/brot-dev)
    - PaperTheme is included as a git submodule
    - GitHub Actions builds html pages from hugo.toml from the `main` branch

{{< figure src="/img/brot-dev/actions.png" caption="Just 5 workflows runs so far" class="normal" >}}

That's it! 🎉🎂

## tl;dr - The Stack
- This is a statically compiled website, using Hugo to build a series of Markdown pages which contain the actual content as Markdown files
- Google Domains 🪦 is used as a registrar for *brot.dev* (soon to be Squarespace domains)
- GitHub Pages hosts the website, acts as a CDN and as DDOS protection (TY Microsoft 💕)
- GitHub Actions reads the Hugo toml and the markdown and compiles the pages itself (this is overkill, but free)

{{< figure src="/img/brot-dev/wip.png" caption="The glamorous static website lifestyle" class="normal" >}}

## Errors? Typos?
Open up a GitHub PR and hopefully I'll get around to reviewing it. Or email at alex (at) brot (dot) dev
[^1]: Image Taken from Library of Congress. Dr. Walter Kato, Brooklyn simulator lab https://www.loc.gov/resource/gtfy.02045/