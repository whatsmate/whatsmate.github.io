---
layout: post
title: How to send an audio file to a Telegram user in PHP
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2022-06-21T00:00:00+08:00
---

This article shows you how to send an audio file (e.g. an MP3 file) to a registered Telegram user in PHP.

Before the recipient can receive your Telegram message, she MUST register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


To send a Telegram message containing an audio file in PHP, do this:

1. First, learn how to send a simple text message on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). 
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/telegram-demos/archive/master.zip).
3. Locate the file `php/send-telegram-mp3.php`. <script src="https://gist.github.com/whatsmate/bdbca5b9e8a4d2b7b7f1bc484b46f80b.js"></script>
4. Study the PHP source code and customize the TODO/FIXME lines.
   * Among other things, put down YOUR OWN number as the recipient. You can't send messages to strangers because we are against SPAMMERS.
5. Visit the PHP page your just created to send your MP3 file.


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

