---
layout: post
title: How to send WhatsApp Messages from Google Apps Script
subtitle: Using the WhatsMate WA Gateway REST API
published: true
---

This article shows you how to send a WhatsApp message from a Google Apps Script.

Before the recipient can receive your WhatsApp message, she will need to register with the WhatsMate WA Gateway. Instructions are available on the [official site](https://www.whatsmate.net/whatsapp-gateway-api.html). *Unregistered users will NEVER receive messages from the Gateway.*


To send a WhatsApp message from a Google Apps Script, do this:

1. Copy the following source code to your Apps Script project.  <script src="https://gist.github.com/whatsmate/96637d1c46e1a199756f18413e739f7b.js"></script>
2. Specify your target recipient on line 2. Remember to include the country code.
3. Specify your message on line 3.
4. Run the function `main()` to send your message.


The trial account allows you to send up to 30 messages per day for the first 1000 messsages. [Upgrade to the Forever Green plan](https://www.whatsmate.net/whatsapp-gateway-subscribe.html) to keep your application running after the trial period.


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

