---
layout: post
title: How to send Telegram Messages in Python
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2017-03-31T00:00:00+08:00
---

This article shows you how to send a Telegram message in Python.

Before the recipient can receive your Telegram message, she will need to register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


<iframe width="560" height="315" src="https://www.youtube.com/embed/D855OS6mXOo?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


To send a Telegram message from a Python script, do this:

1. Copy the following source code to your Python script.  <script src="https://gist.github.com/whatsmate/1a0e56084403c86adef2683d7a137577.js"></script>
2. Specify your recipient's number on line 10.
3. Specify your message on line 11.
5. Install the `Requests` library because the sample script depends on it: `pip install requests`
6. Make your script executable: `chmod 755 send-telegram.py`
7. Run the script to see the result: `./send-telegram.py`


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

