+++
author = "aadi."
title = "getting https:// for free."
date = 2023-04-09 
description = "cloudflare."
+++
how to set up cloudflare for that shiny lockpad and https:// :) (for free.)
<!-- more -->
`(do note that this process is for a github-pages hosted site. you might need to configure sum else in other cases)`

prerequisites: 
- a [cloudflare](https://dash.cloudflare.com/) account (its free).
- a custom domain name. (you do have to pay for it unless you use something like .tk)

### setting up cloudflare nameservers.
> "cloudflare is a company that provides a suite of services designed to improve the security, performance, and reliability of websites and internet applications."

anyways so yeah i used cloudflare's free plan to enable https:// on this website.

once you make a cloudflare account, you need to add your site to it.

to do so, add your site by clicking on the button `add a site`.
![add a site](https://user-images.githubusercontent.com/76528474/235352871-16b854b4-28df-4e7e-acb3-f3d132cb1ddf.png)

after that, put in your site's url, and click on `add site`.
![input ur url](https://user-images.githubusercontent.com/76528474/235352938-579f1450-55a7-4c16-8169-15186a5cc78a.png)

scroll down till you get the free plan, select it and then click on `continue`.
![free plan yay](https://user-images.githubusercontent.com/76528474/235352951-611fa3be-866a-4bf5-aeb7-38e323631f7b.png)

confirm that the dns records are matching by heading over to your domain's registrar's dns records.
![dns records](https://user-images.githubusercontent.com/76528474/235352915-44ff62f2-80f9-4f08-ad0e-87a5cc6cae63.png)

after that click on continue and then complete the nameserver set up by following the steps given.

you will have to change the nameservers provided by your domain registrar and replace them with the nameservers assigned by cloudflare.
![nameservers](https://user-images.githubusercontent.com/76528474/235352962-2197a954-1443-4dbf-8d3e-0305b7d613e3.png)

once that is done, click on `check nameservers`.
![check nameservers](https://user-images.githubusercontent.com/76528474/235352972-837b7ba6-9892-417f-840b-7682d04a87c5.png)

it might take a while (around an hour) but you will recieve an email once the process is done. 

### ssl.
okay so you will have to select ssl/tls from the sidebar on the left.
![sidebar](https://user-images.githubusercontent.com/76528474/235352891-ce76c63e-267a-4302-835f-dd3f261260f5.png)

and then in the overview, you'll have to make sure that the encryption mode is full.
![encryption](https://user-images.githubusercontent.com/76528474/235352903-4627b120-23a0-4400-84d1-2170cf6b9546.png)


### woo shiny lockpad!1!
ayyy we now have this shiny little lockpad :)
![lockpad](https://user-images.githubusercontent.com/76528474/235352983-68e9991d-ceb6-43fe-b4d6-ac165bc95bda.png)