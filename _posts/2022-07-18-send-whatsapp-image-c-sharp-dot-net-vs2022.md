---
layout: post
title: How to send an image to a WhatsApp user in C# (.NET) using Visual Studio 2022
subtitle: Using the WhatsMate WhatsApp Gateway REST API
published: true
last_modified_at: 2025-03-16T00:00:00+08:00
---

This article shows you how to send an image to a registered WhatsApp user in Microsoft's .NET language: C# using Visual Studio 2022.

If you are using Visual Studio 2019, please read [this tutorial](/2017-09-14-send-whatsapp-image-c-sharp-dot-net/) instead.

Before the recipient can receive your WhatsApp message, she MUST register with the WhatsMate WA Gateway. Instructions are available on the [official site](https://www.whatsmate.net/whatsapp-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


To send a WhatsApp message containing an image in C#, do this:

1. First, learn how to send a simple text message on the [official site](https://www.whatsmate.net/whatsapp-gateway-api.html). 
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/wa-demos/archive/master.zip).
3. Locate the file `cs_vs2022/send-image-individual.cs`.  <script src="https://gist.github.com/whatsmate/45bad35fa9d5fa1cc400d4787748e5b0.js"></script>
4. Study the `C#` source code and customize the TODO/FIXME lines.
   * Among other things, put down YOUR OWN number as the recipient. You can't send messages to strangers because we are against SPAMMERS.
5. Run the `C#` program in Visual Studio to send yourself the first image!


Happy coding :) 


<br>

