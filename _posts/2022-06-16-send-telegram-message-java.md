---
layout: post
title: How to send Telegram Messages in Java
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2025-03-16T00:00:00+08:00
---

This article shows you how to send a Telegram message in `Java`.

Before the recipient can receive your Telegram message, she will need to register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


<iframe width="560" height="315" src="https://www.youtube.com/embed/zW2SVh02Vgo?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


To send a Telegram message in `Java`, do this:

1. Copy the following source code to a Java file named `TelegramSender.java`.  <script src="https://gist.github.com/whatsmate/f3660c4b835c5dcdc2ccbb5b871b8e08.js"></script>
2. Customize the TODO lines:
   * Specify your gateway instance ID on line 9.
   * Specify your client ID and secret on lines 10 and 11.
   * Specify your target recipient on line 18. Remember to include the country code.
   * Specify your message on line 19.
3. Compile the Java file:  `javac TelegramSender.java`
4. Execute the class to send your message: `java TelegramSender`


You will need a trial account to call the above API. Go [sign up](https://www.whatsmate.net/telegram-gateway-api.html) now.



<br>

