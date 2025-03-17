---
layout: post
title: How to send a PDF file to a WhatsApp group in Python 3
subtitle: Using the WhatsMate WhatsApp Gateway REST API
published: true
last_modified_at: 2025-03-16T00:00:00+08:00
---

This article shows you how to send a document (e.g. a PDF file, an MP4 file, a WAV file, etc.) to a WhatsApp group in Python 3.


To send a PDF document to a WhatsApp group in Python 3, do this:

1. First, learn how to send a simple text message on the [official site](https://www.whatsmate.net/whatsapp-group-message-api.html). 
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/wa-demos/archive/master.zip).
3. Locate the file `python3/send-pdf-group.py`.  <script src="https://gist.github.com/whatsmate/f0a51f7569a8c007f66c88ed419d3406.js"></script>
4. Study the Python source code and customize the TODO/FIXME lines.
   * Among other things, you must name your group *creatively*. Otherwise, the group may not receive the message.
5. Change to the directory containing the script: `cd python3`
6. Run the Python script to send yourself the first PDF file: `./send-pdf-group.py`


Happy coding :) 


<br>

