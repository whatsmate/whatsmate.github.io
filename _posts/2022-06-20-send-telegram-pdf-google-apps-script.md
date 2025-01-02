---
layout: post
title: How to send a PDF file to a Telegram user from Google Apps Script (GAS)
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2025-01-02T00:00:00+08:00
---

This article shows you how to send a document (e.g. a PDF file) to a registered Telegram user from a Google Apps Script.

Before the recipient can receive your Telegram message, she will need to register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). *Unregistered users will NEVER receive messages from the Gateway.*


To send a Telegram message containing a PDF file from a Google Apps Script, do this:

1. First, learn how to send a simple text message on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). 
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/telegram-demos/archive/master.zip).
3. Copy the following source code to your Apps Script project.  <script src="https://gist.github.com/whatsmate/6d0c2d985a3a4ba9760b8bbc9a9f8e3f.js"></script>
4. Customize the TODO lines:
   * Specify your gateway instance ID on line 19.
   * Specify your client ID and secret on lines 20 and 21.
   * Specify your target recipient on line 3. Remember to include the country code.
   * Specify your PDf document on line 4.
5. Run the function `demoSendTelegramPdfInDrive()` to send your message.


You will need a trial account to call the above API. Go [sign up](https://www.whatsmate.net/telegram-gateway-api.html) now.


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

