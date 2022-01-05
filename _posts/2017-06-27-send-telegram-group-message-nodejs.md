---
layout: post
title: How to send messages to a Telegram group in Node.js
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2022-01-04T00:00:00+08:00
---

This article shows you how to send a message to a Telegram group in Java.

You MUST obtain the secret gateway number by signing up for a Premium account before you can send a message to a Telegram group. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-subscribe.html).


To send a Telegram group message from your Node.js application, do this:

1. Create a New Group from your Telegram client.
2. Add the secret gateway to the group. (You can add other people too!)
3. Give your group a unique and creative name. It's very important!
4. Copy the following source code to your script.  <script src="https://gist.github.com/whatsmate/34c02edb7a9d80a57a1b6bf82f887ce0.js"></script>
5. Customize the TODO lines in the Node.js script:
   * Specify your gateway instance ID on line 5.
   * Specify your Client ID and Client secret on lines 6 and 7.
   * Specify the group name on line 10.
   * Specify the content of the message on line 11.
6. Make your Node.js script executable: `chmod 755 send-telegram-group.js`
7. Run the script to send your message: `./send-telegram-group.js`


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

