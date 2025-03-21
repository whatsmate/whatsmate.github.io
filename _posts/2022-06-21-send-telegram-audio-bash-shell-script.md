---
layout: post
title: How to send an audio file to a Telegram user from bash shell script
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2025-03-16T00:00:00+08:00
---

This article shows you how to send an audio file (e.g. an MP3 file) to a registered Telegram user from a bash shell script.

<iframe width="560" height="315" src="https://www.youtube.com/embed/XT3IIwhT6VQ?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>

To send a Telegram message containing an audio file from a bash shell script, do this:

1. First, learn how to send a simple text message on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). 
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/telegram-demos/archive/master.zip).
3. Locate the file `bash/send-telegram-mp3.sh`.  <script src="https://gist.github.com/whatsmate/1467e4787bfd6153f75c84f3c1d9ae21.js"></script>
4. Study the script and customize the TODO/FIXME lines.
   * Among other things, put down YOUR OWN number as the recipient. You can't send messages to strangers because we are against SPAMMERS.
5. Change to the directory containing the script: `cd bash`
6. Run the script to send yourself the first MP3 file: `./send-telegram-mp3.sh`


Happy coding :) 


<br>

