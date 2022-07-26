---
layout: post
title: How to send messages to a Telegram group in VB.NET
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2022-06-23T00:00:00+08:00
---

This article shows you how to send a message to a Telegram group in Microsoft’s .NET language: Visual Basic.NET

You MUST obtain the secret gateway number by signing up for a Premium account before you can send a message to a Telegram group. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-subscribe.html).


<!--
<iframe width="560" height="315" src="https://www.youtube.com/embed/fnyGwfP1O64?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>
-->


To send a Telegram group message in VB, do this:

1. Create a New Group from your Telegram client.
2. Add the secret gateway to the group. (Of course, you can add other people as well!)
3. Say something in the group from your personal Telegram client. This gives the gateway a chance to learn about the new group.
4. Copy the following source code to the main module file in your Console Application in Visual Studio.  <script src="https://gist.github.com/whatsmate/02c86454e2c4f606d70dca765ee2fa6c.js"></script>
5. Customize the TODO lines in the VB program:
   * Specify your gateway instance ID on line 10.
   * Specify your Client ID and Client secret on lines 11 and 12.
   * Specify the group name, group admin and your message on line 66.
6. Add the reference “System.Web.Extensions” by doing this:
   * Right-click on your project node in the Solution Explorer panel.
   * Choose “Add” -> “Reference…”
   * Choose “Framework” on the left pane.
   * Look for “System.Web.Extensions” in the middle pane. Check the checkbox in front of it.
   * Click OK.
7. Build and run the application in Visual Studio.


As mentioned at the beginning of this tutorial, you will need a Premium account to call the above API. Go [sign up](https://www.whatsmate.net/telegram-gateway-subscribe.html) now.


Happy coding :) 


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

