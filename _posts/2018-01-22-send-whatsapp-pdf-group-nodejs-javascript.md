---
layout: post
title: How to send a PDF file to a WhatsApp group in Node.js
subtitle: Using the WhatsMate WhatsApp Gateway REST API
published: true
last_modified_at: 2026-01-28T20:11:00+08:00
---

This article shows you how to send a document (e.g. a PDF file, an MP4 file, a WAV file, etc.) to a WhatsApp group in Node.js (JavaScript).


To send a PDF document in to a WhatsApp group in `Node.js`, do this:

1. First, learn how to send a simple text message on the [official site](https://www.whatsmate.net/whatsapp-group-message-api.html). 
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/wa-demos/archive/master.zip).
3. Locate the file `nodejs/send-pdf-group.js`.  <script src="https://gist.github.com/whatsmate/cbf97a5b5b9da750222f8061a2a19141.js"></script>
4. Study the `Node.js` source code and customize the TODO/FIXME lines.
   * Among other things, you must name your group *creatively*. Otherwise, the group may not receive the message.
5. Change to the directory containing the script: `cd nodejs`
6. Run the script to send your group the first PDF file: `./send-pdf-group.js`


Happy coding :) 


<br>

