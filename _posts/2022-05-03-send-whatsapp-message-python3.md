---
layout: post
title: How to send WhatsApp Messages in Python 3
subtitle: Using the WhatsMate WA Gateway REST API
published: true
last_modified_at: 2026-01-28T20:11:00+08:00
---

This article shows you how to send a WhatsApp message from a Python script (version 3+).

Before the recipient can receive your WhatsApp message, she will need to register with the WhatsMate WA Gateway. Instructions are available on the [official site](https://www.whatsmate.net/whatsapp-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


<iframe width="560" height="315" src="https://www.youtube.com/embed/iQnzXsuywag?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


To send a WhatsApp message from a Python script, do this:

1. Copy the following source code to your script.  <script src="https://gist.github.com/whatsmate/d08c4272906ab8611e207d746c22fa01.js"></script>
2. Customize the TODO lines:
   * Specify your gateway instance ID on line 6.
   * Specify your Client ID and Secret on lines 7 and 8.
   * Specify your target recipient on line 12. Remember to include the country code.
   * Specify your message on line 13.
3. Make your script executable: `chmod 755 send-whatsapp-text-individual.py`
4. Run the script to send your message: `./send-whatsapp-text-individual.py`


You will need a trial account to call the above API. Go [sign up](https://www.whatsmate.net/whatsapp-gateway-api.html) now.



<br>
