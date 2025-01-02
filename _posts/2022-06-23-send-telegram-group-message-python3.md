---
layout: post
title: How to send messages to a Telegram group in Python 3
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2025-01-02T00:00:00+08:00
---

This article shows you how to send a message to a Telegram group in Python 3.

You MUST obtain the secret gateway number by signing up for a Premium account before you can send a message to a Telegram group. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-subscribe.html).


<iframe width="560" height="315" src="https://www.youtube.com/embed/U8DuyymFRzs?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


To send a Telegram group message from your Node.js application, do this:

1. Create a New Group from your Telegram client.
2. Add the secret gateway to the group. (Of course, you can add other people as well!)
3. Say something in the group from your personal Telegram client. This gives the gateway a chance to learn about the new group.
4. Copy the following source code to your script.  <script src="https://gist.github.com/whatsmate/e46807a91c9c0858e7f173327c581335.js"></script>
5. Customize the TODO lines in the Node.js script:
   * Specify your gateway instance ID on line 6.
   * Specify your Client ID and Client secret on lines 7 and 8.
   * Specify the group name and the group admin on lines 12 and 13.
   * Specify the content of the message on line 14.
6. Make your Node.js script executable: `chmod 755 send-telegram-text-group.py`
7. Run the script to send your message: `./send-telegram-text-group.py`


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

