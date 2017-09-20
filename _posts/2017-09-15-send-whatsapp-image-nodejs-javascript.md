---
layout: post
title: How to send an image to a WhatsApp user in Node.js
subtitle: Using the WhatsMate WhatsApp Gateway REST API
published: true
last_modified_at: 2017-09-19T00:00:00+08:00
---

This article shows you how to send an image to a registered WhatsApp user in Node.js (JavaScript).

Before the recipient can receive your WhatsApp message, she MUST register with the WhatsMate WA Gateway. Instructions are available on the [official site](https://www.whatsmate.net/whatsapp-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


To send a WhatsApp message containing an image in `Node.js`, do this:

1. First, learn how to send a simple text message on the [official site](https://www.whatsmate.net/whatsapp-gateway-api.html). 
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/wa-demos/archive/master.zip).
3. Locate the file `nodejs/send-image-individual.js`.  <script src="http://gist-it.appspot.com/github/whatsmate/wa-demos/blob/master/nodejs/send-image-individual.js?footer=minimal"></script>
4. Study the `Node.js` source code and customize the TODO/FIXME lines.
   * Among other things, put down YOUR OWN number as the recipient. You can't send messages to strangers because we are against SPAMMERS.
5. Change to the directory containing the script: `cd nodejs`
6. Run the script to send yourself the first image: `./send-image-individual.js`


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

