---
layout: post
title: How to send Telegram Messages from shell script
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2025-09-29T00:00:00+08:00
---

This article shows you how to send a Telegram message from a shell script.

Before the recipient can receive your Telegram message, she will need to register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


<iframe width="560" height="315" src="https://www.youtube.com/embed/tuW_WvU_NW8?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


To send a Telegram message from a shell script, do this:

1. Copy the following source code to your script.  <script src="https://gist.github.com/whatsmate/a29b2ba722ff34f657b002dbd0611643.js"></script>
2. Customize the TODO lines:
   * Specify your Telegram gateway instance ID on line 3.
   * Specify your Client ID and Secret on lines 4 and 5.
   * Specify your target recipient on line 10. Remember to include the country code.
   * Specify your message on line 11.
3. Make your script executable: `chmod 755 send-telegram-text.sh`
4. Run the script to send your message: `./send-telegram-text.sh`


You will need a trial account to call the above API. Go [sign up](https://www.whatsmate.net/telegram-gateway-api.html) now.



<br>

