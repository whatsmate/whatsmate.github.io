---
layout: post
title: How to send messages to a WhatsApp group from Google Apps Script
subtitle: Using the WhatsMate WA Gateway REST API
published: true
last_modified_at: 2026-01-28T20:11:00+08:00
---

This article shows you how to send a message to a WhatsApp group from a Google Apps Script.

You MUST obtain the secret gateway number by signing up for a Forever Green account before you can send a message to a WhatsApp group. Instructions are available on the [official site](https://www.whatsmate.net/whatsapp-group-message-api.html). 


To send a WhatsApp group message from a Google Apps Script, do this:

1. Create a new group with a *unique* name. The API won't work if it's not unique.
   * <img src="/img/newgroup.png" alt="Create a new WhatsApp group"> <br><br>
2. Add the secret gateway to the group.
   * <img src="/img/add-gateway-to-group.png" alt="Name the WhatsApp group"> <br><br>
3. Say "Hi" to the group to let the gateway recognize the new group.
4. Copy the following source code to your Apps Script project.  <script src="https://gist.github.com/whatsmate/59b3b6ee47a5f087288680e2ae009945.js"></script>
5. Customize the TODO lines in the Google Apps script:
   * Specify your gateway instance ID on line 10.
   * Specify your Client ID and Client secret on lines 11 and 12.
   * Specify the group admin number (i.e. your WhatsApp number including the country code) on line 2.
   * Specify the group name (e.g. Happy Club) on line 3.
   * Specify the content of the message on line 4.
6. Run the function `main()` to send your message.


As mentioned at the beginning of this tutorial, you will need a trial account to call the above API. Go [sign up](https://www.whatsmate.net/whatsapp-group-message-api.html) now.


Happy coding :) 


<br>

