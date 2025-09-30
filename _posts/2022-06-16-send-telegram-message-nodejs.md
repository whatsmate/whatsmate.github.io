---
layout: post
title: How to send Telegram Messages in Node.js
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2025-03-16T00:00:00+08:00
---

This article shows you how to send a Telegram message in `Node.js`.

Before the recipient can receive your Telegram message, she will need to register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


<iframe width="560" height="315" src="https://www.youtube.com/embed/DBn7kBuaeW0?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


To send a Telegram message in `Node.js`, do this:

1. Copy the following source code to your script.  <script src="https://gist.github.com/whatsmate/c03ab97e1e11f74aa88228ce13bd62f1.js"></script>
2. Customize the TODO lines:
   * Specify your gateway instance ID on line 5.
   * Specify your client ID and secret on lines 6 and 7.
   * Specify your target recipient on line 10. Remember to include the country code.
   * Specify your message on line 11.
4. Make your `Node.js` script executable: `chmod 755 send-telegram-text.js`
5. Run the script to send your message: `./send-telegram-text.js`


You will need a trial account to call the above API. Go [sign up](https://www.whatsmate.net/telegram-gateway-api.html) now.



<br>

