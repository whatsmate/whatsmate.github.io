---
layout: post
title: How to send WhatsApp Messages in Visual Basic Script / VBA
subtitle: Using the WhatsMate WA Gateway REST API
published: true
last_modified_at: 2022-05-03T00:00:00+08:00
---

This article shows you how to send a WhatsApp message in VBA / Visual Basic Script.

Before the recipient can receive your WhatsApp message, she will need to register with the WhatsMate WA Gateway. Instructions are available on the [official site](https://www.whatsmate.net/whatsapp-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


<iframe width="560" height="315" src="https://www.youtube.com/embed/WLg61BEj-FA?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


To send a WhatsApp message in VBA / VB Script, do this:

1. In your Excel / Access / VBA development environment, define the following subroutines:  <script src="https://gist.github.com/whatsmate/dd1a1b80342b87f778ef732bb5a12582.js"></script>
2. Customize the TODO lines:
   * Specify your gateway instance ID on line 15.
   * Specify your client ID and secret on lines 16 and 17.
   * Specify your target recipient and message on line 4. Remember to include the country code in the recipient's number.
3. Run it.


You will need a trial account to call the above API. Go [sign up](https://www.whatsmate.net/whatsapp-gateway-api.html) now.



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

