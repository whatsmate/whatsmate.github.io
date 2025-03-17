---
layout: post
title: How to send an audio file to a Telegram group from Google Apps Script (GAS)
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2025-03-16T00:00:00+08:00
---

This article shows you how to send an audio file (e.g. an MP3 file) to a registered Telegram group from a Google Apps Script.



To send a Telegram message containing an audio file from a Google Apps Script, do this:

1. First, learn how to send a simple text message to a group on the [official site](https://www.whatsmate.net/telegram-group-message-api.html). 
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/telegram-demos/archive/master.zip).
3. Copy the following source code to your Google Apps Script project.  <script src="https://gist.github.com/whatsmate/27291c86a9e30c5a98d33c59b6b5781a.js"></script>
4. Customize the TODO lines:
   * Specify your gateway instance ID on line 19.
   * Specify your client ID and secret on lines 20 and 21.
   * Specify your target group on lines 2 and 3.
   * Specify your MP3 file on line 4.
5. Run the function `demoSendMp3ToTelegramGroup()` to send your first MP3 file.


You will need a trial account to call the above API. Go [sign up](https://www.whatsmate.net/telegram-group-message-api.html) now.


<br>

