---
layout: post
title: How to send an audio file to a Telegram group in Node.js
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2025-03-16T00:00:00+08:00
---

This article shows you how to send an audio file (e.g. an MP3 file) to a registered Telegram group in Node.js (JavaScript).


<iframe width="560" height="315" src="https://www.youtube.com/embed/-U2bS70t8Cg?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


To send a Telegram message containing an audio file in `Node.js`, do this:

1. First, learn how to send a simple text message to a group on the [official site](https://www.whatsmate.net/telegram-group-message-api.html). 
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/telegram-demos/archive/master.zip).
3. Locate the file `nodejs/group-send-telegram-mp3.js`.  <script src="https://gist.github.com/whatsmate/3b66343305e4bde9c2a3abdf4a429d44.js"></script>
4. Study the `Node.js` source code and customize the TODO/FIXME lines.
5. Change to the directory containing the script: `cd nodejs`
6. Run the script to send your group the first MP3 file: `./group-send-telegram-mp3.js`


Happy coding :) 


<br>

