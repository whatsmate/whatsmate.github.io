---
layout: post
title: How to send messages to a WhatsApp group from PowerShell script
subtitle: Using the WhatsMate WA Gateway REST API
published: true
last_modified_at: 2017-04-24T00:00:00+08:00
---

This article shows you how to send a message to a WhatsApp group from a PowerShell script.

You MUST obtain the secret gateway number by signing up for a Forever Green account before you can send a message to a WhatsApp group. Instructions are available on the [official site](https://www.whatsmate.net/whatsapp-group-message-api.html). 


To send a WhatsApp group message from a PowerShell script, do this:

1. Create a new group from your WhatsApp client.
   * <img src="/img/newgroup.png" alt="Create a new WhatsApp group"> <br><br>
2. Add the secret gateway to the group.
   * <img src="/img/add-gateway-to-group.png" alt="Name the WhatsApp group"> <br><br>
3. Remember the name you gave to the group (e.g. "Happy Club")
4. Copy the following source code to your PowerShell script. <script src="https://gist.github.com/whatsmate/09a72c834309494c891a0084cf81abe6.js"></script>
5. Customize the TODO lines in the VB Script program:
   * Specify your gateway instance ID on line 5.
   * Specify your Client ID and Client secret on lines 6 and 7.
   * Specify the group admin number (i.e. your WhatsApp number including the country code) on line 1.
   * Specify the group name (e.g. Happy Club) on line 2.
   * Specify the content of the message on line 3.
6. Run it.


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

