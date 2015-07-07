---
sha: null
title: 'Making my new website'
date: '2015-07-06'
info: 
comment: 'Why I chose github pages for my new website'
tags:
  - Jekyll
  - ' blogs'
  - ' github pages'
  - ' webdesign'
categories:
  - Jekyll
  - ' web design'
  - ' github'
published: true
slug: 

---
###A new website for a new era :metal:

I abandoned my website after only a brief time online. This was primarily due to the fact that my hosting provider was doubling the annual price of my VPS, and that the site itself didn't really suit my needs. 

I built it initially so out of the box anyone could jump in and use it (plain ol' css, html, and some jquery) , but this came with some serious downsides. The build was plain css, html and some jquery. No blog, just a static one page theme. I do mostly theming for my job - so all the pieces were made interchangeably. Switch out the logo, images, and some copy and you're good to go.  This made the site itself too generic and failed to reflect my personality.

So for my new website I had a fairly certain checklist in mind: 
- Cost efficient.
- Have a blog.
- Be representative of my current work flow
- Have complementary and colorful branding

I was looking at a few other platforms before quickly deciding on using my user github page. If you're not familiar you should [read up](https://pages.github.com/), it's an awesome free service that github provides to all it's users. You can use custom URLs, use jekyll to blog, and you can update it simply by pushing commits to github! 

Jekyll is a ruby static site generator that runs on github's servers (or your own if you'd prefer) to create content. It takes care of partials and will produce your blog using markdown files. It also will compile sass and coffeescript files as well. Super handy. If you don't know what markdown is, you've probably used it and not realized it. It's an html preprocessor that formats text so the output is clean, legible, SEO friendly markup. It's in a lot of places these days from social media site Ello, the help forum Stack Overflow, browser editor codepen, and project management software like Trello. The Blogging/social platform Tumblr, has it as an optional feature. It's the :honeybee: 's knees. CMS's like wordpress and blogger will interpret your whitespace in unpredictably, sometimes horrifying ways. Take a peak sometime, it's usually full of excess spans, inline styles, and word breaks. *Ohhh the word breaks...* :scream:

The concept of writing a post in markdown, pushing it through git, and having it published on my site is quite the draw for someone who uses those tools daily. Plus *free*. OMG AWESOME. 

Although github will help you generate a site automatically from inside your repo, why not take a little time and make it your own? 
To save you a little time, I recommend building it out locally first and then pushing the repo out after you get it *somewhat functional* . Using Jekyll does involve some basic command line usage. This freaks some people out, I don't know why. 

[Jekyll's website](http://jekyllrb.com/) has a really greate guide to get you going. Just know that if you're using windows [you'll want to download and install the ruby devkit](http://jekyll-windows.juthilo.com/1-ruby-and-devkit/) for the version and architecture you're using. 

TLTR? Here's the play by play: 

- Download the ruby version listed [here](https://pages.github.com/versions/). I installed a version newer, it was fine.
- Open the terminal and install bundler: `gem install bundler`. 
 - If you're on Mac/Linux, note that you'll probably need to preface it with `sudo` so you don't get permission errors
- install github- pages: `gem install github-pages` This should take care of all the dependencies you'll need, **and save you a lot of time**
- Open the terminal wherever you keep your code and type `jekyll new 'newProjectTitle'`. This will scaffold out the default build. **If you're wanting to use a user github page, title it (your username).github.io**
- `cd 'newProjectTitle' ` aka go into the directory. 
-  `touch Gemfile`. If you're on windows, I don't know the command for this. You can however install git and use git bash to utilize most unix type commands. You should have already done this. It's amazing. Otherwise open your favorite text editor (notepad even. No judgies) and create the *Gemfile*. **It has no extension, so make sure you DON'T save it out as a .txt or .rtf file.**
- inside the Gemfile type: `source 'https://rubygems.org'` on the first line and `gem 'github-pages'` on the second.
- inside the terminal type `bundler exec jekyll serve`. This uses your ruby dependencies to build out jekyll and start it's server. This will get you as close as possible to the github pages enviroment if that's what you're shooting for. 
- Unless you get some nasty errors (which you shouldn't, it's all vanilla right now), jekyll should serve up the files at `http://0.0.0.0:4000`. You can't just type that into the browser though, so type `localhost:4000` in your browser address bar. 

 WELCOME TO JEKYLL. 
While everything is working, I'd create the repo in github and push a commit. Go to (your username).github.io and check it out. 
