---
layout: post
title: How to send a PDF file to a WhatsApp user in Visual Basic Script / VBA
subtitle: Using the WhatsMate WhatsApp Gateway REST API
published: true
last_modified_at: 2025-03-16T00:00:00+08:00
---


This article shows you how to send a document (e.g. a PDF file, an MP4 file, a WAV file, etc.) to a registered WhatsApp user in VBA / Visual Basic Script.

Before the recipient can receive your WhatsApp message, she MUST register with the WhatsMate WA Gateway. Instructions are available on the [official site](https://www.whatsmate.net/whatsapp-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


To send a WhatsApp message containing a PDF document in VBA, do this:

1. First, learn how to send a simple text message on the [official site](https://www.whatsmate.net/whatsapp-gateway-api.html).
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/wa-demos/archive/master.zip).
3. Locate the file `vba/SendDocument.vbs`.  <script src="https://gist.github.com/whatsmate/01ba745741b89a7394db9fa9ab845ae0.js"></script>
4. Study the `VBA` source code and customize the TODO/FIXME lines.
   * Among other things, put down YOUR OWN number as the recipient. You can't send messages to strangers because we are against SPAMMERS.
5. Copy the image `assets\subwaymap.pdf` in the sample code package to `C:\Users\Public\subwaymap.pdf`
6. Run `Main_Routine` in the VBA program.


Happy coding :) 


<br>

