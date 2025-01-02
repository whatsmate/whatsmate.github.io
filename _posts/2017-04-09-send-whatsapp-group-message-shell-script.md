---
layout: post
title: How to send messages to a WhatsApp group from shell script
subtitle: Using the WhatsMate WA Gateway REST API
published: true
last_modified_at: 2025-01-02T00:00:00+08:00
---

This article shows you how to send a message to a WhatsApp group from a shell script.

You MUST obtain the secret gateway number by signing up for a Forever Green account before you can send a message to a WhatsApp group. Instructions are available on the [official site](https://www.whatsmate.net/whatsapp-group-message-api.html). 


To send a WhatsApp group message from a shell script, do this:

1. Create a new group with a *unique* name. The API won't work if it's not unique.
   * <img src="/img/newgroup.png" alt="Create a new WhatsApp group"> <br><br>
2. Add the secret gateway to the group.
   * <img src="/img/add-gateway-to-group.png" alt="Name the WhatsApp group"> <br><br>
3. Say "Hi" to the group to let the gateway recognize the new group.
4. Copy the following source code to your script.  <script src="https://gist.github.com/whatsmate/cc781206fc77896813a9e32f7707ebad.js"></script>
5. Customize the TODO lines in the script:
   * Specify your gateway instance ID on line 3.
   * Specify your Client ID and Client secret on lines 4 and 5.
   * Specify the group admin number (i.e. your WhatsApp number including the country code) on line 10.
   * Specify the group name (e.g. Happy Club) on line 11.
   * Specify the content of the message on line 12.
5. Make your script executable: `chmod 755 send-whatsapp-group-message.sh`
6. Run the script to send your message: `./send-whatsapp-group-message.sh`


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

