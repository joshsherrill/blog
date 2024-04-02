---
layout: post
title: "Using Jekyll & GitHub Pages to Host a Blog"
categories: dev
author: "Josh Sherrill"
meta: "Jekyll, GitHub Pages, Bunny.net"
---

I have had the itch to start a blog recently but knowing myself and how often I start a habit only to abandon it not far after, I decided it needed to be something not only easy to set up but cheap. A quick Google search showed me that going with a hosted option would cost anywhere between $7-12 per month, which is a bit much for something I will post to so seldomly. My next thought was that perhaps I could pay for a VPS and install one of the many self hosted option like Ghost or Wordpress. Using something like DigitalOcean, this would still cost me $4 per month for their smallest droplet. I knew I could do better and that this was something that was already likely a solved problem. After a bit more searching, I found Jekyll.

## Using Jekyll as a Blog

Jekyll is an open source project that turns static files into a website or blog. All of the layout files are done with simple css and html template files. The blog posts and pages are as easy as creating a markdown document with a bit of metadata at the top and specific file naming scheme then placing them into the _posts folder. 

Here is an example of a post:

```
---
layout: post
title: "This post demonstrates post content styles"
categories: junk
author: "Bart Simpson"
meta: "Springfield"
---

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Fusce bibendum neque eget nunc mattis eu sollicitudin enim tincidunt. Vestibulum lacus tortor, ultricies id dignissim ac, bibendum in velit.
```

Since Jekyll uses markdown, it makes it easy to just write the posts directly in VSCode. All of the files are stored locally on my machine where you can back them up in something like iCloud or push them to a GitHub repository. The latter being an important step in making my blog visible to the general public. 

## Hosting on GitHub Pages

GitHub allows you to enable something called GitHub Pages on a repository that allows you to serve up static files like HTML and CSS. GitHub Pages gives you 100GB of bandwidth per month, 1GB of storage and the ability to add a custom domain name. This is all free as long as you are using a public repository. Since this is going to be a public blog there was really no need to go with a private repository anyways. There are many other free options available for hosting a blog but most of them are full of ads and don't offer as much control over your data. I believe Netlify is an alternative to GitHub Pages and has a free tier but after seeing a few horror stories of huge bills from DDOS attacks eating up large amounts of bandwidth, I figured I would steer clear of that option for now. 

The storage is the one place where I ran into a bit of a problem. I was hoping to use this blog as place to display some of the photos I take but the 1GB storage limit means I would run out of space quickly. I needed an external place to host my files.

## Bunny.net Storage

This is where Bunny.net comes in with their file storage plan. For only $1 per month, I can store 100GB of photos which I can then serve up on my blog. Each additional GB is only $0.01 per month. This ensures I am keeping the GitHub repository lean while also having the nice benefit of being able to enable a CDN easily if I wanted to feel fancy. There are many free options out there for image hosting but I wanted something that was ad free, scalable and designed to be reliable. If you are willing to compromise, you could easily use something like imgur or one of the many other image hosting apps to serve up your photos. 

## Final Cost

So all in, I pay $1 per month for Bunny storage and another $1 per month for a custom domain, neither of which are necessary for this to work but offer some quality of life improvements. Not bad for a solution that gives me some control of my data, offers a ton of flexibility and is completely ad free. 