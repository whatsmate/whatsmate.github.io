---
layout: post
title: How to send Telegram Messages in Visual Basic Script / VBA
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2025-03-16T00:00:00+08:00
---

This article shows you how to send a Telegram message in VBA / Visual Basic Script.

Before the recipient can receive your Telegram message, she will need to register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


<iframe width="560" height="315" src="https://www.youtube.com/embed/7SEZkHn514c?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


To send a Telegram message in VBA / VB Script, do this:

1. In your Excel / Access / VBA development environment, define the following subroutines:  <script src="https://gist.github.com/whatsmate/1b4374efdc1d865f2218200a125f45d1.js"></script>
2. Customize the TODO lines:
   * Specify your gateway instance ID on line 15.
   * Specify your client ID and secret on lines 16 and 17.
   * Specify your target recipient and message on line 4. Remember to include the country code in the recipient's number.
3. Run it.


You will need a trial account to call the above API. Go [sign up](https://www.whatsmate.net/telegram-gateway-api.html) now.



<br>

