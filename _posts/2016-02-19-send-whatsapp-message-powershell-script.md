---
layout: post
title: How to send WhatsApp Messages from PowerShell script
subtitle: Using the WhatsMate WA Gateway REST API
published: true
---

This article shows you how to send a WhatsApp message from a PowerShell script.

Before the recipient can receive your WhatsApp message, she will need to register with the WhatsMate WA Gateway. Instructions are available on the [official site](https://www.whatsmate.net/whatsapp-gateway.html). *Unregistered users will never receive messages from the Gateway.*


<iframe width="560" height="315" src="https://www.youtube.com/embed/lbjjqdRPvP0?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


To send a WhatsApp message from a PowerShell script, do this:

1. Copy the following source code to your PowerShell script.  <script src="https://gist.github.com/whatsmate/3ba4213c8aee9a6bfa71.js"></script>
2. Specify your target recipient on line 1. Remember to include the country code.
3. Specify your message on line 2.
4. Run the script in PowerShell to send your message: `.\send-whatsapp.ps1`


The trial account allows you to send up to 40 messages per day. [Upgrade to the Premium Account](https://www.whatsmate.net/premium-account.html) to send unlimited number of messages.



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

