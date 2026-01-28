---
layout: post
title: How to send a voice note file to a Telegram group from Google Apps Script (GAS)
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2026-01-28T20:11:00+08:00
---

This article shows you how to send a voice note file (e.g. an OPUS file) to a registered Telegram group from a Google Apps Script.



To send a Telegram message containing a voice note file from a Google Apps Script, do this:

1. First, learn how to send a simple text message to a group on the [official site](https://www.whatsmate.net/telegram-group-message-api.html). 
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/telegram-demos/archive/master.zip).
3. Copy the following source code to your Google Apps Script project.  <script src="https://gist.github.com/whatsmate/1001b29a9c5a668a89f4f9e80b574307.js"></script>
4. Customize the TODO lines:
   * Specify your gateway instance ID on line 19.
   * Specify your client ID and secret on lines 20 and 21.
   * Specify your target group on lines 2 and 3.
   * Specify your OPUS file on line 4.
5. Run the function `demoSendOpusToTelegramGroup()` to send your first OPUS file to your group.


You will need a trial account to call the above API. Go [sign up](https://www.whatsmate.net/telegram-group-message-api.html) now.


<br>

