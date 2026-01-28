---
layout: post
title: How to send a PDF file to a WhatsApp user in Java
subtitle: Using the WhatsMate WhatsApp Gateway REST API
published: true
last_modified_at: 2026-01-28T20:11:00+08:00
---

This article shows you how to send a document (e.g. a PDF file, an MP4 file, a WAV file, etc.) to a registered WhatsApp user in Java.

Before the recipient can receive your WhatsApp message, she MUST register with the WhatsMate WA Gateway. Instructions are available on the [official site](https://www.whatsmate.net/whatsapp-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


To send a WhatsApp message containing a PDF document in Java, do this:

1. First, learn how to send a simple text message on the [official site](https://www.whatsmate.net/whatsapp-gateway-api.html). 
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/wa-demos/archive/master.zip).
3. Locate the file `Java/WaPdfSender.java`.  <script src="https://gist.github.com/whatsmate/8e034dc5e92ca402436818a5c7701894.js"></script>
4. Study the Java source code and customize the TODO/FIXME lines.
   * Among other things, put down YOUR OWN number as the recipient. You can't send messages to strangers because we are against SPAMMERS.
5. Change to the directory containing the script: `cd Java`
6. Follow the instructions at the top of the source code to compile and run the Java program.


Happy coding :) 


<br>

