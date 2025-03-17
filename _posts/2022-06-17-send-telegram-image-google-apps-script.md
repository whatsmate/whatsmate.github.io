---
layout: post
title: How to send an image to a Telegram user from Google Apps Script (GAS)
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2025-03-16T00:00:00+08:00
---

This article shows you how to send a an image to a Telegram user from a Google Apps Script.

Before the recipient can receive your Telegram message, she will need to register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). *Unregistered users will NEVER receive messages from the Gateway.*


To send a Telegram message from a Google Apps Script, do this:


1. First, learn how to send a simple text message on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). 
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/telegram-demos/archive/master.zip).
3. Copy the following source code to your Apps Script project.  <script src="https://gist.github.com/whatsmate/c8530ef424533a0a11545d07d86e62cf.js"></script>
4. Customize the TODO lines:
   * Specify your gateway instance ID on line 18.
   * Specify your client ID and secret on lines 19 and 20.
   * Specify your target recipient on line 3. Remember to include the country code.
   * Specify the filename of your image on line 4.
5. Run the function `demoSendTelegramImageInDrive()` to send your message.


You will need a trial account to call the above API. Go [sign up](https://www.whatsmate.net/telegram-gateway-api.html) now.


<br>

