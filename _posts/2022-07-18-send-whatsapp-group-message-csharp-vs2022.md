---
layout: post
title: How to send messages to a WhatsApp group in C# using Visual Studio 2022
subtitle: Using the WhatsMate WA Gateway REST API
published: true
last_modified_at: 2025-03-16T00:00:00+08:00
---

This article shows you how to send a message to a WhatsApp group in Microsoft’s .net language: C# using VIsual Studio 2022.

If you are using Visual Studio 2019, please read [this tutorial](/2017-04-13-send-whatsapp-group-message-csharp/) instead.

You MUST obtain the secret gateway number by signing up for a Forever Green account before you can send a message to a WhatsApp group. Instructions are available on the [official site](https://www.whatsmate.net/whatsapp-group-message-api.html). 


To send a WhatsApp group message in C#, do this:

1. Create a new group with a *unique* name. The API won't work if it's not unique.
   * <img src="/img/newgroup.png" alt="Create a new WhatsApp group"> <br><br>
2. Add the secret gateway to the group.
   * <img src="/img/add-gateway-to-group.png" alt="Name the WhatsApp group"> <br><br>
3. Say "Hi" to the group to let the gateway recognize the new group.
4. Copy the following source code to the main class in your Console Application in Visual Studio.  <script src="https://gist.github.com/whatsmate/9c06a22e0f8f3d5daec72ea2c866b84e.js"></script>
5. Customize the TODO lines in the C# program:
   * Specify your gateway instance ID on line 10.
   * Specify your Client ID and Client secret on lines 11 and 12.
   * Specify the group admin number (i.e. your WhatsApp number including the country code) on line 20.
   * Specify the group name (e.g. Happy Club) on line 21.
   * Specify the content of the message on line 22.
7. Build and run the application in Visual Studio.


As mentioned at the beginning of this tutorial, you will need a trial account to call the above API. Go [sign up](https://www.whatsmate.net/whatsapp-group-message-api.html) now.


Happy coding :) 


<br>

