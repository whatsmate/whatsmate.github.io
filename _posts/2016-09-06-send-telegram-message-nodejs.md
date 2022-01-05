---
layout: post
title: How to send Telegram Messages from Node.js script
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2022-01-04T00:00:00+08:00
---

This article shows you how to send a Telegram message from a Node.js script.

Before the recipient can receive your Telegram message, she will need to register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). *Unregistered users will NEVER receive messages from the Gateway.*


<iframe width="560" height="315" src="https://www.youtube.com/embed/hsv3vxwtTlY?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


To send a Telegram message from a Node.js script, do this:

1. Copy the following source code to your script.  <script src="https://gist.github.com/whatsmate/ffaff16a5db1657825ab9f2de0b8323d.js"></script>
2. Customize the TODO lines:
   * Specify your gateway instance ID on line 5.
   * Specify your client ID and secret on lines 6 and 7.
   * Specify your target recipient on line 10. Remember to include the country code.
   * Specify your message on line 11.
3. Make your script executable: `chmod 755 send-telegram.js`
4. Run the script to send your message: `./send-telegram.js`


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

