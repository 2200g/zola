+++
author = "aadi."
title = "getting https:// for free."
date = 2023-04-09 
description = "cloudflare."
+++
how to set up cloudflare for that shiny lockpad and https:// :) (for free.)
<!--more-->
`(do note that this process is for a github-pages hosted site. you might need to configure sum else in other cases)`

prerequisites: 
- a [cloudflare](https://dash.cloudflare.com/) account (its free).
- a custom domain name. (you do have to pay for it unless you use something like .tk)

### setting up cloudflare nameservers.
> "cloudflare is a company that provides a suite of services designed to improve the security, performance, and reliability of websites and internet applications."

anyways so yeah i used cloudflare's free plan to enable https:// on this website.

once you make a cloudflare account, you need to add your site to it.

to do so, add your site by clicking on the button `add a site`.
![add a site](https://raw.githubusercontent.com/2200g/img-repo/main/cloudflare/addasite.png)

after that, put in your site's url, and click on `add site`.
![input ur url](https://raw.githubusercontent.com/2200g/img-repo/main/cloudflare/inputurl.png)

scroll down till you get the free plan, select it and then click on `continue`.
![free plan yay](https://raw.githubusercontent.com/2200g/img-repo/main/cloudflare/freeplanyay.png)

confirm that the dns records are matching by heading over to your domain's registrar's dns records.
![dns records](https://raw.githubusercontent.com/2200g/img-repo/main/cloudflare/dnsrecords.png)

after that click on continue and then complete the nameserver set up by following the steps given.

you will have to change the nameservers provided by your domain registrar and replace them with the nameservers assigned by cloudflare.
![nameservers](https://raw.githubusercontent.com/2200g/img-repo/main/cloudflare/nameservers.png)

once that is done, click on `check nameservers`.
![check nameservers](https://raw.githubusercontent.com/2200g/img-repo/main/cloudflare/check.png)

it might take a while (around an hour) but you will recieve an email once the process is done. 

### ssl.
okay so you will have to select ssl/tls from the sidebar on the left.
![sidebar](https://raw.githubusercontent.com/2200g/img-repo/main/cloudflare/sidebar.png)

and then in the overview, you'll have to make sure that the encryption mode is full.
![encryption](https://raw.githubusercontent.com/2200g/img-repo/main/cloudflare/encrypt.png)


### woo shiny lockpad!1!
ayyy we now have this shiny little lockpad :)
![lockpad](https://raw.githubusercontent.com/2200g/img-repo/main/cloudflare/lockpad.png)