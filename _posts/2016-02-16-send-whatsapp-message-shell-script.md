---
layout: post
title: How to send WhatsApp Messages from shell script
subtitle: Using the WhatsMate WA Gateway REST API
published: true
---

This article shows you how to send a WhatsApp message from a shell script.

Before the recipient can receive your WhatsApp message, she will need to register with the WhatsMate WA Gateway. Instructions are available on the [official site](http://www.whatsmate.net/whatsapp-gateway.html). *Unregistered users will never receive messages from the Gateway.*


<iframe width="560" height="315" src="https://www.youtube.com/embed/XpKUzSD9qu0?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


To send a WhatsApp message from a shell script, do this:

1. Copy the following source code to your script.  <script src="https://gist.github.com/whatsmate/10c75499502a2ededc23.js"></script>
2. Specify your target recipient on line 8. Remember to include the country code.
3. Specify your message on line 9.
4. Make your script executable: `chmod 755 send-whatsapp.sh`
5. Run the script to send your message: `./send-whatsapp.sh`


The trial account allows you to send up to 40 messages per day. [Upgrade to the Premium Account](http://www.whatsmate.net/premium-account.html) to send unlimited number of messages.



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

