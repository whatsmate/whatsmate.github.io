---
layout: post
title: How to send WhatsApp Messages in C# using Visual Studio 2019
subtitle: Using the WhatsMate WA Gateway REST API
published: true
last_modified_at: 2025-03-16T00:00:00+08:00
---

This article shows you how to send a WhatsApp message in Microsoft's .net language: C#.

If you are using Visual Studio 2022, please read [this tutorial](/2022-07-18-send-whatsapp-message-csharp-vs2022/) instead.

Before the recipient can receive your WhatsApp message, she will need to register with the WhatsMate WA Gateway. Instructions are available on the [official site](https://www.whatsmate.net/whatsapp-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


<iframe width="560" height="315" src="https://www.youtube.com/embed/9A7gtNC-_PU?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


To send a WhatsApp message in C#, do this:

1. Copy the following source code to the main class in your Console Application in Visual Studio.  <script src="https://gist.github.com/whatsmate/50e30fb8c2873f5da63e.js"></script>
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


You will need a trial account to call the above API. Go [sign up](https://www.whatsmate.net/whatsapp-gateway-api.html) now.



<br>

