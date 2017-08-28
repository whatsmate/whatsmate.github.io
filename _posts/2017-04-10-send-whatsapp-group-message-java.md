---
layout: post
title: How to send messages to a WhatsApp group in Java
subtitle: Using the WhatsMate WA Gateway REST API
published: true
last_modified_at: 2017-04-24T00:00:00+08:00
---

This article shows you how to send a message to a WhatsApp group in Java.

You MUST obtain the secret gateway number by signing up for a Forever Green account before you can send a message to a WhatsApp group. Instructions are available on the [official site](https://www.whatsmate.net/whatsapp-group-message-api.html). 


To send a WhatsApp group message from your Java application, do this:

1. Create a new group with a *unique* name. The API won't work if it's not unique.
   * <img src="/img/newgroup.png" alt="Create a new WhatsApp group"> <br><br>
2. Add the secret gateway to the group.
   * <img src="/img/add-gateway-to-group.png" alt="Name the WhatsApp group"> <br><br>
3. Say "Hi" to the group to let the gateway recognize the new group.
4. Copy the following source code to a Java file named `WhatsappSender.java`.  <script src="https://gist.github.com/whatsmate/757084bdfebe4e05875ad71bbb92e558.js"></script>
5. Customize the TODO lines in the Java program:
   * Specify your gateway instance ID on line 9.
   * Specify your Client ID and Client secret on lines 10 and 11.
   * Specify the group admin number (i.e. your WhatsApp number including the country code) on line 18.
   * Specify the group name (e.g. Happy Club) on line 19.
   * Specify the content of the message on line 20.
5. Compile the Java file: `javac WhatsappSender.java`
6. Execute the class to send your message: `java WhatsappSender`


As mentioned at the beginning of this tutorial, you will need a trial account to call the above API. Go [sign up](https://www.whatsmate.net/whatsapp-group-message-api.html) now.


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

