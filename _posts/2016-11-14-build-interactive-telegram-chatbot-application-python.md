---
layout: post
title: How to Build an Interactive Price Quoting Application over Telegram in Python
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2025-01-02T00:00:00+08:00
---

This article shows you how to build an interactive price quoting application over Telegram in Python. The application responds to user's requests for price quotes interactively. Don't know what I am talking about? The following screenshot should explain it more clearly:

<p style="text-align:center;">
  <img width="250" height="444" src="/img/interactive-price-quote-application.png"/>
</p>


### Prerequisites:

1. You need an Enterprise Telegram Gateway API account with [WhatsMate](https://www.whatsmate.net/telegram-gateway-comparison.html).
2. You have access to a Linux (such as Ubuntu) machine.
3. Your machine has `Python` and `pip` installed.


### Video Tutorial:

<iframe width="560" height="315" src="https://www.youtube.com/embed/12wKWvXYAz4?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


### Steps:

1. Download the [source code package](https://github.com/whatsmate/telegram-demos/archive/master.zip){:target="_blank"}. Alternatively, you can clone the [demo repository](https://github.com/whatsmate/telegram-demos){:target="_blank"} if you use git.
2. `cd telegram-demos/python`
3. `sudo pip install requests Flask` 
4. Customize the Python script `enterprise-demo-app.py` with your account settings on lines 33-47.
5. Run your application: `./enterprise-demo-app.py`


### Explanation:

If you are new to Python and want to understand how the script `enterprise-demo-app.py` works, we are here to help:

1. Lines 3-4 import the required dependent libraries.
2. Lines 50-71 define the utility function `sendTelegramMessage`. Its name already tells you what it does. You don't need to change it.
3. Line 75 creates the `Flask` web framework instance.
4. Lines 86-103 are the gist of the application. You define how you want to respond to your user's messages here. The sample program implements a simplistic price quoting engine. Feel free to change it to fit your own needs.
5. Lines 106-108 kick start the `Flask` web application server so that it listens on the specified port for incoming webhook events.


### What's Next:

If you are keen to implement an automated interactive application that talks to your users on Telegram, [get in touch](https://www.whatsmate.net/contact.html) with one of our technical representatives to sign up for an Enterprise account now.

Want to look at other innovative ideas? Check out the [interesting use cases](https://www.whatsmate.net/telegram-gateway-use-cases.html) page.


### Disclaimer:

1. We are not affiliated with Telegram in any way. We only provide a gateway for sending out and receiving Telegram messages. We cannot guaranttee the gateway is functional at all times.


<br>
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
     style="display:inline-block;width:728px;height:90px"
     data-ad-client="ca-pub-7383487179928477"
     data-ad-slot="6959057004"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>
<br>

