---
layout: post
title: How to send messages to a Telegram group from PowerShell script
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2019-08-30T00:00:00+08:00
---

This article shows you how to send a message to a Telegram group from a PowerShell script.

You MUST obtain the secret gateway number by signing up for a Premium account before you can send a message to a Telegram group. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-subscribe.html).


To send a Telegram group message from your PowerShell script, do this:

1. Create a New Group from your Telegram client.
2. Add the secret gateway to the group. (You can add other people too!)
3. Give your group a unique and creative name. It's very important!
4. Copy the following source code to your PowerShell script. <script src="https://gist.github.com/whatsmate/2c621494fc38524c6c23fd2639b2dae0.js"></script>
5. Customize the TODO lines in the PowerShell script:
   * Specify your gateway instance ID on line 4.
   * Specify your Client ID and Client secret on lines 5 and 6.
   * Specify the group name on line 1.
   * Specify the content of the message on line 2.
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

