---
layout: post
title: How to send Telegram Messages in Python 3
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2024-04-17T00:00:00+08:00
---

This article shows you how to send a Telegram message from a Python script (version 3+).

Before the recipient can receive your Telegram message, she will need to register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


<iframe width="560" height="315" src="https://www.youtube.com/embed/LwdChr2JEhk?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


To send a Telegram message from a Python script, do this:

1. Copy the following source code to your script.  <script src="https://gist.github.com/whatsmate/d8b7cc36621a54990292c7655849138a.js"></script>
2. Customize the TODO lines:
   * Specify your gateway instance ID on line 6.
   * Specify your Client ID and Secret on lines 7 and 8.
   * Specify your target recipient on line 12. Remember to include the country code.
   * Specify your message on line 13.
3. Make your script executable: `chmod 755 send-telegram-text-individual.py`
4. Run the script to send your message: `./send-telegram-text-individual.py`


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
