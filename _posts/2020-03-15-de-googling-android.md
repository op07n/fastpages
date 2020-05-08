---
toc: false
layout: post
description: De-googling Android Phones.
categories: [markdown]
title: De-googling Android Phones.
---
# De-googling Android Phones.

Borrowed from:

[![Alt text](https://img.youtube.com/vi/UXLo15l2i4c/0.jpg)](https://www.youtube.com/watch?v=UXLo15l2i4c)


Can you **de-google** an Android phone?  yes, you can,  and I'll show you a completely **de-googled** newer phone and then examine the choices I made to ensure privacy. Privacy choices can be impacted by what
to choose to install on this phone. So this is not simple. Let's get started.

For this exercise I'm using a **Motorola** **Moto G7** play, which is a phone released in 2019. It's made by **Lenovo**. The reason I chose this phone is that it's fairly easy to get, it's inexpensive, but with a surprisingly good build quality and performance. And in my personal use of it, I'm satisfied with it as a replacement to my ultra expensive **iPhone**, that I paid $1400 for.

I've said in my last video that I'm done what I found for $1400 at least they could have stopped their spying on me. But you get a double whammy high price and more spine. So yes a standard **Moto G7** play ships with **Android 9** and it's also an extremely bad device if you use it as is due to **Google** spying as well but at least you can get around it this phone here is rooted it comes with **Android 10** **AOSP** which is the **Android Open Source Project** and I customized it for privacy. 

If you want to follow my process here you can certainly do this by yourself. Though this is probably not something that a non-technical person should do themselves. You will likely bricked your phone. It took me a while to get this going and I did **hard brick** the phone. **Hard brick** means you can't even boot the device. It's just a black screen. But I learned how to recover it, and now I've developed some expertise on this particular phone.

Let's talk about **AOSP** first. When **Google** wants to release a new version of **Android** it first creates an open-source version of it called **AOSP**. This is the starting point of **Android** that is received by every phone **OEM** or one manufacturer, because it's open-source **Google** doesn't but any proprietary code in there. There's absolutely no code that shows you how to connect to **Google** directly it doesn't even have code for **Wi-Fi scanning**,  which I mention is how it tracks your location every second. There's no **Google Playstore**, and there are no **Google** services that is used by the **apps** so when you install a plane **AOSP** on a phone in reality it does very little but it can also do very little to spy on you for one thing there's no **Google** login. So I have never logged into **Google** on this phone now in its final form.

I made some compromises that allow some limited **Google** telemetry on this. But at least a phone remains unidentified. And my home network is completely on a **VPN** by **hardware routing**, so I don't have to worry about being tracked using an **IP address** at home.

Let me show you the actual phone so you can see what I've done first I modified the **AOSP** to have **three** particular services, which are very important. The most important is **F-droid**. **F-droid** is an open source repository of **Android apps** it is not associated with **Google Play** and the **apps** on it are not on **Google Play**. **F-droid** is one of the safest sources of **apps** for **Android** because of its strict free and open source requirement. 

Now if I stopped here, these are the only **apps** I would install: **DuckDuckGo** for browsing a search new pipe which is a **Youtube** front-end so you don't have to go to **YouTube** and a weather **app** called **Forecastie**. This is important to think about because weather **apps** are one of the biggest sources of spying so I wouldn't trust any non open-source weather **app**. 

Then I loaded **Brax.Me** since I made this **app** I can load it manually without any store now if you just stop here you're in good shape no telemetry no tracking but also no notifications most of you want more features on your phone. 

In fact if you wanted to stop here you'll be even more secure with a **Linux phone** and install **Linux** **apps** but to get to the next stage you'll need a couple more pieces to get the phone to install some **apps** that you commonly find in the **Google Play Store**. But you don't want ever to install **Google Play** on here so you have to know the alternatives.

As you see here, I've installed two more **apps** on the phone that will allow us access to the major **apps** on **Google Play**. These are the **Aurora Store** and **MicroG** from the project **MicroG**. Both of these are open-source projects and what they will do is to allow us anonymous access to **Google Play**. So we can download many **apps**, get notifications and yet maintain no identity that is attached to the phone. There is still no **Google** login on this phone, in fact I will never login to **Google** at the device level.

I'm going to show you the **apps** I have so far that I've successfully installed on this phone without the use of **Google Play**. I have **Yelp**, **Uber** and **Ways**. Now in case you didn't know, **Waze** is owned by **Google**, but this is the rare **Google** **app** that actually didn't require **Google Services**, in fact, you can use **Waze** without ever logging in. So just turn on location when you're using the **app**. This is probably that killer **app** that explains why the average person cannot survive with a **Linux phone**, but fortunately my car has navigation, so I don't need to use this. But some of you need it and here we show you that it works and there's the **YouTube** space location. 

You cannot install **Uber Driver** **app** by the way, and **Lyft** does not work so that's not an option without **Google Play** then here you can see I have **Spotify**, **Periscope** and **Twitter** since I have many followers on **Periscope** and **Twitter** the only real problem I found is that **Periscope** does not allow login by phone number on this otherwise it works fine including broadcasting, after I **tweet** the phone.

**Email** is always a problem and I have many videos on this. I could not find an open source email that worked with **Gmail** so here I installed **Edison Mail** this is not open source and you will likely get advertising so I have a special email I used only for this phone for other communications choices these work fine **Telegram**, **Viber**, **Zoom**, **Signal** and of course my **app Brax.Me**.  

For financial transactions I installed **PayPal**, **Venmo** in **Assam Bank** I tried **Bank of America**.

For two-factor authentication I installed **Authy**, which works like the same as **Google Authenticator**.

So now this is a very functional phone for the average person there are many **apps** I wouldn't recommend installing on here or I guarantee that that it will break your privacy. These are all **app** from **Facebook**,  including **Whatsapp**, **Instagram** and **Facebook Messenger**. I have another video explaining their special techniques for spying on you. 

There are other **apps** that are *untrustworthy*, like **Tick-tock**, **Snapchat** and I would not install any weather **app** that is not open source, as it will track your location and sell it. 

There are no **Google** **apps** here. There is no **YouTube**, there is no **Gmail** ,no **Google Maps**. If you try to install them they won't work without **Google Play**. 

Now how does this all work without **Google Play** or any **Google** services on all the other **apps** I just showed you. I'm going to show you some of the internals of **Aurora** store and **MicroG** so you can see how it works **Aurora Store** actually gets the **apps** from **Google Play** but in order to maintain privacy it does it by spoofing your **phone's ID** and you can see here where the spoofing is set. 

I turn on all the spoofing options and even my **Gmail** is spoofed this means that your actual **app** loads are up to date versions from the actual **Google Play Store**.

But it's not enough some **apps** require **Google Services** like **Google Maps API** and notifications.

So the other trick is to install **MicroG**. **MicroG** is a **Google Services** **spoofer**, it makes **apps** think that they're talking to **Google** but they're actually being routed externally, through the **MicroG Services**. **MicroG** can even spoof the geolocation services. 

Here are some of the settings that are available on **MicroG** so you can see how the spoofing is done here. There's an option to add a **Google** account for that trouble some **app** that keeps asking you. But I'm not going to do that because it defeats the purpose of this phone I enabled **Google** device registration because this sets up a unique identifier for notifications. Notifications themselves are controlled by **Google Cloud** messaging which is enable here as well. Meaning **MicroG** wills poof it, and that's all I allowed and this should at least ensure that notifications work for the **apps** I have installed.

So I've got a nicely functional phone here with some compromises, each time you use any **app** that uses a **Google Service,** some indirect pinging of **Google** will occur although your phone itself is not specifically identified, and the traffic is routed through the **Aurora** and **microG Services**. 

That should stop specific identification of a phone. Also many **apps** require you to login, so if you're not on a **VPN** those **apps** may get your **IP address** and your location. 

However they should have a problem retrieving more information, such as your **Google ID**. Though you still have individual **app** login there will be no common thread linking the **apps** to you, since there's no common **Google ID** identifier.

For most users I would say this is a good privacy phone and as long as you're careful not to install dangerous **apps**, like **Facebook** **apps**, then it should be good. I've the **apps** that I show here I would really be careful about what **apps** you choose in general. 

Now some will ask if this can be done on a **Samsung Galaxy** or some other phone model the answer is this if you're an expert look for phone supported by the **LineageOS project** and install it without **GAPS**, **Google** **apps**. And then you can modify the phone as I've done here. You'll find though that very few new phones are supported by **LineageOS** they mostly have older phones on their supported list. So certain **AOSP** providers have focused on newer models of specific phones. For example a good **AOSP** is **eFoundation** which will sell you a phone already configured and they only do **Samsung Galaxys**.

So if I wanted to do this to a **Samsung Galaxy** I would go to **eFoundation**. If you want to use the **Google Pixel** then you may want to use **Graphene OS** which should be a fine **AOSP** choice for that I myself will preconfigure **Moto G7** and **Moto G7 Play** phones which are less expensive and practically new so if you want those I have those in my store on **Brax.Me**. And fortunately I can get enough supply of these. I will refer to my customization as **Brax ROM** and I installed in each OS on the **Moto G7** and modified the **LineageOS** in the same way I do with the **Play**.

This does not mean that I preferred these over **Linux** phones. I still have my **PinePhone** and a **Nexus 5** running **Ubuntu Touch**. But sometimes we are reliant on these phones and some **apps** become essential for specific purposes. Like if I have to broadcast on **Periscope** I need access to the **Periscope** **app**, so I simply move the **SIM** card around as needed to whatever phone I need for the purpose.

I hope this helps and provide some guidance. I've tried to give people a range of choices for decision-making that are still privacy focus phones are still dangerous PI devices so at all times you may still need to remove that **SIM** card.


<script src="https://utteranc.es/client.js"
        repo="op07n/fastpages"
        issue-term="pathname"
        theme="github-light"
        crossorigin="anonymous"
        async>
</script>
