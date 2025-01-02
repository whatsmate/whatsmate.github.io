---
layout: post
title: How to send WhatsApp Messages in C# using Visual Studio 2022
subtitle: Using the WhatsMate WA Gateway REST API
published: true
last_modified_at: 2025-01-02T00:00:00+08:00
---

This article shows you how to send a WhatsApp message in Microsoft's .net language: C# using Visual Studio 2022.

If you are using Visual Studio 2019, please read [this tutorial](/2016-02-24-send-whatsapp-message-csharp/) instead.

Before the recipient can receive your WhatsApp message, she will need to register with the WhatsMate WA Gateway. Instructions are available on the [official site](https://www.whatsmate.net/whatsapp-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>



To send a WhatsApp message in C#, do this:

1. Copy the following source code to the main class in your Console Application in Visual Studio.  <script src="https://gist.github.com/whatsmate/14c72f77fb5e1ad4535457c8ff082221.js"></script>
2. Customize the TODO lines:
   * Specify your gateway instance ID on line 10.
   * Specify your client ID and secret on lines 11 and 12.
   * Specify your target recipient and message on line 19. Remember to include the country code in the recipient's number.
5. Build and run the application in Visual Studio.


You will need a trial account to call the above API. Go [sign up](https://www.whatsmate.net/whatsapp-gateway-api.html) now.



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

