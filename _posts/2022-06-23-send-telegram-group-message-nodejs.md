---
layout: post
title: How to send messages to a Telegram group in Node.js
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2025-01-02T00:00:00+08:00
---

This article shows you how to send a message to a Telegram group in Java.

You MUST obtain the secret gateway number by signing up for a Premium account before you can send a message to a Telegram group. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-subscribe.html).


<iframe width="560" height="315" src="https://www.youtube.com/embed/bFogc8tTU0I?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


To send a Telegram group message from your Node.js application, do this:

1. Create a New Group from your Telegram client.
2. Add the secret gateway to the group. (Of course, you can add other people as well!)
3. Say something in the group from your personal Telegram client. This gives the gateway a chance to learn about the new group.
4. Copy the following source code to your script.  <script src="https://gist.github.com/whatsmate/34c02edb7a9d80a57a1b6bf82f887ce0.js"></script>
5. Customize the TODO lines in the Node.js script:
   * Specify your gateway instance ID on line 5.
   * Specify your Client ID and Client secret on lines 6 and 7.
   * Specify the group name and the group admin on lines 10 and 11.
   * Specify the content of the message on line 12.
6. Make your Node.js script executable: `chmod 755 group-send-telegram-text.js`
7. Run the script to send your message: `./group-send-telegram-text.js`


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

