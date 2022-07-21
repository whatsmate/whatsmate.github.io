---
layout: post
title: How to send Telegram Messages in C# using Visual Studio 2019
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2022-07-20T00:00:00+08:00
---

This article shows you how to send a Telegram message in Microsoft's .net language: C# using Visual Studio 2019.

If you are using Visual Studio 2022, please read [this tutorial](/2022-07-20-send-telegram-message-csharp-vs2022/) instead.

Before the recipient can receive your Telegram message, she will need to register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


<iframe width="560" height="315" src="https://www.youtube.com/embed/H6HgQ-VJq2Y?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


To send a Telegram message in C# using Visual Studio 2019, do this:

1. Copy the following source code to the main class in your Console Application in Visual Studio.  <script src="https://gist.github.com/whatsmate/ca80d22bbf4043f0d76f1507fe48aeec.js"></script>
2. Customize the TODO lines:
   * Specify your gateway instance ID on line 10.
   * Specify your client ID and secret on lines 11 and 12.
   * Specify your target recipient and message on line 19. Remember to include the country code in the recipient's number.
4. Add the reference "System.Web.Extensions" by doing this:
   1. Right-click on your project node in the Solution Explorer panel.
   2. Choose "Add" -> "Reference..."
   3. Choose "Framework" on the left pane.
   4. Look for "System.Web.Extensions" in the middle pane. Check the checkbox in front of it.
   5. Click OK.
5. Build and run the application in Visual Studio.


You will need a trial account to call the above API. Go [sign up](https://www.whatsmate.net/telegram-gateway-api.html) now.



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

