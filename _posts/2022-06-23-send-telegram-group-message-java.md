---
layout: post
title: How to send messages to a Telegram group in Java
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2024-04-17T00:00:00+08:00
---

This article shows you how to send a message to a Telegram group in Java.

You MUST obtain the secret gateway number by signing up for a Premium account before you can send a message to a Telegram group. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-subscribe.html).


<iframe width="560" height="315" src="https://www.youtube.com/embed/QttdR3uQ4Ew?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>



To send a Telegram group message from your Java application, do this:

1. Create a New Group from your Telegram client.
2. Add the secret gateway to the group. (Of course, you can add other people as well!)
3. Say something in the group from your personal Telegram client. This gives the gateway a chance to learn about the new group.
4. Copy the following source code to a Java file named `TelegramGroupTextSender.java`.  <script src="https://gist.github.com/whatsmate/f769d88dd5ad6a6777865456543a11e7.js"></script>
5. Customize the TODO lines in the Java program:
   * Specify your gateway instance ID on line 9.
   * Specify your Client ID and Client secret on lines 10 and 11.
   * Specify the group name and group admin on lines 18 and 19.
   * Specify the content of the message on line 20.
5. Compile the Java file: `javac TelegramGroupTextSender.java`
6. Execute the class to send your message: `java TelegramGroupTextSender`


As mentioned at the beginning of this tutorial, you will need a Premium account to call the above API. Go [sign up](https://www.whatsmate.net/telegram-gateway-subscribe.html) now.


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

