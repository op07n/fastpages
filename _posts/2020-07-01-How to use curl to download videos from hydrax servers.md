---
toc: true
layout: post
description: How to use curl to download videos from hydrax servers.
categories: [markdown]
title: How to use curl to download videos from hydrax servers.
---
# How to use curl to download videos from hydrax servers.



I've seen this kind of videos in sites like https://kissanime.ru/ o https://ww2.0123movie.net/ . Probably there are a lot more.

My chrome extension to do this, "Video Download Helper", is not working in these cases.
When I used it, give me the url that is not allowed for uploading the video. 
So, one way to do this is to use the Chrome browser developer tools. While the movie is being played in the developer tools, the url from the stream seems to grow more than the others. Therefore, when we request more information about this link, we get the url of the host and referer. This is all we need to use curl.

For example, if the url host is https://hbxc9pbqqw.xyz/ and the referer is https://playhydrax.com/?v=vD2ss7KTB
then one of the ways to use curl can be as follows:

> curl -o filenametosave -k "https://5wvyakb9zr.buzz/" -H "Referer: https://playhydrax.com/?v=qzH5GkNNx6" --compressed

Bonus:

Also is posible to use powershell:

> Invoke-WebRequest -Uri "https://eno13lwuxv.xyz/" -Headers @{"Referer"="https://playhydrax.com/?v=j4ivrSmiCR"} -OutFile filenametosave

Tip to avoid stop by developer debugger:

Wait to init the movie and pause the player. Go to Application ( in developer tools ) and "clear site data". Next play to continue viewing the movie.
In Network is easy to recognize for the waterfall growing. Mouse right click menu allow to get the Copy as cURL or Copy all as Powershell.

<script src="https://utteranc.es/client.js"
        repo="op07n/fastpages"
        issue-term="pathname"
        theme="github-light"
        crossorigin="anonymous"
        async>
</script>
