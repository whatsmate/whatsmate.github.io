---
layout: post
title: How to send a voice note file to a Telegram group in Node.js
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2026-01-28T20:11:00+08:00
---

This article shows you how to send a voice note file (e.g. an OPUS file) to a registered Telegram group in Node.js (JavaScript).



To send a Telegram message containing a voice note file in `Node.js`, do this:

1. First, learn how to send a simple text message to a group on the [official site](https://www.whatsmate.net/telegram-group-message-api.html). 
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/telegram-demos/archive/master.zip).
3. Locate the file `nodejs/group-send-telegram-opus.js`.  <script src="https://gist.github.com/whatsmate/a6b6c46cf6dbdf85f2a7d4405ebcfe7c.js"></script>
4. Study the `Node.js` source code and customize the TODO/FIXME lines.
5. Change to the directory containing the script: `cd nodejs`
6. Run the script to send your group the first OPUS file: `./group-send-telegram-opus.js`


Happy coding :) 


<br>

