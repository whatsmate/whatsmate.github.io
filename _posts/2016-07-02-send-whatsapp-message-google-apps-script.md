---
layout: post
title: How to send WhatsApp Messages from Google Apps Script
subtitle: Using the WhatsMate WA Gateway REST API
published: true
last_modified_at: 2025-03-16T00:00:00+08:00
---

This article shows you how to send a WhatsApp message from a Google Apps Script.

Before the recipient can receive your WhatsApp message, she will need to register with the WhatsMate WA Gateway. Instructions are available on the [official site](https://www.whatsmate.net/whatsapp-gateway-api.html). *Unregistered users will NEVER receive messages from the Gateway.*


To send a WhatsApp message from a Google Apps Script, do this:

1. Copy the following source code to your Apps Script project.  <script src="https://gist.github.com/whatsmate/96637d1c46e1a199756f18413e739f7b.js"></script>
2. Customize the TODO lines:
   * Specify your gateway instance ID on line 9.
   * Specify your client ID and secret on lines 10 and 11.
   * Specify your target recipient on line 2. Remember to include the country code.
   * Specify your message on line 3.
3. Run the function `main()` to send your message.


You will need a trial account to call the above API. Go [sign up](https://www.whatsmate.net/whatsapp-gateway-api.html) now.


<br>

