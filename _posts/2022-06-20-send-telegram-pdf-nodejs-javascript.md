---
layout: post
title: How to send a PDF file to a Telegram user in Node.js
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2025-03-16T00:00:00+08:00
---

This article shows you how to send a document (e.g. a PDF file) to a registered Telegram user in Node.js (JavaScript).

Before the recipient can receive your Telegram message, she MUST register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


<iframe width="560" height="315" src="https://www.youtube.com/embed/iFj9r08h7Rk?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


To send a Telegram message containing a PDF file in `Node.js`, do this:

1. First, learn how to send a simple text message on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). 
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/telegram-demos/archive/master.zip).
3. Locate the file `nodejs/send-telegram-pdf.js`.  <script src="https://gist.github.com/whatsmate/a2e1a24fd3080e1fb0329168e582f28d.js"></script>
4. Study the `Node.js` source code and customize the TODO/FIXME lines.
   * Among other things, put down YOUR OWN number as the recipient. You can't send messages to strangers because we are against SPAMMERS.
5. Change to the directory containing the script: `cd nodejs`
6. Run the script to send yourself the first PDF file: `./send-telegram-pdf.js`


Happy coding :) 


<br>

