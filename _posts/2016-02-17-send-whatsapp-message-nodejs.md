---
layout: post
title: How to send WhatsApp Messages in Node.js
subtitle: Using the WhatsMate WA Gateway REST API
published: true
---

This article shows you how to send a WhatsApp message in `Node.js`.

Before the recipient can receive your WhatsApp message, she will need to register with the WhatsMate WA Gateway. Instructions are available on the [official site](http://www.whatsmate.net/whatsapp-gateway.html). *Unregistered users will never receive messages from the Gateway.*


To send a WhatsApp message in `Node.js`, do this:

1. Copy the following source code to your script.  <script src="https://gist.github.com/whatsmate/3cdd056532d2e675922c.js"></script>
2. Specify your target recipient on line 9. Remember to include the country code.
3. Specify your message on line 10.
4. Make your `Node.js` script executable: `chmod 755 send-whatsapp.js`
5. Run the script to send your message: `./send-whatsapp.js`


The trial account allows you to send up to 100 messages per day. [Upgrade to the Premium Account](http://www.whatsmate.net/premium-account.html) to send unlimited number of messages.


