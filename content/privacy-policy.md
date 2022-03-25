---
title: "Privacy Policy"
type: "page"
draft: false
---


#  Statement
The `stefanos.io` website is not logging any data,
is not using any scripts/applications for tracking its visitors
and does not place any cookies on your computer.

##  Logging 
The access and error logs are disabled in nginx, but I use cloudflare as a frontend. I don't have any metrics enabled, so to my knowledge there is no tracking. 
I suggest you do the same thing if you can.
The side effect is that I have no idea how many visitors the website gets but let’s say I’m rounding the number down to one million daily visitors.

```nginx
access_log off;
error_log /dev/null;
```
### Data Transfer 
All data is served over the HTTPS protocol , encrypting all data between the browser and the server. 
Your network provider will still be able to see that you are downloading data from stefanos.io, but they will not be able to see the content.

#### HTTP referer
This website is using meta tags to strip referer information (yes, that’s how the HTTP header IS spelled) from all outgoing links as well as placing rel="noreferrer" on the same anchor links, therefore not passing any referral data from this site to any external websites.

```html
<meta name="referrer" content="never" />
<meta name="referrer" content="no-referrer" />
```

All of this is information made public by you, and no information other than information you have made public can be captured by this process.




