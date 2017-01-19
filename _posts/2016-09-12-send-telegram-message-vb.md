---
layout: post
title: How to send Telegram Messages in VB.NET
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
---

This article shows you how to send a Telegram message in Microsoft's .net language: VB.

Before the recipient can receive your Telegram message, she will need to register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). *Unregistered users will never receive messages from the Gateway.*


To send a Telegram message in VB.NET, do this:

1. Copy the following source code to the main module file in your Console Application in Visual Studio.  <script src="https://gist.github.com/whatsmate/6a1ed2f45241e0b36fc516c3fb6daf49.js"></script>
2. Specify your target recipient and message on line 61. Remember to include the country code in the recipient's number.
3. Add the reference "System.Web.Extensions" by doing this:
   1. Right-click on your project node in the Solution Explorer panel.
   2. Choose "Add" -> "Reference..."
   3. Choose "Framework" on the left pane.
   4. Look for "System.Web.Extensions" in the middle pane. Check the checkbox in front of it.
   5. Click OK.
4. Build and run the application in Visual Studio.


The trial account allows you to send up to 50 messages per day for the first 1000 messages. [Upgrade to the Premium Account](https://www.whatsmate.net/telegram-gateway-subscribe.html) to send unlimited number of messages.


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

