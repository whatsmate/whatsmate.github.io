---
layout: post
title: How to send a voice note file to a Telegram user in Python 3
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2025-03-16T00:00:00+08:00
---

This article shows you how to send a voice note file (e.g. an OPUS file) to a registered Telegram user in Python 3.

Before the recipient can receive your Telegram message, she MUST register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


To send a Telegram message containing a voice note file in Python 3, do this:

1. First, learn how to send a simple text message on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). 
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/telegram-demos/archive/master.zip).
3. Locate the file `python/send-telegram-opus-individual.py`.  <script src="https://gist.github.com/whatsmate/c38a2c1227450d13d8524d92b9c5c921.js"></script>
4. Study the Python source code and customize the TODO/FIXME lines.
   * Among other things, put down YOUR OWN number as the recipient. You can't send messages to strangers because we are against SPAMMERS.
5. Change to the directory containing the script: `cd python`
6. Run the Python script to send yourself the first voice note: `./send-telegram-opus-individual.py`


Happy coding :) 


<br>

