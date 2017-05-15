---
layout: post
title: How to send Telegram Messages from shell script
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2017-03-31T00:00:00+08:00
---

This article shows you how to send a Telegram message from a shell script.

Before the recipient can receive your Telegram message, she will need to register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). *Unregistered users will NEVER receive messages from the Gateway.*


<iframe width="560" height="315" src="https://www.youtube.com/embed/NVTLFRtNbLQ?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


To send a Telegram message from a shell script, do this:

1. Copy the following source code to your script.  <script src="https://gist.github.com/whatsmate/c7831b94ff7a97e52f9fe4459e502d2f.js"></script>
2. Customize the TODO lines:
   * Specify your gateway instance ID on line 3.
   * Specify your Client ID and Secret on lines 4 and 5.
   * Specify your target recipient on line 10. Remember to include the country code.
   * Specify your message on line 11.
4. Make your script executable: `chmod 755 send-telegram.sh`
5. Run the script to send your message: `./send-telegram.sh`


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

