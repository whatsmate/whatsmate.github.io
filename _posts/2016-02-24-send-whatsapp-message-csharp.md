---
layout: post
title: How to send WhatsApp Messages in C#
subtitle: Using the WhatsMate WA Gateway REST API
published: true
---

This article shows you how to send a WhatsApp message in Microsoft's .net language: C#.

Before the recipient can receive your WhatsApp message, she will need to register with the WhatsMate WA Gateway. Instructions are available on the [official site](https://www.whatsmate.net/whatsapp-gateway-api.html). *Unregistered users will never receive messages from the Gateway.*


<iframe width="560" height="315" src="https://www.youtube.com/embed/Z7LedIO47Yw?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


To send a WhatsApp message in C#, do this:

1. Copy the following source code to the main class in your Console Application in Visual Studio.  <script src="https://gist.github.com/whatsmate/50e30fb8c2873f5da63e.js"></script>
2. Specify your target recipient and message on line 18. Remember to include the country code in the recipient's number.
3. Add the reference "System.Web.Extensions" by doing this:
   1. Right-click on your project node in the Solution Explorer panel.
   2. Choose "Add" -> "Reference..."
   3. Choose "Framework" on the left pane.
   4. Look for "System.Web.Extensions" in the middle pane. Check the checkbox in front of it.
   5. Click OK.
4. Build and run the application in Visual Studio.


The trial account allows you to send up to 30 messages per day for the first 1000 messsages. [Upgrade to the Forever Green plan](https://www.whatsmate.net/whatsapp-gateway-subscribe.html) to keep your application running after the trial period.



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

