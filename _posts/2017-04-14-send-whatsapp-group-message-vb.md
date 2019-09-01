---
layout: post
title: How to send messages to a WhatsApp group in VB.NET
subtitle: Using the WhatsMate WA Gateway REST API
published: true
last_modified_at: 2019-08-30T00:00:00+08:00
---

This article shows you how to send a message to a WhatsApp group in Microsoft’s .net language: Visual Basic.

You MUST obtain the secret gateway number by signing up for a Forever Green account before you can send a message to a WhatsApp group. Instructions are available on the [official site](https://www.whatsmate.net/whatsapp-group-message-api.html). 


To send a WhatsApp group message in VB, do this:

1. Create a new group with a *unique* name. The API won't work if it's not unique.
   * <img src="/img/newgroup.png" alt="Create a new WhatsApp group"> <br><br>
2. Add the secret gateway to the group.
   * <img src="/img/add-gateway-to-group.png" alt="Name the WhatsApp group"> <br><br>
3. Say "Hi" to the group to let the gateway recognize the new group.
4. Copy the following source code to the main module file in your Console Application in Visual Studio.  <script src="https://gist.github.com/whatsmate/771af0c7ea8e4a40edac44f49a70e28c.js"></script>
5. Customize the TODO lines in the VB program:
   * Specify your gateway instance ID on line 10.
   * Specify your Client ID and Client secret on lines 11 and 12.
   * Specify the group admin number (i.e. your WhatsApp number including the country code) on line 66.
   * Specify the group name (e.g. Happy Club) on line 67.
   * Specify the content of the message on line 68.
6. Add the reference “System.Web.Extensions” by doing this:
   * Right-click on your project node in the Solution Explorer panel.
   * Choose “Add” -> “Reference…”
   * Choose “Framework” on the left pane.
   * Look for “System.Web.Extensions” in the middle pane. Check the checkbox in front of it.
   * Click OK.
7. Build and run the application in Visual Studio.


As mentioned at the beginning of this tutorial, you will need a trial account to call the above API. Go [sign up](https://www.whatsmate.net/whatsapp-group-message-api.html) now.


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

