---
layout: post
title: How to send an audio file to a Telegram user in Java
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2022-06-21T00:00:00+08:00
---

This article shows you how to send an audio file (e.g. an MP3 file) to a registered Telegram user in Java.

Before the recipient can receive your Telegram message, she MUST register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


<iframe width="560" height="315" src="https://www.youtube.com/embed/QTD1Ep9LtlM?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>



To send a Telegram message containing an audio file in Java, do this:

1. First, learn how to send a simple text message on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). 
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/telegram-demos/archive/master.zip).
3. Locate the file `Java/TelegramMp3Sender.java`.  <script src="https://gist.github.com/whatsmate/b528b97c1f1cb23e58df8e120d37e49b.js"></script>
4. Study the Java source code and customize the TODO/FIXME lines.
   * Among other things, put down YOUR OWN number as the recipient. You can't send messages to strangers because we are against SPAMMERS.
5. Change to the directory containing the script: `cd Java`
6. Follow the instructions at the top of the source code to compile and run the Java program.


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

