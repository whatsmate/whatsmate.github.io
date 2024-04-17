---
layout: post
title: How to send messages to a Telegram group from PowerShell script
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2024-04-17T00:00:00+08:00
---

This article shows you how to send a message to a Telegram group from a PowerShell script.

You MUST obtain the secret gateway number by signing up for a Premium account before you can send a message to a Telegram group. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-subscribe.html).


To send a Telegram group message from your PowerShell script, do this:

1. Create a New Group from your Telegram client.
2. Add the secret gateway to the group. (Of course, you can add other people as well!)
3. Say something in the group from your personal Telegram client. This gives the gateway a chance to learn about the new group.
4. Copy the following source code to your PowerShell script. <script src="https://gist.github.com/whatsmate/2c621494fc38524c6c23fd2639b2dae0.js"></script>
5. Customize the TODO lines in the PowerShell script:
   * Specify your gateway instance ID on line 5.
   * Specify your Client ID and Client secret on lines 5 and 7.
   * Specify the group name and group admin on lines 1 and 2.
   * Specify the content of the message on line 3.
6. Run it.


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

