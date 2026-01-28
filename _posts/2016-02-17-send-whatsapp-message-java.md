---
layout: post
title: How to send WhatsApp Messages in Java
subtitle: Using the WhatsMate WA Gateway REST API
published: true
last_modified_at: 2026-01-28T20:11:00+08:00
---

This article shows you how to send a WhatsApp message in `Java`.

Before the recipient can receive your WhatsApp message, she will need to register with the WhatsMate WA Gateway. Instructions are available on the [official site](https://www.whatsmate.net/whatsapp-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


<iframe width="560" height="315" src="https://www.youtube.com/embed/Tpw7pVnpu1A?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


To send a WhatsApp message in `Java`, do this:

1. Copy the following source code to a Java file named `WhatsappSender.java`.  <script src="https://gist.github.com/whatsmate/ada1343baa4f7364d3e1.js"></script>
2. Customize the TODO lines:
   * Specify your gateway instance ID on line 9.
   * Specify your client ID and secret on lines 10 and 11.
   * Specify your target recipient on line 18. Remember to include the country code.
   * Specify your message on line 19.
3. Compile the Java file:  `javac WhatsappSender.java`
4. Execute the class to send your message: `java WhatsappSender`


You will need a trial account to call the above API. Go [sign up](https://www.whatsmate.net/whatsapp-gateway-api.html) now.



<br>

