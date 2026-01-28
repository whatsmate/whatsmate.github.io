---
layout: post
title: How to send Telegram Messages in VB.NET
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2026-01-28T20:11:00+08:00
---

This article shows you how to send a Telegram message in Microsoft's .net language: VB.NET.

Before the recipient can receive your Telegram message, she will need to register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


<iframe width="560" height="315" src="https://www.youtube.com/embed/ur7PBgGhI28?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


To send a Telegram message in VB.NET, do this:

1. Copy the following source code to the main module file in your Console Application in Visual Studio.  <script src="https://gist.github.com/whatsmate/72d4e510e19e7d384e52bbab08a1678e.js"></script>
2. Customize the TODO lines:
   * Specify your gateway instance ID on line 10.
   * Specify your client ID and secret on lines 11 and 12.
   * Specify your target recipient and message on line 60. Remember to include the country code in the recipient's number.
3. Build and run the application in Visual Studio.


You will need a trial account to call the above API. Go [sign up](https://www.whatsmate.net/telegram-gateway-api.html) now.



<br>

