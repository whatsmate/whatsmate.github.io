---
layout: post
title: How to send Telegram Messages from a Google Sheet using Google Apps Script (GAS)
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2025-10-23T00:00:00+08:00
---

This article shows you how to send a Telegram message from a Google Sheet using Google Apps Script.

Before the recipient can receive your Telegram message, she will need to register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). *Unregistered users will NEVER receive messages from the Gateway.*


To send a Telegram message from a Google Apps Script, do this:

1. Copy the following source code to your Apps Script project.  <script src="https://gist.github.com/whatsmate/358914cd35958847111b4bbfa380a1de.js"></script>
2. Customize the TODO lines:
   * Specify your gateway instance ID on line 15.
   * Specify your client ID and secret on lines 16 and 17.
   * Specify your target recipient on line 6. Remember to include the country code.
   * Specify your message on line 9.
3. Run the function `main()` to send your message.


You will need a trial account to call the above API. Go [sign up](https://www.whatsmate.net/telegram-gateway-api.html) now.


<br>

