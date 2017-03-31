---
layout: post
title: How to send Telegram Messages in VB Script / VBA
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2017-03-31T00:00:00+08:00
---

This article shows you how to send a Telegram message in VBA / Visual Basic Script.

Before the recipient can receive your Telegram message, she will need to register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


<iframe width="560" height="315" src="https://www.youtube.com/embed/k-rLSpSbI4A?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


To send a Telegram message in VB Script / VBA, do this:

1. In Excel / Access / your VBA environment, define the following subroutines.  <script src="https://gist.github.com/whatsmate/79eb60c857d994fa7b9ff3e6ff7a491f.js"></script>
2. Specify your target recipient and message on line 4. Remember to include the country code in the recipient's number.
3. Run it.


The trial account allows you to test the API for 2 weeks. Go [sign up](https://www.whatsmate.net/telegram-gateway-api.html) now.


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

