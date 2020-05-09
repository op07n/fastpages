---
toc: false
layout: post
description: How Device Fingerprinting Reveals Your Real Identity.
categories: [markdown]
title: How Device Fingerprinting Reveals Your Real Identity.
---
# How Device Fingerprinting Reveals Your Real Identity.

Borrowed from:

[![Alt text](https://img.youtube.com/vi/673nJQEkhe0/0.jpg)](https://www.youtube.com/watch?v=673nJQEkhe0)

There's a seemingly innocuous piece of data on your phone that actually exposes what you do especially to **Google**, **Apple**, **Facebook**. This is called the device fingerprint. This uniquely identifies your phone to third parties. And likely with your real identity. This is pretty dangerous stuff. And nowadays, this kind of device surveillance will be more rampant in the name of saving lives. 

What I want to do is to examine this little data point on your phone. And see how it can be used against you. Stay put now.

A **device fingerprint** is something available to both **iOS** and **Android**. This is a different thing than the **browser fingerprint** which I talked about in other videos. Because this is specific to a phone. What actually is a **device fingerprint**?. It's any piece of data that uniquely identifies a device among all other devices in existence. Is this a specific piece of data. Actually it's many potential pieces of data which can be combined and some were available in older versions and some are no longer available in **Android 10** for example.

Let me just tell you about some of the unique identifiers on your phone:

First we have the **Google ID** and **Apple ID**. Now these are typically attached to financial information such as *credit cards* so they have a *one-to-one match* with a real identity.  For those would **Apple pay** and other financial services it locks your phone into a *fixed identity*. 

Another identifier on your phone is the **IMEI**. This is the cell modem unique equipment identifier and this can be retrieved by the OS of course and any app that has *telephony permissions*. So any app that has access to phone data and messages can access the **IMEI**.

Another piece of data that is unique is that *notification token*. When your device receives notifications it creates a unique **ID** called a *token* which is available to all apps that handle notifications. This is easily retrieved since most apps have notifications. This is a very important part of **Google GCM** messaging or now **firebase** and there's a lot of telemetry associated with this.

And of course there's an **Apple** equivalent to this called an **APN**.

There are other identifiers that may not always be available such as the *device serial number* .Some of these pieces of device data become part of the *metadata* in a photo. So if you upload a photo to **Facebook** some of this data is included in the *exif metadata*, which also includes locations.

Then, there are other network unique identifiers which are not normally visible to apps,  such as the *MAC* address. But nowadays, this is available to any app that uses the network. There's a Wi-Fi **MAC address** any Bluetooth **MAC address**

And finally, something that is actually sent by the device outside of the phone by default is your **IP address**, something we already know and on browsers. A device info identifier called the *device user data*. That is a major part of *browser fingerprinting*. 

Now it's bad enough that there are all these *unique identifiers* on the phone, but to make it even worse some of these are combined. So if a third party doesn't have current access to one identifier they can correlate to another identifier if it matched in the past if they happen to be able to catch more than one data point at any one time so if any of the above data points are identified what another data point you now have a data pair that can be used to index each other for example a **Google ID** can be combined with a notification **ID** so next time all they need is a notification **ID** and they can derive the **Google ID** an **IMEI** can be combined with a notification **ID** a **Google ID** can be combined with a *MAC address* again if you have a **MAC** address then you can guess what the **Google ID** is this is part the sinister aspect of native apps platforms and device manufacturers this type of tracking can easily be used to identify you and often without your permission.

Just an example of what one could do with this this could be used to generate a social distancing data so we can identify individuals by name not practicing social distancing. This is available to **Apple** and **Google** by identifying a **device fingerprint** together with their 24/7 *location data*. But this is a saving lives kind of application, right. Well, some things are more sinister, for example, every person can be classified according to their *religious beliefs* like converging on churches on Sundays. Or your *health* based on who visited oncology clinics or **AIDS** clinics. Or your *sexual preferences*,  by who was at a *gay bar* or the *strep bar*. Or who was at a protest.

Again, in case you missed, it standard **iOS** and **Android** phones have an **Apple ID** and **Google ID** respectively, which point to your *credit card* with your *real name* and your *home location* . Obviously, **Apple** and **Google** know where the phone is at any one time. This is an insidious threat and it truly bothers me completely.  With those goes another feature called **Wi-Fi scanning**. It can *pinpoint* your movements historically. Again I want to make this clear. With **Google ID** and **Apple ID** your phones are completely identified with your *real name* or your *family's account*. And this is together with whatever behavior is already tracked like *locations apps* used and websites visited. 

So, without the proper consideration of **device fingerprinting** an attempt at *pseudo anonymity* in social media may not work. For example, what happens if you set up multiple **Gmail** accounts on the same phone ? Obviously **Google** will know the owner of these *email accounts* even without a real name. Because they will be connected by a **device fingerprint**. If you try to use multiple **Facebook** accounts you will be spotted immediately. In fact, on any platform where you set up multiple accounts you can be easily identified.

This matters whenever you're trying to create non real name identities on social media. You may be wasting your time if you're not aware of this. So for example, it is clear to a single platform owner such as **Facebook** what your **whatsapp** account is, or your **Instagram** account. Because of the **device fingerprint**. Later on,  I'll tell you how to beat this. 

Now, here's an interesting fact point for you. Many of these data points are available to *native apps* only. This means that some of these identifiers are not available to a *web app* or *browser*. For example, it is a well-known fact that **Facebook** captures your *MAC address* as one of its unique identifiers it also captures the *MAC addresses* of everyone on your network to do relationship tracking. But it requires the app. If you use a *browser* it can't get access to this data. So one of the ways to stump **Facebook** is to never install the app.

*Native apps* can retrieve the **IMEI** of the phone, the cell modem unique *ID*. But *browsers* can't see this. There's another thing that *native apps* can't see and that's the **Google ID** and **Apple ID**. *Browsers* don't see that directly. You have to log in separately to their platforms. Of course, they make it simple now to identify yourself to each platform using something that will match your **phone ID**. Many *apps* offer a **Facebook** and **Google** sign-in. And now, **Apple** is requiring that these apps also now include **Apple sign-in**. These are instead of logging into the *apps* using your own login to the platform. They call this **frictionless logins**. But they are also **frictionless spying** since your * * into giving out multiple pieces of information at once.

By having multiple *apps* identify with a **Google ID**, **Facebook ID** or **Apple ID**. Even *ad trackers* can associate your profile with a real identity while having the platform verify that you're on the same device.

I hope you're seeing that there's a problem here. The moment you use an **iOS** phone an **Android** phone and one of the popular apps with various *ad trackers* like **Facebook** and many apps with **Google ads** on it, then you're basically *chipped* every move you make is now the property of various third parties. And to repeat, this is with some way to reference your *real name*.

Okay. Now let's talk about how we can beat this. It's not easy. It means making some hard choices when it comes to convenience. First, how do we eliminate the connection to our real name with **Google  ID** and **Apple ID**? Well, this is simple don't have an **iOS** phone or a **Google** **Android** phone. If you don't have a **Google** or **Apple** account on the phone, then the data will not be available. Let's say you use a **Linux** phone like **Ubuntu touch** either on a **Pine phone** or a **Nexus 5**. Or let's say you're running a **Libero 5**. These devices have no **Google ID** or **Apple ID**, so that will result in no identifiers sent to those platforms.

Next, 24/7 *location tracking* is done by **Wi-Fi scanning** which sent the data non-stop to **Apple** and **Google** servers. Again a non **iOS** or non **Google** phone can't do this. And fortunately there's another alternative ad googled **AOSP** **Android** does not have this kind of **Wi-Fi scanning** so this data leak will stop.

If you use web apps meaning use browser-based apps the device identifier will be limited. Web apps can do **browser fingerprinting** but that does not reveal a real identity just an indication that you've been seen before. So the less app you load from a **Google Play Store** the less risk of getting *device serial numbers* and things. So web apps also use a different notification token than a *native app*. So they don't cross over.

So web apps are safer. A specific thing with **Android 10**. If you use *de-googled* **Android 10**, some data points are no longer easily retrieved by an app such as a *serial number*. **Android 10** also does *MAC address* spoofing, so it also gives information on that front as well. 

Again with **Android** **AOSP**  *de-googled* there is no identity. In fact your identity on *de-googled* **AOSP** phone like the ones i sell on my store, you share with so many phones. It's called **spoofing**, **identity  spoofing**. So your information becomes *disinformation*, and since you've never logged into a **Google phone** there is nothing to tie it to a real identity.

The main reason for speaking about **device fingerprints** is that some people think they're hiding by using multiple accounts on different platforms. But as you can see, if this is not well thought out, it can nullify your actions. 

Second, it also tells you that as a general rule, found reveal much more information about you than computers. And if given a choice, you should think about separating identities by device, rather than just by accounts. Or by using a computer instead.

Third, the device choice matters. It matters a lot. *Linux phones* and *de-googled* **AOSP Android** phones do not leak the same data as your standard **iOS** or **Android** phone, or some new flagship from **Apple,** **Samsung**, **LG**, **Google** and others.

There's a lot more about this. I can only give you an overview in a short video. When you start planning on a general security plan before you jump into setting up multiple email accounts for example, because I recommend that, you will need to examine your threats and plan to deprive that threat of data.

Now let's briefly compare the difference between **browser fingerprinting** and **device fingerprinting**. **Device fingerprinting** is a capability of *native app* store apps only. You can beat **browser fingerprinting** by having multiple browsers. You cannot beat **device fingerprinting** on a single device, except to have a device that does not send a **device fingerprint** or creates a fake one.

But to me, the worst aspect of **device fingerprinting** is that it is matched to a real identity into location tracking. So, yes, you won't be able to contribute data for social distancing. 

If you follow my tips, sorry about that **Apple** and **Google**. If this video has been helpful to you you might want to subscribe to this channel you get more tools to protect yourself and slam on that notification Bell thank you for watching.

<script src="https://utteranc.es/client.js"
        repo="op07n/fastpages"
        issue-term="pathname"
        theme="github-light"
        crossorigin="anonymous"
        async>
</script>
