---
layout: post
title: How to send Telegram Messages in Python
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
---

This article shows you how to send a Telegram message in Python.

Before the recipient can receive your Telegram message, she will need to register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](http://www.whatsmate.net/telegram-gateway-api.html). *Unregistered users will never receive messages from the Gateway.*

To send a Telegram message from a Python script, do this:

1. Copy the following source code to your Python script.  <script src="https://gist.github.com/whatsmate/1a0e56084403c86adef2683d7a137577.js"></script>
2. Specify your recipient's number on line 10.
3. Specify your message on line 11.
5. Install the `Requests` library because the sample script depends on it: `pip install requests`
6. Make your script executable: `chmod 755 send-telegram.py`
7. Run the script to see the result: `./send-telegram.py`


The trial account allows you to send up to 50 messages per day for the first 1000 messages. [Upgrade to the Premium Account](http://www.whatsmate.net/telegram-gateway-subscribe.html) to send unlimited number of messages.


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

