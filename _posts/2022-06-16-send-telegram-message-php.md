---
layout: post
title: How to send Telegram Messages from PHP
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2025-03-16T00:00:00+08:00
---

This article shows you how to send a Telegram message from PHP.

Before the recipient can receive your Telegram message, she will need to register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


<iframe width="560" height="315" src="https://www.youtube.com/embed/sW7E32wJvUw?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


To send a Telegram message from PHP, do this:

1. Copy the following source code to your script.  <script src="https://gist.github.com/whatsmate/d7bb1a9711703874c9d02de104bf8838.js"></script>
2. Customize the TODO lines:
   * Specify your gateway instance ID on line 2.
   * Specify your client ID and secret on lines 3 and 4.
   * Specify your target recipient on line 7. Remember to include the country code.
   * Specify your message on line 8.
3. Visit the PHP page you just created to send your message.


You will need a trial account to call the above API. Go [sign up](https://www.whatsmate.net/telegram-gateway-api.html) now.



<br>

