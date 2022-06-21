---
layout: post
title: How to send a PDF file to a Telegram user from bash shell script
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2022-06-20T00:00:00+08:00
---

This article shows you how to send a document (e.g. a PDF file) to a registered Telegram user from a bash shell script.

Before the recipient can receive your Telegram message, she MUST register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


To send a Telegram message containing a PDF document from a bash shell script, do this:

1. First, learn how to send a simple text message on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). 
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/telegram-demos/archive/master.zip).
3. Locate the file `bash/send-telegram-pdf.sh`.  <script src="https://gist.github.com/whatsmate/29929061744dc8da5940407810bedae9.js"></script>
4. Study the script and customize the TODO/FIXME lines.
   * Among other things, put down YOUR OWN number as the recipient. You can't send messages to strangers because we are against SPAMMERS.
5. Change to the directory containing the script: `cd bash`
6. Run the script to send yourself the first image: `./send-telegram-pdf.sh`


Happy coding :) 


<br>
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
     style="display:inline-block;width:728px;height:90px"
     data-ad-client="ca-pub-7383487179928477"
     data-ad-slot="6959057004"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>
<br>

