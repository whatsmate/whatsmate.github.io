---
layout: post
title: How to send Telegram Messages from Node.js script
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
---

This article shows you how to send a Telegram message from a Node.js script.

Before the recipient can receive your Telegram message, she will need to register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). *Unregistered users will NEVER receive messages from the Gateway.*


To send a Telegram message from a Node.js script, do this:

1. Copy the following source code to your script.  <script src="https://gist.github.com/whatsmate/ffaff16a5db1657825ab9f2de0b8323d.js"></script>
2. Specify your target recipient on line 10. Remember to include the country code.
3. Specify your message on line 11.
4. Make your script executable: `chmod 755 send-telegram.js`
5. Run the script to send your message: `./send-telegram.js`


The trial account allows you to send up to 50 messages per day for the first 1000 messages. [Upgrade to the Premium Account](https://www.whatsmate.net/telegram-gateway-subscribe.html) to send unlimited number of messages.


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

