---
layout:       post
title:        "Customizing your Heroku domain using Godaddy"
subtitle:     "Pointing any domain you purchase to your Heroku app"
date:         2018-07-17 20:16:00
author:       "ZhouSir"
header-img:   "img/in-post/post-domain-godaddy/share-godaddy-domains.jpg"
header-mask:  0.3
catalog:      true
multilingual: false
tags:
    - Domains
    - Heroku
    - 学习笔记
---

## Before we get started
> What you need to prepare

* A web app deloyed on Heroku
* A domain purchased on [Godaddy](www.godaddy.com). By the way, domain names end with `.me` is really affordable for students. Take my domain as an example: zhousir.me. It only costs 3.8 dollars for the first year and 19 dollars for following years.  

## Go to terminal (or Heroku website)
> Next step

Type: `heroku domains:add www.your-domain`
![](/img/in-post/post-domain-godaddy/terminal.jpg)
You can also complete this process by going to settings of your application on [Heroku](https://dashboard.heroku.com/apps) website. Then go down the page and find **Domains and certificates** section.
![](/img/in-post/post-domain-godaddy/heroku.jpg)

## Go to Godaddy
> Last step

* Go to manage domains, select manage DNS. PS: This website definitely has some bugs in its frontend...
![](/img/in-post/post-domain-godaddy/godaddy.jpg)
* Find the record with Type CNAME, Name WWW, Value @ and then change the Value to your Heroku domain for your app, e.g. your-app.herokuapp.com. Below is a record after this process.
![](/img/in-post/post-domain-godaddy/godaddy1.jpg)

## Your new domain is ready to go!
> What's more you can do?

* There is a little setting you can do to forward the naked domain (without 'www') to your 'www' domain.
* Find the forwarding section on the same page with last step then set 'forward to' to your 'www' domain. Save.
![](/img/in-post/post-domain-godaddy/forwarding.jpg)
* Done!